# Comparing `tmp/parmoo-0.2.0.tar.gz` & `tmp/parmoo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parmoo-0.2.0.tar", last modified: Thu Feb  2 18:58:34 2023, max compression
+gzip compressed data, was "parmoo-0.2.1.tar", last modified: Mon Apr 10 20:02:01 2023, max compression
```

## Comparing `parmoo-0.2.0.tar` & `parmoo-0.2.1.tar`

### file list

```diff
@@ -1,176 +1,180 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.105746 parmoo-0.2.0/
--rw-r--r--   0 tyler      (501) staff       (20)     3248 2023-02-02 18:56:59.000000 parmoo-0.2.0/CHANGELOG.rst
--rw-r--r--   0 tyler      (501) staff       (20)     3111 2022-05-10 21:22:59.000000 parmoo-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1525 2023-02-02 18:56:59.000000 parmoo-0.2.0/LICENSE
--rw-r--r--   0 tyler      (501) staff       (20)      600 2022-05-10 21:22:59.000000 parmoo-0.2.0/MANIFEST.in
--rw-r--r--   0 tyler      (501) staff       (20)     1690 2023-02-02 18:58:34.105440 parmoo-0.2.0/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)    11621 2023-02-02 18:56:59.000000 parmoo-0.2.0/README.rst
--rw-r--r--   0 tyler      (501) staff       (20)      113 2023-02-02 18:56:59.000000 parmoo-0.2.0/REQUIREMENTS
--rw-r--r--   0 tyler      (501) staff       (20)       91 2023-02-02 18:56:59.000000 parmoo-0.2.0/SUPPORT.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.065075 parmoo-0.2.0/docs/
--rw-r--r--   0 tyler      (501) staff       (20)      671 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/Makefile
--rw-r--r--   0 tyler      (501) staff       (20)       45 2022-05-10 21:22:59.000000 parmoo-0.2.0/docs/REQUIREMENTS.txt
--rw-r--r--   0 tyler      (501) staff       (20)    12729 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/about.rst
--rw-r--r--   0 tyler      (501) staff       (20)      257 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/api.rst
--rw-r--r--   0 tyler      (501) staff       (20)     3550 2022-09-09 18:02:05.000000 parmoo-0.2.0/docs/conf.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.065916 parmoo-0.2.0/docs/dev-guide/
--rw-r--r--   0 tyler      (501) staff       (20)       36 2022-05-10 21:22:59.000000 parmoo-0.2.0/docs/dev-guide/contributing.rst
--rw-r--r--   0 tyler      (501) staff       (20)      162 2022-05-10 21:22:59.000000 parmoo-0.2.0/docs/dev-guide/modules.rst
--rw-r--r--   0 tyler      (501) staff       (20)       33 2022-05-10 21:22:59.000000 parmoo-0.2.0/docs/dev-guide/release-notes.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1961 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/dev-guide/release-proc.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2831 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/extras.rst
--rw-r--r--   0 tyler      (501) staff       (20)    30292 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/how-to-write.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.069953 parmoo-0.2.0/docs/img/
--rw-r--r--   0 tyler      (501) staff       (20)   395713 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/img/algorithm-flowchart.png
--rw-r--r--   0 tyler      (501) staff       (20)   142159 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/des-obj-space.png
--rw-r--r--   0 tyler      (501) staff       (20)   133860 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/des-sim-obj-space.png
--rw-r--r--   0 tyler      (501) staff       (20)    24057 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/icon-ParMOO.png
--rw-r--r--   0 tyler      (501) staff       (20)     2551 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/icon-ParMOO.svg
--rw-r--r--   0 tyler      (501) staff       (20)    36996 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/icon-ParMOO_space.png
--rw-r--r--   0 tyler      (501) staff       (20)    51610 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/logo-ParMOO.png
--rw-r--r--   0 tyler      (501) staff       (20)     4441 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/logo-ParMOO.svg
--rw-r--r--   0 tyler      (501) staff       (20)    71259 2022-05-10 21:22:59.000000 parmoo-0.2.0/docs/img/logo-ParMOO_white.png
--rw-r--r--   0 tyler      (501) staff       (20)   175826 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/img/moop-uml.png
--rw-r--r--   0 tyler      (501) staff       (20)   261708 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/img/moop-uml.svg
--rw-r--r--   0 tyler      (501) staff       (20)     1705 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/img/moop.uml
--rw-r--r--   0 tyler      (501) staff       (20)  7658326 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/img/parmoo_movie.gif
--rw-r--r--   0 tyler      (501) staff       (20)     1580 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/index.rst
--rw-r--r--   0 tyler      (501) staff       (20)     4789 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/install.rst
--rw-r--r--   0 tyler      (501) staff       (20)      862 2022-05-10 21:22:59.000000 parmoo-0.2.0/docs/latex_index.rst
--rw-r--r--   0 tyler      (501) staff       (20)      799 2022-05-10 17:20:56.000000 parmoo-0.2.0/docs/make.bat
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.081156 parmoo-0.2.0/docs/modules/
--rw-r--r--   0 tyler      (501) staff       (20)     1090 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/acquisitions.rst
--rw-r--r--   0 tyler      (501) staff       (20)      366 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/class_api.rst
--rw-r--r--   0 tyler      (501) staff       (20)      795 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/constraints.rst
--rw-r--r--   0 tyler      (501) staff       (20)      211 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/dev_tools.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2698 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/dtlz.rst
--rw-r--r--   0 tyler      (501) staff       (20)      493 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/libe.rst
--rw-r--r--   0 tyler      (501) staff       (20)      735 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/libraries.rst
--rw-r--r--   0 tyler      (501) staff       (20)      583 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/moop.rst
--rw-r--r--   0 tyler      (501) staff       (20)      753 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/objectives.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1639 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/optimizers.rst
--rw-r--r--   0 tyler      (501) staff       (20)      853 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/searches.rst
--rw-r--r--   0 tyler      (501) staff       (20)      253 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/simulations.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1098 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/structs.rst
--rw-r--r--   0 tyler      (501) staff       (20)      713 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/surrogates.rst
--rw-r--r--   0 tyler      (501) staff       (20)      338 2022-09-09 18:45:50.000000 parmoo-0.2.0/docs/modules/util.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2890 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/modules/viz.rst
--rw-r--r--   0 tyler      (501) staff       (20)    11145 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/quickstart.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1335 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/refs.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.081564 parmoo-0.2.0/docs/tutorials/
--rw-r--r--   0 tyler      (501) staff       (20)     4527 2023-02-02 18:56:59.000000 parmoo-0.2.0/docs/tutorials/basic-tutorials.rst
--rw-r--r--   0 tyler      (501) staff       (20)      678 2022-05-10 21:22:59.000000 parmoo-0.2.0/docs/tutorials/libe-tutorial.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.085023 parmoo-0.2.0/examples/
--rw-r--r--   0 tyler      (501) staff       (20)     1010 2023-02-02 18:56:59.000000 parmoo-0.2.0/examples/Makefile
--rw-r--r--   0 tyler      (501) staff       (20)    18139 2023-02-02 18:56:59.000000 parmoo-0.2.0/examples/Pareto Front.jpeg
--rw-r--r--   0 tyler      (501) staff       (20)     1972 2022-05-10 21:22:59.000000 parmoo-0.2.0/examples/advanced_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     3765 2022-05-10 17:20:56.000000 parmoo-0.2.0/examples/advanced_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)     1635 2023-02-02 18:56:59.000000 parmoo-0.2.0/examples/checkpointing.out
--rw-r--r--   0 tyler      (501) staff       (20)     2299 2022-05-10 21:22:59.000000 parmoo-0.2.0/examples/checkpointing.py
--rw-r--r--   0 tyler      (501) staff       (20)     1071 2023-02-02 18:56:59.000000 parmoo-0.2.0/examples/libe_basic_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     2243 2023-02-02 18:56:59.000000 parmoo-0.2.0/examples/libe_basic_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)      153 2022-07-11 19:27:11.000000 parmoo-0.2.0/examples/named_var_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     1620 2022-05-10 21:22:59.000000 parmoo-0.2.0/examples/named_var_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)      108 2022-07-11 19:27:11.000000 parmoo-0.2.0/examples/precomputed_data.out
--rw-r--r--   0 tyler      (501) staff       (20)     1409 2022-06-15 17:14:45.000000 parmoo-0.2.0/examples/precomputed_data.py
--rw-r--r--   0 tyler      (501) staff       (20)     1207 2023-02-02 18:56:59.000000 parmoo-0.2.0/examples/quickstart.out
--rw-r--r--   0 tyler      (501) staff       (20)     1575 2023-02-02 18:56:59.000000 parmoo-0.2.0/examples/quickstart.py
--rw-r--r--   0 tyler      (501) staff       (20)      582 2022-07-11 19:27:11.000000 parmoo-0.2.0/examples/unnamed_var_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     2336 2022-05-10 21:22:59.000000 parmoo-0.2.0/examples/unnamed_var_ex.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.086372 parmoo-0.2.0/parmoo/
--rw-r--r--   0 tyler      (501) staff       (20)      363 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.088047 parmoo-0.2.0/parmoo/acquisitions/
--rw-r--r--   0 tyler      (501) staff       (20)      104 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/acquisitions/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     9122 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/acquisitions/epsilon_constraint.py
--rw-r--r--   0 tyler      (501) staff       (20)    15030 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/acquisitions/weighted_sum.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.088694 parmoo-0.2.0/parmoo/constraints/
--rw-r--r--   0 tyler      (501) staff       (20)       60 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/constraints/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/constraints/const_func.py
--rw-r--r--   0 tyler      (501) staff       (20)    18473 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/constraints/const_lib.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.089103 parmoo-0.2.0/parmoo/extras/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/extras/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    36753 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/extras/libe.py
--rw-r--r--   0 tyler      (501) staff       (20)   127470 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/moop.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.090115 parmoo-0.2.0/parmoo/objectives/
--rw-r--r--   0 tyler      (501) staff       (20)       54 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/objectives/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    22933 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/objectives/dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/objectives/obj_func.py
--rw-r--r--   0 tyler      (501) staff       (20)    16981 2022-07-26 17:47:19.000000 parmoo-0.2.0/parmoo/objectives/obj_lib.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.091293 parmoo-0.2.0/parmoo/optimizers/
--rw-r--r--   0 tyler      (501) staff       (20)      122 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/optimizers/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    17274 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/optimizers/gps_search.py
--rw-r--r--   0 tyler      (501) staff       (20)    20784 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/optimizers/lbfgsb.py
--rw-r--r--   0 tyler      (501) staff       (20)     8330 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/optimizers/random_search.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.091806 parmoo-0.2.0/parmoo/searches/
--rw-r--r--   0 tyler      (501) staff       (20)       44 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/searches/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3736 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/searches/latin_hypercube.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.092462 parmoo-0.2.0/parmoo/simulations/
--rw-r--r--   0 tyler      (501) staff       (20)       31 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/simulations/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    31184 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/simulations/dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     1921 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/simulations/sim_func.py
--rw-r--r--   0 tyler      (501) staff       (20)    16723 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/structs.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.092893 parmoo-0.2.0/parmoo/surrogates/
--rw-r--r--   0 tyler      (501) staff       (20)       51 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/surrogates/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    32983 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/surrogates/gaussian_proc.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.093540 parmoo-0.2.0/parmoo/tests/
--rw-r--r--   0 tyler      (501) staff       (20)      103 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/.coveragerc
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.093993 parmoo-0.2.0/parmoo/tests/.pytest_cache/
--rw-r--r--   0 tyler      (501) staff       (20)      194 2022-02-21 21:48:43.000000 parmoo-0.2.0/parmoo/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 tyler      (501) staff       (20)      295 2022-02-21 21:48:43.000000 parmoo-0.2.0/parmoo/tests/.pytest_cache/README.md
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.059294 parmoo-0.2.0/parmoo/tests/.pytest_cache/v/
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.094404 parmoo-0.2.0/parmoo/tests/.pytest_cache/v/cache/
--rw-r--r--   0 tyler      (501) staff       (20)     1948 2022-03-04 02:25:24.000000 parmoo-0.2.0/parmoo/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 tyler      (501) staff       (20)        2 2022-03-04 02:25:24.000000 parmoo-0.2.0/parmoo/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.0/parmoo/tests/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.094987 parmoo-0.2.0/parmoo/tests/libe_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.0/parmoo/tests/libe_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     1305 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/libe_tests/libe_funcs.py
--rw-r--r--   0 tyler      (501) staff       (20)     3003 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/libe_tests/test_libe_gen.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.097374 parmoo-0.2.0/parmoo/tests/regression_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.0/parmoo/tests/regression_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     2984 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz1_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     3032 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz1_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     2456 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz2_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     2411 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz2_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     3042 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz3_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     3391 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz3_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     1941 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz5_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     2173 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_infeasible_prob.py
--rw-r--r--   0 tyler      (501) staff       (20)     2581 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_mixed_variables.py
--rw-r--r--   0 tyler      (501) staff       (20)     2226 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/regression_tests/test_user_func.py
--rwxr-xr-x   0 tyler      (501) staff       (20)     2680 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/run-tests.sh
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.103082 parmoo-0.2.0/parmoo/tests/unit_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     8616 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_const_lib.py
--rw-r--r--   0 tyler      (501) staff       (20)     4027 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_epsilon_constraint.py
--rw-r--r--   0 tyler      (501) staff       (20)    15408 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_gaussian_proc.py
--rw-r--r--   0 tyler      (501) staff       (20)     7507 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_gps_search.py
--rw-r--r--   0 tyler      (501) staff       (20)     1643 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_latin_hypercube.py
--rw-r--r--   0 tyler      (501) staff       (20)     8794 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_lbfgsb.py
--rw-r--r--   0 tyler      (501) staff       (20)     6534 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_libe.py
--rw-r--r--   0 tyler      (501) staff       (20)    92453 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_moop.py
--rw-r--r--   0 tyler      (501) staff       (20)    27887 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_moop_embeddings.py
--rw-r--r--   0 tyler      (501) staff       (20)     6987 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_obj_dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     8342 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_obj_lib.py
--rw-r--r--   0 tyler      (501) staff       (20)     3569 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_random_search.py
--rw-r--r--   0 tyler      (501) staff       (20)     4732 2022-05-10 17:20:56.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_sims_dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     1093 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_structs.py
--rw-r--r--   0 tyler      (501) staff       (20)    10108 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_util.py
--rw-r--r--   0 tyler      (501) staff       (20)    24746 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_viz_without_dash.py
--rw-r--r--   0 tyler      (501) staff       (20)     7366 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/tests/unit_tests/test_weighted_sum.py
--rw-r--r--   0 tyler      (501) staff       (20)    18802 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/util.py
--rw-r--r--   0 tyler      (501) staff       (20)       22 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/version.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.104974 parmoo-0.2.0/parmoo/viz/
--rw-r--r--   0 tyler      (501) staff       (20)      320 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/viz/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    35252 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/viz/dashboard.py
--rw-r--r--   0 tyler      (501) staff       (20)     6079 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/viz/graph.py
--rw-r--r--   0 tyler      (501) staff       (20)    17752 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/viz/plot.py
--rw-r--r--   0 tyler      (501) staff       (20)    14045 2023-02-02 18:56:59.000000 parmoo-0.2.0/parmoo/viz/utilities.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-02-02 18:58:34.087416 parmoo-0.2.0/parmoo.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)     1690 2023-02-02 18:58:33.000000 parmoo-0.2.0/parmoo.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)     4380 2023-02-02 18:58:34.000000 parmoo-0.2.0/parmoo.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2023-02-02 18:58:33.000000 parmoo-0.2.0/parmoo.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)      120 2023-02-02 18:58:33.000000 parmoo-0.2.0/parmoo.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)        7 2023-02-02 18:58:33.000000 parmoo-0.2.0/parmoo.egg-info/top_level.txt
--rw-r--r--   0 tyler      (501) staff       (20)       38 2023-02-02 18:58:34.105843 parmoo-0.2.0/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)     3416 2023-02-02 18:56:59.000000 parmoo-0.2.0/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.935469 parmoo-0.2.1/
+-rw-r--r--   0 tyler      (501) staff       (20)     4084 2023-04-10 20:01:13.000000 parmoo-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     3111 2022-05-10 21:22:59.000000 parmoo-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1525 2023-02-21 22:52:41.000000 parmoo-0.2.1/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)      600 2022-05-10 21:22:59.000000 parmoo-0.2.1/MANIFEST.in
+-rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-10 20:02:01.934879 parmoo-0.2.1/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)    11817 2023-04-10 20:01:13.000000 parmoo-0.2.1/README.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      113 2023-04-10 20:01:13.000000 parmoo-0.2.1/REQUIREMENTS
+-rw-r--r--   0 tyler      (501) staff       (20)       91 2023-02-21 22:52:41.000000 parmoo-0.2.1/SUPPORT.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.778071 parmoo-0.2.1/docs/
+-rw-r--r--   0 tyler      (501) staff       (20)      671 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/Makefile
+-rw-r--r--   0 tyler      (501) staff       (20)       45 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/REQUIREMENTS.txt
+-rw-r--r--   0 tyler      (501) staff       (20)    12729 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/about.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      257 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/api.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     3586 2023-04-10 20:01:13.000000 parmoo-0.2.1/docs/conf.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.779875 parmoo-0.2.1/docs/dev-guide/
+-rw-r--r--   0 tyler      (501) staff       (20)       36 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/dev-guide/contributing.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      162 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/dev-guide/modules.rst
+-rw-r--r--   0 tyler      (501) staff       (20)       33 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/dev-guide/release-notes.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1961 2023-02-21 22:52:43.000000 parmoo-0.2.1/docs/dev-guide/release-proc.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2831 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/extras.rst
+-rw-r--r--   0 tyler      (501) staff       (20)    30292 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/how-to-write.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.793972 parmoo-0.2.1/docs/img/
+-rw-r--r--   0 tyler      (501) staff       (20)   395713 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/algorithm-flowchart.png
+-rw-r--r--   0 tyler      (501) staff       (20)   142159 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/des-obj-space.png
+-rw-r--r--   0 tyler      (501) staff       (20)   133860 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/des-sim-obj-space.png
+-rw-r--r--   0 tyler      (501) staff       (20)    24057 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/icon-ParMOO.png
+-rw-r--r--   0 tyler      (501) staff       (20)     2551 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/icon-ParMOO.svg
+-rw-r--r--   0 tyler      (501) staff       (20)    36996 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/icon-ParMOO_space.png
+-rw-r--r--   0 tyler      (501) staff       (20)    51610 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/logo-ParMOO.png
+-rw-r--r--   0 tyler      (501) staff       (20)     4441 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/logo-ParMOO.svg
+-rw-r--r--   0 tyler      (501) staff       (20)    71259 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/img/logo-ParMOO_white.png
+-rw-r--r--   0 tyler      (501) staff       (20)   175826 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/moop-uml.png
+-rw-r--r--   0 tyler      (501) staff       (20)   261708 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/moop-uml.svg
+-rw-r--r--   0 tyler      (501) staff       (20)     1705 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/moop.uml
+-rw-r--r--   0 tyler      (501) staff       (20)  7658326 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/parmoo_movie.gif
+-rw-r--r--   0 tyler      (501) staff       (20)     1580 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/index.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     4789 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/install.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      862 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/latex_index.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      799 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/make.bat
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.831032 parmoo-0.2.1/docs/modules/
+-rw-r--r--   0 tyler      (501) staff       (20)     1090 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/acquisitions.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      366 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/class_api.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      795 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/constraints.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      211 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/dev_tools.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2698 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/dtlz.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      493 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/libe.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      735 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/libraries.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      583 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/moop.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      753 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/objectives.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1639 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/optimizers.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      853 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/searches.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      253 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/simulations.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1098 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/structs.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      713 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/surrogates.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      338 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/util.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2890 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/modules/viz.rst
+-rw-r--r--   0 tyler      (501) staff       (20)    11145 2023-04-10 20:01:13.000000 parmoo-0.2.1/docs/quickstart.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1390 2023-04-10 20:01:13.000000 parmoo-0.2.1/docs/refs.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.832016 parmoo-0.2.1/docs/tutorials/
+-rw-r--r--   0 tyler      (501) staff       (20)     4527 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/tutorials/basic-tutorials.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      678 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/tutorials/libe-tutorial.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.840847 parmoo-0.2.1/examples/
+-rw-r--r--   0 tyler      (501) staff       (20)     1010 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/Makefile
+-rw-r--r--   0 tyler      (501) staff       (20)    16534 2023-04-10 20:01:13.000000 parmoo-0.2.1/examples/Pareto Front.jpeg
+-rw-r--r--   0 tyler      (501) staff       (20)     1972 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/advanced_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     3765 2022-05-10 17:20:56.000000 parmoo-0.2.1/examples/advanced_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1635 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/checkpointing.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2299 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/checkpointing.py
+-rw-r--r--   0 tyler      (501) staff       (20)      955 2023-04-10 20:01:13.000000 parmoo-0.2.1/examples/libe_basic_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2243 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/libe_basic_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)      153 2022-07-11 19:27:11.000000 parmoo-0.2.1/examples/named_var_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1620 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/named_var_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)      108 2022-07-11 19:27:11.000000 parmoo-0.2.1/examples/precomputed_data.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1409 2022-06-15 17:14:45.000000 parmoo-0.2.1/examples/precomputed_data.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1409 2023-04-10 20:01:13.000000 parmoo-0.2.1/examples/quickstart.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1575 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/quickstart.py
+-rw-r--r--   0 tyler      (501) staff       (20)      582 2022-07-11 19:27:11.000000 parmoo-0.2.1/examples/unnamed_var_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2336 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/unnamed_var_ex.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.845865 parmoo-0.2.1/parmoo/
+-rw-r--r--   0 tyler      (501) staff       (20)      385 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.851040 parmoo-0.2.1/parmoo/acquisitions/
+-rw-r--r--   0 tyler      (501) staff       (20)      104 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/acquisitions/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     9122 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/acquisitions/epsilon_constraint.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15030 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/acquisitions/weighted_sum.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.854205 parmoo-0.2.1/parmoo/constraints/
+-rw-r--r--   0 tyler      (501) staff       (20)       60 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/constraints/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/constraints/const_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18473 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/constraints/const_lib.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.860969 parmoo-0.2.1/parmoo/extras/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/extras/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    36753 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/extras/libe.py
+-rw-r--r--   0 tyler      (501) staff       (20)   127469 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/moop.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.877774 parmoo-0.2.1/parmoo/objectives/
+-rw-r--r--   0 tyler      (501) staff       (20)       54 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/objectives/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    22933 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/objectives/dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/objectives/obj_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16981 2022-07-26 17:47:19.000000 parmoo-0.2.1/parmoo/objectives/obj_lib.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.890171 parmoo-0.2.1/parmoo/optimizers/
+-rw-r--r--   0 tyler      (501) staff       (20)      122 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/optimizers/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17274 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/optimizers/gps_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)    20784 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/optimizers/lbfgsb.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8330 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/optimizers/random_search.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.897334 parmoo-0.2.1/parmoo/searches/
+-rw-r--r--   0 tyler      (501) staff       (20)       44 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/searches/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3736 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/searches/latin_hypercube.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.904690 parmoo-0.2.1/parmoo/simulations/
+-rw-r--r--   0 tyler      (501) staff       (20)       31 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/simulations/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    31184 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/simulations/dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1921 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/simulations/sim_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3905 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/simulations/simple.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16723 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/structs.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.906931 parmoo-0.2.1/parmoo/surrogates/
+-rw-r--r--   0 tyler      (501) staff       (20)       51 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/surrogates/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    33863 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/surrogates/gaussian_proc.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17196 2023-03-17 16:31:56.000000 parmoo-0.2.1/parmoo/surrogates/linear_model.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.909032 parmoo-0.2.1/parmoo/tests/
+-rw-r--r--   0 tyler      (501) staff       (20)      103 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/.coveragerc
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.910518 parmoo-0.2.1/parmoo/tests/.pytest_cache/
+-rw-r--r--   0 tyler      (501) staff       (20)      194 2022-02-21 21:48:43.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 tyler      (501) staff       (20)      295 2022-02-21 21:48:43.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/README.md
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.767136 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.912068 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/
+-rw-r--r--   0 tyler      (501) staff       (20)     1948 2022-03-04 02:25:24.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 tyler      (501) staff       (20)        2 2022-03-04 02:25:24.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.913990 parmoo-0.2.1/parmoo/tests/libe_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/libe_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1305 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/libe_tests/libe_funcs.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3003 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/libe_tests/test_libe_gen.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.921092 parmoo-0.2.1/parmoo/tests/regression_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/regression_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2984 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3032 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2456 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2411 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3042 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3391 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1941 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz5_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2173 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_infeasible_prob.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2581 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_mixed_variables.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2226 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_user_func.py
+-rwxr-xr-x   0 tyler      (501) staff       (20)     2691 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/run-tests.sh
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.930973 parmoo-0.2.1/parmoo/tests/unit_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/unit_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8679 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_const_lib.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4039 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_epsilon_constraint.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15426 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_gaussian_proc.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7513 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_gps_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1649 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_latin_hypercube.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8800 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_lbfgsb.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6545 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_libe.py
+-rw-r--r--   0 tyler      (501) staff       (20)    79942 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_moop.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27995 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_moop_embeddings.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16562 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_moop_grads.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7035 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8378 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_lib.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3572 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_random_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4745 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_sims_dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1708 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_sims_simple.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1093 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_structs.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10127 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_util.py
+-rw-r--r--   0 tyler      (501) staff       (20)    24842 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_viz_without_dash.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7451 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_weighted_sum.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18801 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/util.py
+-rw-r--r--   0 tyler      (501) staff       (20)       22 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/version.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.934050 parmoo-0.2.1/parmoo/viz/
+-rw-r--r--   0 tyler      (501) staff       (20)      320 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    35252 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/dashboard.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6079 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/graph.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17752 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/plot.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14045 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/utilities.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.848597 parmoo-0.2.1/parmoo.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)     4530 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      120 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        7 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2023-04-10 20:02:01.935667 parmoo-0.2.1/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)     3421 2023-04-10 20:01:13.000000 parmoo-0.2.1/setup.py
```

### Comparing `parmoo-0.2.0/CONTRIBUTING.rst` & `parmoo-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/LICENSE` & `parmoo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/MANIFEST.in` & `parmoo-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/PKG-INFO` & `parmoo-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parmoo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library for parallel multiobjective simulation optimization
 Home-page: https://github.com/parmoo/parmoo
-Author: Tyler H. Chang and Stefan M. Wild
+Author: Tyler H. Chang, Stefan M. Wild, et al.
 Author-email: parmoo@mcs.anl.gov
 License: BSD 3-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `parmoo-0.2.0/README.rst` & `parmoo-0.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 .. image:: https://github.com/parmoo/parmoo/actions/workflows/parmoo-ci.yml/badge.svg?/branch=main
     :target: https://github.com/parmoo/parmoo/actions
 
 .. image:: https://readthedocs.org/projects/parmoo/badge/?maxAge=2592000
     :target: https://parmoo.readthedocs.org/en/latest
     :alt: Documentation Status
 
+.. image:: https://joss.theoj.org/papers/10.21105/joss.04468/status.svg
+   :target: https://doi.org/10.21105/joss.04468
+   :alt: JOSS DOI
 
 |
 
 ParMOO: Python library for parallel multiobjective simulation optimization
 ==========================================================================
 
 ParMOO is a parallel multiobjective optimization solver that seeks to
@@ -58,15 +61,15 @@
 Dependencies
 ------------
 
 ParMOO has been tested on Unix/Linux and MacOS systems.
 
 ParMOO's base has the following dependencies:
 
- * Python_ 3.6+
+ * Python_ 3.8+
  * numpy_ -- for data structures and performant numerical linear algebra
  * scipy_ -- for scientific calculations needed for specific modules
  * pyDOE_ -- for generating experimental designs
  * pandas_ -- for exporting the resulting databases
 
 Additional dependencies are needed to use the additional features in
 ``parmoo.extras``:
@@ -280,30 +283,34 @@
 
 Please use one of the following to cite ParMOO.
 
 Our JOSS paper:
 
 .. code-block:: bibtex
 
-    @article{parmoo-joss,
-        title       = {{ParMOO}: A {P}ython library for parallel multiobjective simulation optimization},
-        author      = {Chang, Tyler H. and Wild, Stefan M.},
-        year        = {2023},
-        journal     = {To appear in The Journal of Open Source Software}
+    @article{parmoo,
+        author={Chang, Tyler H. and Wild, Stefan M.},
+        title={{ParMOO}: A {P}ython library for parallel multiobjective simulation optimization},
+        journal = {Journal of Open Source Software},
+        volume = {8},
+        number = {82},
+        pages = {4468},
+        year = {2023},
+        doi = {10.21105/joss.04468}
     }
 
 Our online documentation:
 
 .. code-block:: bibtex
 
     @techreport{parmoo-docs,
         title       = {{ParMOO}: {P}ython library for parallel multiobjective simulation optimization},
         author      = {Chang, Tyler H. and Wild, Stefan M. and Dickinson, Hyrum},
         institution = {Argonne National Laboratory},
-        number      = {Version 0.2.0},
+        number      = {Version 0.2.1},
         year        = {2023},
         url         = {https://parmoo.readthedocs.io/en/latest}
     }
 
 .. _Actions: https://github.com/parmoo/parmoo/actions
 .. _CONTRIBUTING: https://github.com/parmoo/parmoo/blob/main/CONTRIBUTING.rst
 .. _dash: https://dash.plotly.com
```

### Comparing `parmoo-0.2.0/docs/Makefile` & `parmoo-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/about.rst` & `parmoo-0.2.1/docs/about.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/conf.py` & `parmoo-0.2.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 sys.path.insert(0, os.path.abspath('..'))
 sys.path.insert(0, os.path.abspath('../parmoo'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'ParMOO'
-copyright = str(datetime.now().year) + ' Tyler Chang, Stefan Wild'
-author = 'Tyler Chang and Stefan Wild'
+copyright = str(datetime.now().year) + ' Tyler H. Chang, Stefan M. Wild, et al.'
+author = "Tyler H. Chang, Stefan M. Wild, et al."
 
 # The full version, including alpha/beta/rc tags
 exec(open("../parmoo/version.py").read())
 version = __version__
 release = version
 
 
@@ -91,15 +91,15 @@
     \end{lrbox}%
     \colorbox{sphinxnoteBgColor}{\usebox{\mytempbox}}}
     """,
     }
 
 latex_documents = [
     (latex_doc, "parmoo.tex", "ParMOO User's Manual",
-     "Tyler Chang and Stefan Wild", "manual"),
+     "Tyler H. Chang, Stefan M. Wild, et al.", "manual"),
      ]
 
 latex_logo = "img/logo-ParMOO_white.png"
 
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
```

### Comparing `parmoo-0.2.0/docs/dev-guide/release-proc.rst` & `parmoo-0.2.1/docs/dev-guide/release-proc.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/extras.rst` & `parmoo-0.2.1/docs/extras.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/how-to-write.rst` & `parmoo-0.2.1/docs/how-to-write.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/algorithm-flowchart.png` & `parmoo-0.2.1/docs/img/algorithm-flowchart.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/des-obj-space.png` & `parmoo-0.2.1/docs/img/des-obj-space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/des-sim-obj-space.png` & `parmoo-0.2.1/docs/img/des-sim-obj-space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/icon-ParMOO.png` & `parmoo-0.2.1/docs/img/icon-ParMOO.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/icon-ParMOO.svg` & `parmoo-0.2.1/docs/img/icon-ParMOO.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/icon-ParMOO_space.png` & `parmoo-0.2.1/docs/img/icon-ParMOO_space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/logo-ParMOO.png` & `parmoo-0.2.1/docs/img/logo-ParMOO.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/logo-ParMOO.svg` & `parmoo-0.2.1/docs/img/logo-ParMOO.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/logo-ParMOO_white.png` & `parmoo-0.2.1/docs/img/logo-ParMOO_white.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/moop-uml.png` & `parmoo-0.2.1/docs/img/moop-uml.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/moop-uml.svg` & `parmoo-0.2.1/docs/img/moop-uml.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/moop.uml` & `parmoo-0.2.1/docs/img/moop.uml`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/img/parmoo_movie.gif` & `parmoo-0.2.1/docs/img/parmoo_movie.gif`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/index.rst` & `parmoo-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/install.rst` & `parmoo-0.2.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/latex_index.rst` & `parmoo-0.2.1/docs/latex_index.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/make.bat` & `parmoo-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/acquisitions.rst` & `parmoo-0.2.1/docs/modules/acquisitions.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/constraints.rst` & `parmoo-0.2.1/docs/modules/constraints.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/dtlz.rst` & `parmoo-0.2.1/docs/modules/dtlz.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/libraries.rst` & `parmoo-0.2.1/docs/modules/libraries.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/moop.rst` & `parmoo-0.2.1/docs/modules/moop.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/objectives.rst` & `parmoo-0.2.1/docs/modules/objectives.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/optimizers.rst` & `parmoo-0.2.1/docs/modules/optimizers.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/searches.rst` & `parmoo-0.2.1/docs/modules/searches.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/structs.rst` & `parmoo-0.2.1/docs/modules/structs.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/surrogates.rst` & `parmoo-0.2.1/docs/modules/surrogates.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/modules/viz.rst` & `parmoo-0.2.1/docs/modules/viz.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/quickstart.rst` & `parmoo-0.2.1/docs/quickstart.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Dependencies
 ------------
 
 ParMOO has been tested on Unix/Linux and MacOS systems.
 
 ParMOO's base has the following dependencies:
 
- * Python_ 3.6+
+ * Python_ 3.8+
  * numpy_ -- for data structures and performant numerical linear algebra
  * scipy_ -- for scientific calculations needed for specific modules
  * pyDOE_ -- for generating experimental designs
  * pandas_ -- for exporting the resulting databases
 
 Additional dependencies are needed to use the additional features in
 ``parmoo.extras``:
```

### Comparing `parmoo-0.2.0/docs/refs.rst` & `parmoo-0.2.1/docs/refs.rst`

 * *Files 15% similar despite different names*

```diff
@@ -22,31 +22,34 @@
 
 Please use one of the following to cite ParMOO.
 
 Our JOSS paper:
 
 .. code-block:: bibtex
 
-    @article{parmoo-joss,
-        title       = {{ParMOO}: A {P}ython library for parallel multiobjective simulation optimization},
-        author      = {Chang, Tyler H. and Wild, Stefan M.},
-        year        = {2023},
-        journal     = {To appear in The Journal of Open Source Software}
+    @article{parmoo,
+        author={Chang, Tyler H. and Wild, Stefan M.},
+        title={{ParMOO}: A {P}ython library for parallel multiobjective simulation optimization},
+        year={2023},
+        journal = {Journal of Open Source Software},
+        volume = {8},
+        number = {82},
+        pages = {4468},
+        doi = {10.21105/joss.04468}
     }
 
 Our online documentation:
 
 .. code-block:: bibtex
 
     @techreport{parmoo-docs,
         title       = {{ParMOO}: {P}ython library for parallel multiobjective simulation optimization},
         author      = {Chang, Tyler H. and Wild, Stefan M. and Dickinson, Hyrum},
         institution = {Argonne National Laboratory},
-        number      = {Version 0.2.0},
+        number      = {Version 0.2.1},
         year        = {2023},
         url         = {https://parmoo.readthedocs.io/en/latest}
     }
 
-
 .. _CONTRIBUTING: https://github.com/parmoo/parmoo/blob/main/CONTRIBUTING.rst
 .. _LICENSE: https://github.com/parmoo/parmoo/blob/main/LICENSE
 .. _ReadTheDocs: https://parmoo.readthedocs.org
```

### Comparing `parmoo-0.2.0/docs/tutorials/basic-tutorials.rst` & `parmoo-0.2.1/docs/tutorials/basic-tutorials.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/docs/tutorials/libe-tutorial.rst` & `parmoo-0.2.1/docs/tutorials/libe-tutorial.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/Makefile` & `parmoo-0.2.1/examples/Makefile`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/advanced_ex.out` & `parmoo-0.2.1/examples/advanced_ex.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/advanced_ex.py` & `parmoo-0.2.1/examples/advanced_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/checkpointing.out` & `parmoo-0.2.1/examples/checkpointing.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/checkpointing.py` & `parmoo-0.2.1/examples/checkpointing.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/libe_basic_ex.py` & `parmoo-0.2.1/examples/libe_basic_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/named_var_ex.py` & `parmoo-0.2.1/examples/named_var_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/precomputed_data.py` & `parmoo-0.2.1/examples/precomputed_data.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/quickstart.py` & `parmoo-0.2.1/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/unnamed_var_ex.out` & `parmoo-0.2.1/examples/unnamed_var_ex.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/examples/unnamed_var_ex.py` & `parmoo-0.2.1/examples/unnamed_var_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/acquisitions/epsilon_constraint.py` & `parmoo-0.2.1/parmoo/acquisitions/epsilon_constraint.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/acquisitions/weighted_sum.py` & `parmoo-0.2.1/parmoo/acquisitions/weighted_sum.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/constraints/const_func.py` & `parmoo-0.2.1/parmoo/constraints/const_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/constraints/const_lib.py` & `parmoo-0.2.1/parmoo/constraints/const_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/extras/libe.py` & `parmoo-0.2.1/parmoo/extras/libe.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/moop.py` & `parmoo-0.2.1/parmoo/moop.py`

 * *Files 0% similar despite different names*

```diff
@@ -816,16 +816,16 @@
                                              self.n_raw):
                         self.des_order[i] += 1
                 self.des_order.append(self.n_cont + self.n_int +
                                       self.n_cat + self.n_custom + self.n_raw)
                 self.n_raw += 1
                 self.des_tols.append(1.0e-8)
             else:
-                raise(ValueError("des_type=" + arg['des_type'] +
-                                 " is not a recognized value"))
+                raise ValueError("des_type=" + arg['des_type'] +
+                                 " is not a recognized value")
         # Set the effective design dimension
         self.n = (self.n_cat_d + self.n_cont + self.n_int +
                   sum(self.n_custom_d) + self.n_raw)
         # Set the problem scaling
         self.scaled_lb = np.zeros(self.n)
         self.scaled_ub = np.ones(self.n)
         self.scale = np.ones(self.n)
```

### Comparing `parmoo-0.2.0/parmoo/objectives/dtlz.py` & `parmoo-0.2.1/parmoo/objectives/dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/objectives/obj_func.py` & `parmoo-0.2.1/parmoo/objectives/obj_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/objectives/obj_lib.py` & `parmoo-0.2.1/parmoo/objectives/obj_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/optimizers/gps_search.py` & `parmoo-0.2.1/parmoo/optimizers/gps_search.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/optimizers/lbfgsb.py` & `parmoo-0.2.1/parmoo/optimizers/lbfgsb.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/optimizers/random_search.py` & `parmoo-0.2.1/parmoo/optimizers/random_search.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/searches/latin_hypercube.py` & `parmoo-0.2.1/parmoo/searches/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/simulations/dtlz.py` & `parmoo-0.2.1/parmoo/simulations/dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/simulations/sim_func.py` & `parmoo-0.2.1/parmoo/simulations/sim_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/structs.py` & `parmoo-0.2.1/parmoo/structs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/surrogates/gaussian_proc.py` & `parmoo-0.2.1/parmoo/surrogates/gaussian_proc.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     This class implements a RBF surrogate with a Gaussian basis, using the
     SurrogateFunction ABC.
 
     """
 
     # Slots for the UniformRandom class
     __slots__ = ['m', 'n', 'lb', 'ub', 'x_vals', 'f_vals', 'eps', 'std_dev',
-                 'nugget', 'weights']
+                 'nugget', 'weights', 'mean']
 
     def __init__(self, m, lb, ub, hyperparams):
         """ Constructor for the GaussRBF class.
 
         Args:
             m (int): The number of objectives to fit.
 
@@ -57,14 +57,15 @@
         # Check inputs
         xerror(o=m, lb=lb, ub=ub, hyperparams=hyperparams)
         # Initialize problem dimensions
         self.m = m
         self.lb = lb
         self.ub = ub
         self.n = self.lb.size
+        self.mean = np.zeros(self.m)
         self.std_dev = 0.0
         # Create empty database
         self.x_vals = np.zeros((0, self.n))
         self.f_vals = np.zeros((0, self.m))
         self.weights = np.zeros((0, 0))
         # Check for the 'nugget' optional value in hyperparams
         if 'nugget' in hyperparams:
@@ -145,18 +146,23 @@
         w, v = np.linalg.eigh(cov)
         # Check the smallest singular value for a bad solution
         sigma_n = np.min(w)
         if sigma_n < 0.00000001:
             for i in range(self.x_vals.shape[0]):
                 cov[i, i] = cov[i, i] + 0.00000001 - sigma_n
             w, v = np.linalg.eigh(cov)
+        # Calculate RHS
+        rhs = self.f_vals.copy()
+        self.mean[:] = np.sum(rhs, axis=0) / rhs.shape[0]
+        for i in range(rhs.shape[0]):
+            rhs[i, :] = rhs[i, :] - self.mean[:]
         # Finish the solve
-        self.weights = np.zeros((self.m, self.f_vals.shape[0]))
+        self.weights = np.zeros((self.m, rhs.shape[0]))
         for i in range(self.m):
-            tmp = np.dot(v.transpose(), self.f_vals[:, i]) / w[:]
+            tmp = np.dot(v.transpose(), rhs[:, i]) / w[:]
             self.weights[i, :] = np.dot(v, tmp)
         return
 
     def update(self, x, f):
         """ Update an existing Gaussian RBF using new data.
 
         Args:
@@ -201,18 +207,23 @@
         w, v = np.linalg.eigh(cov)
         # Check the smallest singular value for a bad solution
         sigma_n = np.min(w)
         if sigma_n < 0.00000001:
             for i in range(self.x_vals.shape[0]):
                 cov[i, i] = cov[i, i] + 0.00000001 - sigma_n
             w, v = np.linalg.eigh(cov)
+        # Calculate RHS
+        rhs = self.f_vals.copy()
+        self.mean[:] = np.sum(rhs, axis=0) / rhs.shape[0]
+        for i in range(rhs.shape[0]):
+            rhs[i, :] = rhs[i, :] - self.mean[:]
         # Finish the solve
-        self.weights = np.zeros((self.m, self.f_vals.shape[0]))
+        self.weights = np.zeros((self.m, rhs.shape[0]))
         for i in range(self.m):
-            tmp = np.dot(v.transpose(), self.f_vals[:, i]) / w[:]
+            tmp = np.dot(v.transpose(), rhs[:, i]) / w[:]
             self.weights[i, :] = np.dot(v, tmp)
         return
 
     def setCenter(self, center):
         """ This is a dummy subroutine, that does nothing for this class.
 
         Returns:
@@ -243,15 +254,15 @@
             if x.size != self.n:
                 raise ValueError("x must have length n")
             elif (np.any(x < self.lb - self.eps) or
                   np.any(x > self.ub + self.eps)):
                 raise ValueError("x cannot be infeasible")
         # Evaluate all m surrogates at x
         dists = self.__gaussian(cdist(self.x_vals, [x])).flatten()
-        return np.dot(self.weights, dists)
+        return np.dot(self.weights, dists) + self.mean[:]
 
     def gradient(self, x):
         """ Evaluate the gradients of the Gaussian RBF at a design point.
 
         Args:
             x (numpy.ndarray): A 1d array containing the design point at
                 which the gradient of the RBF should be evaluated.
@@ -366,14 +377,15 @@
         # Serialize numpy.ndarray objects
         gp_state['lb'] = self.lb.tolist()
         gp_state['ub'] = self.ub.tolist()
         gp_state['x_vals'] = self.x_vals.tolist()
         gp_state['f_vals'] = self.f_vals.tolist()
         gp_state['eps'] = self.eps.tolist()
         gp_state['weights'] = self.weights.tolist()
+        gp_state['mean'] = self.mean.tolist()
         # Save file
         with open(filename, 'w') as fp:
             json.dump(gp_state, fp)
         return
 
     def load(self, filename):
         """ Reload important data into this class after a previous save.
@@ -397,28 +409,30 @@
         # Deserialize numpy.ndarray objects
         self.lb = np.array(gp_state['lb'])
         self.ub = np.array(gp_state['ub'])
         self.x_vals = np.array(gp_state['x_vals'])
         self.f_vals = np.array(gp_state['f_vals'])
         self.eps = np.array(gp_state['eps'])
         self.weights = np.array(gp_state['weights'])
+        self.mean = np.array(gp_state['mean'])
         return
 
 
 class LocalGaussRBF(SurrogateFunction):
     """ A local RBF surrogate model, using a Gaussian basis.
 
     This class implements a local RBF surrogate with a Gaussian basis,
     using the SurrogateFunction ABC.
 
     """
 
     # Slots for the UniformRandom class
     __slots__ = ['m', 'n', 'lb', 'ub', 'x_vals', 'f_vals', 'eps', 'std_dev',
-                 'nugget', 'n_loc', 'loc_inds', 'tr_center', 'weights']
+                 'nugget', 'n_loc', 'loc_inds', 'tr_center', 'weights',
+                 'mean']
 
     def __init__(self, m, lb, ub, hyperparams):
         """ Constructor for the LocalGaussRBF class.
 
         Args:
             m (int): The number of objectives to fit.
 
@@ -449,14 +463,15 @@
         self.ub = ub
         self.n = self.lb.size
         self.std_dev = 0.0
         # Create empty database
         self.x_vals = np.zeros((0, self.n))
         self.f_vals = np.zeros((0, self.m))
         self.weights = np.zeros((0, 0))
+        self.mean = np.zeros(self.m)
         # Initialize trust-region settings
         self.tr_center = np.zeros(0)
         self.loc_inds = []
         # Check for the 'nugget' optional value in hyperparams
         if 'nugget' in hyperparams:
             if isinstance(hyperparams['nugget'], float):
                 self.nugget = hyperparams['nugget']
@@ -614,19 +629,23 @@
             w, v = np.linalg.eigh(cov)
             # Check the smallest singular value for a bad solution
             sigma_n = np.min(w)
             if sigma_n < 0.00000001:
                 for i in range(len(self.loc_inds)):
                     cov[i, i] = cov[i, i] + 0.00000001 - sigma_n
                 w, v = np.linalg.eigh(cov)
+            # Calculate RHS
+            rhs = self.f_vals[self.loc_inds, :].copy()
+            self.mean[:] = np.sum(rhs, axis=0) / rhs.shape[0]
+            for i in range(rhs.shape[0]):
+                rhs[i, :] = rhs[i, :] - self.mean[:]
             # Finish the solve
-            self.weights = np.zeros((self.m, len(self.loc_inds)))
+            self.weights = np.zeros((self.m, rhs.shape[0]))
             for i in range(self.m):
-                tmp = np.dot(v.transpose(),
-                             self.f_vals[self.loc_inds, i]) / w[:]
+                tmp = np.dot(v.transpose(), rhs[:, i]) / w[:]
                 self.weights[i, :] = np.dot(v, tmp)
         return self.std_dev
 
     def evaluate(self, x):
         """ Evaluate the Gaussian RBF at a design point.
 
         Args:
@@ -647,15 +666,15 @@
                 raise ValueError("x must have length n")
             elif (np.any(x < self.lb - self.eps) or
                   np.any(x > self.ub + self.eps)):
                 raise ValueError("x cannot be infeasible")
         # Evaluate all m surrogates at x
         dists = self.__gaussian(cdist(self.x_vals[self.loc_inds],
                                       [x])).flatten()
-        return np.dot(self.weights, dists)
+        return np.dot(self.weights, dists) + self.mean[:]
 
     def gradient(self, x):
         """ Evaluate the gradients of the Gaussian RBF at a design point.
 
         Args:
             x (numpy.ndarray): A 1d array containing the design point at
                 which the gradient of the RBF should be evaluated.
@@ -774,14 +793,15 @@
         gp_state['lb'] = self.lb.tolist()
         gp_state['ub'] = self.ub.tolist()
         gp_state['x_vals'] = self.x_vals.tolist()
         gp_state['f_vals'] = self.f_vals.tolist()
         gp_state['eps'] = self.eps.tolist()
         gp_state['tr_center'] = self.tr_center.tolist()
         gp_state['weights'] = self.weights.tolist()
+        gp_state['mean'] = self.mean.tolist()
         # Save file
         with open(filename, 'w') as fp:
             json.dump(gp_state, fp)
         return
 
     def load(self, filename):
         """ Reload important data into this class after a previous save.
@@ -808,8 +828,9 @@
         self.lb = np.array(gp_state['lb'])
         self.ub = np.array(gp_state['ub'])
         self.x_vals = np.array(gp_state['x_vals'])
         self.f_vals = np.array(gp_state['f_vals'])
         self.eps = np.array(gp_state['eps'])
         self.tr_center = np.array(gp_state['tr_center'])
         self.weights = np.array(gp_state['weights'])
+        self.mean = np.array(gp_state['mean'])
         return
```

### Comparing `parmoo-0.2.0/parmoo/tests/.pytest_cache/v/cache/nodeids` & `parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/libe_tests/libe_funcs.py` & `parmoo-0.2.1/parmoo/tests/libe_tests/libe_funcs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/libe_tests/test_libe_gen.py` & `parmoo-0.2.1/parmoo/tests/libe_tests/test_libe_gen.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz1_obj.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz1_sim.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz2_obj.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz2_sim.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz3_obj.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz3_sim.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_dtlz5_sim.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz5_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_infeasible_prob.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_infeasible_prob.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_mixed_variables.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_mixed_variables.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/regression_tests/test_user_func.py` & `parmoo-0.2.1/parmoo/tests/regression_tests/test_user_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/run-tests.sh` & `parmoo-0.2.1/parmoo/tests/run-tests.sh`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 fi;
 
 # Run unit tests
 if [ $UNIT_TESTS == true ]; then
   echo
   echo "Running unit tests with pytest and collecting coverage data..."
   echo
-  pytest -v --cov-config=parmoo/tests/.coveragerc --cov=parmoo --cov-report= parmoo/tests/unit_tests -W error::UserWarning;
+  python3 -m pytest -v --cov-config=parmoo/tests/.coveragerc --cov=parmoo --cov-report= parmoo/tests/unit_tests -W error::UserWarning;
 
   code=$? # capture pytest exit code
   if [ "$code" -eq "0" ]; then
     echo
     echo "Unit tests passed. Continuing..."
     echo
   else
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_const_lib.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_const_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
     from parmoo.constraints import single_sim_bound
     import numpy as np
 
     # Create the constraint function
     const_func = single_sim_bound(3, 3, 0, type='upper')
     # Test function evaluation
-    assert(const_func(np.zeros(3), np.eye(3)[0] * 1.5) == 1.5)
+    assert (const_func(np.zeros(3), np.eye(3)[0] * 1.5) == 1.5)
     # Test dx evaluation
-    assert(np.all(const_func(np.zeros(3), np.ones(3) * 4.0, der=1) ==
-                  np.zeros(3)))
+    assert (np.all(const_func(np.zeros(3), np.ones(3) * 4.0, der=1) ==
+                   np.zeros(3)))
     # Test ds evaluation
-    assert(np.all(const_func(np.zeros(3), np.ones(3) * 3.0, der=2) ==
-                  np.eye(3)[0]))
+    assert (np.all(const_func(np.zeros(3), np.ones(3) * 3.0, der=2) ==
+                   np.eye(3)[0]))
 
 
 def test_single_sim_bound_named1():
     """ Test the single_sim_bound() constraint function.
 
     Initialize a named constraint, then evaluate the function value and
     derivative with respect to x and sx.
@@ -38,21 +38,21 @@
     # Create input vectors
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     sx['sim1'] = 2.0
     # Create the constraint function
     const_func = single_sim_bound(xtype, stype, 'sim1', type='lower')
     # Test function evaluation
-    assert(const_func(x, sx) == -2.0)
+    assert (const_func(x, sx) == -2.0)
     # Test dx evaluation
-    assert(np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_bound = np.zeros(1, dtype=stype)[0]
     s_bound['sim1'] = -1.0
-    assert(np.all(const_func(x, sx, der=2) == s_bound))
+    assert (np.all(const_func(x, sx, der=2) == s_bound))
 
 
 def test_single_sim_bound_named2():
     """ Test the single_sim_bound() constraint function.
 
     Initialize a named constraint, then evaluate the function value and
     derivative with respect to x and sx.
@@ -71,21 +71,21 @@
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     sx['sim2'][0] = 1.0
     sx['sim2'][1] = 2.0
     # Create the constraint function
     const_func = single_sim_bound(xtype, stype, ('sim2', 1), type='upper')
     # Test function evaluation
-    assert(const_func(x, sx) == 2.0)
+    assert (const_func(x, sx) == 2.0)
     # Test dx evaluation
-    assert(np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_bound = np.zeros(1, dtype=stype)[0]
     s_bound['sim2'][1] = 1.0
-    assert(np.all(const_func(x, sx, der=2) == s_bound))
+    assert (np.all(const_func(x, sx, der=2) == s_bound))
 
 
 def test_sos_sim_bound_unnamed():
     """ Test the sos_sim_bound() constraint function.
 
     Initialize an unnamed constraint, then evaluate the function value and
     derivative with respect to x and sx.
@@ -94,23 +94,23 @@
 
     from parmoo.constraints import sos_sim_bound
     import numpy as np
 
     # Create the constraint function
     const_func = sos_sim_bound(5, 5, [0, 1, 2, 3], type='upper')
     # Test function evaluation
-    assert(np.abs(const_func(np.zeros(5), np.ones(5) * 2.0) - 16.0) < 1.0e-8)
+    assert (np.abs(const_func(np.zeros(5), np.ones(5) * 2.0) - 16.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(const_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
-                  np.zeros(5)))
+    assert (np.all(const_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
+                   np.zeros(5)))
     # Test ds evaluation
     s_bound = np.ones(5) * 4.0
     s_bound[4] = 0.0
-    assert(np.all(np.abs(const_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
-                         s_bound) < 1.0e-8))
+    assert (np.all(np.abs(const_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
+                          s_bound) < 1.0e-8))
 
 
 def test_sos_sim_bound_named():
     """ Test the sos_sim_bound() constraint function.
 
     Initialize a named constraint, then evaluate the function value and
     derivative with respect to x and sx.
@@ -129,24 +129,25 @@
     sx['sim1'] = 2.0
     sx['sim2'][:] = 2.0
     # Create the constraint function
     const_func = sos_sim_bound(xtype, stype,
                                ['sim1', ('sim2', 0), ('sim2', 1), ('sim2', 2)],
                                type='lower')
     # Test function evaluation
-    assert(np.abs(const_func(x, sx) + 16.0) < 1.0e-8)
+    assert (np.abs(const_func(x, sx) + 16.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_bound = np.zeros(1, dtype=stype)[0]
     s_bound['sim1'] = sx['sim1'] * -2.0
     s_bound['sim2'][:-1] = sx['sim2'][:-1] * -2.0
-    assert(np.abs(const_func(x, sx, der=2)['sim1'] - s_bound['sim1']) < 1.0e-8)
-    assert(np.all(np.abs(const_func(x, sx, der=2)['sim2'] - s_bound['sim2'])
-                  < 1.0e-8))
+    assert (np.abs(const_func(x, sx, der=2)['sim1'] - s_bound['sim1'])
+            < 1.0e-8)
+    assert (np.all(np.abs(const_func(x, sx, der=2)['sim2'] - s_bound['sim2'])
+                   < 1.0e-8))
 
 
 def test_sum_sim_bound_unnamed():
     """ Test the sum_sim_bound() constraint function.
 
     Initialize an unnamed constraint, then evaluate the function value and
     derivative with respect to x and sx.
@@ -155,21 +156,21 @@
 
     from parmoo.constraints import sum_sim_bound
     import numpy as np
 
     # Create the constraint function
     const_func = sum_sim_bound(5, 5, [0, 1, 2, 3], type='upper')
     # Test function evaluation
-    assert(np.abs(const_func(np.zeros(5), np.ones(5) * 2.0) - 8.0) < 1.0e-8)
+    assert (np.abs(const_func(np.zeros(5), np.ones(5) * 2.0) - 8.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(const_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
-                  np.zeros(5)))
+    assert (np.all(const_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
+                   np.zeros(5)))
     # Test ds evaluation
-    assert(np.all(np.abs(const_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
-                         (np.ones(5) - np.eye(5)[4])) < 1.0e-8))
+    assert (np.all(np.abs(const_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
+                          (np.ones(5) - np.eye(5)[4])) < 1.0e-8))
 
 
 def test_sum_sim_bound_named():
     """ Test the sum_sim_bound() constraint function.
 
     Initialize a named constraint, then evaluate the function value and
     derivative with respect to x and sx.
@@ -188,29 +189,30 @@
     sx['sim1'] = 2.0
     sx['sim2'][:] = 2.0
     # Create the constraint function
     const_func = sum_sim_bound(xtype, stype,
                                ['sim1', ('sim2', 0), ('sim2', 1), ('sim2', 2)],
                                type='lower')
     # Test function evaluation
-    assert(np.abs(const_func(x, sx) + 8.0) < 1.0e-8)
+    assert (np.abs(const_func(x, sx) + 8.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_bound = np.ones(1, dtype=stype)[0]
     s_bound['sim1'] *= -1.0
     s_bound['sim2'][:] *= -1.0
     s_bound['sim2'][3] = 0.0
-    assert(np.abs(const_func(x, sx, der=2)['sim1'] - s_bound['sim1']) < 1.0e-8)
-    assert(np.all(np.abs(const_func(x, sx, der=2)['sim2'] - s_bound['sim2'])
-                  < 1.0e-8))
+    assert (np.abs(const_func(x, sx, der=2)['sim1'] - s_bound['sim1'])
+            < 1.0e-8)
+    assert (np.all(np.abs(const_func(x, sx, der=2)['sim2'] - s_bound['sim2'])
+                   < 1.0e-8))
 
 
 def test_sum_sim_bound_named_abs():
-    """ Test the sum_sim_bound() constraint function with "absolute=True" option.
+    """ Test the sum_sim_bound() constraint with "absolute=True" option.
 
     Initialize a named constraint, then evaluate the function value and
     derivative with respect to x and sx.
 
     """
 
     from parmoo.constraints import sum_sim_bound
@@ -225,24 +227,25 @@
     sx['sim1'] = 2.0
     sx['sim2'][:] = -2.0
     # Create the constraint function
     const_func = sum_sim_bound(xtype, stype,
                                ['sim1', ('sim2', 0), ('sim2', 1), ('sim2', 2)],
                                type='upper', absolute=True)
     # Test function evaluation
-    assert(np.abs(const_func(x, sx) - 8.0) < 1.0e-8)
+    assert (np.abs(const_func(x, sx) - 8.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(const_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_bound = np.zeros(1, dtype=stype)[0]
     s_bound['sim1'] = 1.0
     s_bound['sim2'][:-1] = -1.0
-    assert(np.abs(const_func(x, sx, der=2)['sim1'] - s_bound['sim1']) < 1.0e-8)
-    assert(np.all(np.abs(const_func(x, sx, der=2)['sim2'] - s_bound['sim2'])
-                  < 1.0e-8))
+    assert (np.abs(const_func(x, sx, der=2)['sim1'] - s_bound['sim1'])
+            < 1.0e-8)
+    assert (np.all(np.abs(const_func(x, sx, der=2)['sim2'] - s_bound['sim2'])
+                   < 1.0e-8))
 
 
 if __name__ == "__main__":
     test_single_sim_bound_unnamed()
     test_single_sim_bound_named1()
     test_single_sim_bound_named2()
     test_sos_sim_bound_unnamed()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_epsilon_constraint.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_epsilon_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,50 +45,50 @@
         acqu.setTarget(data, lambda x, y: np.zeros(0), {})
     with pytest.raises(ValueError):
         acqu.setTarget({}, lambda x: np.ones(1), {})
     with pytest.raises(ValueError):
         acqu.setTarget(data, lambda x: np.ones(1), {})
     data['c_vals'] = np.zeros((10, 1))
     # Set a few good target
-    assert(np.all(acqu.setTarget({}, lambda x: np.zeros(3), {}) < 1.0))
-    assert(np.all(acqu.setTarget({}, lambda x: np.zeros(3), {}) > 0.0))
-    assert(np.all(acqu.setTarget({'x_vals': np.zeros((1, 3)),
-                                  'f_vals': np.zeros((1, 3)),
-                                  'c_vals': np.zeros((1, 1))},
-                                 lambda x: np.ones(3) * (0.01 - sum(x)),
-                                 {}) < 1.0))
-    assert(acqu.setTarget(data, lambda x: np.zeros(3), {}) in data['x_vals'])
+    assert (np.all(acqu.setTarget({}, lambda x: np.zeros(3), {}) < 1.0))
+    assert (np.all(acqu.setTarget({}, lambda x: np.zeros(3), {}) > 0.0))
+    assert (np.all(acqu.setTarget({'x_vals': np.zeros((1, 3)),
+                                   'f_vals': np.zeros((1, 3)),
+                                   'c_vals': np.zeros((1, 1))},
+                                  lambda x: np.ones(3) * (0.01 - sum(x)),
+                                  {}) < 1.0))
+    assert (acqu.setTarget(data, lambda x: np.zeros(3), {}) in data['x_vals'])
     # Try some bad scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarize(5)
     with pytest.raises(ValueError):
         acqu.scalarize(np.ones(2))
     # Generate a random scalarization target and check the scalarization
     acqu = RandomConstraint(3, np.zeros(3), np.ones(3), {})
     acqu.setTarget({'x_vals': None, 'f_vals': None},
                    lambda x: np.zeros(3), {})
     acqu.setTarget(data, lambda x: np.zeros(3), {})
     # Get a copy of the Pareto front for checking correctness
     pf = updatePF(data, {})
     # Check that the scalar value is either less than the sum of fi or bad
     for fi in pf['f_vals']:
-        assert(acqu.scalarize(fi) <= np.sum(fi) or
-               np.any(fi > acqu.f_ub))
+        assert (acqu.scalarize(fi) <= np.sum(fi) or
+                np.any(fi > acqu.f_ub))
     # Try some bad gradient scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(5, np.zeros((3, 4))[0])
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.ones(2), np.zeros((3, 4)))
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(np.eye(3)[0], 5)
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.eye(3)[0], np.zeros((2, 4)))
     # Check that the scalar grad is either less than the sum of fi or bad
     for fi in pf['f_vals']:
         gi = np.random.random_sample((3, 3))
-        assert(all(acqu.scalarizeGrad(fi, gi) <= np.sum(gi, axis=0)) or
-               np.any(fi > acqu.f_ub))
+        assert (all(acqu.scalarizeGrad(fi, gi) <= np.sum(gi, axis=0)) or
+                np.any(fi > acqu.f_ub))
     return
 
 
 if __name__ == "__main__":
     test_RandomConstraint()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_gaussian_proc.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_gaussian_proc.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,57 +79,57 @@
         rbf1.improve(5, False)
     with pytest.raises(ValueError):
         rbf1.improve(np.zeros(2), False)
     with pytest.raises(ValueError):
         rbf1.improve(-np.ones(3), False)
     # Check that the RBFs match on a random evaluation point
     x = np.random.random_sample((3))
-    assert(all(rbf1.evaluate(x) == rbf2.evaluate(x)))
+    assert (all(rbf1.evaluate(x) == rbf2.evaluate(x)))
     # Check that the RBFs interpolate, up to 8 decimal digits of precision
     for i in range(x_vals_full.shape[0]):
-        assert(np.linalg.norm(rbf1.evaluate(x_vals_full[i])-y_vals_full[i])
-               < 0.00000001)
-        assert(np.linalg.norm(rbf2.evaluate(x_vals_full[i])-y_vals_full[i])
-               < 0.00000001)
+        assert (np.linalg.norm(rbf1.evaluate(x_vals_full[i])-y_vals_full[i])
+                < 0.00000001)
+        assert (np.linalg.norm(rbf2.evaluate(x_vals_full[i])-y_vals_full[i])
+                < 0.00000001)
     # Check that the RBFs compute the same grad, up to 8 digits of precision
     for i in range(x_vals_full.shape[0]):
-        assert(np.linalg.norm(rbf1.gradient(x_vals_full[i]) -
-                              rbf2.gradient(x_vals_full[i])) < 0.00000001)
+        assert (np.linalg.norm(rbf1.gradient(x_vals_full[i]) -
+                               rbf2.gradient(x_vals_full[i])) < 0.00000001)
     # Check that the RBF gradient evaluates correctly on a known dataset
     x_vals3 = np.eye(3)
     x_vals3 = np.append(x_vals3, [[0.5, 0.5, 0.5]], axis=0)
     y_vals3 = np.asarray([[np.dot(xi, xi)] for xi in x_vals3])
     rbf3 = GaussRBF(1, np.zeros(3), np.ones(3), {})
     rbf3.fit(x_vals3, y_vals3)
     rbf3.setCenter(np.zeros(3))
-    y_grad_vals3 = -0.357428774951389 * np.ones((1, 3))
-    assert(np.linalg.norm(rbf3.gradient(x_vals3[-1]) - y_grad_vals3[-1])
-           < 0.00000001)
+    y_grad_vals3 = -0.03661401 * np.ones((1, 3))
+    assert (np.linalg.norm(rbf3.gradient(x_vals3[-1]) - y_grad_vals3[-1])
+            < 1.0e-4)
     # Check that the RBF generates feasible local improvement points
     for i in range(4):
         x_improv = rbf3.improve(np.zeros(3), False)
-        assert(np.all(x_improv[0] <= np.ones(3)) and
-               np.all(x_improv[0] >= np.zeros(3)))
+        assert (np.all(x_improv[0] <= np.ones(3)) and
+                np.all(x_improv[0] >= np.zeros(3)))
     # Check that the RBF generates feasible global improvement points
     x_improv = rbf3.improve(x_vals3[-1], True)
-    assert(np.all(x_improv[0] <= np.ones(3)) and
-           np.all(x_improv[0] >= np.zeros(3)))
+    assert (np.all(x_improv[0] <= np.ones(3)) and
+            np.all(x_improv[0] >= np.zeros(3)))
     # Check that RBF generates good improvements when points are bunched
     x_new = np.ones((3, 3))
     x_new = x_new * 0.5
     f_new = np.zeros((3, 1))
     for i in range(3):
         x_new[i, i] = 0.50000001
         f_new[i, 0] = np.dot(x_new[i, :], x_new[i, :])
     rbf3.update(x_new, f_new)
     x_improv = rbf3.improve(np.asarray([0.5, 0.5, 0.5]), False)
-    assert(np.all(x_improv[0] <= np.ones(3)) and
-           np.all(x_improv[0] >= np.zeros(3)))
-    assert(np.all(np.linalg.norm(x_improv[0] - np.asarray([0.5, 0.5, 0.5]))
-           > 0.00000001))
+    assert (np.all(x_improv[0] <= np.ones(3)) and
+            np.all(x_improv[0] >= np.zeros(3)))
+    assert (np.all(np.linalg.norm(x_improv[0] - np.asarray([0.5, 0.5, 0.5]))
+            > 0.00000001))
     # Now fit redundant data points using a nugget
     x_vals1 = np.append(x_vals1, np.asarray([x_vals1[0, :]]), axis=0)
     y_vals1 = np.append(y_vals1, np.asarray([y_vals1[0, :]]), axis=0)
     rbf4 = GaussRBF(2, np.zeros(3), np.ones(3), {'nugget': 0.0001})
     rbf4.fit(x_vals1, y_vals1)
     rbf4.update(x_vals2, y_vals2)
     # Now create a really tiny design space with a large tolerance
@@ -137,18 +137,18 @@
                     {'des_tols': 0.3 * np.ones(1)})
     xdat5 = np.asarray([[0.4], [0.6]])
     ydat5 = np.asarray([[0.4], [0.6]])
     rbf5.fit(xdat5, ydat5)
     # Test that improve() is able to find points outside the design tolerance
     for i in range(5):
         x_improv = rbf5.improve(xdat5[0], False)
-        assert(x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
+        assert (x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
     for i in range(5):
         x_improv = rbf5.improve(xdat5[0], True)
-        assert(x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
+        assert (x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
     # Now fit redundant data points without a nugget
     rbf6 = GaussRBF(2, np.zeros(3), np.ones(3), {})
     rbf6.fit(x_vals1, y_vals1)
     rbf6.update(x_vals2, y_vals2)
     # Now fit datapoints in a plane
     x_vals3 = np.zeros((4, 3))
     x_vals3[1, 0] = 0.1
@@ -158,15 +158,15 @@
     rbf7 = GaussRBF(2, np.zeros(3), np.ones(3), {})
     rbf7.fit(x_vals3, y_vals3)
     rbf7.update(x_vals3, y_vals3)
     # Test save and load
     rbf6.save("parmoo.surrogate")
     rbf7.load("parmoo.surrogate")
     xx = np.random.random_sample(3)
-    assert(np.all(rbf6.evaluate(xx) == rbf7.evaluate(xx)))
+    assert (np.all(rbf6.evaluate(xx) == rbf7.evaluate(xx)))
     os.remove("parmoo.surrogate")
     return
 
 
 def test_LocalGaussRBF():
     """ Test the LocalGaussRBF class in surrogates.py.
 
@@ -260,62 +260,62 @@
         rbf1.improve(5, False)
     with pytest.raises(ValueError):
         rbf1.improve(np.zeros(2), False)
     with pytest.raises(ValueError):
         rbf1.improve(-np.ones(3), False)
     # Check that the RBFs match on a random evaluation point
     x = np.random.random_sample((3))
-    assert(all(rbf1.evaluate(x) == rbf2.evaluate(x)))
+    assert (all(rbf1.evaluate(x) == rbf2.evaluate(x)))
     # Check that the RBFs interpolate, up to 8 decimal digits of precision
     for i in range(x_vals_full.shape[0]):
         rbf1.setCenter(x_vals_full[i])
         rbf2.setCenter(x_vals_full[i])
-        assert(np.linalg.norm(rbf1.evaluate(x_vals_full[i])-y_vals_full[i])
-               < 0.00000001)
-        assert(np.linalg.norm(rbf2.evaluate(x_vals_full[i])-y_vals_full[i])
-               < 0.00000001)
+        assert (np.linalg.norm(rbf1.evaluate(x_vals_full[i])-y_vals_full[i])
+                < 0.00000001)
+        assert (np.linalg.norm(rbf2.evaluate(x_vals_full[i])-y_vals_full[i])
+                < 0.00000001)
     # Check that the RBFs compute the same grad, up to 8 digits of precision
     rbf1.setCenter(0.5 * np.ones(3))
     rbf2.setCenter(0.5 * np.ones(3))
     for i in range(x_vals_full.shape[0]):
-        assert(np.linalg.norm(rbf1.gradient(x_vals_full[i]) -
-                              rbf2.gradient(x_vals_full[i])) < 0.00000001)
+        assert (np.linalg.norm(rbf1.gradient(x_vals_full[i]) -
+                               rbf2.gradient(x_vals_full[i])) < 0.00000001)
     # Check that the RBF gradient evaluates correctly on a known dataset
     x_vals3 = np.eye(3)
     x_vals3 = np.append(x_vals3, [[0.5, 0.5, 0.5]], axis=0)
     y_vals3 = np.asarray([[np.dot(xi, xi)] for xi in x_vals3])
     rbf3 = LocalGaussRBF(1, np.zeros(3), np.ones(3), {})
     rbf3.fit(x_vals3, y_vals3)
     rbf3.setCenter(x_vals3[-1])
-    y_grad_vals3 = -0.484569593266457 * np.ones((1, 3))
-    assert(np.linalg.norm(rbf3.gradient(x_vals3[-1]) - y_grad_vals3[-1])
-           < 0.00000001)
+    y_grad_vals3 = -0.08798618 * np.ones((1, 3))
+    assert (np.linalg.norm(rbf3.gradient(x_vals3[-1]) - y_grad_vals3[-1])
+            < 1.0e-4)
     # Check that the RBF generates feasible local improvement points
     for i in range(4):
         x_improv = rbf3.improve(np.zeros(3), False)
-        assert(np.all(x_improv[0] <= np.ones(3)) and
-               np.all(x_improv[0] >= np.zeros(3)))
+        assert (np.all(x_improv[0] <= np.ones(3)) and
+                np.all(x_improv[0] >= np.zeros(3)))
     # Check that the RBF generates feasible global improvement points
     x_improv = rbf3.improve(x_vals3[-1], True)
-    assert(np.all(x_improv[0] <= np.ones(3)) and
-           np.all(x_improv[0] >= np.zeros(3)))
+    assert (np.all(x_improv[0] <= np.ones(3)) and
+            np.all(x_improv[0] >= np.zeros(3)))
     # Check that RBF generates good improvements when points are bunched
     x_new = np.ones((3, 3))
     x_new = x_new * 0.5
     f_new = np.zeros((3, 1))
     for i in range(3):
         x_new[i, i] = 0.50000001
         f_new[i, 0] = np.dot(x_new[i, :], x_new[i, :])
     rbf3.update(x_new, f_new)
     rbf3.setCenter(0.5 * np.ones(3))
     x_improv = rbf3.improve(np.asarray([0.5, 0.5, 0.5]), False)
-    assert(np.all(x_improv[0] <= np.ones(3)) and
-           np.all(x_improv[0] >= np.zeros(3)))
-    assert(np.all(np.linalg.norm(x_improv[0] - np.asarray([0.5, 0.5, 0.5]))
-           > 0.00000001))
+    assert (np.all(x_improv[0] <= np.ones(3)) and
+            np.all(x_improv[0] >= np.zeros(3)))
+    assert (np.all(np.linalg.norm(x_improv[0] - np.asarray([0.5, 0.5, 0.5]))
+            > 0.00000001))
     # Now fit redundant data points using a nugget
     x_vals1 = np.append(x_vals1, np.asarray([x_vals1[0, :]]), axis=0)
     y_vals1 = np.append(y_vals1, np.asarray([y_vals1[0, :]]), axis=0)
     rbf4 = LocalGaussRBF(2, np.zeros(3), np.ones(3), {'nugget': 0.0001})
     rbf4.fit(x_vals1, y_vals1)
     rbf4.setCenter(x_vals1[0])
     rbf4.evaluate(x_vals1[0])
@@ -327,18 +327,18 @@
                          {'des_tols': 0.3 * np.ones(1)})
     xdat5 = np.asarray([[0.4], [0.6]])
     ydat5 = np.asarray([[0.4], [0.6]])
     rbf5.fit(xdat5, ydat5)
     # Test that improve() is able to find points outside the design tolerance
     for i in range(5):
         x_improv = rbf5.improve(xdat5[0], False)
-        assert(x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
+        assert (x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
     for i in range(5):
         x_improv = rbf5.improve(xdat5[0], True)
-        assert(x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
+        assert (x_improv[0][0] < 0.1 or x_improv[0][0] > 0.9)
     # Now fit redundant data points to test adaptive nugget
     rbf6 = LocalGaussRBF(2, np.zeros(3), np.ones(3), {})
     rbf6.fit(x_vals1, y_vals1)
     rbf6.update(x_vals2, y_vals2)
     rbf6.setCenter(x_vals1[0])
     # Now fit datapoints in a plane
     x_vals3 = np.zeros((4, 3))
@@ -349,15 +349,15 @@
     rbf7 = LocalGaussRBF(2, np.zeros(3), np.ones(3), {})
     rbf7.fit(x_vals3, y_vals3)
     rbf7.update(x_vals3, y_vals3)
     # Test save and load
     rbf6.save("parmoo.surrogate")
     rbf7.load("parmoo.surrogate")
     xx = np.random.random_sample(3)
-    assert(np.all(rbf6.evaluate(xx) == rbf7.evaluate(xx)))
+    assert (np.all(rbf6.evaluate(xx) == rbf7.evaluate(xx)))
     os.remove("parmoo.surrogate")
     return
 
 
 if __name__ == "__main__":
     test_GaussRBF()
     test_LocalGaussRBF()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_gps_search.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_gps_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,17 @@
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
     x2_soln = np.eye(n)[1]
     x2_soln[n-1] = 0.1
     # eps is the tolerance for rejecting a solution as incorrect
     eps = 0.01
     # Check that the computed solutions are within eps of the truth
-    assert(np.linalg.norm(x1 - x1_soln) < eps)
-    assert(np.linalg.norm(x2 - x2_soln) < eps)
-    assert(np.abs(x3[n-1] - 0.1) < eps)
+    assert (np.linalg.norm(x1 - x1_soln) < eps)
+    assert (np.linalg.norm(x2 - x2_soln) < eps)
+    assert (np.abs(x3[n-1] - 0.1) < eps)
     return
 
 
 def test_GlobalGPS():
     """ Test the GlobalGPS class in optimizers.py.
 
     Perform a test of the globalGPS class by minimizing the three variable,
@@ -197,16 +197,16 @@
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
     x2_soln = np.eye(n)[1]
     x2_soln[n-1] = 0.1
     # eps is the tolerance for rejecting a solution as incorrect
     eps = 0.01
     # Check that the computed solutions are within eps of the truth
-    assert(np.linalg.norm(x1 - x1_soln) < eps)
-    assert(np.linalg.norm(x2 - x2_soln) < eps)
-    assert(np.abs(x3[n-1] - 0.1) < eps)
+    assert (np.linalg.norm(x1 - x1_soln) < eps)
+    assert (np.linalg.norm(x2 - x2_soln) < eps)
+    assert (np.abs(x3[n-1] - 0.1) < eps)
     return
 
 
 if __name__ == "__main__":
     test_LocalGPS()
     test_GlobalGPS()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_latin_hypercube.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_latin_hypercube.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,25 @@
         LatinHypercube(2, lb, ub, {'search_budget': 2.0})
     with pytest.raises(ValueError):
         LatinHypercube(2, lb, ub, {'search_budget': -1})
     # Create a good LHS object
     latin_search = LatinHypercube(2, lb, ub, {'search_budget': 0})
     # Generate a design of size 0 and confirm that it is an empty array
     des1 = latin_search.startSearch(lb, ub)
-    assert(np.size(des1) == 0)
+    assert (np.size(des1) == 0)
     # Resume the search with size 0 and check that it is an empty array
     des2 = latin_search.resumeSearch()
-    assert(np.size(des2) == 0)
+    assert (np.size(des2) == 0)
     # Generate a new design and check that it conforms to the dimensions
     latin_search = LatinHypercube(2, lb, ub, {})
     des3 = latin_search.startSearch(lb, ub)
-    assert(np.shape(des3) == (100, 5))
-    assert(all([all(xi <= ub) and all(xi >= lb) for xi in des3]))
+    assert (np.shape(des3) == (100, 5))
+    assert (all([all(xi <= ub) and all(xi >= lb) for xi in des3]))
     # Resume the search and check that it conforms to the dimensions
     des4 = latin_search.resumeSearch()
-    assert(np.shape(des4) == (100, 5))
-    assert(all([all(xi <= ub) and all(xi >= lb) for xi in des4]))
+    assert (np.shape(des4) == (100, 5))
+    assert (all([all(xi <= ub) and all(xi >= lb) for xi in des4]))
     return
 
 
 if __name__ == "__main__":
     test_LatinHypercube()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_lbfgsb.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_lbfgsb.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,17 @@
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
     x2_soln = np.eye(n)[1]
     x2_soln[n-1] = 0.1
     # eps is the tolerance for rejecting a solution as incorrect
     eps = 0.01
     # Check that the computed solutions are within eps of the truth
-    assert(np.linalg.norm(x1 - x1_soln) < eps)
-    assert(np.linalg.norm(x2 - x2_soln) < eps)
-    assert(np.abs(x3[n-1] - 0.1) < eps)
+    assert (np.linalg.norm(x1 - x1_soln) < eps)
+    assert (np.linalg.norm(x2 - x2_soln) < eps)
+    assert (np.abs(x3[n-1] - 0.1) < eps)
     return
 
 
 def test_TR_LBFGSB():
     """ Test the TR_LBFGSB class in optimizers.py.
 
     Perform a test of the TR_LBFGSB class by minimizing the three variable,
@@ -241,16 +241,16 @@
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
     x2_soln = np.eye(n)[1]
     x2_soln[n-1] = 0.1
     # eps is the tolerance for rejecting a solution as incorrect
     eps = 0.01
     # Check that the computed solutions are within eps of the truth
-    assert(np.linalg.norm(x1 - x1_soln) < eps)
-    assert(np.linalg.norm(x2 - x2_soln) < eps)
-    assert(np.abs(x3[n-1] - 0.1) < eps)
+    assert (np.linalg.norm(x1 - x1_soln) < eps)
+    assert (np.linalg.norm(x2 - x2_soln) < eps)
+    assert (np.abs(x3[n-1] - 0.1) < eps)
     return
 
 
 if __name__ == "__main__":
     test_LBFGSB()
     test_TR_LBFGSB()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_libe.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_libe.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,62 +79,62 @@
         for i, name in enumerate(moop.moop.des_names):
             xx[i] = x[name[0]]
         # Return ID
         return xx[:3]
 
     # Create a libE_MOOP with named variables
     moop = libE_MOOP(LocalGPS)
-    assert(isinstance(moop.moop, MOOP))
+    assert (isinstance(moop.moop, MOOP))
     moop = libE_MOOP(LocalGPS, hyperparams={})
-    assert(isinstance(moop.moop, MOOP))
+    assert (isinstance(moop.moop, MOOP))
     # Add n design vars
     for i in range(n):
         moop.addDesign({'name': "x" + str(i + 1), 'lb': 0.0, 'ub': 1.0})
-    assert(len(moop.getDesignType().names) == n)
+    assert (len(moop.getDesignType().names) == n)
     # Add simulation
     moop.addSimulation({'name': "Eye",
                         'm': o,
                         'sim_func': id_named,
                         'hyperparams': {'search_budget': 100},
                         'search': LatinHypercube,
                         'surrogate': GaussRBF,
                         'sim_db': {},
                         'des_tol': 0.00000001})
-    assert(len(moop.getSimulationType().names) == 1)
+    assert (len(moop.getSimulationType().names) == 1)
     # Add o objectives
     def obj1(x, s): return s['Eye'][0]
     def obj2(x, s): return s['Eye'][1]
     def obj3(x, s): return s['Eye'][2]
     moop.addObjective({'name': "obj1", 'obj_func': obj1})
     moop.addObjective({'name': "obj2", 'obj_func': obj2})
     moop.addObjective({'name': "obj3", 'obj_func': obj3})
-    assert(len(moop.getObjectiveType().names) == 3)
+    assert (len(moop.getObjectiveType().names) == 3)
     # Add 1 constraint
     def const1(x, s): return x["x5"] - 0.5
     moop.addConstraint({'name': "c1", 'constraint': const1})
-    assert(len(moop.getConstraintType().names) == 1)
+    assert (len(moop.getConstraintType().names) == 1)
     # Add 4 acquisition functions
     for i in range(4):
         moop.addAcquisition({'acquisition': RandomConstraint})
-    assert(len(moop.moop.acquisitions) == 4)
+    assert (len(moop.moop.acquisitions) == 4)
     # Perform 0 iteration manually
     batch = moop.iterate(0)
     for (xi, i) in batch:
         moop.evaluateSimulation(xi, i)
     moop.updateAll(0, batch)
     # Add a value in the simulation database
     x_val = np.zeros(1, dtype=moop.getDesignType())[0]
     sx_val = np.zeros(1, dtype=moop.getSimulationType())[0]
     moop.update_sim_db(x_val, sx_val["Eye"], "Eye")
-    assert(np.all(moop.check_sim_db(x_val, "Eye") == 0))
+    assert (np.all(moop.check_sim_db(x_val, "Eye") == 0))
     moop.addData(x_val, sx_val)
     # Check Pareto front, objective data, sim data
-    assert(moop.getPF()['x1'].shape[0] == 1)
-    assert(moop.getObjectiveData()['x1'].shape[0] == 101)
-    assert(moop.getSimulationData()['Eye']['x1'].shape[0] == 101)
+    assert (moop.getPF()['x1'].shape[0] == 1)
+    assert (moop.getObjectiveData()['x1'].shape[0] == 101)
+    assert (moop.getSimulationData()['Eye']['x1'].shape[0] == 101)
     # Test checkpointing features
     moop.setCheckpoint(True)
     moop.save()
     moop.load()
     # Clean up test directory
     os.remove("parmoo.moop")
     os.remove("parmoo.surrogate.1")
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_moop.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_moop.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     with pytest.raises(TypeError):
         MOOP(lambda w, x, y, z: 0.0)
     # Test bad hyperparams dictionary
     with pytest.raises(TypeError):
         MOOP(LocalGPS, hyperparams=[])
     # Initialize a MOOP with no hyperparameters
     moop = MOOP(LocalGPS)
-    assert(moop.n == 0 and moop.n_cont == 0 and moop.n_cat == 0 and
-           moop.n_cat_d == 0 and moop.s == 0 and moop.m_total == 0 and
-           moop.o == 0 and moop.p == 0)
+    assert (moop.n == 0 and moop.n_cont == 0 and moop.n_cat == 0 and
+            moop.n_cat_d == 0 and moop.s == 0 and moop.m_total == 0 and
+            moop.o == 0 and moop.p == 0)
     # Initialize a MOOP with a hyperparameter list
     moop = MOOP(LocalGPS, hyperparams={'test': 0})
-    assert(moop.n == 0 and moop.n_cont == 0 and moop.n_cat == 0 and
-           moop.n_cat_d == 0 and moop.s == 0 and moop.m_total == 0 and
-           moop.o == 0 and moop.p == 0)
-    assert(moop.hyperparams['test'] == 0)
+    assert (moop.n == 0 and moop.n_cont == 0 and moop.n_cat == 0 and
+            moop.n_cat_d == 0 and moop.s == 0 and moop.m_total == 0 and
+            moop.o == 0 and moop.p == 0)
+    assert (moop.hyperparams['test'] == 0)
 
 
 def test_MOOP_addSimulation():
     """ Check that the MOOP class handles adding new simulations properly.
 
     Initialize several MOOPs, and add several simulations. Check that
     the metadata is updated correctly.
@@ -77,86 +77,86 @@
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     # Now add one simulation and check
     moop.addSimulation(g1)
-    assert(moop.n == 3 and moop.s == 1 and moop.m_total == 1
-           and moop.o == 0 and moop.p == 0)
+    assert (moop.n == 3 and moop.s == 1 and moop.m_total == 1
+            and moop.o == 0 and moop.p == 0)
     # Initialize another MOOP with 3 design variables
     moop = MOOP(LocalGPS)
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addSimulation(g1, g2)
-    assert(moop.n == 3 and moop.s == 2 and moop.m_total == 3
-           and moop.o == 0 and moop.p == 0)
+    assert (moop.n == 3 and moop.s == 2 and moop.m_total == 3
+            and moop.o == 0 and moop.p == 0)
     # Now test adding simulations with empty precomputed databases
     g1['sim_db'] = {}
     moop = MOOP(LocalGPS)
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addSimulation(g1)
-    assert(moop.n == 3 and moop.s == 1 and moop.m_total == 1
-           and moop.o == 0 and moop.p == 0)
-    assert(moop.sim_db[0]['n'] == 0)
+    assert (moop.n == 3 and moop.s == 1 and moop.m_total == 1
+            and moop.o == 0 and moop.p == 0)
+    assert (moop.sim_db[0]['n'] == 0)
     # Now test adding a simulation with nonempty database, but empty lists
     g1['sim_db'] = {'x_vals': [], 's_vals': []}
     moop = MOOP(LocalGPS)
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addSimulation(g1)
-    assert(moop.n == 3 and moop.s == 1 and moop.m_total == 1
-           and moop.o == 0 and moop.p == 0)
-    assert(moop.sim_db[0]['n'] == 0)
+    assert (moop.n == 3 and moop.s == 1 and moop.m_total == 1
+            and moop.o == 0 and moop.p == 0)
+    assert (moop.sim_db[0]['n'] == 0)
     # Now try a simulation with some data
     g1['sim_db'] = {'x_vals': [[0.0, 0.0, 0.0]], 's_vals': [[0.0]]}
     moop = MOOP(LocalGPS)
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
     moop.addSimulation(g1)
-    assert(moop.n == 3 and moop.s == 1 and moop.m_total == 1
-           and moop.o == 0 and moop.p == 0)
-    assert(moop.sim_db[0]['n'] == 1)
+    assert (moop.n == 3 and moop.s == 1 and moop.m_total == 1
+            and moop.o == 0 and moop.p == 0)
+    assert (moop.sim_db[0]['n'] == 1)
     moop.addSimulation(g3, g4)
     # Try to use a repeated name to test error handling
     with pytest.raises(ValueError):
         moop.addSimulation(g4)
     # Check the names
-    assert(moop.sim_names[0][0] == "sim1")
-    assert(moop.sim_names[1][0] == "Bobo1")
-    assert(moop.sim_names[2][0] == "Bobo2")
+    assert (moop.sim_names[0][0] == "sim1")
+    assert (moop.sim_names[1][0] == "Bobo1")
+    assert (moop.sim_names[2][0] == "Bobo2")
 
 
 def test_pack_unpack_sim():
     """ Check that the MOOP class handles simulation packing correctly.
 
     Initialize a MOOP objecti with and without design variable names.
     Add 2 simulations and pack/unpack each output.
@@ -186,32 +186,32 @@
     sx[2] = 3.0
     # Create a MOOP without named variables and test simulation unpacking
     moop = MOOP(LocalGPS)
     # Add two continuous variables and two simulations
     moop.addDesign({'lb': 0.0, 'ub': 1000.0},
                    {'lb': -1.0, 'ub': 0.0})
     moop.addSimulation(g1, g2)
-    assert(all(moop.__pack_sim__(sx)[:] == sx[:]))
-    assert(all(moop.__unpack_sim__(sx)[:] == sx[:]))
+    assert (all(moop.__pack_sim__(sx)[:] == sx[:]))
+    assert (all(moop.__unpack_sim__(sx)[:] == sx[:]))
     # Create a MOOP with named variables and test simulation unpacking
     moop = MOOP(LocalGPS)
     # Add two continuous variables and two simulations
     moop.addDesign({'name': "x0", 'lb': 0.0, 'ub': 1000.0},
                    {'name': "x1", 'lb': -1.0, 'ub': 0.0})
     moop.addSimulation(g1, g2)
     # Create a solution vector
     sxx = np.zeros(1, dtype=moop.sim_names)
     sxx[0]['sim1'] = 1.0
     sxx[0]['sim2'][:] = np.array([2.0, 3.0])
     # Check packing
-    assert(all(moop.__pack_sim__(sxx) == sx))
+    assert (all(moop.__pack_sim__(sxx) == sx))
     # Check unpacking
-    assert(moop.__unpack_sim__(sx)['sim1'] == sxx[0]['sim1'])
-    assert(moop.__unpack_sim__(sx)['sim2'][0] == sxx[0]['sim2'][0])
-    assert(moop.__unpack_sim__(sx)['sim2'][1] == sxx[0]['sim2'][1])
+    assert (moop.__unpack_sim__(sx)['sim1'] == sxx[0]['sim1'])
+    assert (moop.__unpack_sim__(sx)['sim2'][0] == sxx[0]['sim2'][0])
+    assert (moop.__unpack_sim__(sx)['sim2'][1] == sxx[0]['sim2'][1])
 
 
 def test_MOOP_addObjective():
     """ Check that the MOOP class handles adding objectives properly.
 
     Initialize a MOOP object and check that the addObjective() function works
     correctly.
@@ -256,30 +256,30 @@
         moop.addObjective({'name': 5, 'obj_func': lambda x, s: 0.0})
     # Add an objective after an acquisition
     with pytest.raises(RuntimeError):
         moop1 = MOOP(LocalGPS)
         moop1.acquisitions.append(0)
         moop1.addObjective({'obj_func': lambda x, s: 0.0})
     # Check that no objectives were added yet
-    assert(moop.o == 0)
+    assert (moop.o == 0)
     # Now add 3 good objectives
     moop.addObjective({'obj_func': lambda x, s: x[0]})
-    assert(moop.o == 1)
+    assert (moop.o == 1)
     moop.addObjective({'obj_func': lambda x, s: s[0]},
                       {'obj_func': lambda x, s, der=0: s[1]})
-    assert(moop.o == 3)
+    assert (moop.o == 3)
     moop.addObjective({'name': "Bobo", 'obj_func': lambda x, s: s[0]})
-    assert(moop.o == 4)
+    assert (moop.o == 4)
     # Try to use a repeated name to test error handling
     with pytest.raises(ValueError):
         moop.addObjective({'name': "Bobo", 'obj_func': lambda x, s: s[0]})
-    assert(moop.obj_names[0] == ("f1", 'f8'))
-    assert(moop.obj_names[1] == ("f2", 'f8'))
-    assert(moop.obj_names[2] == ("f3", 'f8'))
-    assert(moop.obj_names[3] == ("Bobo", 'f8'))
+    assert (moop.obj_names[0] == ("f1", 'f8'))
+    assert (moop.obj_names[1] == ("f2", 'f8'))
+    assert (moop.obj_names[2] == ("f3", 'f8'))
+    assert (moop.obj_names[3] == ("Bobo", 'f8'))
 
 
 def test_MOOP_addConstraint():
     """ Check that the MOOP class handles adding constraints properly.
 
     Initialize a MOOP object and check that the addConstraint() function works
     correctly.
@@ -319,30 +319,30 @@
     with pytest.raises(TypeError):
         moop.addConstraint({'constraint': 0})
     with pytest.raises(ValueError):
         moop.addConstraint({'constraint': lambda x: 0.0})
     with pytest.raises(TypeError):
         moop.addConstraint({'name': 5, 'constraint': lambda x, s: 0.0})
     # Check that no constraints were added yet
-    assert(moop.p == 0)
+    assert (moop.p == 0)
     # Now add 3 good constraints
     moop.addConstraint({'constraint': lambda x, s: x[0]})
-    assert(moop.p == 1)
+    assert (moop.p == 1)
     moop.addConstraint({'constraint': lambda x, s: s[0]},
                        {'constraint': lambda x, s, der=0: s[1] + s[2]})
-    assert(moop.p == 3)
+    assert (moop.p == 3)
     moop.addConstraint({'name': "Bobo", 'constraint': lambda x, s: s[0]})
-    assert(moop.p == 4)
+    assert (moop.p == 4)
     # Try to use a repeated name to test error handling
     with pytest.raises(ValueError):
         moop.addConstraint({'name': "Bobo", 'constraint': lambda x, s: s[0]})
-    assert(moop.const_names[0] == ("c1", 'f8'))
-    assert(moop.const_names[1] == ("c2", 'f8'))
-    assert(moop.const_names[2] == ("c3", 'f8'))
-    assert(moop.const_names[3] == ("Bobo", 'f8'))
+    assert (moop.const_names[0] == ("c1", 'f8'))
+    assert (moop.const_names[1] == ("c2", 'f8'))
+    assert (moop.const_names[2] == ("c3", 'f8'))
+    assert (moop.const_names[3] == ("Bobo", 'f8'))
 
 
 def test_MOOP_addAcquisition():
     """ Check that the MOOP class handles adding acquisitions properly.
 
     Initialize a MOOP object and check that the addAcquisition() function works
     correctly.
@@ -395,21 +395,21 @@
     with pytest.raises(TypeError):
         moop.addAcquisition({'acquisition': 0,
                              'hyperparams': {}})
     with pytest.raises(TypeError):
         moop.addAcquisition({'acquisition': GaussRBF,
                              'hyperparams': {}})
     # Check that no acquisitions were added yet
-    assert(len(moop.acquisitions) == 0)
+    assert (len(moop.acquisitions) == 0)
     # Now add 3 good acquisitions
     moop.addAcquisition({'acquisition': UniformWeights})
-    assert(len(moop.acquisitions) == 1)
+    assert (len(moop.acquisitions) == 1)
     moop.addAcquisition({'acquisition': UniformWeights},
                         {'acquisition': UniformWeights, 'hyperparams': {}})
-    assert(len(moop.acquisitions) == 3)
+    assert (len(moop.acquisitions) == 3)
 
 
 def test_MOOP_getTypes():
     """ Check that the MOOP class handles getting dtypes properly.
 
     Initialize a MOOP object, add design variables, simulations, objectives,
     and constraints, and get the corresponding types.
@@ -428,39 +428,39 @@
           'search': LatinHypercube,
           'sim_func': lambda x: [np.linalg.norm(x)],
           'surrogate': GaussRBF}
 
     # Create a new MOOP
     moop = MOOP(LocalGPS)
     # Check that all types are None
-    assert(moop.getDesignType() is None)
-    assert(moop.getSimulationType() is None)
-    assert(moop.getObjectiveType() is None)
-    assert(moop.getConstraintType() is None)
+    assert (moop.getDesignType() is None)
+    assert (moop.getSimulationType() is None)
+    assert (moop.getObjectiveType() is None)
+    assert (moop.getConstraintType() is None)
     # Add some unnamed variables, simulations, objectives, and constraints
     moop.addDesign({'des_type': "continuous", 'lb': 0.0, 'ub': 1.0})
     moop.addDesign({'des_type': "categorical", 'levels': 3})
     moop.addSimulation(g1)
     moop.addObjective({'obj_func': lambda x, s: [sum(s)]})
     moop.addConstraint({'constraint': lambda x, s: [sum(s) - 1]})
-    assert(np.zeros(1, dtype=moop.getDesignType()).size == 2)
-    assert(np.zeros(1, dtype=moop.getSimulationType()).size == 1)
-    assert(np.zeros(1, dtype=moop.getObjectiveType()).size == 1)
-    assert(np.zeros(1, dtype=moop.getConstraintType()).size == 1)
+    assert (np.zeros(1, dtype=moop.getDesignType()).size == 2)
+    assert (np.zeros(1, dtype=moop.getSimulationType()).size == 1)
+    assert (np.zeros(1, dtype=moop.getObjectiveType()).size == 1)
+    assert (np.zeros(1, dtype=moop.getConstraintType()).size == 1)
     # Add some named variables, simulations, objectives, and constraints
     moop = MOOP(LocalGPS)
     moop.addDesign({'name': "x1", 'lb': 0.0, 'ub': 1.0})
     moop.addDesign({'name': "x2", 'des_type': "categorical", 'levels': 3})
     moop.addSimulation(g1)
     moop.addObjective({'obj_func': lambda x, s: [sum(s)]})
     moop.addConstraint({'constraint': lambda x, s: [sum(s) - 1]})
-    assert(np.zeros(1, dtype=moop.getDesignType()).size == 1)
-    assert(np.zeros(1, dtype=moop.getSimulationType()).size == 1)
-    assert(np.zeros(1, dtype=moop.getObjectiveType()).size == 1)
-    assert(np.zeros(1, dtype=moop.getConstraintType()).size == 1)
+    assert (np.zeros(1, dtype=moop.getDesignType()).size == 1)
+    assert (np.zeros(1, dtype=moop.getSimulationType()).size == 1)
+    assert (np.zeros(1, dtype=moop.getObjectiveType()).size == 1)
+    assert (np.zeros(1, dtype=moop.getConstraintType()).size == 1)
 
 
 def test_MOOP_evaluateSimulation():
     """ Check that the MOOP class handles evaluating simulations properly.
 
     Initialize a MOOP object and check that the evaluateSimulation() function
     works correctly.
@@ -521,21 +521,21 @@
         moop1.check_sim_db(x1, 5.0)
     with pytest.raises(ValueError):
         moop1.check_sim_db(x1, -1)
     with pytest.raises(ValueError):
         moop2.check_sim_db(x2, "hello world")
     # Try 2 good evaluations
     moop1.evaluateSimulation(x1, 0)
-    assert(moop1.check_sim_db(x1, 0) is not None)
+    assert (moop1.check_sim_db(x1, 0) is not None)
     moop1.evaluateSimulation(y1, 0)
-    assert(moop1.check_sim_db(y1, 0) is not None)
+    assert (moop1.check_sim_db(y1, 0) is not None)
     moop2.evaluateSimulation(x2, "g2")
-    assert(moop2.check_sim_db(x2, "g2") is not None)
+    assert (moop2.check_sim_db(x2, "g2") is not None)
     moop2.evaluateSimulation(y2, "g2")
-    assert(moop2.check_sim_db(y2, "g2") is not None)
+    assert (moop2.check_sim_db(y2, "g2") is not None)
     return
 
 
 def test_MOOP_evaluateSurrogates():
     """ Check that the MOOP class handles evaluating objectives properly.
 
     Initialize a MOOP object and check that the evaluateSurrogates() function
@@ -593,35 +593,40 @@
     moop1.resetSurrogates(np.ones(3) * 0.5)
     # Now try some bad evaluations
     with pytest.raises(TypeError):
         moop1.evaluateSurrogates(10.0)
     with pytest.raises(ValueError):
         moop1.evaluateSurrogates(np.zeros(1))
     # Now do some good evaluations and check the results
-    assert(np.linalg.norm(moop1.evaluateSurrogates(np.zeros(3)) -
-                          np.asarray([0.0, 0.0, np.sqrt(3.0) + np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.5, 0.5, 0.5]))
-                          - np.asarray([0.5, np.sqrt(0.75), np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateSurrogates(np.asarray([1.0, 0.0, 0.0]))
-                          - np.asarray([1.0, 1.0, np.sqrt(2.0) +
-                                        np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 1.0, 0.0]))
-                          - np.asarray([0.0, 1.0, np.sqrt(2.0) +
-                                        np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 0.0, 1.0]))
-                          - np.asarray([0.0, 1.0, np.sqrt(2.0) +
-                                        np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateSurrogates(np.ones(3)) -
-                          np.asarray([1.0, np.sqrt(3.0), np.sqrt(0.75)]))
-           < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.zeros(3)) -
+                           np.asarray([0.0, 0.0, np.sqrt(3.0) +
+                                       np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.5,
+                                                                0.5, 0.5]))
+                           - np.asarray([0.5, np.sqrt(0.75), np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([1.0, 0.0,
+                                                                0.0]))
+                           - np.asarray([1.0, 1.0, np.sqrt(2.0) +
+                                         np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 1.0,
+                                                                0.0]))
+                           - np.asarray([0.0, 1.0, np.sqrt(2.0) +
+                                         np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 0.0,
+                                                                1.0]))
+                           - np.asarray([0.0, 1.0, np.sqrt(2.0) +
+                                         np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.ones(3)) -
+                           np.asarray([1.0, np.sqrt(3.0), np.sqrt(0.75)]))
+            < 0.00000001)
     # Adjust the scale and try again
     moop2 = MOOP(LocalGPS)
     moop2.addDesign({'lb': -1.0, 'ub': 1.0},
                     {'lb': 0.0, 'ub': 2.0},
                     {'lb': -0.5, 'ub': 1.5})
     moop2.addObjective({'obj_func': lambda x, s: x[0]},
                        {'obj_func': lambda x, s: s[0]},
@@ -640,20 +645,20 @@
     moop2.evaluateSimulation(np.asarray([0.0, 0.0, 1.0]), 1)
     moop2.evaluateSimulation(np.ones(3), 0)
     moop2.evaluateSimulation(np.ones(3), 1)
     moop2.fitSurrogates()
     # Now compare evaluations against the original surrogate
     x = moop1.__embed__(np.zeros(3))
     xx = moop2.__embed__(np.zeros(3))
-    assert(np.linalg.norm(moop1.evaluateSurrogates(x) -
-                          moop2.evaluateSurrogates(xx)) < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(x) -
+                           moop2.evaluateSurrogates(xx)) < 0.00000001)
     x = moop1.__embed__(np.ones(3))
     xx = moop2.__embed__(np.ones(3))
-    assert(np.linalg.norm(moop1.evaluateSurrogates(x) -
-                          moop2.evaluateSurrogates(xx)) < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(x) -
+                           moop2.evaluateSurrogates(xx)) < 0.00000001)
 
 
 def test_MOOP_evaluateConstraints():
     """ Check that the MOOP class handles evaluating constraints properly.
 
     Initialize a MOOP object and check that the evaluateConstraints() function
     works correctly.
@@ -682,15 +687,15 @@
           'surrogate': GaussRBF}
     # Initialize a MOOP with 2 SimGroups and 3 objectives
     moop1 = MOOP(LocalGPS)
     for i in range(3):
         moop1.addDesign({'lb': 0.0, 'ub': 1.0})
     moop1.addSimulation(g1, g2)
     # Evaluate an empty constraint and check that a zero array is returned
-    assert(all(moop1.evaluateConstraints(np.zeros(3)) == np.zeros(1)))
+    assert (all(moop1.evaluateConstraints(np.zeros(3)) == np.zeros(1)))
     # Now add 3 constraints
     moop1.addConstraint({'constraint': lambda x, s: x[0]})
     moop1.addConstraint({'constraint': lambda x, s: s[0]})
     moop1.addConstraint({'constraint': lambda x, s: s[1] + s[2]})
     # Evaluate some data points and fit the surrogates
     moop1.evaluateSimulation(np.zeros(3), 0)
     moop1.evaluateSimulation(np.zeros(3), 1)
@@ -707,39 +712,40 @@
     moop1.fitSurrogates()
     # Now try some bad evaluations
     with pytest.raises(TypeError):
         moop1.evaluateConstraints(10.0)
     with pytest.raises(ValueError):
         moop1.evaluateConstraints(np.zeros(1))
     # Now do some good evaluations and check the results
-    assert(np.linalg.norm(moop1.evaluateConstraints(np.zeros(3)) -
-                          np.asarray([0.0, 0.0, np.sqrt(3.0) + np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateConstraints(np.asarray([0.5, 0.5,
-                                                                0.5]))
-                          - np.asarray([0.5, np.sqrt(0.75), np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateConstraints(np.asarray([1.0, 0.0,
-                                                                0.0]))
-                          - np.asarray([1.0, 1.0, np.sqrt(2.0)
-                                        + np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateConstraints(np.asarray([0.0, 1.0,
-                                                                0.0]))
-                          - np.asarray([0.0, 1.0, np.sqrt(2.0)
-                                        + np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateConstraints(np.asarray([0.0, 0.0,
-                                                                1.0]))
-                          - np.asarray([0.0, 1.0, np.sqrt(2.0)
-                                        + np.sqrt(0.75)]))
-           < 0.00000001)
-    assert(np.linalg.norm(moop1.evaluateConstraints(np.ones(3)) -
-                          np.asarray([1.0, np.sqrt(3.0), np.sqrt(0.75)]))
-           < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(np.zeros(3)) -
+                           np.asarray([0.0, 0.0, np.sqrt(3.0) +
+                                       np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(np.asarray([0.5, 0.5,
+                                                                 0.5]))
+                           - np.asarray([0.5, np.sqrt(0.75), np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(np.asarray([1.0, 0.0,
+                                                                 0.0]))
+                           - np.asarray([1.0, 1.0, np.sqrt(2.0)
+                                         + np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(np.asarray([0.0, 1.0,
+                                                                 0.0]))
+                           - np.asarray([0.0, 1.0, np.sqrt(2.0)
+                                         + np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(np.asarray([0.0, 0.0,
+                                                                 1.0]))
+                           - np.asarray([0.0, 1.0, np.sqrt(2.0)
+                                         + np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(np.ones(3)) -
+                           np.asarray([1.0, np.sqrt(3.0), np.sqrt(0.75)]))
+            < 0.00000001)
     # Adjust the scale and try again
     moop2 = MOOP(LocalGPS)
     moop2.addDesign({'lb': -1.0, 'ub': 1.0},
                     {'lb': 0.0, 'ub': 2.0},
                     {'lb': -0.5, 'ub': 1.5})
     moop2.addSimulation(g1, g2)
     moop2.addConstraint({'constraint': lambda x, s: x[0]})
@@ -758,375 +764,20 @@
     moop2.evaluateSimulation(np.asarray([0.0, 0.0, 1.0]), 1)
     moop2.evaluateSimulation(np.ones(3), 0)
     moop2.evaluateSimulation(np.ones(3), 1)
     moop2.fitSurrogates()
     # Now compare evaluations against the original surrogate
     x = moop1.__embed__(np.zeros(3))
     xx = moop2.__embed__(np.zeros(3))
-    assert(np.linalg.norm(moop1.evaluateConstraints(x) -
-                          moop2.evaluateConstraints(xx)) < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(x) -
+                           moop2.evaluateConstraints(xx)) < 0.00000001)
     x = moop1.__embed__(np.ones(3))
     xx = moop2.__embed__(np.ones(3))
-    assert(np.linalg.norm(moop1.evaluateConstraints(x) -
-                          moop2.evaluateConstraints(xx)) < 0.00000001)
-
-
-def test_MOOP_evaluatePenalty():
-    """ Check that the MOOP class handles evaluating penalty function properly.
-
-    Initialize a MOOP object and check that the evaluatePenalty() function
-    works correctly.
-
-    """
-
-    from parmoo import MOOP
-    from parmoo.surrogates import GaussRBF
-    from parmoo.searches import LatinHypercube
-    from parmoo.optimizers import LocalGPS
-    import numpy as np
-    import pytest
-
-    # Create 2 SimGroups for later
-    g1 = {'n': 3,
-          'm': 1,
-          'hyperparams': {},
-          'search': LatinHypercube,
-          'sim_func': lambda x: [np.linalg.norm(x)],
-          'surrogate': GaussRBF}
-    g2 = {'n': 3,
-          'm': 2,
-          'hyperparams': {},
-          'search': LatinHypercube,
-          'sim_func': lambda x: [np.linalg.norm(x-1.0), np.linalg.norm(x-0.5)],
-          'surrogate': GaussRBF}
-
-    # Create several differentiable functions and constraints.
-    def f1(x, s, der=0):
-        if der == 0:
-            return np.dot(x, x)
-        if der == 1:
-            return 2.0 * x
-        if der == 2:
-            return np.zeros(s.size)
-
-    def f2(x, s, der=0):
-        if der == 0:
-            return np.dot(s - 0.5, s - 0.5)
-        if der == 1:
-            return np.zeros(x.size)
-        if der == 2:
-            return 2.0 * s - 1.0
-
-    def c1(x, s, der=0):
-        if der == 0:
-            return x[0] - 0.25
-        if der == 1:
-            return np.ones(x.size)
-        if der == 2:
-            return np.zeros(x.size)
-
-    def c2(x, s, der=0):
-        if der == 0:
-            return s[0] - 0.25
-        if der == 1:
-            return np.zeros(s.size)
-        if der == 2:
-            return np.ones(s.size)
-
-    # Initialize a MOOP with 2 SimGroups and 3 objectives
-    moop1 = MOOP(LocalGPS)
-    for i in range(3):
-        moop1.addDesign({'lb': 0.0, 'ub': 1.0})
-    moop1.addObjective({'obj_func': f1})
-    assert(np.all(moop1.evaluatePenalty(np.zeros(3)) == np.zeros(1)))
-    assert(np.all(moop1.evaluatePenalty(np.ones(3)) == 3.0 * np.ones(1)))
-    moop1.addConstraint({'constraint': c1})
-    assert(np.all(moop1.evaluatePenalty(np.zeros(3)) == np.zeros(1)))
-    assert(np.all(moop1.evaluatePenalty(np.ones(3)) == 3.75 * np.ones(1)))
-    moop1 = MOOP(LocalGPS)
-    for i in range(3):
-        moop1.addDesign({'lb': 0.0, 'ub': 1.0})
-    moop1.addSimulation(g1, g2)
-    moop1.evaluateSimulation(np.ones(3), 0)
-    moop1.evaluateSimulation(np.ones(3), 1)
-    moop1.fitSurrogates()
-    moop1.addObjective({'obj_func': f1})
-    moop1.addObjective({'obj_func': f1})
-    assert(np.all(moop1.evaluatePenalty(np.zeros(3)) == np.zeros(1)))
-    assert(np.all(moop1.evaluatePenalty(np.ones(3)) == 3.0 * np.ones(1)))
-    moop1.addConstraint({'constraint': c1})
-    assert(np.all(moop1.evaluatePenalty(np.zeros(3)) == np.zeros(1)))
-    assert(np.all(moop1.evaluatePenalty(np.ones(3)) == 3.75 * np.ones(1)))
-    # Now try some bad evaluations
-    with pytest.raises(TypeError):
-        moop1.evaluatePenalty(10.0)
-    with pytest.raises(ValueError):
-        moop1.evaluatePenalty(np.zeros(1))
-    # Adjust the scaling and compare
-    moop2 = MOOP(LocalGPS)
-    moop2.addDesign({'lb': -1.0, 'ub': 1.0},
-                    {'lb': 0.0, 'ub': 2.0},
-                    {'lb': -0.5, 'ub': 1.5})
-    moop2.addSimulation(g1, g2)
-    moop2.evaluateSimulation(np.ones(3), 0)
-    moop2.evaluateSimulation(np.ones(3), 1)
-    moop2.fitSurrogates()
-    moop2.addObjective({'obj_func': f1})
-    moop2.addObjective({'obj_func': f1})
-    moop2.addConstraint({'constraint': c1})
-    x = moop1.__embed__(np.ones(3))
-    xx = moop2.__embed__(np.ones(3))
-    assert(np.linalg.norm(moop1.evaluatePenalty(x) -
-                          moop2.evaluatePenalty(xx)) < 0.00000001)
-
-
-def test_MOOP_evaluateGradients():
-    """ Check that the MOOP class handles evaluating gradients properly.
-
-    Initialize a MOOP object and check that the evaluateGradients() function
-    works correctly.
-
-    """
-
-    from parmoo import MOOP
-    from parmoo.surrogates import GaussRBF
-    from parmoo.searches import LatinHypercube
-    from parmoo.optimizers import LocalGPS
-    import numpy as np
-    import pytest
-
-    # Create 2 SimGroups for later
-    g1 = {'n': 3,
-          'm': 1,
-          'hyperparams': {},
-          'search': LatinHypercube,
-          'sim_func': lambda x: [np.linalg.norm(x)],
-          'surrogate': GaussRBF}
-    g2 = {'n': 3,
-          'm': 2,
-          'hyperparams': {},
-          'search': LatinHypercube,
-          'sim_func': lambda x: [np.linalg.norm(x-1.0), np.linalg.norm(x-0.5)],
-          'surrogate': GaussRBF}
-
-    # Create several differentiable functions and constraints.
-    def f1(x, s, der=0):
-        if der == 0:
-            return np.dot(x, x)
-        if der == 1:
-            return 2.0 * x
-        if der == 2:
-            return np.zeros(s.size)
-
-    def f2(x, s, der=0):
-        if der == 0:
-            return np.dot(s - 0.5, s - 0.5)
-        if der == 1:
-            return np.zeros(x.size)
-        if der == 2:
-            return 2.0 * s - 1.0
-
-    def c1(x, s, der=0):
-        if der == 0:
-            return x[0] - 0.25
-        if der == 1:
-            return np.eye(x.size)[0]
-        if der == 2:
-            return np.zeros(s.size)
-
-    def c2(x, s, der=0):
-        if der == 0:
-            return s[0] - 0.25
-        if der == 1:
-            return np.zeros(x.size)
-        if der == 2:
-            return np.eye(s.size)[0]
-
-    # Initialize a MOOP with 2 SimGroups and 3 objectives
-    moop1 = MOOP(LocalGPS)
-    for i in range(3):
-        moop1.addDesign({'lb': 0.0, 'ub': 1.0})
-    moop1.addObjective({'obj_func': f1})
-    assert(np.all(moop1.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) ==
-                  2.0 * np.ones((1, 3))))
-    moop1.addConstraint({'constraint': c1})
-    assert(np.all(moop1.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    result = 2.0 * np.ones((1, 3))
-    result[0, 0] = 3.0
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) == result))
-    moop1 = MOOP(LocalGPS)
-    for i in range(3):
-        moop1.addDesign({'lb': 0.0, 'ub': 1.0})
-    moop1.addSimulation(g1, g2)
-    moop1.evaluateSimulation(np.ones(3), 0)
-    moop1.evaluateSimulation(np.ones(3), 1)
-    moop1.fitSurrogates()
-    moop1.addObjective({'obj_func': f1})
-    assert(np.all(moop1.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) ==
-                  2.0 * np.ones((1, 3))))
-    moop1.addConstraint({'constraint': c1})
-    assert(np.all(moop1.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) == result))
-    result = np.zeros((2, 3))
-    result[1, 0] = 1.0
-    result[0, :] = 2.0
-    result[0, 0] = 3.0
-    moop1.addObjective({'obj_func': f2})
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) == result))
-    moop1.addConstraint({'constraint': c2})
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) == result))
-    # Now try some bad evaluations
-    with pytest.raises(TypeError):
-        moop1.evaluateGradients(10.0)
-    with pytest.raises(ValueError):
-        moop1.evaluateGradients(np.zeros(1))
-    # Adjust the scaling and try again
-    moop2 = MOOP(LocalGPS)
-    moop2.addDesign({'lb': -1.0, 'ub': 1.0},
-                    {'lb': 0.0, 'ub': 2.0},
-                    {'lb': -0.5, 'ub': 1.5})
-    moop2.addSimulation(g1, g2)
-    moop2.evaluateSimulation(np.ones(3), 0)
-    moop2.evaluateSimulation(np.ones(3), 1)
-    moop2.fitSurrogates()
-    moop2.addObjective({'obj_func': f1})
-    moop2.addConstraint({'constraint': c1})
-    moop2.addObjective({'obj_func': f2})
-    moop2.addConstraint({'constraint': c2})
-    x = moop1.__embed__(np.ones(3))
-    xx = moop2.__embed__(np.ones(3))
-    assert(np.linalg.norm(moop1.evaluatePenalty(x) -
-                          moop2.evaluatePenalty(xx)) < 0.00000001)
-
-    # Initialize a MOOP with 2 SimGroups and 3 objectives with named designs
-    g3 = {'n': 3,
-          'm': 1,
-          'hyperparams': {},
-          'search': LatinHypercube,
-          'sim_func': lambda x: sum([x[name] ** 2.0
-                                     for name in x.dtype.names]),
-          'surrogate': GaussRBF}
-    g4 = {'n': 3,
-          'm': 2,
-          'hyperparams': {},
-          'search': LatinHypercube,
-          'sim_func': lambda x: sum([(x[name] - 1.0) * (x[name] - 0.5)
-                                     for name in x.dtype.names]),
-          'surrogate': GaussRBF}
-
-    def f3(x, s, der=0):
-        if der == 0:
-            result = 0.0
-            for name in x.dtype.names:
-                result = result + x[name] ** 2
-            return result
-        if der == 1:
-            result = np.zeros(1, dtype=x.dtype)
-            for name in x.dtype.names:
-                result[name] = 2.0 * x[name]
-            return result[0]
-        if der == 2:
-            return np.zeros(1, dtype=s.dtype)[0]
-
-    def f4(x, s, der=0):
-        if der == 0:
-            result = 0.0
-            for name in s.dtype.names:
-                if isinstance(s[name], np.ndarray):
-                    result = result + np.dot(s[name] - 0.5, s[name] - 0.5)
-                else:
-                    result = result + (s[name] - 0.5) ** 2
-            return result
-        if der == 1:
-            return np.zeros(1, dtype=x.dtype)[0]
-        if der == 2:
-            result = np.zeros(1, dtype=s.dtype)
-            for name in s.dtype.names:
-                result[name] = 2.0 * s[name] - 1.0
-            return result[0]
-
-    def c3(x, s, der=0):
-        if der == 0:
-            return x["x1"] - 0.25
-        if der == 1:
-            result = np.zeros(1, dtype=x.dtype)
-            result["x1"] = 1.0
-            return result[0]
-        if der == 2:
-            return np.zeros(1, dtype=s.dtype)[0]
-
-    def c4(x, s, der=0):
-        if der == 0:
-            return s['sim1'] - 0.25
-        if der == 1:
-            return np.zeros(1, dtype=x.dtype)[0]
-        if der == 2:
-            result = np.zeros(1, dtype=s.dtype)
-            result['sim1'] = 1.0
-            return result[0]
-
-    moop3 = MOOP(LocalGPS)
-    for i in range(3):
-        moop3.addDesign({'name': ('x' + str(i + 1)), 'lb': 0.0, 'ub': 1.0})
-    moop3.addObjective({'obj_func': f3})
-    assert(np.all(moop3.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    assert(np.all(moop3.evaluateGradients(np.ones(3)) ==
-                  2.0 * np.ones((1, 3))))
-    moop3.addConstraint({'constraint': c3})
-    assert(np.all(moop3.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    result = 2.0 * np.ones((1, 3))
-    result[0, 0] = 3.0
-    assert(np.all(moop3.evaluateGradients(np.ones(3)) == result))
-    moop3 = MOOP(LocalGPS)
-    for i in range(3):
-        moop3.addDesign({'name': ('x' + str(i + 1)), 'lb': 0.0, 'ub': 1.0})
-    moop3.addSimulation(g3, g4)
-    moop3.evaluateSimulation(np.ones(1, dtype=[("x1", float), ("x2", float),
-                                               ("x3", float)]), 0)
-    moop3.evaluateSimulation(np.ones(1, dtype=[("x1", float), ("x2", float),
-                                               ("x3", float)]), 1)
-    moop3.fitSurrogates()
-    moop3.addObjective({'obj_func': f3})
-    assert(np.all(moop3.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    assert(np.all(moop3.evaluateGradients(np.ones(3)) ==
-                  2.0 * np.ones((1, 3))))
-    moop3.addConstraint({'constraint': c3})
-    assert(np.all(moop3.evaluateGradients(np.zeros(3)) == np.zeros((1, 3))))
-    assert(np.all(moop3.evaluateGradients(np.ones(3)) == result))
-    result = np.zeros((2, 3))
-    result[1, 0] = 1.0
-    result[0, :] = 2.0
-    result[0, 0] = 3.0
-    moop3.addObjective({'obj_func': f4})
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) == result))
-    moop3.addConstraint({'constraint': c4})
-    assert(np.all(moop1.evaluateGradients(np.ones(3)) == result))
-    # Adjust the scaling and try again
-    moop4 = MOOP(LocalGPS)
-    moop4.addDesign({'name': "x1", 'lb': -1.0, 'ub': 1.0},
-                    {'name': "x2", 'lb': 0.0, 'ub': 2.0},
-                    {'name': "x3", 'lb': -0.5, 'ub': 1.5})
-    moop4.addSimulation(g3, g4)
-    moop4.evaluateSimulation(np.ones(1, dtype=[("x1", float), ("x2", float),
-                                               ("x3", float)]), 0)
-    moop4.evaluateSimulation(np.ones(1, dtype=[("x1", float), ("x2", float),
-                                               ("x3", float)]), 1)
-    moop4.fitSurrogates()
-    moop4.addObjective({'obj_func': f3})
-    moop4.addConstraint({'constraint': c3})
-    moop4.addObjective({'obj_func': f4})
-    moop4.addConstraint({'constraint': c4})
-    x = moop3.__embed__(np.ones(1, dtype=[("x1", float), ("x2", float),
-                                          ("x3", float)]))
-    xx = moop4.__embed__(np.ones(1, dtype=[("x1", float), ("x2", float),
-                                           ("x3", float)]))
-    assert(np.linalg.norm(moop3.evaluatePenalty(x) -
-                          moop4.evaluatePenalty(xx)) < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateConstraints(x) -
+                           moop2.evaluateConstraints(xx)) < 0.00000001)
 
 
 def test_MOOP_addData():
     """ Check that the MOOP class is able to add data to its internal database.
 
     Initialize a MOOP object and check that the addData(s, sx) function
     works correctly.
@@ -1160,18 +811,18 @@
     moop1.addObjective({'obj_func': lambda x, s: s[1]})
     moop1.addObjective({'obj_func': lambda x, s: s[0]})
     # Test adding some data
     moop1.iterate(0)
     moop1.addData(np.zeros(3), np.zeros(3))
     moop1.addData(np.zeros(3), np.zeros(3))
     moop1.addData(np.ones(3), np.ones(3))
-    assert(moop1.data['f_vals'].shape == (2, 2))
-    assert(moop1.data['x_vals'].shape == (2, 3))
-    assert(moop1.data['c_vals'].shape == (2, 1))
-    assert(moop1.n_dat == 2)
+    assert (moop1.data['f_vals'].shape == (2, 2))
+    assert (moop1.data['x_vals'].shape == (2, 3))
+    assert (moop1.data['c_vals'].shape == (2, 1))
+    assert (moop1.n_dat == 2)
     # Initialize a new MOOP with 2 SimGroups and 2 objectives
     moop2 = MOOP(LocalGPS)
     for i in range(3):
         moop2.addDesign({'lb': 0.0, 'ub': 1.0})
     moop2.addSimulation(g1, g2)
     moop2.addObjective({'obj_func': lambda x, s: s[1]})
     moop2.addObjective({'obj_func': lambda x, s: s[0]})
@@ -1181,18 +832,18 @@
     moop2.addConstraint({'constraint': lambda x, s: s[1] + s[2]})
     # Test adding some data
     moop2.iterate(0)
     moop2.addData(np.zeros(3), np.zeros(3))
     moop2.addData(np.zeros(3), np.zeros(3))
     moop2.addData(np.asarray([0.0, 0.0, 1.0]), np.zeros(3))
     moop2.addData(np.ones(3), np.ones(3))
-    assert(moop2.data['f_vals'].shape == (3, 2))
-    assert(moop2.data['x_vals'].shape == (3, 3))
-    assert(moop2.data['c_vals'].shape == (3, 3))
-    assert(moop2.n_dat == 3)
+    assert (moop2.data['f_vals'].shape == (3, 2))
+    assert (moop2.data['x_vals'].shape == (3, 3))
+    assert (moop2.data['c_vals'].shape == (3, 3))
+    assert (moop2.n_dat == 3)
     # Initialize a new MOOP with 2 SimGroups and 2 objectives
     moop3 = MOOP(LocalGPS)
     for i in range(3):
         moop3.addDesign({'lb': 0.0, 'ub': 1.0})
     moop3.addDesign({'des_type': "categorical", 'levels': 3})
     moop3.addSimulation(g1, g2)
     moop3.addObjective({'obj_func': lambda x, s: s[1]})
@@ -1200,18 +851,18 @@
     # Now add 3 constraints
     moop3.addConstraint({'constraint': lambda x, s: x[0]})
     moop3.addConstraint({'constraint': lambda x, s: s[0]})
     moop3.addConstraint({'constraint': lambda x, s: s[1] + s[2]})
     # Test adding some data
     moop3.iterate(0)
     moop3.addData(np.ones(4), np.ones(3))
-    assert(moop3.data['f_vals'].shape == (1, 2))
-    assert(moop3.data['x_vals'].shape == (1, 5))
-    assert(moop3.data['c_vals'].shape == (1, 3))
-    assert(moop3.n_dat == 1)
+    assert (moop3.data['f_vals'].shape == (1, 2))
+    assert (moop3.data['x_vals'].shape == (1, 5))
+    assert (moop3.data['c_vals'].shape == (1, 3))
+    assert (moop3.n_dat == 1)
 
 
 def test_MOOP_iterate():
     """ Test the MOOP class's iterator in objectives.py.
 
     Initialize several MOOP objects and perform iterations to produce
     a batch of candidate solutions.
@@ -1272,21 +923,21 @@
     moop1.updateAll(0, batch)
     batch = moop1.iterate(1)
     for (x, i) in batch:
         moop1.evaluateSimulation(x, i)
     moop1.updateAll(1, batch)
     soln = moop1.getPF()
     # Assert that solutions were found
-    assert(np.size(soln['x_vals']) > 0)
+    assert (np.size(soln['x_vals']) > 0)
     # Assert that the x_vals and f_vals match
     for i in range(np.shape(soln['x_vals'])[0]):
-        assert(np.linalg.norm(np.asarray([g1['sim_func'](soln['x_vals'][i]),
-                                          g2['sim_func'](soln['x_vals'][i])]
-                                         ).flatten() - soln['f_vals'][i])
-               < 0.00000001)
+        assert (np.linalg.norm(np.asarray([g1['sim_func'](soln['x_vals'][i]),
+                                           g2['sim_func'](soln['x_vals'][i])]
+                                          ).flatten() - soln['f_vals'][i])
+                < 0.00000001)
 
     g3 = {'m': 4,
           'hyperparams': {},
           'search': LatinHypercube,
           'sim_func': lambda x: x[0:4],
           'surrogate': LocalGaussRBF,
           'search_budget': 500,
@@ -1347,26 +998,26 @@
     moop2.updateAll(0, batch)
     batch = moop2.iterate(1)
     for (x, i) in batch:
         moop2.evaluateSimulation(x, i)
     moop2.updateAll(1, batch)
     soln = moop2.getPF()
     # Assert that solutions were found
-    assert(np.size(soln['x_vals']) > 0)
+    assert (np.size(soln['x_vals']) > 0)
     # Assert that the x_vals and f_vals match
     sim = np.zeros(4)
     for i in range(np.shape(soln['x_vals'])[0]):
         sim = soln['x_vals'][i]
-        assert(np.linalg.norm(np.asarray([f3(soln['x_vals'][i], sim),
-                                          f4(soln['x_vals'][i], sim),
-                                          f5(soln['x_vals'][i], sim)]
-                                         ).flatten()
-                              - soln['f_vals'][i])
-               < 0.00000001)
-        assert(all(soln['x_vals'][i, :4] <= 0.2))
+        assert (np.linalg.norm(np.asarray([f3(soln['x_vals'][i], sim),
+                                           f4(soln['x_vals'][i], sim),
+                                           f5(soln['x_vals'][i], sim)]
+                                          ).flatten()
+                               - soln['f_vals'][i])
+                < 0.00000001)
+        assert (all(soln['x_vals'][i, :4] <= 0.2))
 
     g4 = {'m': 4,
           'hyperparams': {},
           'search': LatinHypercube,
           'sim_func': lambda x: x[0:4] + abs(x[4] - 1.0),
           'surrogate': LocalGaussRBF,
           'search_budget': 500,
@@ -1428,26 +1079,26 @@
     moop3.updateAll(0, batch)
     batch = moop3.iterate(1)
     for (x, i) in batch:
         moop3.evaluateSimulation(x, i)
     moop3.updateAll(1, batch)
     soln = moop3.getPF()
     # Assert that solutions were found
-    assert(np.size(soln['x_vals']) > 0)
+    assert (np.size(soln['x_vals']) > 0)
     # Assert that the x_vals and f_vals match
     sim = np.zeros(4)
     for i in range(np.shape(soln['x_vals'])[0]):
         sim = soln['x_vals'][i, :4] - abs(soln['x_vals'][i, 4] - 1.0)
-        assert(np.linalg.norm(np.asarray([f6(soln['x_vals'][i], sim),
-                                          f7(soln['x_vals'][i], sim),
-                                          f8(soln['x_vals'][i], sim)]
-                                         ).flatten()
-                              - soln['f_vals'][i])
-               < 0.00000001)
-        assert(soln['x_vals'][i, 3] <= 0.1 and soln['x_vals'][i, 4] == 1.0)
+        assert (np.linalg.norm(np.asarray([f6(soln['x_vals'][i], sim),
+                                           f7(soln['x_vals'][i], sim),
+                                           f8(soln['x_vals'][i], sim)]
+                                          ).flatten()
+                               - soln['f_vals'][i])
+                < 0.00000001)
+        assert (soln['x_vals'][i, 3] <= 0.1 and soln['x_vals'][i, 4] == 1.0)
 
     x_entry = np.zeros(1, dtype=np.dtype([("x0", float), ("x1", float),
                                           ("x2", object)]))
     x_entry[0]["x2"] = "0"
     g5 = {'m': 1,
           'hyperparams': {},
           'search': LatinHypercube,
@@ -1500,33 +1151,33 @@
     moop4.updateAll(0, batch)
     batch = moop4.iterate(1)
     for (x, i) in batch:
         moop4.evaluateSimulation(x, i)
     moop4.updateAll(1, batch)
     soln = moop4.getPF()
     # Assert that solutions were found
-    assert(soln.size > 0)
+    assert (soln.size > 0)
     # Assert that the x_vals and f_vals match
     sim = np.zeros(1)
     for i, xi in enumerate(soln):
         sim[0] = ((xi["x0"] - 1.0) * (xi["x0"] - 1.0) +
                   (xi["x1"]) * (xi["x1"]) + float(xi["x2"]))
-        assert(f9(soln[i], sim) - soln['f1'][i] < 1.0e-8 and
-               f10(soln[i], sim) - soln['f2'][i] < 1.0e-8)
-        assert(xi["x2"] == "0")
+        assert (f9(soln[i], sim) - soln['f1'][i] < 1.0e-8 and
+                f10(soln[i], sim) - soln['f2'][i] < 1.0e-8)
+        assert (xi["x2"] == "0")
 
 
 def test_MOOP_solve():
     """ Test the MOOP class's solver in objectives.py.
 
     Perform a test of the MOOP solver class by minimizing a 5 variable,
     biobjective convex function s.t. $x in [0, 1]^n$.
 
-    The correctness of the solutions is difficult to assert, but we can
-    assert that the efficient points map onto the Pareto front, as
+    The correctness of the solutions is difficult to assert , but we can
+    assert  that the efficient points map onto the Pareto front, as
     expected.
 
     """
 
     from parmoo import MOOP
     from parmoo.searches import LatinHypercube
     from parmoo.surrogates import GaussRBF
@@ -1570,20 +1221,20 @@
         moop1.solve(-1)
     with pytest.raises(TypeError):
         moop1.solve(2.0)
     # Solve the MOOP with 6 iterations
     moop1.solve(6)
     soln = moop1.data
     # Assert that solutions were found
-    assert(np.size(soln['x_vals']) > 0)
+    assert (np.size(soln['x_vals']) > 0)
     # Assert that the x_vals and f_vals match
     for i in range(np.shape(soln['x_vals'])[0]):
-        assert(np.linalg.norm(np.asarray([g1['sim_func'](soln['x_vals'][i]),
-                                          g2['sim_func'](soln['x_vals'][i])]
-                                         ).flatten() - soln['f_vals'][i])
+        assert (np.linalg.norm(np.asarray([g1['sim_func'](soln['x_vals'][i]),
+                                           g2['sim_func'](soln['x_vals'][i])]
+                                          ).flatten() - soln['f_vals'][i])
                < 0.00000001)
     # Create new single objective toy problem
     g3 = {'m': 1,
           'sim_func': lambda x: [x[0] + x[1]],
           'surrogate': GaussRBF,
           'search': LatinHypercube,
           'hyperparams': {'search_budget': 10}}
@@ -1602,20 +1253,20 @@
     # Add 3 acquisition functions
     for i in range(3):
         moop2.addAcquisition({'acquisition': RandomConstraint})
     # Solve the MOOP and extract the final database with 6 iterations
     moop2.solve(6)
     soln = moop2.data
     # Assert that solutions were found
-    assert(np.size(soln['x_vals']) > 0)
+    assert (np.size(soln['x_vals']) > 0)
     # Assert that the x_vals and f_vals match
     for i in range(np.shape(soln['x_vals'])[0]):
-        assert(np.linalg.norm(np.asarray(g3['sim_func'](soln['x_vals'][i])) +
-                              np.asarray(g4['sim_func'](soln['x_vals'][i])) -
-                              soln['f_vals'][i]) < 0.00000001)
+        assert (np.linalg.norm(np.asarray(g3['sim_func'](soln['x_vals'][i])) +
+                               np.asarray(g4['sim_func'](soln['x_vals'][i])) -
+                               soln['f_vals'][i]) < 0.00000001)
 
     # Create a 3 objective toy problem, with no simulations
     moop3 = MOOP(LBFGSB, hyperparams={})
     for i in range(4):
         moop3.addDesign({'lb': 0.0, 'ub': 1.0})
 
     # Now add the three objectives
@@ -1659,24 +1310,24 @@
     # Add 3 acquisition functions
     for i in range(3):
         moop3.addAcquisition({'acquisition': UniformWeights})
     # Solve the MOOP and extract the final database with 6 iterations
     moop3.solve(6)
     soln = moop3.data
     # Assert that solutions were found
-    assert(np.size(soln['x_vals']) > 0)
+    assert (np.size(soln['x_vals']) > 0)
     # Assert that the x_vals and f_vals match
     sim = np.zeros(0)
     for i in range(np.shape(soln['x_vals'])[0]):
-        assert(np.linalg.norm(np.asarray([f4(soln['x_vals'][i], sim),
-                                          f5(soln['x_vals'][i], sim),
-                                          f6(soln['x_vals'][i], sim)]
-                                         ).flatten()
-                              - soln['f_vals'][i])
-               < 0.00000001)
+        assert (np.linalg.norm(np.asarray([f4(soln['x_vals'][i], sim),
+                                           f5(soln['x_vals'][i], sim),
+                                           f6(soln['x_vals'][i], sim)]
+                                          ).flatten()
+                               - soln['f_vals'][i])
+                < 0.00000001)
 
     # Create a 3 objective toy problem, with no simulations and 1 categorical
     moop4 = MOOP(LBFGSB, hyperparams={})
     for i in range(3):
         moop4.addDesign({'lb': 0.0, 'ub': 1.0})
     moop4.addDesign({'des_type': "categorical", 'levels': 3})
     moop4.addObjective({'obj_func': f4},
@@ -1685,24 +1336,24 @@
     # Add 3 acquisition functions
     for i in range(3):
         moop4.addAcquisition({'acquisition': UniformWeights})
     # Solve the MOOP and extract the final database with 6 iterations
     moop4.solve(6)
     soln = moop4.getPF()
     # Assert that solutions were found
-    assert(np.size(soln['x_vals']) > 0)
+    assert (np.size(soln['x_vals']) > 0)
     # Assert that the x_vals and f_vals match
     sim = np.zeros(0)
     for i in range(np.shape(soln['x_vals'])[0]):
-        assert(np.linalg.norm(np.asarray([f4(soln['x_vals'][i], sim),
+        assert (np.linalg.norm(np.asarray([f4(soln['x_vals'][i], sim),
                                           f5(soln['x_vals'][i], sim),
-                                          f6(soln['x_vals'][i], sim)]
-                                         ).flatten()
-                              - soln['f_vals'][i])
-               < 0.00000001)
+                                           f6(soln['x_vals'][i], sim)]
+                                          ).flatten()
+                               - soln['f_vals'][i])
+                < 0.00000001)
 
 
 def test_MOOP_getPF():
     """ Test the getPF function.
 
     Create several MOOPs, evaluate simulations, and check the final Pareto
     front for correctness.
@@ -1746,15 +1397,15 @@
     moop.data['f_vals'][3, :] = moop.evaluateSurrogates(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
     moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getPF()
-    assert(soln['f_vals'].shape == (4, 3))
+    assert (soln['f_vals'].shape == (4, 3))
     # Create a toy problem with 4 design variables
     moop = MOOP(LocalGPS, hyperparams={})
     for i in range(4):
         moop.addDesign({'name': ('x' + str(i+1)), 'lb': 0.0, 'ub': 1.0})
 
     # Now add three objectives
     def f1(x, sim):
@@ -1799,15 +1450,15 @@
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
     moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.data['c_vals'][4, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getPF()
-    assert(soln.shape[0] == 4)
+    assert (soln.shape[0] == 4)
 
 
 def test_MOOP_getSimulationData():
     """ Test the getSimulationData function.
 
     Create several MOOPs, evaluate simulations, and check the simulation
     database.
@@ -1846,38 +1497,38 @@
           'surrogate': GaussRBF}
     # Create a toy problem with 4 design variables
     moop = MOOP(LocalGPS, hyperparams={})
     for i in range(4):
         moop.addDesign({'lb': 0.0, 'ub': 1.0})
     moop.addSimulation(g1, g2)
     soln = moop.getSimulationData()
-    assert(soln[0]['s_vals'].size == 0)
-    assert(soln[1]['s_vals'].size == 0)
+    assert (soln[0]['s_vals'].size == 0)
+    assert (soln[1]['s_vals'].size == 0)
     # Evaluate 5 simulations
     moop.evaluateSimulation(np.asarray([0.0, 0.0, 0.0, 0.0]), 0)
     moop.evaluateSimulation(np.asarray([0.0, 0.0, 0.0, 0.0]), 1)
     moop.evaluateSimulation(np.asarray([1.0, 0.0, 0.0, 0.0]), 0)
     moop.evaluateSimulation(np.asarray([1.0, 0.0, 0.0, 0.0]), 1)
     moop.evaluateSimulation(np.asarray([0.0, 1.0, 0.0, 0.0]), 0)
     moop.evaluateSimulation(np.asarray([0.0, 1.0, 0.0, 0.0]), 1)
     moop.evaluateSimulation(np.asarray([0.0, 0.0, 1.0, 0.0]), 0)
     moop.evaluateSimulation(np.asarray([0.0, 0.0, 1.0, 0.0]), 1)
     moop.evaluateSimulation(np.asarray([0.0, 0.0, 0.0, 1.0]), 0)
     moop.evaluateSimulation(np.asarray([0.0, 0.0, 0.0, 1.0]), 1)
     soln = moop.getSimulationData()
-    assert(soln[0]['s_vals'].shape == (5, 1))
-    assert(soln[1]['s_vals'].shape == (5, 2))
+    assert (soln[0]['s_vals'].shape == (5, 1))
+    assert (soln[1]['s_vals'].shape == (5, 2))
     # Create a toy problem with 4 design variables
     moop = MOOP(LocalGPS, hyperparams={})
     for i in range(4):
         moop.addDesign({'name': ("x" + str(i + 1)), 'lb': 0.0, 'ub': 1.0})
     moop.addSimulation(g3, g4)
     soln = moop.getSimulationData()
-    assert(soln['Bobo1']['out'].size == 0)
-    assert(soln['Bobo2']['out'].size == 0)
+    assert (soln['Bobo1']['out'].size == 0)
+    assert (soln['Bobo2']['out'].size == 0)
     # Evaluate 5 simulations
     sample_x = np.zeros(1, dtype=moop.des_names)
     moop.evaluateSimulation(sample_x[0], 0)
     moop.evaluateSimulation(sample_x[0], 1)
     sample_x["x1"] = 1.0
     moop.evaluateSimulation(sample_x[0], 0)
     moop.evaluateSimulation(sample_x[0], 1)
@@ -1890,16 +1541,16 @@
     moop.evaluateSimulation(sample_x[0], 0)
     moop.evaluateSimulation(sample_x[0], 1)
     sample_x["x3"] = 0.0
     sample_x["x4"] = 1.0
     moop.evaluateSimulation(sample_x[0], 0)
     moop.evaluateSimulation(sample_x[0], 1)
     soln = moop.getSimulationData()
-    assert(soln['Bobo1']['out'].shape == (5,))
-    assert(soln['Bobo2']['out'].shape == (5, 2))
+    assert (soln['Bobo1']['out'].shape == (5,))
+    assert (soln['Bobo2']['out'].shape == (5, 2))
 
 
 def test_MOOP_getObjectiveData():
     """ Test the getObjectiveData function.
 
     Create several MOOPs, evaluate simulations, and check the objective
     database.
@@ -1953,15 +1604,15 @@
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
     moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.data['c_vals'][4, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getObjectiveData()
-    assert(soln['f_vals'].shape == (5, 3))
+    assert (soln['f_vals'].shape == (5, 3))
     # Create a toy problem with 4 design variables
     moop = MOOP(LocalGPS, hyperparams={})
     for i in range(4):
         moop.addDesign({'name': ('x' + str(i+1)), 'lb': 0.0, 'ub': 1.0})
 
     # Now add three objectives
     def f1(x, sim):
@@ -2006,15 +1657,15 @@
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
     moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.data['c_vals'][4, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getObjectiveData()
-    assert(soln.shape[0] == 5)
+    assert (soln.shape[0] == 5)
 
 
 def test_MOOP_save_load1():
     """ Check that a MOOP object can be correctly saved/reloaded.
 
     Create and save a MOOP object, then reload and check that it is the same.
 
@@ -2250,103 +1901,101 @@
         moop2 (MOOP): Second moop to compare
 
     """
 
     import numpy as np
 
     # Check scalars
-    assert(moop2.n == moop1.n and moop2.m_total == moop1.m_total and
-           moop2.o == moop1.o and moop2.p == moop1.p and
-           moop2.s == moop1.s and moop2.n_dat == moop1.n_dat and
-           moop2.n_cat_d == moop1.n_cat_d and moop2.n_cat == moop1.n_cat and
-           moop2.n_cont == moop1.n_cont and moop2.lam == moop1.lam and
-           moop2.use_names == moop1.use_names and
-           moop2.iteration == moop1.iteration)
+    assert (moop2.n == moop1.n and moop2.m_total == moop1.m_total and
+            moop2.o == moop1.o and moop2.p == moop1.p and
+            moop2.s == moop1.s and moop2.n_dat == moop1.n_dat and
+            moop2.n_cat_d == moop1.n_cat_d and moop2.n_cat == moop1.n_cat and
+            moop2.n_cont == moop1.n_cont and moop2.lam == moop1.lam and
+            moop2.use_names == moop1.use_names and
+            moop2.iteration == moop1.iteration)
     # Check lists
-    assert(all([dt2i == dt1i for dt2i, dt1i in zip(moop2.des_tols,
-                                                   moop1.des_tols)]))
-    assert(all([m2i == m1i for m2i, m1i in zip(moop2.m, moop1.m)]))
-    assert(all([lb2i == lb1i for lb2i, lb1i in zip(moop2.cont_lb,
-                                                   moop1.cont_lb)]))
-    assert(all([ub2i == ub1i for ub2i, ub1i in zip(moop2.cont_ub,
-                                                   moop1.cont_ub)]))
-    assert(all([lb2i == lb1i for lb2i, lb1i in zip(moop2.int_lb,
-                                                   moop1.int_lb)]))
-    assert(all([ub2i == ub1i for ub2i, ub1i in zip(moop2.int_ub,
-                                                   moop1.int_ub)]))
-    assert(all([nl2i == nl1i for nl2i, nl1i in zip(moop2.n_lvls,
-                                                   moop1.n_lvls)]))
-    assert(all([do2i == do1i for do2i, do1i in zip(moop2.des_order,
-                                                   moop1.des_order)]))
-    assert(all([n2i == n1i for n2i, n1i in zip(moop2.cat_names,
-                                               moop1.cat_names)]))
-    assert(all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.sim_names,
-                                                     moop1.sim_names)]))
-    assert(all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.des_names,
-                                                     moop1.des_names)]))
-    assert(all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.obj_names,
-                                                     moop1.obj_names)]))
-    assert(all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.const_names,
-                                                     moop1.const_names)]))
+    assert (all([dt2i == dt1i for dt2i, dt1i in zip(moop2.des_tols,
+                                                    moop1.des_tols)]))
+    assert (all([m2i == m1i for m2i, m1i in zip(moop2.m, moop1.m)]))
+    assert (all([lb2i == lb1i for lb2i, lb1i in zip(moop2.cont_lb,
+                                                    moop1.cont_lb)]))
+    assert (all([ub2i == ub1i for ub2i, ub1i in zip(moop2.cont_ub,
+                                                    moop1.cont_ub)]))
+    assert (all([lb2i == lb1i for lb2i, lb1i in zip(moop2.int_lb,
+                                                    moop1.int_lb)]))
+    assert (all([ub2i == ub1i for ub2i, ub1i in zip(moop2.int_ub,
+                                                    moop1.int_ub)]))
+    assert (all([nl2i == nl1i for nl2i, nl1i in zip(moop2.n_lvls,
+                                                    moop1.n_lvls)]))
+    assert (all([do2i == do1i for do2i, do1i in zip(moop2.des_order,
+                                                    moop1.des_order)]))
+    assert (all([n2i == n1i for n2i, n1i in zip(moop2.cat_names,
+                                                moop1.cat_names)]))
+    assert (all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.sim_names,
+                                                      moop1.sim_names)]))
+    assert (all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.des_names,
+                                                      moop1.des_names)]))
+    assert (all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.obj_names,
+                                                      moop1.obj_names)]))
+    assert (all([n2i[0] == n1i[0] for n2i, n1i in zip(moop2.const_names,
+                                                      moop1.const_names)]))
     # Check dictionaries
-    assert(all([ki in moop2.hyperparams.keys()
-                for ki in moop1.hyperparams.keys()]))
-    assert(all([ki in moop2.history.keys() for ki in moop1.history.keys()]))
+    assert (all([ki in moop2.hyperparams.keys()
+                 for ki in moop1.hyperparams.keys()]))
+    assert (all([ki in moop2.history.keys() for ki in moop1.history.keys()]))
     # Check np.ndarrays
-    assert(np.all(moop2.scale == np.asarray(moop1.scale)))
-    assert(np.all(moop2.scaled_lb == np.asarray(moop1.scaled_lb)))
-    assert(np.all(moop2.scaled_ub == np.asarray(moop1.scaled_ub)))
-    assert(np.all(moop2.scaled_des_tols == np.asarray(moop1.scaled_des_tols)))
-    assert(np.all(moop2.cat_lb == np.asarray(moop1.cat_lb)))
-    assert(np.all(moop2.cat_scale == np.asarray(moop1.cat_scale)))
-    assert(np.all(moop2.RSVT == np.asarray(moop1.RSVT)))
-    assert(np.all(moop2.mean == np.asarray(moop1.mean)))
-    assert(all([moop2.data[ki].shape == moop1.data[ki].shape
-                for ki in moop2.data.keys()]))
-    assert(all([all([moop2.sim_db[j][ki].shape == moop1.sim_db[j][ki].shape
-                     for ki in ["x_vals", "s_vals"]])
-                for j in range(len(moop1.sim_db))]))
+    assert (np.all(moop2.scale == np.asarray(moop1.scale)))
+    assert (np.all(moop2.scaled_lb == np.asarray(moop1.scaled_lb)))
+    assert (np.all(moop2.scaled_ub == np.asarray(moop1.scaled_ub)))
+    assert (np.all(moop2.scaled_des_tols == np.asarray(moop1.scaled_des_tols)))
+    assert (np.all(moop2.cat_lb == np.asarray(moop1.cat_lb)))
+    assert (np.all(moop2.cat_scale == np.asarray(moop1.cat_scale)))
+    assert (np.all(moop2.RSVT == np.asarray(moop1.RSVT)))
+    assert (np.all(moop2.mean == np.asarray(moop1.mean)))
+    assert (all([moop2.data[ki].shape == moop1.data[ki].shape
+                 for ki in moop2.data.keys()]))
+    assert (all([all([moop2.sim_db[j][ki].shape == moop1.sim_db[j][ki].shape
+                      for ki in ["x_vals", "s_vals"]])
+                 for j in range(len(moop1.sim_db))]))
     for obj1, obj2 in zip(moop1.objectives, moop2.objectives):
         if hasattr(obj1, "__name__"):
-            assert(obj1.__name__ == obj2.__name__)
+            assert (obj1.__name__ == obj2.__name__)
         else:
-            assert(obj1.__class__.__name__ == obj2.__class__.__name__)
+            assert (obj1.__class__.__name__ == obj2.__class__.__name__)
     for sim1, sim2 in zip(moop1.sim_funcs, moop2.sim_funcs):
         if hasattr(sim1, "__name__"):
-            assert(sim1.__name__ == sim2.__name__)
+            assert (sim1.__name__ == sim2.__name__)
         else:
-            assert(sim1.__class__.__name__ == sim2.__class__.__name__)
+            assert (sim1.__class__.__name__ == sim2.__class__.__name__)
     for const1, const2 in zip(moop1.constraints, moop2.constraints):
         if hasattr(const1, "__name__"):
-            assert(const1.__name__ == const2.__name__)
+            assert (const1.__name__ == const2.__name__)
         else:
-            assert(const1.__class__.__name__ == const2.__class__.__name__)
+            assert (const1.__class__.__name__ == const2.__class__.__name__)
     # Check functions
-    assert(moop2.optimizer.__name__ == moop1.optimizer.__name__)
-    assert(all([s1.__class__.__name__ == s2.__class__.__name__
-                for s1, s2 in zip(moop1.searches, moop2.searches)]))
-    assert(all([s1.__class__.__name__ == s2.__class__.__name__
-                for s1, s2 in zip(moop1.surrogates, moop2.surrogates)]))
-    assert(all([s1.__class__.__name__ == s2.__class__.__name__
-                for s1, s2 in zip(moop1.acquisitions, moop2.acquisitions)]))
+    assert (moop2.optimizer.__name__ == moop1.optimizer.__name__)
+    assert (all([s1.__class__.__name__ == s2.__class__.__name__
+                 for s1, s2 in zip(moop1.searches, moop2.searches)]))
+    assert (all([s1.__class__.__name__ == s2.__class__.__name__
+                 for s1, s2 in zip(moop1.surrogates, moop2.surrogates)]))
+    assert (all([s1.__class__.__name__ == s2.__class__.__name__
+                 for s1, s2 in zip(moop1.acquisitions, moop2.acquisitions)]))
 
 
 if __name__ == "__main__":
     test_MOOP_init()
     test_MOOP_addSimulation()
     test_pack_unpack_sim()
     test_MOOP_addObjective()
     test_MOOP_addConstraint()
     test_MOOP_addAcquisition()
     test_MOOP_getTypes()
     test_MOOP_evaluateSimulation()
     test_MOOP_evaluateSurrogates()
     test_MOOP_evaluateConstraints()
-    test_MOOP_evaluatePenalty()
-    test_MOOP_evaluateGradients()
     test_MOOP_addData()
     test_MOOP_iterate()
     test_MOOP_solve()
     test_MOOP_getPF()
     test_MOOP_getSimulationData()
     test_MOOP_getObjectiveData()
     test_MOOP_save_load1()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_moop_embeddings.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_moop_embeddings.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,77 +170,77 @@
 
     from parmoo import MOOP
     from parmoo.optimizers import LocalGPS
 
     # Initialize a MOOP with no hyperparameters
     moop = MOOP(LocalGPS)
     # Now add some continuous and integer design variables
-    assert(moop.n == 0)
+    assert (moop.n == 0)
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
-    assert(moop.n == 1)
+    assert (moop.n == 1)
     moop.addDesign({'des_type': "integer",
                     'lb': 0,
                     'ub': 4})
-    assert(moop.n == 2)
-    assert(moop.n_int == 1)
+    assert (moop.n == 2)
+    assert (moop.n_int == 1)
     moop.addDesign({'name': "x_3",
                     'des_type': "continuous",
                     'des_tol': 0.01,
                     'lb': 0.0,
                     'ub': 1.0})
-    assert(moop.n == 3)
+    assert (moop.n == 3)
     moop.addDesign({'lb': 0.0,
                     'ub': 1.0})
-    assert(moop.n == 4)
+    assert (moop.n == 4)
     moop.addDesign({'des_tol': 0.01,
                     'lb': 0.0,
                     'ub': 1.0})
-    assert(moop.n == 5)
+    assert (moop.n == 5)
     moop.addDesign({'name': "x_6",
                     'des_tol': 0.01,
                     'lb': 0.0,
                     'ub': 1.0})
-    assert(moop.n == 6)
+    assert (moop.n == 6)
     # Now add some categorical design variables
-    assert(moop.n_cat == 0)
+    assert (moop.n_cat == 0)
     moop.addDesign({'des_type': "categorical",
                     'levels': 2})
-    assert(moop.n_cat == 1)
+    assert (moop.n_cat == 1)
     moop.addDesign({'des_type': "categorical",
                     'levels': 3})
-    assert(moop.n_cat == 2)
+    assert (moop.n_cat == 2)
     moop.addDesign({'name': "x_9",
                     'des_type': "categorical",
                     'levels': 3})
-    assert(moop.n_cat == 3)
+    assert (moop.n_cat == 3)
     moop.addDesign({'name': "x_10",
                     'des_type': "categorical",
                     'levels': ["boy", "girl", "doggo"]})
-    assert(moop.n_cat == 4)
+    assert (moop.n_cat == 4)
     # Now add a custom design variables
     moop.addDesign({'des_type': "custom",
                     'embedding_size': 1,
                     'embedder': lambda x: x,
                     'extracter': lambda x: x})
-    assert(moop.n_custom == 1)
+    assert (moop.n_custom == 1)
     moop.addDesign({'des_type': "raw"})
-    assert(moop.n_raw == 1)
+    assert (moop.n_raw == 1)
     # Now add more continuous design variables
     moop.addDesign({'des_type': "continuous",
                     'lb': 0.0,
                     'ub': 1.0})
-    assert(moop.n_cont == 6)
+    assert (moop.n_cont == 6)
     moop.addDesign({'lb': 0.0,
                     'ub': 1.0})
-    assert(moop.n_cont == 7)
+    assert (moop.n_cont == 7)
     # Check the design order
     right_order = [0, 7, 1, 2, 3, 4, 8, 9, 10, 11, 12, 13, 5, 6]
-    assert(all([moop.des_order[i] == right_order[i] for i in range(14)]))
+    assert (all([moop.des_order[i] == right_order[i] for i in range(14)]))
 
 
 def test_MOOP_embed_extract_unnamed1():
     """ Test that the MOOP class can embed/extract unnamed design variables.
 
     Add several design variables and generate an embedding. Then embed and
     extract several inputs, and check that the results match up to the
@@ -266,77 +266,77 @@
     # Test 5 random variables
     for i in range(5):
         xi = np.random.random_sample(2)
         xi[0] *= 1000.0
         xi[1] -= 1.0
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(moop.__extract__(xxi)[0] - xi[0] <= 0.5)
-        assert(moop.__extract__(xxi)[1] - xi[1] < 1.0e-8)
+        assert (moop.__extract__(xxi)[0] - xi[0] <= 0.5)
+        assert (moop.__extract__(xxi)[1] - xi[1] < 1.0e-8)
     # Test upper and lower bounds
     x0 = np.zeros(2)
     x0[0] *= 1000.0
     x0[1] -= 1.0
     xx0 = moop.__embed__(x0)
     # Check that embedding is legal
-    assert(all(xx0 >= 0.0) and all(xx0 <= 1.0))
-    assert(xx0.size == moop.n)
+    assert (all(xx0 >= 0.0) and all(xx0 <= 1.0))
+    assert (xx0.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx0) - x0 < 1.0e-8))
+    assert (all(moop.__extract__(xx0) - x0 < 1.0e-8))
     x1 = np.ones(2)
     x1[0] *= 1000.0
     x1[1] -= 1.0
     xx1 = moop.__embed__(x1)
     # Check that embedding is legal
-    assert(all(xx1 >= 0.0) and all(xx1 <= 1.0))
-    assert(xx1.size == moop.n)
+    assert (all(xx1 >= 0.0) and all(xx1 <= 1.0))
+    assert (xx1.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx1) - x1 < 1.0e-8))
+    assert (all(moop.__extract__(xx1) - x1 < 1.0e-8))
     # Add two categorical variables and check that they embed correctly
     moop.addDesign({'des_type': "categorical",
                     'levels': 2})
     moop.addDesign({'des_type': "categorical",
                     'levels': 3})
     # Test 5 random variables
     for i in range(5):
         xi = np.random.random_sample(4)
         xi[0] *= 1000
         xi[0] = int(xi[0])
         xi[1] -= 1.0
         xi[2:] = np.round(xi[2:])
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all(moop.__extract__(xxi) - xi < 1.0e-8))
+        assert (all(moop.__extract__(xxi) - xi < 1.0e-8))
     # Test upper and lower bounds
     x0 = np.zeros(4)
     x0[0] *= 1000.0
     x0[1] -= 1.0
     x0[2:] = np.round(x0[2:])
     xx0 = moop.__embed__(x0)
     # Check that embedding is legal
-    assert(all(xx0 >= 0.0) and all(xx0 <= 1.0))
-    assert(xx0.size == moop.n)
+    assert (all(xx0 >= 0.0) and all(xx0 <= 1.0))
+    assert (xx0.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx0) - x0 < 1.0e-8))
+    assert (all(moop.__extract__(xx0) - x0 < 1.0e-8))
     x1 = np.ones(4)
     x1[0] *= 1000.0
     x1[1] -= 1.0
     x1[2:] = np.round(x1[2:])
     xx1 = moop.__embed__(x1)
     # Check that embedding is legal
-    assert(all(xx1 >= 0.0) and all(xx1 <= 1.0))
-    assert(xx1.size == moop.n)
+    assert (all(xx1 >= 0.0) and all(xx1 <= 1.0))
+    assert (xx1.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx1) - x1 < 1.0e-8))
+    assert (all(moop.__extract__(xx1) - x1 < 1.0e-8))
     # Add a custom variable and raw variable and check that they embed
     moop.addDesign({'des_type': "custom",
                     'embedding_size': 1,
                     'embedder': lambda x: x,
                     'extracter': lambda x: x})
     moop.addDesign({'des_type': "raw"})
     # Test 5 random variables
@@ -345,43 +345,43 @@
         xi[0] *= 1000
         xi[0] = int(xi[0])
         xi[1] -= 1.0
         xi[2:4] = np.round(xi[2:4])
         xi[5] *= 5.0
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi[:5] >= 0.0) and all(xxi[:5] <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi[:5] >= 0.0) and all(xxi[:5] <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all(moop.__extract__(xxi) - xi < 1.0e-8))
+        assert (all(moop.__extract__(xxi) - xi < 1.0e-8))
     # Test upper and lower bounds
     x0 = np.zeros(6)
     x0[0] *= 1000.0
     x0[1] -= 1.0
     x0[2:] = np.round(x0[2:])
     x0[2:4] = np.round(xi[2:4])
     x0[5] *= 5.0
     xx0 = moop.__embed__(x0)
     # Check that embedding is legal
-    assert(all(xx0 >= 0.0) and all(xx0 <= 1.0))
-    assert(xx0.size == moop.n)
+    assert (all(xx0 >= 0.0) and all(xx0 <= 1.0))
+    assert (xx0.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx0) - x0 < 1.0e-8))
+    assert (all(moop.__extract__(xx0) - x0 < 1.0e-8))
     x1 = np.ones(6)
     x1[0] *= 1000.0
     x1[1] -= 1.0
     x1[2:] = np.round(x1[2:])
     x1[2:4] = np.round(xi[2:4])
     x1[5] *= 5.0
     xx1 = moop.__embed__(x1)
     # Check that embedding is legal
-    assert(all(xx1[:5] >= 0.0) and all(xx1[:5] <= 1.0))
-    assert(xx1.size == moop.n)
+    assert (all(xx1[:5] >= 0.0) and all(xx1[:5] <= 1.0))
+    assert (xx1.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx1) - x1 < 1.0e-8))
+    assert (all(moop.__extract__(xx1) - x1 < 1.0e-8))
 
 
 def test_MOOP_embed_extract_unnamed2():
     """ Test that the MOOP class can embed/extract unnamed design variables.
 
     Add several design variables and generate an embedding. Then embed and
     extract several inputs, and check that the results match up to the
@@ -412,37 +412,37 @@
     # Test 5 random variables
     for i in range(5):
         xi = np.random.random_sample(4)
         xi[0] *= 0.5
         xi[2:] = np.round(xi[2:])
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all(moop.__extract__(xxi) - xi < 1.0e-8))
+        assert (all(moop.__extract__(xxi) - xi < 1.0e-8))
     # Test upper and lower bounds
     x0 = np.zeros(4)
     x0[0] *= 0.5
     x0[2:] = np.round(x0[2:])
     xx0 = moop.__embed__(x0)
     # Check that embedding is legal
-    assert(all(xx0 >= 0.0) and all(xx0 <= 1.0))
-    assert(xx0.size == moop.n)
+    assert (all(xx0 >= 0.0) and all(xx0 <= 1.0))
+    assert (xx0.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx0) - x0 < 1.0e-8))
+    assert (all(moop.__extract__(xx0) - x0 < 1.0e-8))
     x1 = np.ones(4)
     x1[0] *= 0.5
     x1[2:] = np.round(x1[2:])
     xx1 = moop.__embed__(x1)
     # Check that embedding is legal
-    assert(all(xx1 >= 0.0) and all(xx1 <= 1.0))
-    assert(xx1.size == moop.n)
+    assert (all(xx1 >= 0.0) and all(xx1 <= 1.0))
+    assert (xx1.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx1) - x1 < 1.0e-8))
+    assert (all(moop.__extract__(xx1) - x1 < 1.0e-8))
     # Add two continuous variables and check that they are embedded correctly
     moop.addDesign({'lb': -1.0,
                     'ub': 0.0})
     moop.addDesign({'des_type': "integer",
                     'lb': 0,
                     'ub': 1000})
     # Test 5 random variables
@@ -450,41 +450,41 @@
         xi = np.random.random_sample(6)
         xi[0] *= 0.5
         xi[2:4] = np.round(xi[2:4])
         xi[4] -= 1.0
         xi[5] *= 1000.0
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all(moop.__extract__(xxi) - xi < 1.0e-8))
+        assert (all(moop.__extract__(xxi) - xi < 1.0e-8))
     # Test upper and lower bounds
     x0 = np.zeros(6)
     x0[0] *= 0.5
     x0[2:4] = np.round(x0[:2])
     x0[4] -= 1.0
     x0[5] *= 1000.0
     xx0 = moop.__embed__(x0)
     # Check that embedding is legal
-    assert(all(xx0 >= 0.0) and all(xx0 <= 1.0))
-    assert(xx0.size == moop.n)
+    assert (all(xx0 >= 0.0) and all(xx0 <= 1.0))
+    assert (xx0.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx0) - x0 < 1.0e-8))
+    assert (all(moop.__extract__(xx0) - x0 < 1.0e-8))
     x1 = np.ones(6)
     x1[0] *= 0.5
     x1[2:4] = np.round(x1[2:4])
     x1[4] -= 1.0
     x1[5] *= 1000.0
     xx1 = moop.__embed__(x1)
     # Check that embedding is legal
-    assert(all(xx1 >= 0.0) and all(xx1 <= 1.0))
-    assert(xx1.size == moop.n)
+    assert (all(xx1 >= 0.0) and all(xx1 <= 1.0))
+    assert (xx1.size == moop.n)
     # Check extraction
-    assert(all(moop.__extract__(xx1) - x1 < 1.0e-8))
+    assert (all(moop.__extract__(xx1) - x1 < 1.0e-8))
 
 
 def test_MOOP_embed_extract_named1():
     """ Test that the MOOP class can embed/extract named design variables.
 
     Add several design variables and generate an embedding. Then embed and
     extract several inputs, and check that the results match up to the
@@ -513,19 +513,19 @@
     for i in range(5):
         nums = np.random.random_sample(2)
         xi = np.zeros(1, dtype=[("x0", float), ("x1", float)])
         xi["x0"] = int(1000.0 * nums[0])
         xi["x1"] = nums[1] - 1.0
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
-                    for key in ["x0", "x1"]]))
+        assert (all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
+                     for key in ["x0", "x1"]]))
     # Add two categorical variables and check that they are embedded correctly
     moop.addDesign({'name': "x2",
                     'des_type': "categorical",
                     'levels': 2})
     moop.addDesign({'name': "x3",
                     'des_type': "categorical",
                     'levels': ["biggie", "shortie", "shmedium"]})
@@ -536,20 +536,20 @@
                                 ("x3", object)])
         xi["x0"] = int(1000.0 * num[0])
         xi["x1"] = num[1] - 1.0
         xi["x2"] = np.round(num[2])
         xi["x3"] = np.random.choice(["biggie", "shortie", "shmedium"])
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
-                    for key in ["x0", "x1", "x2"]]))
-        assert(moop.__extract__(xxi)["x3"] == xi["x3"])
+        assert (all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
+                     for key in ["x0", "x1", "x2"]]))
+        assert (moop.__extract__(xxi)["x3"] == xi["x3"])
     # Add an integer variables and check that it is embedded correctly
     moop.addDesign({'name': "x4",
                     'des_type': "int",
                     'lb': -5,
                     'ub': 5})
     # Test 5 random variables
     for i in range(5):
@@ -559,20 +559,20 @@
         xi["x0"] = int(1000.0 * num[0])
         xi["x1"] = num[1] - 1.0
         xi["x2"] = np.round(num[2])
         xi["x3"] = np.random.choice(["biggie", "shortie", "shmedium"])
         xi["x4"] = np.random.randint(-5, 5)
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
-                    for key in ["x0", "x1", "x2", "x4"]]))
-        assert(moop.__extract__(xxi)["x3"] == xi["x3"])
+        assert (all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
+                     for key in ["x0", "x1", "x2", "x4"]]))
+        assert (moop.__extract__(xxi)["x3"] == xi["x3"])
     # Add a custom variable and check that it is embedded correctly
     moop.addDesign({'name': "x5",
                     'des_type': "custom",
                     'embedding_size': 1,
                     'embedder': lambda x: float(x),
                     'extracter': lambda x: str(x)})
     # Test 5 random variables
@@ -584,22 +584,22 @@
         xi["x1"] = num[1] - 1.0
         xi["x2"] = np.round(num[2])
         xi["x3"] = np.random.choice(["biggie", "shortie", "shmedium"])
         xi["x4"] = np.random.randint(-5, 5)
         xi["x5"] = str(num[5])
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
-                    for key in ["x0", "x1", "x2", "x4"]]))
-        assert(moop.__extract__(xxi)["x3"] == xi["x3"])
-        assert(abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
-               < 1.0e-8)
+        assert (all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
+                     for key in ["x0", "x1", "x2", "x4"]]))
+        assert (moop.__extract__(xxi)["x3"] == xi["x3"])
+        assert (abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
+                < 1.0e-8)
     # Add a raw variable
     moop.addDesign({'name': "x6",
                     'des_type': "raw"})
     # Test 5 random variables
     for i in range(5):
         num = np.random.random_sample(7)
         xi = np.zeros(1, dtype=[("x0", float), ("x1", float), ("x2", float),
@@ -610,22 +610,22 @@
         xi["x2"] = np.round(num[2])
         xi["x3"] = np.random.choice(["biggie", "shortie", "shmedium"])
         xi["x4"] = np.random.randint(-5, 5)
         xi["x5"] = str(num[5])
         xi["x6"] = num[6]
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
-                    for key in ["x0", "x1", "x2", "x4", "x6"]]))
-        assert(moop.__extract__(xxi)["x3"] == xi["x3"])
-        assert(abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
-               < 1.0e-8)
+        assert (all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
+                     for key in ["x0", "x1", "x2", "x4", "x6"]]))
+        assert (moop.__extract__(xxi)["x3"] == xi["x3"])
+        assert (abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
+                < 1.0e-8)
     # Add another custom variable and check that it is embedded correctly
     moop.addDesign({'name': "x7",
                     'des_type': "custom",
                     'embedding_size': 3,
                     'embedder': lambda x: [float(x[0]), float(x[1]),
                                            float(x[2])],
                     'extracter': lambda x: (str(int(x[0])) + str(int(x[1])) +
@@ -642,23 +642,23 @@
         xi["x3"] = np.random.choice(["biggie", "shortie", "shmedium"])
         xi["x4"] = np.random.randint(-5, 5)
         xi["x5"] = str(num[5])
         xi["x6"] = num[6]
         xi["x7"] = "010"
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
-                    for key in ["x0", "x1", "x2", "x4", "x6"]]))
-        assert(moop.__extract__(xxi)["x3"] == xi["x3"])
-        assert(abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
-               < 1.0e-8)
-        assert(moop.__extract__(xxi)["x7"] == xi["x7"])
+        assert (all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
+                     for key in ["x0", "x1", "x2", "x4", "x6"]]))
+        assert (moop.__extract__(xxi)["x3"] == xi["x3"])
+        assert (abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
+                < 1.0e-8)
+        assert (moop.__extract__(xxi)["x7"] == xi["x7"])
 
 
 def test_MOOP_embed_extract_named2():
     """ Test that the MOOP class can embed/extract named design variables.
 
     Add several design variables and generate an embedding. Then embed and
     extract several inputs, and check that the results match up to the
@@ -727,23 +727,23 @@
         xi["x3"] = np.random.choice(["biggie", "shortie", "shmedium"])
         xi["x4"] = np.random.randint(-5, 5)
         xi["x5"] = str(num[5])
         xi["x6"] = num[6]
         xi["x7"] = "010"
         xxi = moop.__embed__(xi)
         # Check that embedding is legal
-        assert(all(xxi >= 0.0) and all(xxi <= 1.0))
-        assert(xxi.size == moop.n)
+        assert (all(xxi >= 0.0) and all(xxi <= 1.0))
+        assert (xxi.size == moop.n)
         # Check extraction
-        assert(all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
-                    for key in ["x0", "x1", "x2", "x4", "x6"]]))
-        assert(moop.__extract__(xxi)["x3"] == xi["x3"])
-        assert(abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
-               < 1.0e-8)
-        assert(moop.__extract__(xxi)["x7"] == xi["x7"])
+        assert (all([abs(moop.__extract__(xxi)[key] - xi[key]) < 1.0e-8
+                     for key in ["x0", "x1", "x2", "x4", "x6"]]))
+        assert (moop.__extract__(xxi)["x3"] == xi["x3"])
+        assert (abs(float(moop.__extract__(xxi)["x5"]) - float(xi["x5"]))
+                < 1.0e-8)
+        assert (moop.__extract__(xxi)["x7"] == xi["x7"])
 
 
 if __name__ == "__main__":
     test_MOOP_addDesign_bad_cont()
     test_MOOP_addDesign_bad_cat()
     test_MOOP_addDesign_bad_int()
     test_MOOP_addDesign()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_obj_dtlz.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_dtlz.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,35 @@
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     # Create the objective function
     obj1 = dtlz1_obj(xtype, stype, 0, num_obj=3)
     obj2 = dtlz1_obj(xtype, stype, 1, num_obj=3)
     obj3 = dtlz1_obj(xtype, stype, 2, num_obj=3)
     # Test function evaluation
-    assert(np.abs(obj1(x, sx) - 0.0) < 1.0e-8)
-    assert(np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
-    assert(np.abs(obj3(x, sx) - 0.5) < 1.0e-8)
+    assert (np.abs(obj1(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj3(x, sx) - 0.5) < 1.0e-8)
     # Test dx evaluation
     df1x = np.zeros(1, dtype=xtype)[0]
     df2x = np.zeros(1, dtype=xtype)[0]
     df2x['x1'] = 0.5
     df3x = np.zeros(1, dtype=xtype)[0]
     df3x['x1'] = -0.5
-    assert(np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]]) < 1.0e-8
-                   for name in xtype]))
+    assert (np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]])
+                    < 1.0e-8 for name in xtype]))
     # Test ds evaluation
     dfds = np.zeros(1, dtype=stype)[0]
-    assert(np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
-    assert(np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
     dfds['sim1'] = 0.5
-    assert(np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
 
 
 def test_dtlz2_obj_named():
     """ Test the dtlz2_obj() objective function.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -61,36 +61,36 @@
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     # Create the objective function
     obj1 = dtlz2_obj(xtype, stype, 0, num_obj=3)
     obj2 = dtlz2_obj(xtype, stype, 1, num_obj=3)
     obj3 = dtlz2_obj(xtype, stype, 2, num_obj=3)
     # Test function evaluation
-    assert(np.abs(obj1(x, sx) - 1.0) < 1.0e-8)
-    assert(np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
-    assert(np.abs(obj3(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj1(x, sx) - 1.0) < 1.0e-8)
+    assert (np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj3(x, sx) - 0.0) < 1.0e-8)
     # Test dx evaluation
     df1x = np.zeros(1, dtype=xtype)[0]
     df2x = np.zeros(1, dtype=xtype)[0]
     df2x['x2'] = np.pi / 2.0
     df3x = np.zeros(1, dtype=xtype)[0]
     df3x['x1'] = np.pi / 2.0
-    assert(np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]]) < 1.0e-8
-                   for name in xtype]))
+    assert (np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]])
+                    < 1.0e-8 for name in xtype]))
     # Test ds evaluation
     dfds = np.zeros(1, dtype=stype)[0]
     dfds['sim1'] = 1.0
-    assert(np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
     dfds['sim1'] = 0.0
-    assert(np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
-    assert(np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
 
 
 def test_dtlz3_obj_named():
     """ Test the dtlz3_obj() objective function.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -107,36 +107,36 @@
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     # Create the objective function
     obj1 = dtlz3_obj(xtype, stype, 0, num_obj=3)
     obj2 = dtlz3_obj(xtype, stype, 1, num_obj=3)
     obj3 = dtlz3_obj(xtype, stype, 2, num_obj=3)
     # Test function evaluation
-    assert(np.abs(obj1(x, sx) - 1.0) < 1.0e-8)
-    assert(np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
-    assert(np.abs(obj3(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj1(x, sx) - 1.0) < 1.0e-8)
+    assert (np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj3(x, sx) - 0.0) < 1.0e-8)
     # Test dx evaluation
     df1x = np.zeros(1, dtype=xtype)[0]
     df2x = np.zeros(1, dtype=xtype)[0]
     df2x['x2'] = np.pi / 2.0
     df3x = np.zeros(1, dtype=xtype)[0]
     df3x['x1'] = np.pi / 2.0
-    assert(np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]]) < 1.0e-8
-                   for name in xtype]))
+    assert (np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]])
+                    < 1.0e-8 for name in xtype]))
     # Test ds evaluation
     dfds = np.zeros(1, dtype=stype)[0]
     dfds['sim1'] = 1.0
-    assert(np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
     dfds['sim1'] = 0.0
-    assert(np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
-    assert(np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
 
 
 def test_dtlz4_obj_named():
     """ Test the dtlz4_obj() objective function.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -153,34 +153,34 @@
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     # Create the objective function
     obj1 = dtlz4_obj(xtype, stype, 0, num_obj=3)
     obj2 = dtlz4_obj(xtype, stype, 1, num_obj=3)
     obj3 = dtlz4_obj(xtype, stype, 2, num_obj=3)
     # Test function evaluation
-    assert(np.abs(obj1(x, sx) - 1.0) < 1.0e-8)
-    assert(np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
-    assert(np.abs(obj3(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj1(x, sx) - 1.0) < 1.0e-8)
+    assert (np.abs(obj2(x, sx) - 0.0) < 1.0e-8)
+    assert (np.abs(obj3(x, sx) - 0.0) < 1.0e-8)
     # Test dx evaluation
     df1x = np.zeros(1, dtype=xtype)[0]
     df2x = np.zeros(1, dtype=xtype)[0]
     df3x = np.zeros(1, dtype=xtype)[0]
-    assert(np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]]) < 1.0e-8
-                   for name in xtype]))
-    assert(np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]]) < 1.0e-8
-                   for name in xtype]))
+    assert (np.all([np.abs(obj1(x, sx, der=1)[name[0]] - df1x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj2(x, sx, der=1)[name[0]] - df2x[name[0]])
+                    < 1.0e-8 for name in xtype]))
+    assert (np.all([np.abs(obj3(x, sx, der=1)[name[0]] - df3x[name[0]])
+                    < 1.0e-8 for name in xtype]))
     # Test ds evaluation
     dfds = np.zeros(1, dtype=stype)[0]
     dfds['sim1'] = 1.0
-    assert(np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj1(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
     dfds['sim1'] = 0.0
-    assert(np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
-    assert(np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj2(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
+    assert (np.abs(obj3(x, sx, der=2)['sim1'] - dfds['sim1']) < 1.0e-8)
 
 
 if __name__ == "__main__":
     test_dtlz1_obj_named()
     test_dtlz2_obj_named()
     test_dtlz3_obj_named()
     test_dtlz4_obj_named()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_obj_lib.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
     from parmoo.objectives import single_sim_out
     import numpy as np
 
     # Create the objective function
     obj_func = single_sim_out(3, 3, 0, goal='min')
     # Test function evaluation
-    assert(obj_func(np.zeros(3), np.eye(3)[0] * 1.5) == 1.5)
+    assert (obj_func(np.zeros(3), np.eye(3)[0] * 1.5) == 1.5)
     # Test dx evaluation
-    assert(np.all(obj_func(np.zeros(3), np.ones(3) * 4.0, der=1) ==
-                  np.zeros(3)))
+    assert (np.all(obj_func(np.zeros(3), np.ones(3) * 4.0, der=1) ==
+                   np.zeros(3)))
     # Test ds evaluation
-    assert(np.all(obj_func(np.zeros(3), np.ones(3) * 3.0, der=2) ==
-                  np.eye(3)[0]))
+    assert (np.all(obj_func(np.zeros(3), np.ones(3) * 3.0, der=2) ==
+                   np.eye(3)[0]))
 
 
 def test_single_sim_out_named1():
     """ Test the single_sim_out() objective function.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -38,21 +38,21 @@
     # Create input vectors
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     sx['sim1'] = 2.0
     # Create the objective function
     obj_func = single_sim_out(xtype, stype, 'sim1', goal='max')
     # Test function evaluation
-    assert(obj_func(x, sx) == -2.0)
+    assert (obj_func(x, sx) == -2.0)
     # Test dx evaluation
-    assert(np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_out = np.zeros(1, dtype=stype)[0]
     s_out['sim1'] = -1.0
-    assert(np.all(obj_func(x, sx, der=2) == s_out))
+    assert (np.all(obj_func(x, sx, der=2) == s_out))
 
 
 def test_single_sim_out_named2():
     """ Test the single_sim_out() objective function.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -71,21 +71,21 @@
     x = np.zeros(1, dtype=xtype)[0]
     sx = np.zeros(1, dtype=stype)[0]
     sx['sim2'][0] = 1.0
     sx['sim2'][1] = 2.0
     # Create the objective function
     obj_func = single_sim_out(xtype, stype, ('sim2', 1), goal='min')
     # Test function evaluation
-    assert(obj_func(x, sx) == 2.0)
+    assert (obj_func(x, sx) == 2.0)
     # Test dx evaluation
-    assert(np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_out = np.zeros(1, dtype=stype)[0]
     s_out['sim2'][1] = 1.0
-    assert(np.all(obj_func(x, sx, der=2) == s_out))
+    assert (np.all(obj_func(x, sx, der=2) == s_out))
 
 
 def test_sos_sim_out_unnamed():
     """ Test the sos_sim_out() objective function.
 
     Initialize an unnamed objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -94,23 +94,23 @@
 
     from parmoo.objectives import sos_sim_out
     import numpy as np
 
     # Create the objective function
     obj_func = sos_sim_out(5, 5, [0, 1, 2, 3], goal='min')
     # Test function evaluation
-    assert(np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0) - 16.0) < 1.0e-8)
+    assert (np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0) - 16.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(obj_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
-                  np.zeros(5)))
+    assert (np.all(obj_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
+                   np.zeros(5)))
     # Test ds evaluation
     s_out = np.ones(5) * 4.0
     s_out[4] = 0.0
-    assert(np.all(np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
-                         s_out) < 1.0e-8))
+    assert (np.all(np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
+                          s_out) < 1.0e-8))
 
 
 def test_sos_sim_out_named():
     """ Test the sos_sim_out() objective function.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -129,24 +129,24 @@
     sx['sim1'] = 2.0
     sx['sim2'][:] = 2.0
     # Create the objective function
     obj_func = sos_sim_out(xtype, stype,
                            ['sim1', ('sim2', 0), ('sim2', 1), ('sim2', 2)],
                            goal='max')
     # Test function evaluation
-    assert(np.abs(obj_func(x, sx) + 16.0) < 1.0e-8)
+    assert (np.abs(obj_func(x, sx) + 16.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_out = np.zeros(1, dtype=stype)[0]
     s_out['sim1'] = sx['sim1'] * -2.0
     s_out['sim2'][:-1] = sx['sim2'][:-1] * -2.0
-    assert(np.abs(obj_func(x, sx, der=2)['sim1'] - s_out['sim1']) < 1.0e-8)
-    assert(np.all(np.abs(obj_func(x, sx, der=2)['sim2'] - s_out['sim2'])
-                  < 1.0e-8))
+    assert (np.abs(obj_func(x, sx, der=2)['sim1'] - s_out['sim1']) < 1.0e-8)
+    assert (np.all(np.abs(obj_func(x, sx, der=2)['sim2'] - s_out['sim2'])
+                   < 1.0e-8))
 
 
 def test_sum_sim_out_unnamed():
     """ Test the sum_sim_out() objective function.
 
     Initialize an unnamed objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -155,21 +155,21 @@
 
     from parmoo.objectives import sum_sim_out
     import numpy as np
 
     # Create the objective function
     obj_func = sum_sim_out(5, 5, [0, 1, 2, 3], goal='min')
     # Test function evaluation
-    assert(np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0) - 8.0) < 1.0e-8)
+    assert (np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0) - 8.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(obj_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
-                  np.zeros(5)))
+    assert (np.all(obj_func(np.zeros(5), np.ones(5) * 2.0, der=1) ==
+                   np.zeros(5)))
     # Test ds evaluation
-    assert(np.all(np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
-                         (np.ones(5) - np.eye(5)[4])) < 1.0e-8))
+    assert (np.all(np.abs(obj_func(np.zeros(5), np.ones(5) * 2.0, der=2) -
+                          (np.ones(5) - np.eye(5)[4])) < 1.0e-8))
 
 
 def test_sum_sim_out_named():
     """ Test the sum_sim_out() objective function.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -188,25 +188,25 @@
     sx['sim1'] = 2.0
     sx['sim2'][:] = 2.0
     # Create the objective function
     obj_func = sum_sim_out(xtype, stype,
                            ['sim1', ('sim2', 0), ('sim2', 1), ('sim2', 2)],
                            goal='max')
     # Test function evaluation
-    assert(np.abs(obj_func(x, sx) + 8.0) < 1.0e-8)
+    assert (np.abs(obj_func(x, sx) + 8.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_out = np.ones(1, dtype=stype)[0]
     s_out['sim1'] *= -1.0
     s_out['sim2'][:] *= -1.0
     s_out['sim2'][3] = 0.0
-    assert(np.abs(obj_func(x, sx, der=2)['sim1'] - s_out['sim1']) < 1.0e-8)
-    assert(np.all(np.abs(obj_func(x, sx, der=2)['sim2'] - s_out['sim2'])
-                  < 1.0e-8))
+    assert (np.abs(obj_func(x, sx, der=2)['sim1'] - s_out['sim1']) < 1.0e-8)
+    assert (np.all(np.abs(obj_func(x, sx, der=2)['sim2'] - s_out['sim2'])
+                   < 1.0e-8))
 
 
 def test_sum_sim_out_named_abs():
     """ Test the sum_sim_out() objective function with "absolute=True" option.
 
     Initialize a named objective, then evaluate the function value and
     derivative with respect to x and sx.
@@ -225,24 +225,24 @@
     sx['sim1'] = 2.0
     sx['sim2'][:] = -2.0
     # Create the objective function
     obj_func = sum_sim_out(xtype, stype,
                            ['sim1', ('sim2', 0), ('sim2', 1), ('sim2', 2)],
                            goal='min', absolute=True)
     # Test function evaluation
-    assert(np.abs(obj_func(x, sx) - 8.0) < 1.0e-8)
+    assert (np.abs(obj_func(x, sx) - 8.0) < 1.0e-8)
     # Test dx evaluation
-    assert(np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
+    assert (np.all(obj_func(x, sx, der=1) == np.zeros(1, dtype=xtype)[0]))
     # Test ds evaluation
     s_out = np.zeros(1, dtype=stype)[0]
     s_out['sim1'] = 1.0
     s_out['sim2'][:-1] = -1.0
-    assert(np.abs(obj_func(x, sx, der=2)['sim1'] - s_out['sim1']) < 1.0e-8)
-    assert(np.all(np.abs(obj_func(x, sx, der=2)['sim2'] - s_out['sim2'])
-                  < 1.0e-8))
+    assert (np.abs(obj_func(x, sx, der=2)['sim1'] - s_out['sim1']) < 1.0e-8)
+    assert (np.all(np.abs(obj_func(x, sx, der=2)['sim2'] - s_out['sim2'])
+                   < 1.0e-8))
 
 
 if __name__ == "__main__":
     test_single_sim_out_unnamed()
     test_single_sim_out_named1()
     test_single_sim_out_named2()
     test_sos_sim_out_unnamed()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_random_search.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_random_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
     x2_soln = np.eye(n)[1]
     x2_soln[n-1] = 0.1
     # eps is the tolerance for rejecting a solution as incorrect
     eps = 0.25
     # Check that the computed solutions are within eps of the truth
-    assert(np.linalg.norm(x1 - x1_soln) < eps)
-    assert(np.linalg.norm(x2 - x2_soln) < eps)
-    assert(np.abs(x3[n-1] - 0.1) < eps)
+    assert (np.linalg.norm(x1 - x1_soln) < eps)
+    assert (np.linalg.norm(x2 - x2_soln) < eps)
+    assert (np.abs(x3[n-1] - 0.1) < eps)
     return
 
 
 if __name__ == "__main__":
     test_RandomSearch()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_sims_dtlz.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_sims_dtlz.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,141 +6,141 @@
 
     """
 
     from parmoo.simulations.dtlz import g1_sim
     import numpy as np
 
     g1 = g1_sim(5, num_obj=3, offset=0.6)
-    assert(np.abs(g1(np.ones(5) * 0.6)) < 1.0e-8)
+    assert (np.abs(g1(np.ones(5) * 0.6)) < 1.0e-8)
 
 
 def test_sims_dtlz_g2():
     """ Test the g2 kernel function.
 
     Create an instance of g2 and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import g2_sim
     import numpy as np
 
     g2 = g2_sim(5, num_obj=3, offset=0.6)
-    assert(np.abs(g2(np.ones(5) * 0.6)) < 1.0e-8)
+    assert (np.abs(g2(np.ones(5) * 0.6)) < 1.0e-8)
 
 
 def test_sims_dtlz_g3():
     """ Test the g3 kernel function.
 
     Create an instance of g3 and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import g3_sim
     import numpy as np
 
     g3 = g3_sim(5, num_obj=3, offset=0.6)
-    assert(np.abs(g3(np.ones(5) * 0.6)) < 1.0e-8)
+    assert (np.abs(g3(np.ones(5) * 0.6)) < 1.0e-8)
 
 
 def test_sims_dtlz_g4():
     """ Test the g4 kernel function.
 
     Create an instance of g4 and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import g4_sim
     import numpy as np
 
     g4 = g4_sim(5, num_obj=3, offset=0.6)
-    assert(np.abs(g4(np.ones(5) * 0.6) - 1.0) < 1.0e-8)
+    assert (np.abs(g4(np.ones(5) * 0.6) - 1.0) < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz1():
     """ Test the dtlz1 simulation function.
 
     Create an instance of dtlz1_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz1_sim
     import numpy as np
 
     dtlz1 = dtlz1_sim(5, num_obj=3, offset=0.6)
-    assert(sum(dtlz1(np.ones(5) * 0.6)) - 0.5 < 1.0e-8)
+    assert (sum(dtlz1(np.ones(5) * 0.6)) - 0.5 < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz2():
     """ Test the dtlz2 simulation function.
 
     Create an instance of dtlz2_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz2_sim
     import numpy as np
 
     dtlz2 = dtlz2_sim(5, num_obj=3, offset=0.6)
-    assert(np.linalg.norm(dtlz2(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
+    assert (np.linalg.norm(dtlz2(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz3():
     """ Test the dtlz3 simulation function.
 
     Create an instance of dtlz3_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz3_sim
     import numpy as np
 
     dtlz3 = dtlz3_sim(5, num_obj=3, offset=0.6)
-    assert(np.linalg.norm(dtlz3(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
+    assert (np.linalg.norm(dtlz3(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz4():
     """ Test the dtlz4 simulation function.
 
     Create an instance of dtlz4_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz4_sim
     import numpy as np
 
     dtlz4 = dtlz4_sim(5, num_obj=3, offset=0.6)
-    assert(np.linalg.norm(dtlz4(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
+    assert (np.linalg.norm(dtlz4(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz5():
     """ Test the dtlz5 simulation function.
 
     Create an instance of dtlz5_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz5_sim
     import numpy as np
 
     dtlz5 = dtlz5_sim(5, num_obj=3, offset=0.6)
-    assert(np.linalg.norm(dtlz5(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
+    assert (np.linalg.norm(dtlz5(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz6():
     """ Test the dtlz6 simulation function.
 
     Create an instance of dtlz6_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz6_sim
     import numpy as np
 
     dtlz6 = dtlz6_sim(5, num_obj=3, offset=0.6)
-    assert(np.linalg.norm(dtlz6(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
+    assert (np.linalg.norm(dtlz6(np.ones(5) * 0.6)) - 1.0 < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz7():
     """ Test the dtlz7 simulation function.
 
     Create an instance of dtlz7_sim and check that its output is correct.
 
@@ -148,43 +148,43 @@
 
     from parmoo.simulations.dtlz import dtlz7_sim
     import numpy as np
 
     dtlz7 = dtlz7_sim(5, num_obj=3, offset=0.6)
     x_in = np.ones(5) * 0.6
     x_in[:2] = 0.0
-    assert(np.abs(dtlz7(x_in)[2] - 6.0) < 1.0e-8)
+    assert (np.abs(dtlz7(x_in)[2] - 6.0) < 1.0e-8)
 
 
 def test_sims_dtlz_dtlz8():
     """ Test the dtlz8 simulation function.
 
     Create an instance of dtlz8_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz8_sim
     import numpy as np
 
     dtlz8 = dtlz8_sim(5, num_obj=3, offset=0.6)
-    assert(np.all(np.abs(dtlz8(np.ones(5) * 0.6)) < 1.0e-8))
+    assert (np.all(np.abs(dtlz8(np.ones(5) * 0.6)) < 1.0e-8))
 
 
 def test_sims_dtlz_dtlz9():
     """ Test the dtlz9 simulation function.
 
     Create an instance of dtlz9_sim and check that its output is correct.
 
     """
 
     from parmoo.simulations.dtlz import dtlz9_sim
     import numpy as np
 
     dtlz9 = dtlz9_sim(5, num_obj=3, offset=0.6)
-    assert(np.all(np.abs(dtlz9(np.ones(5) * 0.6)) < 1.0e-8))
+    assert (np.all(np.abs(dtlz9(np.ones(5) * 0.6)) < 1.0e-8))
 
 
 if __name__ == "__main__":
     test_sims_dtlz_g1()
     test_sims_dtlz_g2()
     test_sims_dtlz_g3()
     test_sims_dtlz_g4()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_structs.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_util.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,30 +136,30 @@
 
     """
 
     from parmoo.util import lex_leq
     import numpy as np
 
     # Check for a < b
-    assert(lex_leq(np.zeros(3), np.ones(3)))
-    assert(lex_leq(np.zeros(3), np.asarray([0.1, 0.0, 0.0])))
-    assert(lex_leq(np.asarray([100.0, 0.0]), np.asarray([0.0, 0.1])))
-    assert(lex_leq(np.zeros(1), np.ones(1)))
+    assert (lex_leq(np.zeros(3), np.ones(3)))
+    assert (lex_leq(np.zeros(3), np.asarray([0.1, 0.0, 0.0])))
+    assert (lex_leq(np.asarray([100.0, 0.0]), np.asarray([0.0, 0.1])))
+    assert (lex_leq(np.zeros(1), np.ones(1)))
     # Check for a = b
-    assert(lex_leq(np.zeros(3), np.zeros(3)))
-    assert(lex_leq(np.ones(1), np.ones(1)))
+    assert (lex_leq(np.zeros(3), np.zeros(3)))
+    assert (lex_leq(np.ones(1), np.ones(1)))
     # Check for a > b
-    assert(not lex_leq(np.ones(3), np.zeros(3)))
-    assert(not lex_leq(np.ones(1), np.zeros(1)))
-    assert(not lex_leq(np.asarray([0.1, 0.0, 0.0]), np.zeros(3)))
-    assert(not lex_leq(np.asarray([0.0, 0.1]), np.asarray([1.0, 0.0])))
+    assert (not lex_leq(np.ones(3), np.zeros(3)))
+    assert (not lex_leq(np.ones(1), np.zeros(1)))
+    assert (not lex_leq(np.asarray([0.1, 0.0, 0.0]), np.zeros(3)))
+    assert (not lex_leq(np.asarray([0.0, 0.1]), np.asarray([1.0, 0.0])))
     # Check for mismatched dimensions
-    assert(lex_leq(np.zeros(3), np.zeros(4)))
-    assert(lex_leq(np.zeros(4), np.zeros(3)))
-    assert(lex_leq(np.zeros(1), np.zeros(1)))
+    assert (lex_leq(np.zeros(3), np.zeros(4)))
+    assert (lex_leq(np.zeros(4), np.zeros(3)))
+    assert (lex_leq(np.zeros(1), np.zeros(1)))
 
 
 def test_updatePF():
     """ Test the updatePF function.
 
     Perform a test of the updatePF() function by extracting the Pareto front
     from a 3 objective problem with a 5 point database. Then perform an
@@ -206,35 +206,35 @@
     data['f_vals'][9, :] = obj(np.asarray([1.0, 0.0, 0.0, 0.0]))
     # Extract the Pareto front for the first 5 points
     soln = {}
     def NoConstraints(x): return np.asarray([])
     soln = updatePF({'x_vals': data['x_vals'][:5, :],
                      'f_vals': data['f_vals'][:5, :],
                      'c_vals': data['c_vals'][:5, :]}, soln)
-    assert(soln['f_vals'].shape == (4, 3))
+    assert (soln['f_vals'].shape == (4, 3))
     # Update the Pareto front with the last 5 points
     soln = updatePF({'x_vals': data['x_vals'][5:, :],
                      'f_vals': data['f_vals'][5:, :],
                      'c_vals': data['c_vals'][:5, :]}, soln)
-    assert(soln['f_vals'].shape == (5, 3))
+    assert (soln['f_vals'].shape == (5, 3))
     # Add a constraint and re-filter
     def Constraints(x): return np.asarray([0.1 - obj(x)[0]])
     for i in range(10):
         data['c_vals'][i, :] = Constraints(data['x_vals'][i, :])
     # Extract the Pareto front for the first 5 points
     soln = {}
     soln = updatePF({'x_vals': data['x_vals'][:5, :],
                      'f_vals': data['f_vals'][:5, :],
                      'c_vals': data['c_vals'][:5, :]}, soln)
-    assert(soln['f_vals'].shape == (3, 3))
+    assert (soln['f_vals'].shape == (3, 3))
     # Update the Pareto front with the last 5 points
     soln = updatePF({'x_vals': data['x_vals'][5:, :],
                      'f_vals': data['f_vals'][5:, :],
                      'c_vals': data['c_vals'][5:, :]}, soln)
-    assert(soln['f_vals'].shape == (4, 3))
+    assert (soln['f_vals'].shape == (4, 3))
 
 
 def test_unpack():
     """ Test the unpack function.
 
     Create a named and unnamed output, and try to unpack each.
 
@@ -258,17 +258,17 @@
     with pytest.raises(TypeError):
         unpack(x_unnamed, dt_bad)
     with pytest.raises(TypeError):
         unpack(x_unnamed, dt_named)
     with pytest.raises(TypeError):
         unpack(x_unnamed, [("x4", "f8")])
     # Test unnamed unpack
-    assert(np.all(x_unnamed == unpack(x_unnamed, dt_unnamed)))
+    assert (np.all(x_unnamed == unpack(x_unnamed, dt_unnamed)))
     # Test named unpack
-    assert(np.all(x_unnamed == unpack(x_named, dt_named)))
+    assert (np.all(x_unnamed == unpack(x_named, dt_named)))
 
 
 if __name__ == "__main__":
     test_xerror()
     test_check_sims()
     test_lex_leq()
     test_updatePF()
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_viz_without_dash.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_viz_without_dash.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,40 +14,40 @@
     import os
 
     # Pre-calculate a moop object
     moop1 = run_quickstart()
 
     # * html output
     scatter(moop1, output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * svg output
     parallel_coordinates(moop1, output='svg')
-    assert(os.path.exists("Pareto Front.svg"))
+    assert (os.path.exists("Pareto Front.svg"))
     os.remove("Pareto Front.svg")
 
     # * pdf output
     radar(moop1, output='pdf')
-    assert(os.path.exists("Pareto Front.pdf"))
+    assert (os.path.exists("Pareto Front.pdf"))
     os.remove("Pareto Front.pdf")
 
     # * jpeg output
     scatter(moop1, output='jpeg')
-    assert(os.path.exists("Pareto Front.jpeg"))
+    assert (os.path.exists("Pareto Front.jpeg"))
     os.remove("Pareto Front.jpeg")
 
     # * png output
     parallel_coordinates(moop1, output='png')
-    assert(os.path.exists("Pareto Front.png"))
+    assert (os.path.exists("Pareto Front.png"))
     os.remove("Pareto Front.png")
 
     # * webp output
     radar(moop1, output='webp')
-    assert(os.path.exists("Pareto Front.webp"))
+    assert (os.path.exists("Pareto Front.webp"))
     os.remove("Pareto Front.webp")
 
 
 def test_quantity_constraints_objectives():
     """ Create a MOOP object and plot PF with and w/o constraint data. """
 
     from parmoo.viz.plot import (
@@ -59,40 +59,40 @@
 
     # Pre-calculate two moop objects
     moop1 = run_quickstart()
     moop2 = run_dtlz2()
 
     # * 2 objective scatter with constraint
     scatter(moop1, output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * 2 objective parallel with constraint
     parallel_coordinates(moop1, output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * 2 objective radar with constraint
     radar(moop1, output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * 5 objective scatter without constraint
     scatter(moop2, output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * 5 objective parallel without constraint
     parallel_coordinates(moop2, output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * 5 objective radar without constraint
     radar(moop2, output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
 
 def test_database_options():
     """ Create a MOOP object and plot the full database.
 
     Generates plots with and without constraint violations.
@@ -112,406 +112,406 @@
 
     # * pf x constraint_satisfying x constraints in MOOP
     scatter(
         moop1,
         db='pf',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop1,
         db='pf',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop1,
         db='pf',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x constraint_satisfying x constraints in MOOP
     scatter(
         moop1,
         db='obj',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop1,
         db='obj',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop1,
         db='obj',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     # * pf x constraint_violating x constraints in MOOP
     scatter(
         moop1,
         db='pf',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop1,
         db='pf',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop1,
         db='pf',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x constraint_violating x constraints in MOOP
     scatter(
         moop1,
         db='obj',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop1,
         db='obj',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop1,
         db='obj',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     # * pf x all x constraints in MOOP
     scatter(
         moop1,
         db='pf',
         points='all',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop1,
         db='pf',
         points='all',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop1,
         db='pf',
         points='all',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x all x constraints in MOOP
     scatter(
         moop1,
         db='obj',
         points='all',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop1,
         db='obj',
         points='all',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop1,
         db='obj',
         points='all',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     # * pf x none x constraints in MOOP
     scatter(
         moop1,
         db='pf',
         points='none',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop1,
         db='pf',
         points='none',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop1,
         db='pf',
         points='none',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x none x constraints in MOOP
     scatter(
         moop1,
         db='obj',
         points='none',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop1,
         db='obj',
         points='none',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop1,
         db='obj',
         points='none',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     # * pf x constraint_satisfying x no constraints in MOOP
     scatter(
         moop2,
         db='pf',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop2,
         db='pf',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop2,
         db='pf',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x constraint_satisfying x no constraints in MOOP
     scatter(
         moop2,
         db='obj',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop2,
         db='obj',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop2,
         db='obj',
         points='constraint_satisfying',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     # * pf x constraint_violating x no constraints in MOOP
     scatter(
         moop2,
         db='pf',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop2,
         db='pf',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop2,
         db='pf',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x constraint_violating x no constraints in MOOP
     scatter(
         moop2,
         db='obj',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop2,
         db='obj',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop2,
         db='obj',
         points='constraint_violating',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     # * pf x all x no constraints in MOOP
     scatter(
         moop2,
         db='pf',
         points='all',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop2,
         db='pf',
         points='all',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop2,
         db='pf',
         points='all',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x all x no constraints in MOOP
     scatter(
         moop2,
         db='obj',
         points='all',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop2,
         db='obj',
         points='all',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop2,
         db='obj',
         points='all',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     # * pf x none x no constraints in MOOP
     scatter(
         moop2,
         db='pf',
         points='none',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     parallel_coordinates(
         moop2,
         db='pf',
         points='none',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     radar(
         moop2,
         db='pf',
         points='none',
         output='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # * obj x none x no constraints in MOOP
     scatter(
         moop2,
         db='obj',
         points='none',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     parallel_coordinates(
         moop2,
         db='obj',
         points='none',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
     radar(
         moop2,
         db='obj',
         points='none',
         output='html')
-    assert(os.path.exists("Objective Data.html"))
+    assert (os.path.exists("Objective Data.html"))
     os.remove("Objective Data.html")
 
 
 def test_inputs_to_dash():
     """ Stress-test the dash app's error handling. """
 
     from parmoo.viz.plot import scatter
@@ -547,236 +547,236 @@
 
     with pytest.raises(ValueError):
         scatter(moop1, output='html', points=1234)
 
     # * height
     # test valid height values
     scatter(moop1, output='html', height=1)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', height=50)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', height=92.2678)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', height=7789)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid height values
     with pytest.raises(ValueError):
         scatter(moop1, output='html', height='asdf')
 
     # * width
     # test valid width values
     scatter(moop1, output='html', width=1)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', width=50)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', width=92.2678)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', width=7789)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid width values
     with pytest.raises(ValueError):
         scatter(moop1, output='html', width='asdf')
 
     # * font
     # test valid font values
     scatter(moop1, output='html', font='Verdana')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', font='Times New Roman')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid font values
     # currently all inputs that can be cast to a string are valid
     # if str(font) != a font in the computer, font=Times New Roman
 
     # * fontsize
     # test valid fontsize values
     scatter(moop1, output='html', fontsize=1)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', fontsize=50)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', fontsize=55.71)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', fontsize=100)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid fontsize values
     with pytest.raises(ValueError):
         scatter(moop1, output='html', fontsize=-1)
 
     with pytest.raises(ValueError):
         scatter(moop1, output='html', fontsize=101)
 
     # * background_color
     # test valid background_color values
     scatter(moop1, output='html', background_color='white')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', background_color='black')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(
         moop1,
         output='html',
         background_color='transparent'
     )
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', background_color='white')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', background_color='grey')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid background_color values
     # currently all inputs that can be cast to a string are valid
     # if str(background_color) != a supported background_color
     # background_color=white
 
     # * screenshot
     # test valid screenshot values
     scatter(moop1, output='html', screenshot='png')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', screenshot='jpeg')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', screenshot='svg')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', screenshot='webp')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid screenshot values
     with pytest.raises(ValueError):
         scatter(moop1, output='html', screenshot='asdf')
 
     with pytest.raises(ValueError):
         scatter(moop1, output='html', screenshot=1234)
 
     # * image_export_format
     # test valid image_export_format values (except eps)
     scatter(moop1, output='html', image_export_format='html')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', image_export_format='svg')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', image_export_format='pdf')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', image_export_format='png')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', image_export_format='jpeg')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', image_export_format='webp')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid image_export_format values
     with pytest.raises(ValueError):
         scatter(moop1, output='html', image_export_format='asdf')
 
     with pytest.raises(ValueError):
         scatter(moop1, output='html', image_export_format=1234)
 
     # * data_export_format
     # test valid data_export_format values
     scatter(moop1, output='html', data_export_format='csv')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', data_export_format='json')
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid data_export_format values
     with pytest.raises(ValueError):
         scatter(moop1, output='html', data_export_format='asdf')
 
     with pytest.raises(ValueError):
         scatter(moop1, output='html', data_export_format=1234)
 
     # * dev_mode
     # test valid dev_mode values
     scatter(moop1, output='html', dev_mode=True)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', dev_mode=False)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid dev_mode values
     # currently all inputs that can be cast to a boolean are valid
     # in Python, everything can be cast to a boolean
 
     # * pop_up
     # test valid pop_up values
     scatter(moop1, output='html', pop_up=True)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     scatter(moop1, output='html', pop_up=False)
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid pop_up values
     # currently all inputs that can be cast to a boolean are valid
     # in Python, everything can be cast to a boolean
 
     # * port
     # test valid port values
     scatter(
         moop1,
         output='html',
         port='http://127.0.0.1:8050/'
     )
-    assert(os.path.exists("Pareto Front.html"))
+    assert (os.path.exists("Pareto Front.html"))
     os.remove("Pareto Front.html")
 
     # test invalid port values
     with pytest.raises(ValueError):
         scatter(moop1, output='html', port='asdf')
 
     with pytest.raises(ValueError):
```

### Comparing `parmoo-0.2.0/parmoo/tests/unit_tests/test_weighted_sum.py` & `parmoo-0.2.1/parmoo/tests/unit_tests/test_weighted_sum.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     from parmoo.acquisitions import UniformWeights
     import numpy as np
     import pytest
 
     # Initilaize a good acquisition for future testing
     acqu = UniformWeights(3, np.zeros(4), np.ones(4), {})
-    assert(np.all(acqu.lb[:] == 0.0) and np.all(acqu.ub[:] == 1.0))
+    assert (np.all(acqu.lb[:] == 0.0) and np.all(acqu.ub[:] == 1.0))
     # Set some bad targets to check error handling
     with pytest.raises(TypeError):
         acqu.setTarget(5, lambda x: np.zeros(3), {})
     with pytest.raises(AttributeError):
         acqu.setTarget({'x_vals': []}, lambda x: np.zeros(3), {})
     with pytest.raises(ValueError):
         acqu.setTarget({'x_vals': np.ones(1), 'f_vals': np.ones(2)},
@@ -30,56 +30,59 @@
                        lambda x: np.zeros(3), {})
     with pytest.raises(TypeError):
         acqu.setTarget({}, 4, {})
     with pytest.raises(ValueError):
         acqu.setTarget({}, lambda x, y: np.zeros(3), {})
     # Set a good target for future usage
     x0 = acqu.setTarget({}, lambda x: np.zeros(3), {})
-    assert(abs(sum(acqu.weights) - 1.0) < 0.00000001)
-    assert(np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
+    assert (abs(sum(acqu.weights) - 1.0) < 0.00000001)
+    assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     # Try some bad scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarize(5)
     with pytest.raises(ValueError):
         acqu.scalarize(np.ones(2))
     # Generate 3 random weight vector
     acqu1 = UniformWeights(3, np.zeros(4), np.ones(4), {})
     acqu1.setTarget({}, lambda x: np.zeros(3), {})
     acqu2 = UniformWeights(3, np.zeros(4), np.ones(4), {})
     acqu2.setTarget({}, lambda x: np.zeros(3), {})
     acqu3 = UniformWeights(3, np.zeros(4), np.ones(4), {})
     acqu3.setTarget({'x_vals': None, 'f_vals': None},
                     lambda x: np.zeros(3), {})
     # Check that the weights are all greater than 0
-    assert(all(acqu1.weights[:] >= 0.0))
-    assert(all(acqu2.weights[:] >= 0.0))
-    assert(all(acqu3.weights[:] >= 0.0))
+    assert (all(acqu1.weights[:] >= 0.0))
+    assert (all(acqu2.weights[:] >= 0.0))
+    assert (all(acqu3.weights[:] >= 0.0))
     # Use the scalarization function to check that the weights sum to 1
-    assert(np.abs(acqu1.scalarize(np.eye(3)[0]) + acqu1.scalarize(np.eye(3)[1])
-                  + acqu1.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
-    assert(np.abs(acqu2.scalarize(np.eye(3)[0]) + acqu2.scalarize(np.eye(3)[1])
-                  + acqu2.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
-    assert(np.abs(acqu3.scalarize(np.eye(3)[0]) + acqu3.scalarize(np.eye(3)[1])
-                  + acqu3.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
+    assert (np.abs(acqu1.scalarize(np.eye(3)[0])
+                   + acqu1.scalarize(np.eye(3)[1])
+                   + acqu1.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
+    assert (np.abs(acqu2.scalarize(np.eye(3)[0])
+                   + acqu2.scalarize(np.eye(3)[1])
+                   + acqu2.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
+    assert (np.abs(acqu3.scalarize(np.eye(3)[0])
+                   + acqu3.scalarize(np.eye(3)[1])
+                   + acqu3.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
     # Try some bad gradient scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(5, np.zeros((3, 4))[0])
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.ones(2), np.zeros((3, 4)))
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(np.eye(3)[0], 5)
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.eye(3)[0], np.zeros((2, 4)))
     # Use the gradient scalarization to check that the weights sum to 1
-    assert(np.abs(np.sum(acqu1.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
-                  - 1.0) < 0.00000001)
-    assert(np.abs(np.sum(acqu2.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
-                  - 1.0) < 0.00000001)
-    assert(np.abs(np.sum(acqu3.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
-                  - 1.0) < 0.00000001)
+    assert (np.abs(np.sum(acqu1.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
+                   - 1.0) < 0.00000001)
+    assert (np.abs(np.sum(acqu2.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
+                   - 1.0) < 0.00000001)
+    assert (np.abs(np.sum(acqu3.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
+                   - 1.0) < 0.00000001)
     return
 
 
 def test_FixedWeights():
     """ Test the FixedWeights class in acquisitions.py.
 
     Use the FixedWeights class to try 2 sets of fixed convex weights
@@ -94,18 +97,18 @@
     # Try some bad initializations to test error handling
     with pytest.raises(TypeError):
         FixedWeights(3, np.zeros(4), np.ones(4), {'weights': 5.0})
     with pytest.raises(ValueError):
         FixedWeights(3, np.zeros(4), np.ones(4), {'weights': np.ones(2)})
     # Initilaize a good acquisition for future testing
     acqu = FixedWeights(3, np.zeros(4), np.ones(4), {'weights': np.ones((3))})
-    assert(np.all(acqu.lb[:] == 0.0) and np.all(acqu.ub[:] == 1.0))
+    assert (np.all(acqu.lb[:] == 0.0) and np.all(acqu.ub[:] == 1.0))
     acqu = FixedWeights(3, np.zeros(4), np.ones(4), {})
-    assert(np.all(acqu.lb[:] == 0.0) and np.all(acqu.ub[:] == 1.0))
-    assert(np.all(acqu.weights[:] - (1.0 / 3.0) < 0.00000001))
+    assert (np.all(acqu.lb[:] == 0.0) and np.all(acqu.ub[:] == 1.0))
+    assert (np.all(acqu.weights[:] - (1.0 / 3.0) < 0.00000001))
     # Set some bad targets to check error handling
     with pytest.raises(TypeError):
         acqu.setTarget(5, lambda x: np.zeros(3), {})
     with pytest.raises(AttributeError):
         acqu.setTarget({'x_vals': []}, lambda x: np.zeros(3), {})
     with pytest.raises(ValueError):
         acqu.setTarget({'x_vals': np.ones(1), 'f_vals': np.ones(2)},
@@ -119,41 +122,41 @@
     with pytest.raises(TypeError):
         acqu.setTarget({}, 4, {})
     with pytest.raises(ValueError):
         acqu.setTarget({}, lambda x, y: np.zeros(3), {})
     # Set some good targets
     x0 = acqu.setTarget({'x_vals': None, 'f_vals': None},
                         lambda x: np.zeros(3), {})
-    assert(np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
+    assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     x0 = acqu.setTarget({'x_vals': np.zeros((1, 4)),
                          'f_vals': np.zeros((1, 3)),
                          'c_vals': np.zeros((1, 1))},
                         lambda x: np.zeros(3), {})
-    assert(np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
+    assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     x0 = acqu.setTarget({}, lambda x: np.zeros(3), {})
-    assert(np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
+    assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     # Try some bad scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarize(5)
     with pytest.raises(ValueError):
         acqu.scalarize(np.ones(2))
     # Use the scalarization function to check that the weights sum to 1
-    assert(np.abs(acqu.scalarize(np.eye(3)[0]) + acqu.scalarize(np.eye(3)[1])
-                  + acqu.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
+    assert (np.abs(acqu.scalarize(np.eye(3)[0]) + acqu.scalarize(np.eye(3)[1])
+                   + acqu.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
     # Try some bad gradient scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(5, np.zeros((3, 4))[0])
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.ones(2), np.zeros((3, 4)))
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(np.eye(3)[0], 5)
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.eye(3)[0], np.zeros((2, 4)))
     # Use the gradient scalarization to check that the weights sum to 1
-    assert(np.abs(np.sum(acqu.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
-                  - 1.0) < 0.00000001)
+    assert (np.abs(np.sum(acqu.scalarizeGrad(np.eye(3)[0], np.eye(4)[0:3, :]))
+                   - 1.0) < 0.00000001)
     return
 
 
 if __name__ == "__main__":
     test_UniformWeights()
     test_FixedWeights()
```

### Comparing `parmoo-0.2.0/parmoo/util.py` & `parmoo-0.2.1/parmoo/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,17 +134,17 @@
                 if not isinstance(arg['hyperparams'], dict):
                     raise TypeError("sims[" + str(s)
                                     + "]: 'hyperparams'"
                                     + " key must be a dict when present")
             # Check the search technique
             if 'search' in arg:
                 try:
-                    assert(isinstance(arg['search'](m, np.zeros(n),
+                    assert isinstance(arg['search'](m, np.zeros(n),
                                                     np.ones(n), {}),
-                                      structs.GlobalSearch))
+                                      structs.GlobalSearch)
                 except BaseException:
                     raise TypeError("sims[" + str(s) + "]['search']"
                                     + " must be a derivative of the"
                                     + " GlobalSearch abstract class")
             else:
                 raise AttributeError("sims[" + str(s) + "] is missing"
                                      + " the key 'search'")
```

### Comparing `parmoo-0.2.0/parmoo/viz/dashboard.py` & `parmoo-0.2.1/parmoo/viz/dashboard.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/viz/graph.py` & `parmoo-0.2.1/parmoo/viz/graph.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/viz/plot.py` & `parmoo-0.2.1/parmoo/viz/plot.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo/viz/utilities.py` & `parmoo-0.2.1/parmoo/viz/utilities.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.0/parmoo.egg-info/PKG-INFO` & `parmoo-0.2.1/parmoo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parmoo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library for parallel multiobjective simulation optimization
 Home-page: https://github.com/parmoo/parmoo
-Author: Tyler H. Chang and Stefan M. Wild
+Author: Tyler H. Chang, Stefan M. Wild, et al.
 Author-email: parmoo@mcs.anl.gov
 License: BSD 3-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `parmoo-0.2.0/parmoo.egg-info/SOURCES.txt` & `parmoo-0.2.1/parmoo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,18 @@
 parmoo/optimizers/lbfgsb.py
 parmoo/optimizers/random_search.py
 parmoo/searches/__init__.py
 parmoo/searches/latin_hypercube.py
 parmoo/simulations/__init__.py
 parmoo/simulations/dtlz.py
 parmoo/simulations/sim_func.py
+parmoo/simulations/simple.py
 parmoo/surrogates/__init__.py
 parmoo/surrogates/gaussian_proc.py
+parmoo/surrogates/linear_model.py
 parmoo/tests/.coveragerc
 parmoo/tests/__init__.py
 parmoo/tests/run-tests.sh
 parmoo/tests/.pytest_cache/CACHEDIR.TAG
 parmoo/tests/.pytest_cache/README.md
 parmoo/tests/.pytest_cache/v/cache/nodeids
 parmoo/tests/.pytest_cache/v/cache/stepwise
@@ -130,18 +132,20 @@
 parmoo/tests/unit_tests/test_gaussian_proc.py
 parmoo/tests/unit_tests/test_gps_search.py
 parmoo/tests/unit_tests/test_latin_hypercube.py
 parmoo/tests/unit_tests/test_lbfgsb.py
 parmoo/tests/unit_tests/test_libe.py
 parmoo/tests/unit_tests/test_moop.py
 parmoo/tests/unit_tests/test_moop_embeddings.py
+parmoo/tests/unit_tests/test_moop_grads.py
 parmoo/tests/unit_tests/test_obj_dtlz.py
 parmoo/tests/unit_tests/test_obj_lib.py
 parmoo/tests/unit_tests/test_random_search.py
 parmoo/tests/unit_tests/test_sims_dtlz.py
+parmoo/tests/unit_tests/test_sims_simple.py
 parmoo/tests/unit_tests/test_structs.py
 parmoo/tests/unit_tests/test_util.py
 parmoo/tests/unit_tests/test_viz_without_dash.py
 parmoo/tests/unit_tests/test_weighted_sum.py
 parmoo/viz/__init__.py
 parmoo/viz/dashboard.py
 parmoo/viz/graph.py
```

### Comparing `parmoo-0.2.0/setup.py` & `parmoo-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 setup(
     name="parmoo",
     version=__version__,
     description="Python library for parallel multiobjective simulation optimization",
     long_description="\n".join(DOCLINES[2:]),
     url="https://github.com/parmoo/parmoo",
-    author="Tyler H. Chang and Stefan M. Wild",
+    author="Tyler H. Chang, Stefan M. Wild, et al.",
     author_email="parmoo@mcs.anl.gov",
     license="BSD 3-clause",
 
     packages=["parmoo",
               "parmoo.acquisitions",
               "parmoo.extras",
               "parmoo.viz",
```

