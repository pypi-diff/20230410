# Comparing `tmp/openjij-0.6.8.tar.gz` & `tmp/openjij-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjij-0.6.8.tar", last modified: Wed Nov  2 05:06:52 2022, max compression
+gzip compressed data, was "openjij-0.6.9.tar", last modified: Thu Nov 17 07:58:45 2022, max compression
```

## Comparing `openjij-0.6.8.tar` & `openjij-0.6.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.876590 openjij-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-11-02 05:06:37.000000 openjij-0.6.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-11-02 05:06:37.000000 openjij-0.6.8/.gitattribute
--rw-r--r--   0 runner    (1001) docker     (121)     8430 2022-11-02 05:06:37.000000 openjij-0.6.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-11-02 05:06:37.000000 openjij-0.6.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-02 05:06:37.000000 openjij-0.6.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-02 05:06:37.000000 openjij-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-02 05:06:37.000000 openjij-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9048 2022-11-02 05:06:52.876590 openjij-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7917 2022-11-02 05:06:37.000000 openjij-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.872590 openjij-0.6.8/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     5228 2022-11-02 05:06:37.000000 openjij-0.6.8/cmake/FindGcov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    12711 2022-11-02 05:06:37.000000 openjij-0.6.8/cmake/FindLcov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9023 2022-11-02 05:06:37.000000 openjij-0.6.8/cmake/Findcodecov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4580 2022-11-02 05:06:37.000000 openjij-0.6.8/cmake/GenerateDocs.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-11-02 05:06:37.000000 openjij-0.6.8/cmake/PythonAutoDetectOSX.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-11-02 05:06:37.000000 openjij-0.6.8/cmake/llvm-cov-wrapper
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-11-02 05:06:37.000000 openjij-0.6.8/doc-requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.872590 openjij-0.6.8/external/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-11-02 05:06:37.000000 openjij-0.6.8/external/cimod.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-11-02 05:06:37.000000 openjij-0.6.8/external/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-02 05:06:37.000000 openjij-0.6.8/external/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-02 05:06:37.000000 openjij-0.6.8/external/json.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-02 05:06:37.000000 openjij-0.6.8/external/pybind11-json.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.872590 openjij-0.6.8/openjij/
--rw-r--r--   0 runner    (1001) docker     (121)     2170 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-02 05:06:52.000000 openjij-0.6.8/openjij/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/compile_config.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    38685 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/declare.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    11849 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.876590 openjij-0.6.8/openjij/model/
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13961 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/model/chimera_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8740 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/model/king_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    22833 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.876590 openjij-0.6.8/openjij/sampler/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.876590 openjij-0.6.8/openjij/sampler/chimera_gpu/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/chimera_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/chimera_gpu/base_gpu_chimera.py
--rw-r--r--   0 runner    (1001) docker     (121)     4734 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/chimera_gpu/gpu_sa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4993 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/csqa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/response.py
--rw-r--r--   0 runner    (1001) docker     (121)    21218 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/sa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     8623 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)    12393 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/sampler/sqa_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.876590 openjij-0.6.8/openjij/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9754 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/utils/res_convertor.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/utils/time_measure.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-02 05:06:37.000000 openjij-0.6.8/openjij/variable_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.876590 openjij-0.6.8/openjij.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9048 2022-11-02 05:06:52.000000 openjij-0.6.8/openjij.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-11-02 05:06:52.000000 openjij-0.6.8/openjij.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 05:06:52.000000 openjij-0.6.8/openjij.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 05:06:52.000000 openjij-0.6.8/openjij.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-02 05:06:52.000000 openjij-0.6.8/openjij.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-02 05:06:52.000000 openjij-0.6.8/openjij.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-11-02 05:06:37.000000 openjij-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-11-02 05:06:52.876590 openjij-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-11-02 05:06:37.000000 openjij-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:52.876590 openjij-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51087 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/cxxtest.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    36692 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/polynomial_test.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    13559 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/speed_test_poly_VS_quad.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    27147 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/test_cxx.py
--rw-r--r--   0 runner    (1001) docker     (121)     5570 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)    57730 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/test_hubo.py
--rw-r--r--   0 runner    (1001) docker     (121)     6126 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     9776 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/test_sqa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13959 2022-11-02 05:06:37.000000 openjij-0.6.8/tests/testcase.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.703297 openjij-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2022-11-17 07:58:22.000000 openjij-0.6.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2022-11-17 07:58:22.000000 openjij-0.6.9/.gitattribute
+-rw-r--r--   0 runner    (1001) docker     (122)     8430 2022-11-17 07:58:22.000000 openjij-0.6.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5202 2022-11-17 07:58:22.000000 openjij-0.6.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2022-11-17 07:58:22.000000 openjij-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2022-11-17 07:58:22.000000 openjij-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2022-11-17 07:58:22.000000 openjij-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9125 2022-11-17 07:58:45.707297 openjij-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7994 2022-11-17 07:58:22.000000 openjij-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.695297 openjij-0.6.9/cmake/
+-rw-r--r--   0 runner    (1001) docker     (122)     5228 2022-11-17 07:58:22.000000 openjij-0.6.9/cmake/FindGcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)    12711 2022-11-17 07:58:22.000000 openjij-0.6.9/cmake/FindLcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     9023 2022-11-17 07:58:22.000000 openjij-0.6.9/cmake/Findcodecov.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     4580 2022-11-17 07:58:22.000000 openjij-0.6.9/cmake/GenerateDocs.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2022-11-17 07:58:22.000000 openjij-0.6.9/cmake/PythonAutoDetectOSX.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2022-11-17 07:58:22.000000 openjij-0.6.9/cmake/llvm-cov-wrapper
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2022-11-17 07:58:22.000000 openjij-0.6.9/doc-requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.699297 openjij-0.6.9/external/
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2022-11-17 07:58:22.000000 openjij-0.6.9/external/cimod.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2022-11-17 07:58:22.000000 openjij-0.6.9/external/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-17 07:58:22.000000 openjij-0.6.9/external/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2022-11-17 07:58:22.000000 openjij-0.6.9/external/json.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2022-11-17 07:58:22.000000 openjij-0.6.9/external/pybind11-json.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.699297 openjij-0.6.9/openjij/
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2022-11-17 07:58:45.000000 openjij-0.6.9/openjij/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/compile_config.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    38685 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/declare.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11849 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.699297 openjij-0.6.9/openjij/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13961 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/model/chimera_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8740 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/model/king_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22833 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.703297 openjij-0.6.9/openjij/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.703297 openjij-0.6.9/openjij/sampler/chimera_gpu/
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/chimera_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/chimera_gpu/base_gpu_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4734 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/chimera_gpu/gpu_sa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5553 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4993 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/csqa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21218 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/sa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8623 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12393 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/sampler/sqa_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.703297 openjij-0.6.9/openjij/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9754 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/utils/res_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/utils/time_measure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2022-11-17 07:58:22.000000 openjij-0.6.9/openjij/variable_type.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.699297 openjij-0.6.9/openjij.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9125 2022-11-17 07:58:45.000000 openjij-0.6.9/openjij.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2022-11-17 07:58:45.000000 openjij-0.6.9/openjij.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-17 07:58:45.000000 openjij-0.6.9/openjij.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-17 07:58:45.000000 openjij-0.6.9/openjij.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2022-11-17 07:58:45.000000 openjij-0.6.9/openjij.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-17 07:58:45.000000 openjij-0.6.9/openjij.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4460 2022-11-17 07:58:22.000000 openjij-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2022-11-17 07:58:45.707297 openjij-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2022-11-17 07:58:22.000000 openjij-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:45.703297 openjij-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51087 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/cxxtest.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    36692 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/polynomial_test.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13559 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/speed_test_poly_VS_quad.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    27147 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/test_cxx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5570 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57730 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/test_hubo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6126 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9776 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/test_sqa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13959 2022-11-17 07:58:22.000000 openjij-0.6.9/tests/testcase.hpp
```

### Comparing `openjij-0.6.8/.gitattribute` & `openjij-0.6.9/.gitattribute`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/CMakeLists.txt` & `openjij-0.6.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/CODE_OF_CONDUCT.md` & `openjij-0.6.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/LICENSE` & `openjij-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/MANIFEST.in` & `openjij-0.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/PKG-INFO` & `openjij-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openjij
-Version: 0.6.8
+Version: 0.6.9
 Summary: Framework for the Ising model and QUBO.
 Home-page: https://www.openjij.org
 Author: Jij Inc.
 Author-email: info@openjij.org
 License: Apache License 2.0
 Project-URL: Source, https://github.com/OpenJij/OpenJij
 Project-URL: Documentation, https://openjij.github.io/OpenJij
@@ -32,15 +32,15 @@
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI implementation](https://img.shields.io/pypi/implementation/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI format](https://img.shields.io/pypi/format/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI license](https://img.shields.io/pypi/l/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI download month](https://img.shields.io/pypi/dm/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![Downloads](https://pepy.tech/badge/openjij)](https://pepy.tech/project/openjij)
 
-![build-test](https://github.com/OpenJij/OpenJij/workflows/build-test/badge.svg)
+[![build-test](https://github.com/OpenJij/OpenJij/actions/workflows/ci-test.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/ci-test.yml)
 [![Build Documentation](https://github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml)
 [![CodeQL](https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/0204475dc07d48ffa851480d03db759e)](https://www.codacy.com/gh/OpenJij/OpenJij/dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/OpenJij&utm_campaign=Badge_Grade)
 [![Maintainability](https://api.codeclimate.com/v1/badges/3b2f43f3e601ae74c497/maintainability)](https://codeclimate.com/github/OpenJij/OpenJij/maintainability)
 [![codecov](https://codecov.io/gh/OpenJij/OpenJij/branch/main/graph/badge.svg?token=WMSK3GS8E5)](https://codecov.io/gh/OpenJij/OpenJij)
 
 ## Coverage Graph
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openjij Version: 0.6.8 Summary: Framework for the
+Metadata-Version: 2.1 Name: openjij Version: 0.6.9 Summary: Framework for the
 Ising model and QUBO. Home-page: https://www.openjij.org Author: Jij Inc.
 Author-email: info@openjij.org License: Apache License 2.0 Project-URL: Source,
 https://github.com/OpenJij/OpenJij Project-URL: Documentation, https://
 openjij.github.io/OpenJij Project-URL: Reference, https://ref.openjij.org/
 index.html Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
@@ -19,17 +19,18 @@
 openjij.svg)](https://pypi.python.org/pypi/openjij/) [![PyPI implementation]
 (https://img.shields.io/pypi/implementation/openjij.svg)](https://
 pypi.python.org/pypi/openjij/) [![PyPI format](https://img.shields.io/pypi/
 format/openjij.svg)](https://pypi.python.org/pypi/openjij/) [![PyPI license]
 (https://img.shields.io/pypi/l/openjij.svg)](https://pypi.python.org/pypi/
 openjij/) [![PyPI download month](https://img.shields.io/pypi/dm/openjij.svg)]
 (https://pypi.python.org/pypi/openjij/) [![Downloads](https://pepy.tech/badge/
-openjij)](https://pepy.tech/project/openjij) ![build-test](https://github.com/
-OpenJij/OpenJij/workflows/build-test/badge.svg) [![Build Documentation](https:/
-/github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://
+openjij)](https://pepy.tech/project/openjij) [![build-test](https://github.com/
+OpenJij/OpenJij/actions/workflows/ci-test.yml/badge.svg)](https://github.com/
+OpenJij/OpenJij/actions/workflows/ci-test.yml) [![Build Documentation](https://
+github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://
 github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml) [![CodeQL](https://
 github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml/badge.svg)]
 (https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml) [!
 [Codacy Badge](https://app.codacy.com/project/badge/Grade/
 0204475dc07d48ffa851480d03db759e)](https://www.codacy.com/gh/OpenJij/OpenJij/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/
 OpenJij&utm_campaign=Badge_Grade) [![Maintainability](https://
```

### Comparing `openjij-0.6.8/README.md` & `openjij-0.6.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI implementation](https://img.shields.io/pypi/implementation/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI format](https://img.shields.io/pypi/format/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI license](https://img.shields.io/pypi/l/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI download month](https://img.shields.io/pypi/dm/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![Downloads](https://pepy.tech/badge/openjij)](https://pepy.tech/project/openjij)
 
-![build-test](https://github.com/OpenJij/OpenJij/workflows/build-test/badge.svg)
+[![build-test](https://github.com/OpenJij/OpenJij/actions/workflows/ci-test.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/ci-test.yml)
 [![Build Documentation](https://github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml)
 [![CodeQL](https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/0204475dc07d48ffa851480d03db759e)](https://www.codacy.com/gh/OpenJij/OpenJij/dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/OpenJij&utm_campaign=Badge_Grade)
 [![Maintainability](https://api.codeclimate.com/v1/badges/3b2f43f3e601ae74c497/maintainability)](https://codeclimate.com/github/OpenJij/OpenJij/maintainability)
 [![codecov](https://codecov.io/gh/OpenJij/OpenJij/branch/main/graph/badge.svg?token=WMSK3GS8E5)](https://codecov.io/gh/OpenJij/OpenJij)
 
 ## Coverage Graph
```

#### html2text {}

```diff
@@ -4,17 +4,18 @@
 openjij.svg)](https://pypi.python.org/pypi/openjij/) [![PyPI implementation]
 (https://img.shields.io/pypi/implementation/openjij.svg)](https://
 pypi.python.org/pypi/openjij/) [![PyPI format](https://img.shields.io/pypi/
 format/openjij.svg)](https://pypi.python.org/pypi/openjij/) [![PyPI license]
 (https://img.shields.io/pypi/l/openjij.svg)](https://pypi.python.org/pypi/
 openjij/) [![PyPI download month](https://img.shields.io/pypi/dm/openjij.svg)]
 (https://pypi.python.org/pypi/openjij/) [![Downloads](https://pepy.tech/badge/
-openjij)](https://pepy.tech/project/openjij) ![build-test](https://github.com/
-OpenJij/OpenJij/workflows/build-test/badge.svg) [![Build Documentation](https:/
-/github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://
+openjij)](https://pepy.tech/project/openjij) [![build-test](https://github.com/
+OpenJij/OpenJij/actions/workflows/ci-test.yml/badge.svg)](https://github.com/
+OpenJij/OpenJij/actions/workflows/ci-test.yml) [![Build Documentation](https://
+github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://
 github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml) [![CodeQL](https://
 github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml/badge.svg)]
 (https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml) [!
 [Codacy Badge](https://app.codacy.com/project/badge/Grade/
 0204475dc07d48ffa851480d03db759e)](https://www.codacy.com/gh/OpenJij/OpenJij/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/
 OpenJij&utm_campaign=Badge_Grade) [![Maintainability](https://
```

### Comparing `openjij-0.6.8/cmake/FindGcov.cmake` & `openjij-0.6.9/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/cmake/FindLcov.cmake` & `openjij-0.6.9/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/cmake/Findcodecov.cmake` & `openjij-0.6.9/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/cmake/GenerateDocs.cmake` & `openjij-0.6.9/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/cmake/PythonAutoDetectOSX.cmake` & `openjij-0.6.9/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/cmake/llvm-cov-wrapper` & `openjij-0.6.9/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/doc-requirements.in` & `openjij-0.6.9/doc-requirements.in`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,16 @@
 -c requirements.txt
 -c build-requirements.txt
 
 matplotlib
 networkx
 scikit-learn
 
-openjij
-
 jijmodeling-transpiler
 pyqubo
-dimod
 dwave-cloud-client
 dwave-greedy
 dwave-hybrid
 dwave-inspector
 dwave-neal
 dwave-networkx
 dwave-preprocessing
```

### Comparing `openjij-0.6.8/external/cimod.cmake` & `openjij-0.6.9/external/cimod.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/external/eigen.cmake` & `openjij-0.6.9/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/external/googletest.cmake` & `openjij-0.6.9/external/googletest.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/external/json.cmake` & `openjij-0.6.9/external/json.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/CMakeLists.txt` & `openjij-0.6.9/openjij/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/__init__.py` & `openjij-0.6.9/openjij/__init__.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/compile_config.hpp` & `openjij-0.6.9/openjij/compile_config.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/declare.hpp` & `openjij-0.6.9/openjij/declare.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/main.cpp` & `openjij-0.6.9/openjij/main.cpp`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/model/__init__.py` & `openjij-0.6.9/openjij/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/model/chimera_model.py` & `openjij-0.6.9/openjij/model/chimera_model.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/model/king_graph.py` & `openjij-0.6.9/openjij/model/king_graph.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/model/model.py` & `openjij-0.6.9/openjij/model/model.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/chimera_gpu/base_gpu_chimera.py` & `openjij-0.6.9/openjij/sampler/chimera_gpu/base_gpu_chimera.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/chimera_gpu/gpu_sa_sampler.py` & `openjij-0.6.9/openjij/sampler/chimera_gpu/gpu_sa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py` & `openjij-0.6.9/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/csqa_sampler.py` & `openjij-0.6.9/openjij/sampler/csqa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/response.py` & `openjij-0.6.9/openjij/sampler/response.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/sa_sampler.py` & `openjij-0.6.9/openjij/sampler/sa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/sampler.py` & `openjij-0.6.9/openjij/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/sampler/sqa_sampler.py` & `openjij-0.6.9/openjij/sampler/sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/utils/__init__.py` & `openjij-0.6.9/openjij/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/utils/benchmark.py` & `openjij-0.6.9/openjij/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/utils/decorator.py` & `openjij-0.6.9/openjij/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/utils/graph_utils.py` & `openjij-0.6.9/openjij/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/utils/res_convertor.py` & `openjij-0.6.9/openjij/utils/res_convertor.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij/variable_type.py` & `openjij-0.6.9/openjij/variable_type.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/openjij.egg-info/PKG-INFO` & `openjij-0.6.9/openjij.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openjij
-Version: 0.6.8
+Version: 0.6.9
 Summary: Framework for the Ising model and QUBO.
 Home-page: https://www.openjij.org
 Author: Jij Inc.
 Author-email: info@openjij.org
 License: Apache License 2.0
 Project-URL: Source, https://github.com/OpenJij/OpenJij
 Project-URL: Documentation, https://openjij.github.io/OpenJij
@@ -32,15 +32,15 @@
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI implementation](https://img.shields.io/pypi/implementation/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI format](https://img.shields.io/pypi/format/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI license](https://img.shields.io/pypi/l/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI download month](https://img.shields.io/pypi/dm/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![Downloads](https://pepy.tech/badge/openjij)](https://pepy.tech/project/openjij)
 
-![build-test](https://github.com/OpenJij/OpenJij/workflows/build-test/badge.svg)
+[![build-test](https://github.com/OpenJij/OpenJij/actions/workflows/ci-test.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/ci-test.yml)
 [![Build Documentation](https://github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml)
 [![CodeQL](https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/0204475dc07d48ffa851480d03db759e)](https://www.codacy.com/gh/OpenJij/OpenJij/dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/OpenJij&utm_campaign=Badge_Grade)
 [![Maintainability](https://api.codeclimate.com/v1/badges/3b2f43f3e601ae74c497/maintainability)](https://codeclimate.com/github/OpenJij/OpenJij/maintainability)
 [![codecov](https://codecov.io/gh/OpenJij/OpenJij/branch/main/graph/badge.svg?token=WMSK3GS8E5)](https://codecov.io/gh/OpenJij/OpenJij)
 
 ## Coverage Graph
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openjij Version: 0.6.8 Summary: Framework for the
+Metadata-Version: 2.1 Name: openjij Version: 0.6.9 Summary: Framework for the
 Ising model and QUBO. Home-page: https://www.openjij.org Author: Jij Inc.
 Author-email: info@openjij.org License: Apache License 2.0 Project-URL: Source,
 https://github.com/OpenJij/OpenJij Project-URL: Documentation, https://
 openjij.github.io/OpenJij Project-URL: Reference, https://ref.openjij.org/
 index.html Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
@@ -19,17 +19,18 @@
 openjij.svg)](https://pypi.python.org/pypi/openjij/) [![PyPI implementation]
 (https://img.shields.io/pypi/implementation/openjij.svg)](https://
 pypi.python.org/pypi/openjij/) [![PyPI format](https://img.shields.io/pypi/
 format/openjij.svg)](https://pypi.python.org/pypi/openjij/) [![PyPI license]
 (https://img.shields.io/pypi/l/openjij.svg)](https://pypi.python.org/pypi/
 openjij/) [![PyPI download month](https://img.shields.io/pypi/dm/openjij.svg)]
 (https://pypi.python.org/pypi/openjij/) [![Downloads](https://pepy.tech/badge/
-openjij)](https://pepy.tech/project/openjij) ![build-test](https://github.com/
-OpenJij/OpenJij/workflows/build-test/badge.svg) [![Build Documentation](https:/
-/github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://
+openjij)](https://pepy.tech/project/openjij) [![build-test](https://github.com/
+OpenJij/OpenJij/actions/workflows/ci-test.yml/badge.svg)](https://github.com/
+OpenJij/OpenJij/actions/workflows/ci-test.yml) [![Build Documentation](https://
+github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml/badge.svg)](https://
 github.com/OpenJij/OpenJij/actions/workflows/buid-doc.yml) [![CodeQL](https://
 github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml/badge.svg)]
 (https://github.com/OpenJij/OpenJij/actions/workflows/codeql-analysis.yml) [!
 [Codacy Badge](https://app.codacy.com/project/badge/Grade/
 0204475dc07d48ffa851480d03db759e)](https://www.codacy.com/gh/OpenJij/OpenJij/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/
 OpenJij&utm_campaign=Badge_Grade) [![Maintainability](https://
```

### Comparing `openjij-0.6.8/openjij.egg-info/SOURCES.txt` & `openjij-0.6.9/openjij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/pyproject.toml` & `openjij-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/setup.cfg` & `openjij-0.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/setup.py` & `openjij-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/CMakeLists.txt` & `openjij-0.6.9/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/cxxtest.cpp` & `openjij-0.6.9/tests/cxxtest.cpp`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/polynomial_test.hpp` & `openjij-0.6.9/tests/polynomial_test.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/speed_test_poly_VS_quad.cpp` & `openjij-0.6.9/tests/speed_test_poly_VS_quad.cpp`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/test_cxx.py` & `openjij-0.6.9/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/test_gpu.py` & `openjij-0.6.9/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/test_hubo.py` & `openjij-0.6.9/tests/test_hubo.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/test_model.py` & `openjij-0.6.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/test_sampler.py` & `openjij-0.6.9/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/test_sqa.py` & `openjij-0.6.9/tests/test_sqa.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/test_utils.py` & `openjij-0.6.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `openjij-0.6.8/tests/testcase.hpp` & `openjij-0.6.9/tests/testcase.hpp`

 * *Files identical despite different names*

