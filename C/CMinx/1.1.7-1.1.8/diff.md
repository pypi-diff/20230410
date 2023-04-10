# Comparing `tmp/CMinx-1.1.7.tar.gz` & `tmp/CMinx-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMinx-1.1.7.tar", last modified: Mon Mar 27 22:57:18 2023, max compression
+gzip compressed data, was "CMinx-1.1.8.tar", last modified: Mon Apr 10 15:51:01 2023, max compression
```

## Comparing `CMinx-1.1.7.tar` & `CMinx-1.1.8.tar`

### file list

```diff
@@ -1,153 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.991823 CMinx-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 22:57:09.000000 CMinx-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-27 22:57:09.000000 CMinx-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-03-27 22:57:18.991823 CMinx-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-03-27 22:57:09.000000 CMinx-1.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.975823 CMinx-1.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.975823 CMinx-1.1.7/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.971823 CMinx-1.1.7/docs/source/.templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.975823 CMinx-1.1.7/docs/source/.templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/.templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.975823 CMinx-1.1.7/docs/source/developer/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/ci.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/repo_structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.975823 CMinx-1.1.7/docs/source/developer/uml_diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/uml_diagrams/aggregation.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    86638 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/uml_diagrams/aggregation.png
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/uml_diagrams/parsing.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    84711 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/developer/uml_diagrams/parsing.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.979823 CMinx-1.1.7/docs/source/documenting/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/cmaketest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/ctest_add_test.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/macro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/types_of_comments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/documenting/variable.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/full_example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-27 22:57:09.000000 CMinx-1.1.7/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-27 22:57:09.000000 CMinx-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 22:57:18.991823 CMinx-1.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-03-27 22:57:09.000000 CMinx-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.979823 CMinx-1.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.979823 CMinx-1.1.7/src/CMinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-03-27 22:57:18.000000 CMinx-1.1.7/src/CMinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-03-27 22:57:18.000000 CMinx-1.1.7/src/CMinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 22:57:18.000000 CMinx-1.1.7/src/CMinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 22:57:18.000000 CMinx-1.1.7/src/CMinx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-27 22:57:18.000000 CMinx-1.1.7/src/CMinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 22:57:18.000000 CMinx-1.1.7/src/CMinx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.979823 CMinx-1.1.7/src/cminx/
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23467 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/documentation_types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4160 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/documenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.979823 CMinx-1.1.7/src/cminx/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMake.g4
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMake.interp
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMake.tokens
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMakeLexer.interp
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMakeLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMakeLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMakeListener.py
--rw-r--r--   0 runner    (1001) docker     (123)    20386 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMakeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/CMakeVisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/parser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20831 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/cminx/rstwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-27 22:57:09.000000 CMinx-1.1.7/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.983823 CMinx-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.983823 CMinx-1.1.7/tests/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/cmake/gen_rst.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.983823 CMinx-1.1.7/tests/cmake_input/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/cmake_input/example.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.983823 CMinx-1.1.7/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/aggregator_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.983823 CMinx-1.1.7/tests/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/configs/exclude_filters_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/configs/exclude_input_file_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/configs/no_auto_exclude_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/configs/no_include_undocumented_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/example.cmake
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/example_2.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.983823 CMinx-1.1.7/tests/examples/more_cmake_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/more_cmake_files/empty.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/rst_validator_example.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/rstwriter_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.975823 CMinx-1.1.7/tests/examples/sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.983823 CMinx-1.1.7/tests/examples/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/example_no_undocumented.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/example_prefix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/index_exclusion_filters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/examples/sphinx/source/index_no_auto_exclude.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.987823 CMinx-1.1.7/tests/test_samples/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/add_test_and_func_after.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/advanced_function.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/advanced_macro.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/advanced_module.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/basic_function.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/basic_macro.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/basic_module.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.987823 CMinx-1.1.7/tests/test_samples/corr_rst/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/add_test_and_func_after.rst
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/advanced_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/advanced_macro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/advanced_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/basic_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/basic_macro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/basic_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/ct_test.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/ctest_add_test.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.987823 CMinx-1.1.7/tests/test_samples/corr_rst/index/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/index/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/index/index_prefix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/undocumented_commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/corr_rst/variable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/ct_test.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/ctest_add_test.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/quickstart.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/undocumented_commands.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/test_samples/variable.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:57:18.991823 CMinx-1.1.7/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13343 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/rst_validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19345 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4782 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_documenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_error_listener.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6615 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4914 2023-03-27 22:57:09.000000 CMinx-1.1.7/tests/unit_tests/test_rstwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.351490 CMinx-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 15:50:52.000000 CMinx-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 15:50:52.000000 CMinx-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-10 15:51:01.351490 CMinx-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-10 15:50:52.000000 CMinx-1.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.335490 CMinx-1.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.335490 CMinx-1.1.8/docs/source/.templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/.templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/.templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/ci.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/repo_structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/developer/uml_diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    86638 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    84711 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/docs/source/documenting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/cmaketest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/ctest_add_test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/macro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/types_of_comments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/documenting/variable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/full_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-10 15:50:52.000000 CMinx-1.1.8/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-10 15:50:52.000000 CMinx-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:51:01.351490 CMinx-1.1.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-04-10 15:50:52.000000 CMinx-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.339490 CMinx-1.1.8/src/CMinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 15:51:01.000000 CMinx-1.1.8/src/CMinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/src/cminx/
+-rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24540 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/documentation_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4160 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/documenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/src/cminx/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMake.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMake.interp
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMake.tokens
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20386 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/CMakeVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/parser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20831 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/cminx/rstwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-10 15:50:52.000000 CMinx-1.1.8/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/cmake/gen_rst.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/cmake_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/cmake_input/example.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/aggregator_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/exclude_filters_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/exclude_input_file_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/no_auto_exclude_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/configs/no_include_undocumented_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/example.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/example_2.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/more_cmake_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/more_cmake_files/empty.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/rst_validator_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/rstwriter_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.335490 CMinx-1.1.8/tests/examples/sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.343490 CMinx-1.1.8/tests/examples/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/example_prefix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/index_exclusion_filters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/examples/sphinx/source/index_no_auto_exclude.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.347490 CMinx-1.1.8/tests/test_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/add_test_and_func_after.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/advanced_function.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/advanced_macro.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/advanced_module.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/basic_function.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/basic_macro.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/basic_module.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.347490 CMinx-1.1.8/tests/test_samples/corr_rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/add_test_and_func_after.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/advanced_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/advanced_macro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/advanced_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/basic_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/basic_macro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/basic_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/ct_test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/ctest_add_test.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.347490 CMinx-1.1.8/tests/test_samples/corr_rst/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/index/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/index/index_prefix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/option.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/undocumented_commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/undocumented_option_no_default.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/corr_rst/variable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/ct_test.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/ctest_add_test.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/option.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/quickstart.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/undocumented_commands.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/undocumented_option_no_default.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/test_samples/variable.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:51:01.351490 CMinx-1.1.8/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13343 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/rst_validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19868 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4782 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_documenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_error_listener.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6615 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4914 2023-04-10 15:50:52.000000 CMinx-1.1.8/tests/unit_tests/test_rstwriter.py
```

### Comparing `CMinx-1.1.7/LICENSE` & `CMinx-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/PKG-INFO` & `CMinx-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMinx
-Version: 1.1.7
+Version: 1.1.8
 Summary: Documentation Generator for the CMake Language
 Author: CMakePP
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CMinx-1.1.7/README.rst` & `CMinx-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/Makefile` & `CMinx-1.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/README.rst` & `CMinx-1.1.8/docs/README.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/about.rst` & `CMinx-1.1.8/docs/source/about.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/conf.py` & `CMinx-1.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/config.rst` & `CMinx-1.1.8/docs/source/config.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/api.rst` & `CMinx-1.1.8/docs/source/developer/api.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/ci.rst` & `CMinx-1.1.8/docs/source/developer/ci.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/dependencies.rst` & `CMinx-1.1.8/docs/source/developer/dependencies.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/documentation.rst` & `CMinx-1.1.8/docs/source/developer/documentation.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/index.rst` & `CMinx-1.1.8/docs/source/developer/index.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/overview.rst` & `CMinx-1.1.8/docs/source/developer/overview.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/repo_structure.rst` & `CMinx-1.1.8/docs/source/developer/repo_structure.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/uml_diagrams/aggregation.drawio` & `CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.drawio`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/uml_diagrams/aggregation.png` & `CMinx-1.1.8/docs/source/developer/uml_diagrams/aggregation.png`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/uml_diagrams/parsing.drawio` & `CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.drawio`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/developer/uml_diagrams/parsing.png` & `CMinx-1.1.8/docs/source/developer/uml_diagrams/parsing.png`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/cmaketest.rst` & `CMinx-1.1.8/docs/source/documenting/cmaketest.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/ctest_add_test.rst` & `CMinx-1.1.8/docs/source/documenting/ctest_add_test.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/function.rst` & `CMinx-1.1.8/docs/source/documenting/function.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/index.rst` & `CMinx-1.1.8/docs/source/documenting/index.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/macro.rst` & `CMinx-1.1.8/docs/source/documenting/macro.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/module.rst` & `CMinx-1.1.8/docs/source/documenting/module.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/types_of_comments.rst` & `CMinx-1.1.8/docs/source/documenting/types_of_comments.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/documenting/variable.rst` & `CMinx-1.1.8/docs/source/documenting/variable.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/full_example.rst` & `CMinx-1.1.8/docs/source/full_example.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/index.rst` & `CMinx-1.1.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/installation.rst` & `CMinx-1.1.8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/quickstart.rst` & `CMinx-1.1.8/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/docs/source/usage.rst` & `CMinx-1.1.8/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/pyproject.toml` & `CMinx-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/setup.py` & `CMinx-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/CMinx.egg-info/PKG-INFO` & `CMinx-1.1.8/src/CMinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMinx
-Version: 1.1.7
+Version: 1.1.8
 Summary: Documentation Generator for the CMake Language
 Author: CMakePP
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CMinx-1.1.7/src/CMinx.egg-info/SOURCES.txt` & `CMinx-1.1.8/src/CMinx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -92,30 +92,34 @@
 tests/test_samples/advanced_macro.cmake
 tests/test_samples/advanced_module.cmake
 tests/test_samples/basic_function.cmake
 tests/test_samples/basic_macro.cmake
 tests/test_samples/basic_module.cmake
 tests/test_samples/ct_test.cmake
 tests/test_samples/ctest_add_test.cmake
+tests/test_samples/option.cmake
 tests/test_samples/quickstart.cmake
 tests/test_samples/test_samples.py
 tests/test_samples/undocumented_commands.cmake
+tests/test_samples/undocumented_option_no_default.cmake
 tests/test_samples/variable.cmake
 tests/test_samples/corr_rst/add_test_and_func_after.rst
 tests/test_samples/corr_rst/advanced_function.rst
 tests/test_samples/corr_rst/advanced_macro.rst
 tests/test_samples/corr_rst/advanced_module.rst
 tests/test_samples/corr_rst/basic_function.rst
 tests/test_samples/corr_rst/basic_macro.rst
 tests/test_samples/corr_rst/basic_module.rst
 tests/test_samples/corr_rst/ct_test.rst
 tests/test_samples/corr_rst/ctest_add_test.rst
 tests/test_samples/corr_rst/index.rst
+tests/test_samples/corr_rst/option.rst
 tests/test_samples/corr_rst/quickstart.rst
 tests/test_samples/corr_rst/undocumented_commands.rst
+tests/test_samples/corr_rst/undocumented_option_no_default.rst
 tests/test_samples/corr_rst/variable.rst
 tests/test_samples/corr_rst/index/index.rst
 tests/test_samples/corr_rst/index/index_prefix.rst
 tests/unit_tests/__init__.py
 tests/unit_tests/rst_validator.py
 tests/unit_tests/test_aggregator.py
 tests/unit_tests/test_config.py
```

### Comparing `CMinx-1.1.7/src/cminx/__init__.py` & `CMinx-1.1.8/src/cminx/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/aggregator.py` & `CMinx-1.1.8/src/cminx/aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # limitations under the License.
 
 import logging
 from typing import List
 
 from .documentation_types import AttributeDocumentation, FunctionDocumentation, MacroDocumentation, \
     VariableDocumentation, GenericCommandDocumentation, ClassDocumentation, TestDocumentation, SectionDocumentation, \
-    MethodDocumentation, VarType, CTestDocumentation, ModuleDocumentation, AbstractCommandDefinitionDocumentation
+    MethodDocumentation, VarType, CTestDocumentation, ModuleDocumentation, AbstractCommandDefinitionDocumentation, \
+    OptionDocumentation
 from .exceptions import CMakeSyntaxException
 from .parser.CMakeListener import CMakeListener
 # Annoyingly, the Antl4 Python libraries use camelcase since it was originally Java, so we have convention
 # inconsistencies here
 from .parser.CMakeParser import CMakeParser
 from cminx import Settings
 
@@ -433,14 +434,40 @@
 
                     self.logger.error(f"add_test() called with incorrect parameters: {params}\n\n{pretty_text}")
                     return
 
         test_doc = CTestDocumentation(name, docstring, [p for p in params if p != name and p != "NAME"])
         self.documented.append(test_doc)
 
+    def process_option(self, ctx: CMakeParser.Command_invocationContext, docstring: str):
+        """
+        Extracts information from an :code:`option()` command and creates
+        an OptionDocumentation from it. It extracts the option name,
+        the help text, and the default value if any.
+
+        :param ctx: Documented command context. Constructed by the Antlr4 parser.
+        :param docstring: Cleaned docstring.
+        """
+        params = [param.getText() for param in ctx.single_argument()]  # Extract parameters
+        if len(params) < 2 or len(params) > 3:
+            pretty_text = docstring
+            pretty_text += f"\n{ctx.getText()}"
+
+            self.logger.error(
+                f"ct_add_section() called with incorrect parameters: {params}\n\n{pretty_text}")
+            return
+        option_doc = OptionDocumentation(
+            params[0],
+            docstring,
+            "bool",
+            params[2] if len(params) == 3 else None,
+            params[1]
+        )
+        self.documented.append(option_doc)
+
     def process_generic_command(self, command_name: str, ctx: CMakeParser.Command_invocationContext, docstring: str):
         """
         Extracts command invocation and arguments for a documented command that does not
         have a dedicated processor function.
 
         :param command_name: The documented command's name, such as add_library.
```

### Comparing `CMinx-1.1.7/src/cminx/config.py` & `CMinx-1.1.8/src/cminx/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             "include_undocumented_cpp_class": bool,
             "include_undocumented_cpp_attr": bool,
             "include_undocumented_cpp_constructor": bool,
             "include_undocumented_cpp_member": bool,
             "include_undocumented_ct_add_test": bool,
             "include_undocumented_add_test": bool,
             "include_undocumented_ct_add_section": bool,
+            "include_undocumented_option": bool,
             "auto_exclude_directories_without_cmake": bool,
             "kwargs_doc_trigger_string": confuse.Optional(confuse.String(), default=":keyword"),
             "exclude_filters": confuse.Optional(list, default=()),
             "recursive": bool,
             "follow_symlinks": bool
         },
         "output": {
@@ -67,14 +68,15 @@
     include_undocumented_cpp_class: bool = True
     include_undocumented_cpp_attr: bool = True
     include_undocumented_cpp_constructor: bool = True
     include_undocumented_cpp_member: bool = True
     include_undocumented_ct_add_test: bool = True
     include_undocumented_ct_add_section: bool = True
     include_undocumented_add_test: bool = True
+    include_undocumented_option: bool = True
     auto_exclude_directories_without_cmake: bool = True
     kwargs_doc_trigger_string: str = ":param **kwargs:"
     exclude_filters: List[str] = ()
     recursive: bool = False
     follow_symlinks: bool = False
```

### Comparing `CMinx-1.1.7/src/cminx/config_default.yaml` & `CMinx-1.1.8/src/cminx/config_default.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,18 @@
   # auto-generated.
   include_undocumented_ct_add_test: true
 
   # Whether undocumented test sections should have documentation
   # auto-generated.
   include_undocumented_ct_add_section: true
 
+  # Whether undocumented options should have documentation
+  # auto-generated.
+  include_undocumented_option: true
+
   # Whether undocumented CTest tests should have documentation
   # auto-generated. This controls whether all vanilla
   # CMake add_test() commands should be documented,
   # it has no relation to CMakeTest tests.
   include_undocumented_add_test: true
 
   # Whether directories not containing .cmake
```

### Comparing `CMinx-1.1.7/src/cminx/documentation_types.py` & `CMinx-1.1.8/src/cminx/documentation_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     well as the :code:`UNSET` subcommand.
 
     This class translates the definition into a Sphinx
     :code:`data` directive, with a :code:`Default value` field
     and a :code:`type` field.
     """
 
-    type: VarType
+    type: Union[VarType, str]
     """The type that the variable is."""
 
     value: Union[str, None]
     """A default value that the variable has"""
 
     def process(self, writer: RSTWriter):
         d = writer.directive("data", f"{self.name}")
@@ -150,14 +150,42 @@
             var_type = "UNSET"
         else:
             raise ValueError(f"Unknown variable type: {self.type}")
         d.field("type", var_type)
 
 
 @dataclass
+class OptionDocumentation(VariableDocumentation):
+    """
+    This class documents a CMake option() command,
+    representing a user-configurable option that can
+    be selected via the cache. The RST form of this documentation
+    also uses the :code:`data` directive, but includes a note
+    specifying the variable is an option.
+    """
+
+    help_text: str
+    """The help text that the option has."""
+
+    def process(self, writer: RSTWriter):
+        d = writer.directive("data", f"{self.name}")
+        note = d.directive("note")
+        note.text(
+            f"""
+            This variable is a user-editable option,
+            meaning it appears within the cache and can be
+            edited on the command line by the :code:`-D` flag.
+            """)
+        d.text(self.doc)
+        d.field("Help text", self.help_text)
+        d.field("Default value", self.value if self.value is not None else "OFF")
+        d.field("type", self.type)
+
+
+@dataclass
 class GenericCommandDocumentation(DocumentationType):
     """
     This class represents any documented command that does
     not fit into any of the other documentation types.
 
     All this class does is translate the documented
     command into a Sphinx :code:`function` directive with
```

### Comparing `CMinx-1.1.7/src/cminx/documenter.py` & `CMinx-1.1.8/src/cminx/documenter.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/exceptions.py` & `CMinx-1.1.8/src/cminx/exceptions.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/CMake.g4` & `CMinx-1.1.8/src/cminx/parser/CMake.g4`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/CMake.interp` & `CMinx-1.1.8/src/cminx/parser/CMake.interp`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/CMakeLexer.interp` & `CMinx-1.1.8/src/cminx/parser/CMakeLexer.interp`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/CMakeLexer.py` & `CMinx-1.1.8/src/cminx/parser/CMakeLexer.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/CMakeListener.py` & `CMinx-1.1.8/src/cminx/parser/CMakeListener.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/CMakeParser.py` & `CMinx-1.1.8/src/cminx/parser/CMakeParser.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/CMakeVisitor.py` & `CMinx-1.1.8/src/cminx/parser/CMakeVisitor.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/parser/__init__.py` & `CMinx-1.1.8/src/cminx/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/cminx/rstwriter.py` & `CMinx-1.1.8/src/cminx/rstwriter.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/src/main.py` & `CMinx-1.1.8/src/main.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/CMakeLists.txt` & `CMinx-1.1.8/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/README.rst` & `CMinx-1.1.8/tests/README.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/cmake/gen_rst.cmake` & `CMinx-1.1.8/tests/cmake/gen_rst.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/cmake_input/example.cmake` & `CMinx-1.1.8/tests/cmake_input/example.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/context.py` & `CMinx-1.1.8/tests/context.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/__init__.py` & `CMinx-1.1.8/tests/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/aggregator_example.py` & `CMinx-1.1.8/tests/examples/aggregator_example.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/configs/exclude_filters_config.yaml` & `CMinx-1.1.8/tests/examples/configs/exclude_filters_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/configs/exclude_input_file_config.yaml` & `CMinx-1.1.8/tests/examples/configs/exclude_input_file_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/configs/no_auto_exclude_config.yaml` & `CMinx-1.1.8/tests/examples/configs/no_auto_exclude_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/configs/no_include_undocumented_config.yaml` & `CMinx-1.1.8/tests/examples/configs/no_include_undocumented_config.yaml`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/example.cmake` & `CMinx-1.1.8/tests/examples/example.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -282,7 +282,12 @@
 # command
 #]]
 add_test(
     NAME ctest_test_undocumented
     COMMAND bash -c echo test
 )
 
+#[[[
+# This is a documented option
+#]]
+option(TEST_OPTION "This is a test option" OFF)
+
```

### Comparing `CMinx-1.1.7/tests/examples/rst_validator_example.py` & `CMinx-1.1.8/tests/examples/rst_validator_example.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/rstwriter_example.py` & `CMinx-1.1.8/tests/examples/rstwriter_example.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/sphinx/source/conf.py` & `CMinx-1.1.8/tests/examples/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/examples/sphinx/source/example.rst` & `CMinx-1.1.8/tests/examples/sphinx/source/example.rst`

 * *Files 4% similar despite different names*

```diff
@@ -335,7 +335,28 @@
 .. function:: ctest_test_undocumented(COMMAND bash -c echo test)
 
 
    .. warning:: This is a CTest test definition, do not call this manually. Use the "ctest" program to execute this test.
 
    
 
+
+.. data:: TEST_OPTION
+
+
+   .. note:: 
+
+      
+                  This variable is a user-editable option,
+                  meaning it appears within the cache and can be
+                  edited on the command line by the :code:`-D` flag.
+                  
+
+   This is a documented option
+   
+
+   :Help text: "This is a test option"
+
+   :Default value: OFF
+
+   :type: bool
+
```

### Comparing `CMinx-1.1.7/tests/examples/sphinx/source/example_no_undocumented.rst` & `CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented.rst`

 * *Files 11% similar despite different names*

```diff
@@ -135,7 +135,28 @@
 
    This is a documented CTest test.
    Note that this is a vanilla CMake
    add_test() command, not a ct_add_test()
    command
    
 
+
+.. data:: TEST_OPTION
+
+
+   .. note:: 
+
+      
+                  This variable is a user-editable option,
+                  meaning it appears within the cache and can be
+                  edited on the command line by the :code:`-D` flag.
+                  
+
+   This is a documented option
+   
+
+   :Help text: "This is a test option"
+
+   :Default value: OFF
+
+   :type: bool
+
```

### Comparing `CMinx-1.1.7/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst` & `CMinx-1.1.8/tests/examples/sphinx/source/example_no_undocumented_diff_header.rst`

 * *Files 5% similar despite different names*

```diff
@@ -135,7 +135,28 @@
 
    This is a documented CTest test.
    Note that this is a vanilla CMake
    add_test() command, not a ct_add_test()
    command
    
 
+
+.. data:: TEST_OPTION
+
+
+   .. note:: 
+
+      
+                  This variable is a user-editable option,
+                  meaning it appears within the cache and can be
+                  edited on the command line by the :code:`-D` flag.
+                  
+
+   This is a documented option
+   
+
+   :Help text: "This is a test option"
+
+   :Default value: OFF
+
+   :type: bool
+
```

### Comparing `CMinx-1.1.7/tests/examples/sphinx/source/example_prefix.rst` & `CMinx-1.1.8/tests/examples/sphinx/source/example_prefix.rst`

 * *Files 2% similar despite different names*

```diff
@@ -335,7 +335,28 @@
 .. function:: ctest_test_undocumented(COMMAND bash -c echo test)
 
 
    .. warning:: This is a CTest test definition, do not call this manually. Use the "ctest" program to execute this test.
 
    
 
+
+.. data:: TEST_OPTION
+
+
+   .. note:: 
+
+      
+                  This variable is a user-editable option,
+                  meaning it appears within the cache and can be
+                  edited on the command line by the :code:`-D` flag.
+                  
+
+   This is a documented option
+   
+
+   :Help text: "This is a test option"
+
+   :Default value: OFF
+
+   :type: bool
+
```

### Comparing `CMinx-1.1.7/tests/helpers.py` & `CMinx-1.1.8/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_all.py` & `CMinx-1.1.8/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/__init__.py` & `CMinx-1.1.8/tests/test_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/advanced_function.cmake` & `CMinx-1.1.8/tests/test_samples/advanced_function.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/advanced_macro.cmake` & `CMinx-1.1.8/tests/test_samples/advanced_macro.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/corr_rst/advanced_function.rst` & `CMinx-1.1.8/tests/test_samples/corr_rst/advanced_function.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/corr_rst/advanced_macro.rst` & `CMinx-1.1.8/tests/test_samples/corr_rst/advanced_macro.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/corr_rst/undocumented_commands.rst` & `CMinx-1.1.8/tests/test_samples/corr_rst/undocumented_commands.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/corr_rst/variable.rst` & `CMinx-1.1.8/tests/test_samples/corr_rst/variable.rst`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/test_samples.py` & `CMinx-1.1.8/tests/test_samples/test_samples.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/test_samples/undocumented_commands.cmake` & `CMinx-1.1.8/tests/test_samples/undocumented_commands.cmake`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/__init__.py` & `CMinx-1.1.8/tests/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/rst_validator.py` & `CMinx-1.1.8/tests/unit_tests/rst_validator.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/test_aggregator.py` & `CMinx-1.1.8/tests/unit_tests/test_aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,24 @@
         command = f'{command_name}({" ".join(params)})'
         docstring = f"This is documentation for an incorrect {command_name}() call"
         self.input_stream = InputStream(f'#[[[\n{docstring}\n#]]\n{command}')
         self.reset()
         self.assertEqual(0, len(self.aggregator.documented),
                          f"Incorrect {command_name}() call was still added to documented list: {self.aggregator.documented}")
 
+    def test_incorrect_option_params(self):
+        params = []
+        command_name = "option"
+        command = f'{command_name}({" ".join(params)})'
+        docstring = f"This is documentation for an incorrect {command_name}() call"
+        self.input_stream = InputStream(f'#[[[\n{docstring}\n#]]\n{command}')
+        self.reset()
+        self.assertEqual(0, len(self.aggregator.documented),
+                         f"Incorrect {command_name}() call was still added to documented list: {self.aggregator.documented}")
+
     def test_cpp_attr_outside_class(self):
         self.input_stream = InputStream("#[[[\n# cpp_attr() outside class\n#]]\ncpp_attr()")
         self.reset()
         self.assertEqual(0, len(self.aggregator.documented),
                          f"cpp_attr() call outside class was still added to documented list: {self.aggregator.documented}")
 
     def test_cpp_member_outside_class(self):
```

### Comparing `CMinx-1.1.7/tests/unit_tests/test_config.py` & `CMinx-1.1.8/tests/unit_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/test_documenter.py` & `CMinx-1.1.8/tests/unit_tests/test_documenter.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/test_error_listener.py` & `CMinx-1.1.8/tests/unit_tests/test_error_listener.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/test_init.py` & `CMinx-1.1.8/tests/unit_tests/test_init.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/test_lexer.py` & `CMinx-1.1.8/tests/unit_tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/test_parser.py` & `CMinx-1.1.8/tests/unit_tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `CMinx-1.1.7/tests/unit_tests/test_rstwriter.py` & `CMinx-1.1.8/tests/unit_tests/test_rstwriter.py`

 * *Files identical despite different names*

