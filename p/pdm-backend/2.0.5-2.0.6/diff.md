# Comparing `tmp/pdm_backend-2.0.5.tar.gz` & `tmp/pdm_backend-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_backend-2.0.5.tar", last modified: Tue Feb 28 03:20:15 2023, max compression
+gzip compressed data, was "pdm_backend-2.0.6.tar", last modified: Mon Apr 10 11:46:53 2023, max compression
```

## Comparing `pdm_backend-2.0.5.tar` & `pdm_backend-2.0.6.tar`

### file list

```diff
@@ -1,219 +1,219 @@
--rw-r--r--   0        0        0     1067 2023-02-28 03:20:01.107412 pdm_backend-2.0.5/LICENSE
--rw-r--r--   0        0        0     1725 2023-02-28 03:20:01.107412 pdm_backend-2.0.5/README.md
--rw-r--r--   0        0        0     2271 2023-02-28 03:20:15.147596 pdm_backend-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     3282 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      197 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      661 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3265 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9606 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5115 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     7928 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3264 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    38937 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16469 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16315 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1113 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    19827 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/pyproject_metadata/py.typed
--rw-r--r--   0        0        0     1072 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      177 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0     1491 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/LICENSE
--rw-r--r--   0        0        0    15922 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/LICENSE.txt
--rw-r--r--   0        0        0      589 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/__init__.py
--rw-r--r--   0        0        0       30 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/__main__.py
--rw-r--r--   0        0        0        0 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/__init__.py
--rw-r--r--   0        0        0     1491 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/LICENSE
--rw-r--r--   0        0        0     8769 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__init__.py
--rw-r--r--   0        0        0      312 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__main__.py
--rw-r--r--   0        0        0    29451 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft04.py
--rw-r--r--   0        0        0     7661 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft06.py
--rw-r--r--   0        0        0     4222 2023-02-28 03:20:01.111412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft07.py
--rw-r--r--   0        0        0     1612 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/exceptions.py
--rw-r--r--   0        0        0    12576 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/generator.py
--rw-r--r--   0        0        0      920 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/indent.py
--rw-r--r--   0        0        0     5527 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py
--rw-r--r--   0        0        0       19 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/version.py
--rw-r--r--   0        0        0     1812 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/vendoring_instructions.rst
--rw-r--r--   0        0        0     8721 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/api.py
--rw-r--r--   0        0        0     8626 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/cli.py
--rw-r--r--   0        0        0    11263 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1634 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/errors.py
--rw-r--r--   0        0        0     1153 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     8756 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/formats.py
--rw-r--r--   0        0        0     4183 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/plugins/__init__.py
--rw-r--r--   0        0        0      807 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/plugins/distutils.schema.json
--rw-r--r--   0        0        0    11372 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/plugins/setuptools.schema.json
--rw-r--r--   0        0        0      997 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/NOTICE.template
--rw-r--r--   0        0        0     4718 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__init__.py
--rw-r--r--   0        0        0       61 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__main__.py
--rw-r--r--   0        0        0      101 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/api-notice.template
--rw-r--r--   0        0        0      145 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli-notice.template
--rw-r--r--   0        0        0     2938 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli.py
--rw-r--r--   0        0        0     1038 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/main_file.template
--rw-r--r--   0        0        0    11087 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/project_metadata.schema.json
--rw-r--r--   0        0        0       27 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/py.typed
--rw-r--r--   0        0        0     2124 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pyproject_toml.schema.json
--rw-r--r--   0        0        0      821 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/types.py
--rw-r--r--   0        0        0      624 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/vendoring/__init__.py
--rw-r--r--   0        0        0       61 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/vendoring/__main__.py
--rw-r--r--   0        0        0      222 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/vendoring/cli.py
--rw-r--r--   0        0        0       97 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/_vendor/vendor.txt
--rw-r--r--   0        0        0    11879 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/base.py
--rw-r--r--   0        0        0     9412 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/config.py
--rw-r--r--   0        0        0     4063 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/editable.py
--rw-r--r--   0        0        0      436 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/exceptions.py
--rw-r--r--   0        0        0      108 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/hooks/__init__.py
--rw-r--r--   0        0        0     4069 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/hooks/base.py
--rw-r--r--   0        0        0     6364 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/hooks/setuptools.py
--rw-r--r--   0        0        0     4894 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/hooks/version/__init__.py
--rw-r--r--   0        0        0    10064 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/hooks/version/scm.py
--rw-r--r--   0        0        0      759 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/intree.py
--rw-r--r--   0        0        0    14958 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/macosx_platform.py
--rw-r--r--   0        0        0        0 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/py.typed
--rw-r--r--   0        0        0     3596 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/sdist.py
--rw-r--r--   0        0        0     1381 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/structures.py
--rw-r--r--   0        0        0     7080 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/utils.py
--rw-r--r--   0        0        0    10949 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/src/pdm/backend/wheel.py
--rw-r--r--   0        0        0       72 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/__init__.py
--rw-r--r--   0        0        0      747 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/conftest.py
--rw-r--r--   0        0        0      856 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/hooks/hook_class.py
--rw-r--r--   0        0        0      599 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/hooks/hook_module.py
--rw-r--r--   0        0        0      599 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/hooks/local_hook.py
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      138 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      234 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
--rw-r--r--   0        0        0      558 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      230 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension/pdm_build.py
--rw-r--r--   0        0        0      554 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      379 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      433 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      402 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      406 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-no-license/src/foo_module.py
-lrwxr-xr-x   0        0        0        0 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      330 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      555 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-02-28 03:20:01.115412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      555 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      574 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      513 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      598 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      464 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      277 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-purelib-with-build/my_build.py
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      549 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      413 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      500 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      395 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      406 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       36 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-using-scm/.gitignore
--rw-r--r--   0        0        0       12 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-using-scm/foo/__init__.py
--rw-r--r--   0        0        0      369 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0    16264 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/test_api.py
--rw-r--r--   0        0        0     5324 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/test_file_finder.py
--rw-r--r--   0        0        0     1632 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/test_hooks.py
--rw-r--r--   0        0        0     3058 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/test_metadata.py
--rw-r--r--   0        0        0      311 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/test_utils.py
--rw-r--r--   0        0        0      832 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/test_wheel.py
--rw-r--r--   0        0        0      598 2023-02-28 03:20:01.119412 pdm_backend-2.0.5/tests/testutils.py
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-10 11:46:39.233671 pdm_backend-2.0.6/LICENSE
+-rw-r--r--   0        0        0     1725 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/README.md
+-rw-r--r--   0        0        0     2271 2023-04-10 11:46:53.281793 pdm_backend-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3282 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      661 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3265 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9606 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5115 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     7928 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    38937 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16469 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16315 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1113 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    19827 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0     1072 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      177 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0     1491 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/LICENSE
+-rw-r--r--   0        0        0    15922 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/LICENSE.txt
+-rw-r--r--   0        0        0      589 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/__init__.py
+-rw-r--r--   0        0        0     1491 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/LICENSE
+-rw-r--r--   0        0        0     8769 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__init__.py
+-rw-r--r--   0        0        0      312 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__main__.py
+-rw-r--r--   0        0        0    29451 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft04.py
+-rw-r--r--   0        0        0     7661 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft06.py
+-rw-r--r--   0        0        0     4222 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft07.py
+-rw-r--r--   0        0        0     1612 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/exceptions.py
+-rw-r--r--   0        0        0    12576 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/generator.py
+-rw-r--r--   0        0        0      920 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/indent.py
+-rw-r--r--   0        0        0     5527 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py
+-rw-r--r--   0        0        0       19 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/version.py
+-rw-r--r--   0        0        0     1812 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/vendoring_instructions.rst
+-rw-r--r--   0        0        0     8721 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/api.py
+-rw-r--r--   0        0        0     8626 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/cli.py
+-rw-r--r--   0        0        0    11263 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1634 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/errors.py
+-rw-r--r--   0        0        0     1153 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     8756 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/formats.py
+-rw-r--r--   0        0        0     4183 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/__init__.py
+-rw-r--r--   0        0        0      807 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/distutils.schema.json
+-rw-r--r--   0        0        0    11372 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/setuptools.schema.json
+-rw-r--r--   0        0        0      997 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/NOTICE.template
+-rw-r--r--   0        0        0     4718 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__main__.py
+-rw-r--r--   0        0        0      101 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/api-notice.template
+-rw-r--r--   0        0        0      145 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli-notice.template
+-rw-r--r--   0        0        0     2938 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli.py
+-rw-r--r--   0        0        0     1038 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/main_file.template
+-rw-r--r--   0        0        0    11087 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/project_metadata.schema.json
+-rw-r--r--   0        0        0       27 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/py.typed
+-rw-r--r--   0        0        0     2124 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pyproject_toml.schema.json
+-rw-r--r--   0        0        0      821 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/types.py
+-rw-r--r--   0        0        0      624 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/vendoring/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/vendoring/__main__.py
+-rw-r--r--   0        0        0      222 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/vendoring/cli.py
+-rw-r--r--   0        0        0       97 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/vendor.txt
+-rw-r--r--   0        0        0    11879 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/base.py
+-rw-r--r--   0        0        0     9412 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/config.py
+-rw-r--r--   0        0        0     4063 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/editable.py
+-rw-r--r--   0        0        0      436 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/exceptions.py
+-rw-r--r--   0        0        0      108 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/__init__.py
+-rw-r--r--   0        0        0     4069 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/base.py
+-rw-r--r--   0        0        0     6364 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/setuptools.py
+-rw-r--r--   0        0        0     4894 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/version/__init__.py
+-rw-r--r--   0        0        0    10064 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/version/scm.py
+-rw-r--r--   0        0        0      759 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/intree.py
+-rw-r--r--   0        0        0    14958 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/macosx_platform.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/py.typed
+-rw-r--r--   0        0        0     3596 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/sdist.py
+-rw-r--r--   0        0        0     1381 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/structures.py
+-rw-r--r--   0        0        0     7080 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/utils.py
+-rw-r--r--   0        0        0    10573 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/wheel.py
+-rw-r--r--   0        0        0       72 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      747 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/conftest.py
+-rw-r--r--   0        0        0      856 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/hooks/hook_class.py
+-rw-r--r--   0        0        0      599 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/hooks/hook_module.py
+-rw-r--r--   0        0        0      599 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/hooks/local_hook.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      138 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      234 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
+-rw-r--r--   0        0        0      558 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      230 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pdm_build.py
+-rw-r--r--   0        0        0      554 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      379 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      433 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      402 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      406 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-license/src/foo_module.py
+lrwxr-xr-x   0        0        0        0 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      555 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      555 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      574 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      513 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      598 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      464 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      277 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/my_build.py
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      549 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      413 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      500 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      395 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      406 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/.gitignore
+-rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/foo/__init__.py
+-rw-r--r--   0        0        0      369 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0    16264 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_api.py
+-rw-r--r--   0        0        0     5324 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_file_finder.py
+-rw-r--r--   0        0        0     1632 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_hooks.py
+-rw-r--r--   0        0        0     3058 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_metadata.py
+-rw-r--r--   0        0        0      311 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_utils.py
+-rw-r--r--   0        0        0     1176 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_wheel.py
+-rw-r--r--   0        0        0      598 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/testutils.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.0.6/PKG-INFO
```

### Comparing `pdm_backend-2.0.5/LICENSE` & `pdm_backend-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/README.md` & `pdm_backend-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/pyproject.toml` & `pdm_backend-2.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
-version = "2.0.5"
+version = "2.0.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/pdm-project/pdm-backend"
 Repository = "https://github.com/pdm-project/pdm-backend"
```

### Comparing `pdm_backend-2.0.5/src/pdm/backend/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/LICENSE.APACHE` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/LICENSE.BSD` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/__about__.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_elffile.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_manylinux.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_musllinux.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_parser.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_structures.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/_tokenizer.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/markers.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/requirements.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/specifiers.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/tags.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/utils.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/packaging/version.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/pyproject_metadata/LICENSE` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/pyproject_metadata/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/LICENSE` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/_parser.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli/_re.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli_w/LICENSE` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/tomli_w/_writer.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/LICENSE` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/LICENSE.txt` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/LICENSE` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft04.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft04.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft06.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft06.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft07.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft07.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/exceptions.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/generator.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/generator.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/indent.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/indent.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/_vendor/vendoring_instructions.rst` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/vendoring_instructions.rst`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/api.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/api.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/cli.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/error_reporting.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/errors.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/errors.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/extra_validations.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/formats.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/plugins/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/plugins/distutils.schema.json` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/distutils.schema.json`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/plugins/setuptools.schema.json` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/NOTICE.template` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/NOTICE.template`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pre_compile/main_file.template` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/main_file.template`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/project_metadata.schema.json` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/project_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/pyproject_toml.schema.json` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pyproject_toml.schema.json`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/types.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/types.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/_vendor/validate_pyproject/vendoring/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/vendoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/base.py` & `pdm_backend-2.0.6/src/pdm/backend/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/config.py` & `pdm_backend-2.0.6/src/pdm/backend/config.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/editable.py` & `pdm_backend-2.0.6/src/pdm/backend/editable.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/hooks/base.py` & `pdm_backend-2.0.6/src/pdm/backend/hooks/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/hooks/setuptools.py` & `pdm_backend-2.0.6/src/pdm/backend/hooks/setuptools.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/hooks/version/__init__.py` & `pdm_backend-2.0.6/src/pdm/backend/hooks/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/hooks/version/scm.py` & `pdm_backend-2.0.6/src/pdm/backend/hooks/version/scm.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/intree.py` & `pdm_backend-2.0.6/src/pdm/backend/intree.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/macosx_platform.py` & `pdm_backend-2.0.6/src/pdm/backend/macosx_platform.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/sdist.py` & `pdm_backend-2.0.6/src/pdm/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/structures.py` & `pdm_backend-2.0.6/src/pdm/backend/structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/utils.py` & `pdm_backend-2.0.6/src/pdm/backend/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/src/pdm/backend/wheel.py` & `pdm_backend-2.0.6/src/pdm/backend/wheel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import csv
 import hashlib
 import io
 import os
-import re
 import shutil
 import stat
 import sys
 import tempfile
 import time
 import zipfile
 from base64 import urlsafe_b64encode
@@ -37,15 +36,14 @@
 WHEEL_FILE_FORMAT = """\
 Wheel-Version: 1.0
 Generator: pdm-backend ({version})
 Root-Is-Purelib: {is_purelib}
 Tag: {tag}
 """
 
-PY_LIMITED_API_PATTERN = r"cp3\d{1,2}"
 # Fix the date time for reproducible builds
 try:
     _env_date = time.gmtime(int(os.environ["SOURCE_DATE_EPOCH"]))[:6]
 except (ValueError, KeyError):
     ZIPINFO_DATE_TIME = (2016, 1, 1, 0, 0, 0)
 else:
     if _env_date[0] < 1980:
@@ -80,18 +78,14 @@
         plat_name: str | None = None
         if not self.config_settings:
             return python_tag, py_limited_api, plat_name
         if "--python-tag" in self.config_settings:
             python_tag = self.config_settings["--python-tag"]
         if "--py-limited-api" in self.config_settings:
             py_limited_api = cast(str, self.config_settings["--py-limited-api"])
-            if not re.match(PY_LIMITED_API_PATTERN, py_limited_api):
-                raise ValueError(
-                    "py-limited-api must match '%s'" % PY_LIMITED_API_PATTERN
-                )
         if "--plat-name" in self.config_settings:
             plat_name = self.config_settings["--plat-name"]
         return python_tag, py_limited_api, plat_name
 
     def _fix_dependencies(self) -> None:
         """Fix the dependencies and remove dynamic variables from the metadata"""
         metadata = self.config.metadata
@@ -161,32 +155,29 @@
         impl, abi, platform = self._get_platform_tags()
         is_purelib = self.config.build_config.is_purelib
         if not is_purelib:
             if not platform:
                 platform = get_platform(self.location / "build")
             if not impl:
                 impl = tags.interpreter_name() + tags.interpreter_version()
-            if abi and impl.startswith("cp3"):  # type: ignore[union-attr]
-                impl = abi
-                abi_tag = "abi3"
-            else:
-                abi_tag = str(get_abi_tag()).lower()
+            if not abi:
+                abi = str(get_abi_tag()).lower()
         else:
             if not platform:
                 platform = "any"
-            abi_tag = "none"
+            abi = "none"
             if not impl:
                 requires_python = self.config.metadata.get("requires-python", "")
                 if SpecifierSet(requires_python).contains("2.7"):
                     impl = "py2.py3"
                 else:
                     impl = "py3"
 
         platform = platform.lower().replace("-", "_").replace(".", "_")  # type: ignore
-        tag = (impl, abi_tag, platform)
+        tag = (impl, abi, platform)
         if not is_purelib:
             supported_tags = [(t.interpreter, t.abi, platform) for t in tags.sys_tags()]
             assert (
                 tag in supported_tags
             ), f"would build wheel with unsupported tag {tag}"
         return "-".join(tag)  # type: ignore[arg-type]
 
@@ -257,15 +248,15 @@
         try:
             version = get_version("pdm-backend")
         except ModuleNotFoundError:
             version = "0.0.0+local"
 
         fp.write(
             WHEEL_FILE_FORMAT.format(
-                is_purelib=is_purelib, tag=self.tag, version=version
+                is_purelib=str(is_purelib).lower(), tag=self.tag, version=version
             )
         )
 
     def _write_entry_points(
         self, fp: IO[str], entry_points: dict[str, dict[str, str]]
     ) -> None:
         for group_name in sorted(entry_points):
```

### Comparing `pdm_backend-2.0.5/tests/conftest.py` & `pdm_backend-2.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/hooks/hook_class.py` & `pdm_backend-2.0.6/tests/fixtures/hooks/hook_class.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/hooks/hook_module.py` & `pdm_backend-2.0.6/tests/fixtures/hooks/hook_module.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/hooks/local_hook.py` & `pdm_backend-2.0.6/tests/fixtures/hooks/local_hook.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package/pdm.lock` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package/requirements.txt` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/test_api.py` & `pdm_backend-2.0.6/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 
         with zipfile.ZipFile(tmp_path / wheel_name) as zf:
             wheel_metadata = email.message_from_bytes(
                 zf.read("demo_package-0.1.0.dist-info/WHEEL")
             )
             version = zf.read("my_package/version.txt").decode("utf-8").strip()
             assert version == "0.1.0"
-            assert wheel_metadata["Root-Is-Purelib"] == "True"
+            assert wheel_metadata["Root-Is-Purelib"] == "true"
 
 
 @pytest.mark.skipif(
     sys.platform.startswith("win"), reason="Check file mode on Unix only"
 )
 def test_build_wheel_preserve_permission(tmp_path: Path) -> None:
     with build_fixture_project("demo-package"):
```

### Comparing `pdm_backend-2.0.5/tests/test_file_finder.py` & `pdm_backend-2.0.6/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/test_hooks.py` & `pdm_backend-2.0.6/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/test_metadata.py` & `pdm_backend-2.0.6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/tests/testutils.py` & `pdm_backend-2.0.6/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.5/PKG-INFO` & `pdm_backend-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-backend
-Version: 2.0.5
+Version: 2.0.6
 Summary: The build backend used by PDM that supports latest packaging standards
 Keywords: packaging PEP 517 build
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm-backend Version: 2.0.5 Summary: The build
+Metadata-Version: 2.1 Name: pdm-backend Version: 2.0.6 Summary: The build
 backend used by PDM that supports latest packaging standards Keywords:
 packaging PEP 517 build Author-Email: Frost Ming
 frostming.com> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

