# Comparing `tmp/pyradiosky-0.2.0.tar.gz` & `tmp/pyradiosky-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyradiosky-0.2.0.tar", last modified: Thu Feb  2 22:51:42 2023, max compression
+gzip compressed data, was "pyradiosky-0.3.0.tar", last modified: Mon Apr 10 19:47:49 2023, max compression
```

## Comparing `pyradiosky-0.2.0.tar` & `pyradiosky-0.3.0.tar`

### file list

```diff
@@ -1,107 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.121514 pyradiosky-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.101514 pyradiosky-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.101514 pyradiosky-0.2.0/.github/original_pr_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/original_pr_templates/bug_fix.md
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/original_pr_templates/build_ci_change.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/original_pr_templates/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/original_pr_templates/new_feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/original_pr_templates/other.md
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/original_pr_templates/version_change.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.101514 pyradiosky-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/workflows/externaltests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/workflows/publish-to-test-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.github/workflows/testsuite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-02-02 22:51:42.121514 pyradiosky-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.101514 pyradiosky-0.2.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/ci/min_deps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/ci/min_versions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/ci/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/ci/tests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.105514 pyradiosky-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.109514 pyradiosky-0.2.0/docs/Images/
--rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/fhd_catalog_refflux_nonzerospec.png
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/fhd_catalog_refflux_zerospec.png
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_fluxcounts.png
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_radec.png
--rw-r--r--   0 runner    (1001) docker     (123)    24876 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_radec_32768.png
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_refspec.png
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_fluxcounts.png
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_freqflux.png
--rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_Jy.png
--rw-r--r--   0 runner    (1001) docker     (123)    20213 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_K.png
--rw-r--r--   0 runner    (1001) docker     (123)    51546 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_compare.png
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_fluxselect.png
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_lonselect.png
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_newfreq.png
--rw-r--r--   0 runner    (1001) docker     (123)    18440 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_oldfreq.png
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_fluxcounts.png
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_fluxcounts_150MHzatfreq.png
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_fluxcounts_150MHzfreqind.png
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_glgb_coneselect.png
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_glgb_neighborselect.png
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_phiz_nested.png
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_phiz_ring.png
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_radec.png
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/gsm_icrs_radec_indselect.png
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/pointsource_catalog_radec.png
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Images/pointsource_catalog_radec_concat.png
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/developer_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/make_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/make_skymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35506 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/docs/utility_functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.109514 pyradiosky-0.2.0/pyradiosky/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/branch_scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.121514 pyradiosky-0.2.0/pyradiosky/data/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/extended_source_test.sav
--rw-r--r--   0 runner    (1001) docker     (123)   630964 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/fhd_catalog.sav
--rw-r--r--   0 runner    (1001) docker     (123)   574180 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/fhd_catalog_with_beam_values.sav
--rw-r--r--   0 runner    (1001) docker     (123)    81302 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/gleam_50srcs.vot
--rw-r--r--   0 runner    (1001) docker     (123)   280816 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/gsm_galactic.skyh5
--rw-r--r--   0 runner    (1001) docker     (123)   280816 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/gsm_icrs.skyh5
--rw-r--r--   0 runner    (1001) docker     (123)  1089728 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/healpix_disk.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)  4055984 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/healpix_disk.skyh5
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/mock_hera_text_2458098.27471.txt
--rw-r--r--   0 runner    (1001) docker     (123)    63632 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/old_skyh5_point_sources.skyh5
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/pointsource_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/simple_test.vot
--rw-r--r--   0 runner    (1001) docker     (123)    19623 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/data/single_source_old.vot
--rw-r--r--   0 runner    (1001) docker     (123)   222170 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/skymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/spherical_coords_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.121514 pyradiosky-0.2.0/pyradiosky/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   138085 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/tests/test_skymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/tests/test_spherical_coords_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/pyradiosky/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.109514 pyradiosky-0.2.0/pyradiosky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-02-02 22:51:42.000000 pyradiosky-0.2.0/pyradiosky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-02-02 22:51:42.000000 pyradiosky-0.2.0/pyradiosky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 22:51:42.000000 pyradiosky-0.2.0/pyradiosky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-02 22:51:42.000000 pyradiosky-0.2.0/pyradiosky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-02 22:51:42.000000 pyradiosky-0.2.0/pyradiosky.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:51:42.121514 pyradiosky-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/scripts/download_gleam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/scripts/make_flat_spectrum_eor.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-02 22:51:42.125514 pyradiosky-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-02 22:50:37.000000 pyradiosky-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.637531 pyradiosky-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.617531 pyradiosky-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.621531 pyradiosky-0.3.0/.github/original_pr_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/original_pr_templates/bug_fix.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/original_pr_templates/build_ci_change.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/original_pr_templates/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/original_pr_templates/new_feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/original_pr_templates/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/original_pr_templates/version_change.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.621531 pyradiosky-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/workflows/externaltests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/workflows/publish-to-test-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-10 19:47:49.637531 pyradiosky-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.621531 pyradiosky-0.3.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/ci/min_deps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/ci/min_versions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/ci/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/ci/tests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.621531 pyradiosky-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.625531 pyradiosky-0.3.0/docs/Images/
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/fhd_catalog_refflux_nonzerospec.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/fhd_catalog_refflux_zerospec.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_fluxcounts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_radec.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24876 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_radec_32768.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_refspec.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_fluxcounts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_freqflux.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_Jy.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20213 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_K.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51546 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_compare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_fluxselect.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_lonselect.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_newfreq.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18440 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_oldfreq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_fluxcounts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_fluxcounts_150MHzatfreq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_fluxcounts_150MHzfreqind.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_glgb_coneselect.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_glgb_neighborselect.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_phiz_nested.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_phiz_ring.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_radec.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/gsm_icrs_radec_indselect.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/pointsource_catalog_radec.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Images/pointsource_catalog_radec_concat.png
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/developer_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/make_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/make_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35506 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/docs/utility_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.625531 pyradiosky-0.3.0/pyradiosky/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/branch_scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.633531 pyradiosky-0.3.0/pyradiosky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/extended_source_test.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   630964 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/fhd_catalog.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   574180 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/fhd_catalog_with_beam_values.sav
+-rw-r--r--   0 runner    (1001) docker     (123)    81302 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/gleam_50srcs.vot
+-rw-r--r--   0 runner    (1001) docker     (123)   280816 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/gsm_galactic.skyh5
+-rw-r--r--   0 runner    (1001) docker     (123)   280816 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/gsm_icrs.skyh5
+-rw-r--r--   0 runner    (1001) docker     (123)  4055984 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/healpix_disk.skyh5
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/mock_hera_text_2458098.27471.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    63632 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/old_skyh5_point_sources.skyh5
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/pointsource_catalog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/simple_test.vot
+-rw-r--r--   0 runner    (1001) docker     (123)    19623 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/data/single_source_old.vot
+-rw-r--r--   0 runner    (1001) docker     (123)   204362 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/spherical_coords_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.633531 pyradiosky-0.3.0/pyradiosky/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129788 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/tests/test_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/tests/test_spherical_coords_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/pyradiosky/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.625531 pyradiosky-0.3.0/pyradiosky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-10 19:47:49.000000 pyradiosky-0.3.0/pyradiosky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-10 19:47:49.000000 pyradiosky-0.3.0/pyradiosky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:47:49.000000 pyradiosky-0.3.0/pyradiosky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 19:47:49.000000 pyradiosky-0.3.0/pyradiosky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 19:47:49.000000 pyradiosky-0.3.0/pyradiosky.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:47:49.637531 pyradiosky-0.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/scripts/download_gleam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/scripts/make_flat_spectrum_eor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-10 19:47:49.637531 pyradiosky-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 19:46:43.000000 pyradiosky-0.3.0/setup.py
```

### Comparing `pyradiosky-0.2.0/.github/CONTRIBUTING.md` & `pyradiosky-0.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `pyradiosky-0.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/original_pr_templates/bug_fix.md` & `pyradiosky-0.3.0/.github/original_pr_templates/bug_fix.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/original_pr_templates/build_ci_change.md` & `pyradiosky-0.3.0/.github/original_pr_templates/build_ci_change.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/original_pr_templates/documentation.md` & `pyradiosky-0.3.0/.github/original_pr_templates/documentation.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/original_pr_templates/new_feature.md` & `pyradiosky-0.3.0/.github/original_pr_templates/new_feature.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/original_pr_templates/other.md` & `pyradiosky-0.3.0/.github/original_pr_templates/other.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/original_pr_templates/version_change.md` & `pyradiosky-0.3.0/.github/original_pr_templates/version_change.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/workflows/externaltests.yaml` & `pyradiosky-0.3.0/.github/workflows/externaltests.yaml`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/workflows/publish-to-test-pypi.yaml` & `pyradiosky-0.3.0/.github/workflows/publish-to-test-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.github/workflows/testsuite.yaml` & `pyradiosky-0.3.0/.github/workflows/testsuite.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -48,25 +48,31 @@
 
       - name: Install
         run: |
           pip install --no-deps .
 
       - name: Run Tests
         run: |
-          python -m pytest --cov=pyradiosky --cov-config=.coveragerc --cov-report xml:./coverage.xml --junitxml=test-reports/xunit.xml
-          # mkdir -p empty
-          # cd empty
-          # pytest --pyargs pyradiosky --cov=pyradiosky --cov-config=../.coveragerc --cov-report xml:../coverage.xml --junitxml=../test-reports/xunit.xml
-          # cd ..
+          mkdir test-reports
+          mkdir -p empty
+          cd empty
+          python -m pytest --pyargs pyradiosky --cov=../pyradiosky --cov-config="../.coveragerc" --cov-report xml:".././coverage.xml" --junitxml="../test-reports/xunit.xml"
+          ls
+          cd ..
+
+      - name: check coverage report
+        run: |
+          ls
+          cat coverage.xml
 
-      - uses: codecov/codecov-action@v2.0.2
+      - uses: codecov/codecov-action@v3
         if: success()
         with:
           token: ${{secrets.CODECOV_TOKEN}} #required
-          file: ./coverage.xml #optional
+          files: ./coverage.xml #optional
 
   min_deps:
     env:
       ENV_NAME: min_deps
       PYTHON: 3.8
     name: Min Deps Testing
     runs-on: ubuntu-latest
@@ -104,30 +110,31 @@
         run: |
           pip install --no-deps .
 
       - name: Run Tests
         run: |
           python -m pytest --cov=pyradiosky --cov-config=.coveragerc --cov-report xml:./coverage.xml --junitxml=test-reports/xunit.xml
 
-      - uses: codecov/codecov-action@v2.0.2
+      - name: check coverage report
+        run: |
+          ls
+          cat coverage.xml
+
+      - uses: codecov/codecov-action@v3
         if: success()
         with:
           token: ${{secrets.CODECOV_TOKEN}} #required
-          file: ./coverage.xml #optional
+          files: ./coverage.xml #optional
 
   min_versions:
     env:
       ENV_NAME: min_versions
       PYTHON: 3.8
     name: Min Versions Testing
-    runs-on: macos-latest
-      # should go to ubuntu instead when we require at least pyuvdata 2.2.4
-      # there are no linux packages on conda forge between 2.1.15 and 2.2.4 for some
-      # reason
-    # runs-on: ubuntu-latest
+    runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     defaults:
       run:
         # Adding -l {0} helps ensure conda can be found properly.
         shell: bash -l {0}
     steps:
@@ -158,19 +165,24 @@
         run: |
           pip install --no-deps .
 
       - name: Run Tests
         run: |
           python -m pytest --cov=pyradiosky --cov-config=.coveragerc --cov-report xml:./coverage.xml --junitxml=test-reports/xunit.xml
 
-      - uses: codecov/codecov-action@v2.0.2
+      - name: check coverage report
+        run: |
+          ls
+          cat coverage.xml
+
+      - uses: codecov/codecov-action@v3
         if: success()
         with:
           token: ${{secrets.CODECOV_TOKEN}} #required
-          file: ./coverage.xml #optional
+          files: ./coverage.xml #optional
 
   warning_test:
     env:
       ENV_NAME: tests
       PYTHON: 3.8
     name: Warning Test
     runs-on: ubuntu-latest
@@ -207,22 +219,28 @@
           pip install --no-deps .
 
       - name: Run Tests
         run: |
           mkdir test-reports
           mkdir -p empty
           cd empty
-          python -m pytest -W error --pyargs pyradiosky --cov=pyradiosky --cov-config="../.coveragerc" --cov-report xml:".././coverage.xml" --junitxml="../test-reports/xunit.xml"
+          python -m pytest -W error --pyargs pyradiosky --cov=../pyradiosky --cov-config="../.coveragerc" --cov-report xml:".././coverage.xml" --junitxml="../test-reports/xunit.xml"
+          ls
           cd ..
 
-      - uses: codecov/codecov-action@v2.0.2
+      - name: check coverage report
+        run: |
+          ls
+          cat coverage.xml
+
+      - uses: codecov/codecov-action@v3
         if: success()
         with:
           token: ${{secrets.CODECOV_TOKEN}} #required
-          file: ./coverage.xml #optional
+          files: ./coverage.xml #optional
 
   docs_test:
       env:
         ENV_NAME: tests
         PYTHON: 3.9
       name: Tutorial Testing
       runs-on: ubuntu-latest
```

### Comparing `pyradiosky-0.2.0/.gitignore` & `pyradiosky-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/.pre-commit-config.yaml` & `pyradiosky-0.3.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,20 @@
           - flake8-comprehensions
           - flake8-docstrings
           - flake8-pytest-style
           - flake8-rst-docstrings
           - pep8-naming
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
         - id: black
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args: [--skip, "B101", --recursive, pyuvdata]
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
```

### Comparing `pyradiosky-0.2.0/.readthedocs.yml` & `pyradiosky-0.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/CHANGELOG.md` & `pyradiosky-0.3.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,49 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.3.0] - 2023-03-06
 
-## [0.2.0] - 2023-01-01
+### Added
+- A `freq_edge_array` parameter to store the top and bottom of the sub-bands with shape
+(2, Nfreqs). This will become required for objects with "subband" spectral types in
+version 0.5. A `freq_edge_array` parameter was also added to the `read_votable_file`,
+`read` and `from_file` methods.
+
+### Changed
+- When writing to text files, "subband" spectral types are represented in the same
+way as "full" spectral types (losing the frequency edge array information).
+- Increase the minimum compatible version for lunarsky to 0.2.1 to fix astropy
+deprecation warnings.
+
+### Deprecated
+- Not setting the `freq_edge_array` parameter for subband spectral types.
+
+### Removed
+- Defaulting for the coordinate frame, `frame` is now required to be passed to
+the `__init__` method for Healpix maps and point-like components when passing individual
+components rather than a SkyCoord object. It is also required to be passed to the `read_votable_file` method.
+- Handling for accessing the deprecated `ra_dec_coherency`, `lon`, `lat` attributes.
+- Handling for accessing galactic `l` and `b` coordinates as `gl` and `gb`.
+- The `point_to_healpix` method, use the `assign_to_healpix` instead.
+- The `frame` parameter to the `assign_to_healpix` method. The frame from the object's
+skycoord parameter is now always used for the Healpix frame, use `transform_to` to
+convert to the desired frame before calling `assign_to_healpix`.
+- The `source_cuts` method and the associated `source_select_keywords` parameters from
+the various `read` methods.
+- The `to_recarray` and `from_recarray` methods.
+- Support for reading old `healvis` style Healpix hdf5 files (via the associated
+`read_healpix_hdf5`, `from_healpix_hdf5` and `write_healpix_hdf5` methods). skyh5
+files are now the only supported hdf5 file format.
+- The `ra_column` and `dec_column` parameters to the `read` and `from_file` methods. Use
+the more generic `lon_column` and `lat_column` parameters instead.
+
+
+## [0.2.0] - 2023-02-01
 
 ### Added
 - Add support for all astropy coordinate frames with the new `skycoord` attribute (which
 contains an astropy SkyCoord object) on point objects and the new `hpx_frame` attribute
 on healpix objects. Users can interact with the SkyCoord object directly or use
 convenience methods on SkyModel as appropriate. References to older SkyModel attributes
 are handled for backwards compatibility.
```

### Comparing `pyradiosky-0.2.0/CODE_OF_CONDUCT.md` & `pyradiosky-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/LICENSE` & `pyradiosky-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/PKG-INFO` & `pyradiosky-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyradiosky
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python objects and interfaces for representing diffuse, extended and compact astrophysical radio sources
 Home-page: https://github.com/RadioAstronomySoftwareGroup/pyradiosky
 Author: Radio Astronomy Software Group
 License: BSD
 Keywords: radio astronomy
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -82,15 +82,15 @@
 * pyuvdata>=2.2.10
 * setuptools_scm>=7.0.3
 
 Optional:
 
 * astropy-healpix>=0.6 (for working with beams in HEALPix formats)
 * astroquery>=0.4.4 (for downloading GLEAM and other VizieR catalogs)
-* lunarsky>=0.1.2 (for supporting telescope locations on the moon)
+* lunarsky>=0.2.1 (for supporting telescope locations on the moon)
 
 We suggest using conda to install all the dependencies. To install
 pyuvdata, astropy-healpix and astroquery, you'll need to add conda-forge as a channel
 (```conda config --add channels conda-forge```).
 
 If you do not want to use conda, the packages are also available on PyPI.
 You can install the optional dependencies via pip by specifying an option
```

### Comparing `pyradiosky-0.2.0/README.md` & `pyradiosky-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 * pyuvdata>=2.2.10
 * setuptools_scm>=7.0.3
 
 Optional:
 
 * astropy-healpix>=0.6 (for working with beams in HEALPix formats)
 * astroquery>=0.4.4 (for downloading GLEAM and other VizieR catalogs)
-* lunarsky>=0.1.2 (for supporting telescope locations on the moon)
+* lunarsky>=0.2.1 (for supporting telescope locations on the moon)
 
 We suggest using conda to install all the dependencies. To install
 pyuvdata, astropy-healpix and astroquery, you'll need to add conda-forge as a channel
 (```conda config --add channels conda-forge```).
 
 If you do not want to use conda, the packages are also available on PyPI.
 You can install the optional dependencies via pip by specifying an option
```

### Comparing `pyradiosky-0.2.0/docs/Images/fhd_catalog_refflux_nonzerospec.png` & `pyradiosky-0.3.0/docs/Images/fhd_catalog_refflux_nonzerospec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/fhd_catalog_refflux_zerospec.png` & `pyradiosky-0.3.0/docs/Images/fhd_catalog_refflux_zerospec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_fluxcounts.png` & `pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_fluxcounts.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_radec.png` & `pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_radec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_radec_32768.png` & `pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_radec_32768.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/fhd_catalog_with_beam_values_refspec.png` & `pyradiosky-0.3.0/docs/Images/fhd_catalog_with_beam_values_refspec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_fluxcounts.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_fluxcounts.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_freqflux.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_freqflux.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_Jy.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_Jy.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_K.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_K.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_compare.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_compare.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_fluxselect.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_fluxselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_lonselect.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_lonselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_newfreq.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_newfreq.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gleam_50srcs_radec_oldfreq.png` & `pyradiosky-0.3.0/docs/Images/gleam_50srcs_radec_oldfreq.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_fluxcounts.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_fluxcounts.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_fluxcounts_150MHzatfreq.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_fluxcounts_150MHzatfreq.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_fluxcounts_150MHzfreqind.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_fluxcounts_150MHzfreqind.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_glgb_coneselect.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_glgb_coneselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_glgb_neighborselect.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_glgb_neighborselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_phiz_nested.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_phiz_nested.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_phiz_ring.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_phiz_ring.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_radec.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_radec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/gsm_icrs_radec_indselect.png` & `pyradiosky-0.3.0/docs/Images/gsm_icrs_radec_indselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/pointsource_catalog_radec.png` & `pyradiosky-0.3.0/docs/Images/pointsource_catalog_radec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Images/pointsource_catalog_radec_concat.png` & `pyradiosky-0.3.0/docs/Images/pointsource_catalog_radec_concat.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/Makefile` & `pyradiosky-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/conf.py` & `pyradiosky-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/conftest.py` & `pyradiosky-0.3.0/docs/conftest.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/make.bat` & `pyradiosky-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/make_index.py` & `pyradiosky-0.3.0/docs/make_index.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/make_skymodel.py` & `pyradiosky-0.3.0/docs/make_skymodel.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/docs/tutorial.rst` & `pyradiosky-0.3.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/__init__.py` & `pyradiosky-0.3.0/pyradiosky/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Define namespace."""
+from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 
-from pkg_resources import DistributionNotFound, get_distribution
 from setuptools_scm import get_version
 
 from .branch_scheme import branch_scheme
 
-try:  # pragma: nocover
+try:
     # get accurate version for developer installs
     version_str = get_version(Path(__file__).parent.parent, local_scheme=branch_scheme)
 
     __version__ = version_str
 
 except (LookupError, ImportError):
     try:
         # Set the version automatically from the package details.
-        __version__ = get_distribution(__name__).version
-    except DistributionNotFound:  # pragma: nocover
+        __version__ = version("pyradiosky")
+
+    except PackageNotFoundError:  # pragma: nocover
         # package is not installed
         pass
 
 from .skymodel import SkyModel
```

### Comparing `pyradiosky-0.2.0/pyradiosky/branch_scheme.py` & `pyradiosky-0.3.0/pyradiosky/branch_scheme.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/extended_source_test.sav` & `pyradiosky-0.3.0/pyradiosky/data/extended_source_test.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/fhd_catalog.sav` & `pyradiosky-0.3.0/pyradiosky/data/fhd_catalog.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/fhd_catalog_with_beam_values.sav` & `pyradiosky-0.3.0/pyradiosky/data/fhd_catalog_with_beam_values.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/gleam_50srcs.vot` & `pyradiosky-0.3.0/pyradiosky/data/gleam_50srcs.vot`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/gsm_galactic.skyh5` & `pyradiosky-0.3.0/pyradiosky/data/gsm_galactic.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/gsm_icrs.skyh5` & `pyradiosky-0.3.0/pyradiosky/data/gsm_icrs.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/healpix_disk.skyh5` & `pyradiosky-0.3.0/pyradiosky/data/healpix_disk.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/mock_hera_text_2458098.27471.txt` & `pyradiosky-0.3.0/pyradiosky/data/mock_hera_text_2458098.27471.txt`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/old_skyh5_point_sources.skyh5` & `pyradiosky-0.3.0/pyradiosky/data/old_skyh5_point_sources.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/simple_test.vot` & `pyradiosky-0.3.0/pyradiosky/data/simple_test.vot`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/data/single_source_old.vot` & `pyradiosky-0.3.0/pyradiosky/data/single_source_old.vot`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky/skymodel.py` & `pyradiosky-0.3.0/pyradiosky/skymodel.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,45 +6,52 @@
 import os
 import re
 import warnings
 
 import astropy.units as units
 import h5py
 import numpy as np
-import pyuvdata.utils as uvutils
 import scipy.io
 from astropy.coordinates import (
-    ICRS,
     AltAz,
     Angle,
     BaseCoordinateFrame,
     EarthLocation,
-    Galactic,
     Latitude,
     Longitude,
     SkyCoord,
 )
 from astropy.coordinates import concatenate as sc_concatenate
 from astropy.coordinates import frame_transform_graph
 from astropy.io import votable
 from astropy.time import Time
 from astropy.units import Quantity
-from pyuvdata.parameter import SkyCoordParameter, UVParameter
-from pyuvdata.uvbase import UVBase
-from pyuvdata.uvbeam.cst_beam import CSTBeam
 from scipy.linalg import orthogonal_procrustes as ortho_procr
 
+with warnings.catch_warnings():
+    # This filter can be removed when we require pyuvdata>=2.3
+    # is updated to use importlib.metadata rather than pkg_resources
+    warnings.filterwarnings(
+        "ignore", "Deprecated call to `pkg_resources.declare_namespace"
+    )
+    warnings.filterwarnings("ignore", "pkg_resources is deprecated as an API")
+    import pyuvdata.utils as uvutils
+    from pyuvdata.parameter import SkyCoordParameter, UVParameter
+    from pyuvdata.uvbase import UVBase
+    from pyuvdata.uvbeam.cst_beam import CSTBeam
+
 from . import __version__
 from . import spherical_coords_transforms as sct
 from . import utils as skyutils
 
 __all__ = ["hasmoon", "SkyModel"]
 
 try:
     from lunarsky import LunarTopo, MoonLocation
+    from lunarsky import SkyCoord as LunarSkyCoord
 
     hasmoon = True
 except ImportError:
     hasmoon = False
 
 
 class TelescopeLocationParameter(UVParameter):
@@ -291,14 +298,45 @@
         if isinstance(value, np.ndarray):
             value = np.array([n.tobytes().decode("utf8") for n in value[:]])
         else:
             value = value.tobytes().decode("utf8")
     return value
 
 
+def _get_freq_edges_from_centers(freq_array, tols, raise_error=True):
+    freq_unit = freq_array.unit
+    tols_use = []
+    for tol in tols:
+        if isinstance(tol, Quantity):
+            tols_use.append(tol.to(freq_unit).value)
+        else:
+            tols_use.append(tol)
+    tols_use = tuple(tols_use)
+    if freq_array.size == 1:
+        raise ValueError(
+            "Cannot calculate frequency edges from frequency center array because "
+            "there is only one frequency center."
+        )
+    if not uvutils._test_array_constant_spacing(freq_array.value, tols=tols_use):
+        raise ValueError(
+            "Cannot calculate frequency edges from frequency center array because "
+            "frequency center spacing is not constant."
+        )
+    freq_delta = np.mean(np.diff(freq_array.value)) * freq_unit
+
+    freq_edge_array = np.zeros((2, freq_array.size), dtype=freq_array.dtype) * freq_unit
+    freq_edge_array[0, :] = freq_array - freq_delta / 2.0
+    freq_edge_array[1, :] = freq_array + freq_delta / 2.0
+    return freq_edge_array
+
+
+def _get_freq_centers_from_edges(freq_edge_array):
+    return np.mean(freq_edge_array, axis=0)
+
+
 class SkyModel(UVBase):
     """
     Object to hold point source and diffuse models.
 
     Can be initialized using the :meth:`from_file` class method or :meth:`read` method,
     or by passing parameters listed below on object initialization. It can also be
     initialized as an empty object (by passing no parameters on object initialization),
@@ -341,20 +379,30 @@
         the polarization as [I, Q, U, V].
     spectral_type : str
         Indicates how fluxes should be calculated at each frequency.
 
         Options:
 
             - 'flat' : Flat spectrum.
-            - 'full' : Flux is defined by a saved value at each frequency.
+            - 'full' : Flux is defined by a value at each frequency.
             - 'subband' : Flux is given at a set of band centers.
             - 'spectral_index' : Flux is given at a reference frequency.
 
     freq_array : :class:`astropy.units.Quantity`
-        Array of frequencies that fluxes are provided for, shape (Nfreqs,).
+        Array of frequencies that fluxes are provided for, shape (Nfreqs,). If
+        freq_edge_array is passed and freq_array is not set, freq_array will be
+        calculated as the mean of the frequency edges per channel.
+    freq_edge_array : :class:`astropy.units.Quantity`
+        Array of frequencies giving the edges of the frequency bands, shape (2, Nfreqs).
+        The zeroth index in the first dimension is for the lower edge of the band, the
+        first index is for the upper edge. Only required for the `subband`
+        spectral_type. If freq_array is a regularly spaced array and freq_edge_array
+        is not set, freq_edge_array will be calculated from the freq_array assuming the
+        band edges are directly between the band centers. An error will be raised if
+        freq_array is not regularly spaced and freq_edge_array is not set.
     reference_frequency : :class:`astropy.units.Quantity`
         Reference frequencies of flux values, shape (Ncomponents,).
     spectral_index : array_like of float
         Spectral index of each source, shape (Ncomponents).
         None if spectral_type is not 'spectral_index'.
     component_type : str
         Component type, either 'point' or 'healpix'. If this is not set, the type is
@@ -396,23 +444,26 @@
             self._name.required = True
             self._skycoord.required = True
             self._hpx_inds.required = False
             self._nside.required = False
             self._hpx_order.required = False
             self._hpx_frame.required = False
 
-    @units.quantity_input(freq_array=units.Hz, reference_frequency=units.Hz)
+    @units.quantity_input(
+        freq_array=units.Hz, freq_edge_array=units.Hz, reference_frequency=units.Hz
+    )
     def __init__(
         self,
         name=None,
         ra=None,
         dec=None,
         stokes=None,
         spectral_type=None,
         freq_array=None,
+        freq_edge_array=None,
         lon=None,
         lat=None,
         gl=None,
         gb=None,
         frame=None,
         skycoord=None,
         reference_frequency=None,
@@ -506,25 +557,42 @@
             "hpx_inds",
             description=desc,
             form=("Ncomponents",),
             expected_type=int,
             required=False,
         )
 
-        desc = "Frequency array in Hz, only required if spectral_type is 'full' or 'subband'."
+        desc = (
+            "Frequency array giving the center frequency in Hz, only required if "
+            "spectral_type is 'full' or 'subband'."
+        )
         self._freq_array = UVParameter(
             "freq_array",
             description=desc,
             form=("Nfreqs",),
             expected_type=Quantity,
             required=False,
             tols=self.freq_tol,
         )
 
         desc = (
+            "Array giving the frequency  band edges in Hz, only required if "
+            "spectral_type is 'subband'. The zeroth index in the first dimension holds "
+            "the lower band edge and the first index holds the upper band edge."
+        )
+        self._freq_edge_array = UVParameter(
+            "freq_edge_array",
+            description=desc,
+            form=(2, "Nfreqs"),
+            expected_type=Quantity,
+            required=False,
+            tols=self.freq_tol,
+        )
+
+        desc = (
             "Reference frequency in Hz, only required if spectral_type is "
             "'spectral_index'. shape (Ncomponents,)"
         )
         self._reference_frequency = UVParameter(
             "reference_frequency",
             description=desc,
             form=("Ncomponents",),
@@ -686,17 +754,18 @@
             self._set_component_type_params(component_type)
         elif nside is not None:
             self._set_component_type_params("healpix")
         else:
             self._set_component_type_params("point")
 
         if self.component_type == "healpix":
-            req_args = ["nside", "hpx_inds", "stokes", "spectral_type"]
+            req_args = ["nside", "frame", "hpx_inds", "stokes", "spectral_type"]
             args_set_req = [
                 nside is not None,
+                frame is not None,
                 hpx_inds is not None,
                 stokes is not None,
                 spectral_type is not None,
             ]
         else:
             if skycoord is not None:
                 location_param_names = ["lon", "lat", "ra", "dec", "gl", "gb", "frame"]
@@ -728,51 +797,34 @@
                 input_combo = {k for k, v in coords_given.items() if v}
 
                 if input_combo not in valid_combos:
                     raise ValueError(
                         f"Invalid input coordinate combination: {input_combo}"
                     )
 
-                if input_combo == {"lat", "lon"} and frame is None:
+                if len(input_combo) > 0 and frame is None:
                     raise ValueError(
-                        "The 'frame' keyword must be set to initialize from lat/lon."
+                        "The 'frame' keyword must be set to initialize from coordinates."
                     )
 
-                if (ra is not None) and (dec is not None):
-                    lon = ra
-                    lat = dec
-                    if frame is None:
-                        warnings.warn(
-                            "No frame was specified for RA and Dec. Defaulting to ICRS, "
-                            "but this will become an error in version 0.3 and later.",
-                            DeprecationWarning,
-                        )
-                        frame = ICRS
-                elif (gl is not None) and (gb is not None):
-                    lon = gl
-                    lat = gb
-                    if frame is None:
-                        warnings.warn(
-                            "No frame was specified for gl and gb. Defaulting to galactic, "
-                            "but this will become an error in version 0.3 and later.",
-                            DeprecationWarning,
-                        )
-                        frame = Galactic
-
                 frame = _get_frame_obj(frame)
 
                 if (ra is not None) and (dec is not None):
+                    lon = ra
+                    lat = dec
                     dummy_skycoord = SkyCoord(0, 0, unit="deg", frame=frame)
                     comp_names = _get_lon_lat_component_names(dummy_skycoord)
                     if comp_names[0] != "ra" or comp_names[1] != "dec":
                         raise ValueError(
                             f"ra or dec supplied but specified frame {frame.name} does "
                             "not support ra and dec coordinates."
                         )
                 elif (gl is not None) and (gb is not None):
+                    lon = gl
+                    lat = gb
                     dummy_skycoord = SkyCoord(0, 0, unit="deg", frame=frame)
                     comp_names = _get_lon_lat_component_names(dummy_skycoord)
                     if comp_names[0] != "l" or comp_names[1] != "b":
                         raise ValueError(
                             f"gl or gb supplied but specified frame {frame.name} does "
                             "not support gl and gb coordinates."
                         )
@@ -820,22 +872,34 @@
             ]
 
         if spectral_type == "spectral_index":
             req_args.extend(["spectral_index", "reference_frequency"])
             args_set_req.extend(
                 [spectral_index is not None, reference_frequency is not None]
             )
-        elif spectral_type in ["full", "subband"]:
+        elif spectral_type == "subband":
+            if freq_edge_array is not None:
+                req_args.append("freq_edge_array")
+                args_set_req.append(freq_edge_array is not None)
+            else:
+                req_args.append("freq_array")
+                args_set_req.append(freq_array is not None)
+        elif spectral_type == "full":
             req_args.append("freq_array")
             args_set_req.append(freq_array is not None)
 
         args_set_req = np.array(args_set_req, dtype=bool)
 
         arg_set_opt = np.array(
-            [freq_array is not None, reference_frequency is not None], dtype=bool
+            [
+                freq_array is not None,
+                reference_frequency is not None,
+                freq_edge_array is not None,
+            ],
+            dtype=bool,
         )
 
         if np.any(np.concatenate((args_set_req, arg_set_opt))):
             if not np.all(args_set_req):
                 isset = [k for k, v in zip(req_args, args_set_req) if v]
                 raise ValueError(
                     f"If initializing with values, all of {req_args} must be set."
@@ -859,44 +923,46 @@
                         f"hpx_order must be one of {self._hpx_order.acceptable_vals}"
                     )
 
             if self.component_type == "healpix":
                 if self.hpx_order is None:
                     self.hpx_order = "ring"
 
-                if frame is None:
-                    warnings.warn(
-                        "In version 0.3.0, the frame keyword will be required for "
-                        "HEALPix maps. Defaulting to ICRS",
-                        category=DeprecationWarning,
-                    )
-                    dummy_skycoord = SkyCoord(0, 0, unit="deg", frame="icrs")
-                    self.hpx_frame = dummy_skycoord.frame.replicate_without_data(
-                        copy=True
-                    )
-                else:
-                    frame = _get_frame_obj(frame)
-                    dummy_skycoord = SkyCoord(0, 0, unit="deg", frame=frame)
+                frame = _get_frame_obj(frame)
+                dummy_skycoord = SkyCoord(0, 0, unit="deg", frame=frame)
 
-                    self.hpx_frame = dummy_skycoord.frame.replicate_without_data(
-                        copy=True
-                    )
+                self.hpx_frame = dummy_skycoord.frame.replicate_without_data(copy=True)
 
                 self.Ncomponents = self.hpx_inds.size
 
             else:
                 self.Ncomponents = self.name.size
 
             self._set_spectral_type_params(spectral_type)
 
             if freq_array is not None:
                 self.freq_array = np.atleast_1d(freq_array)
                 self.Nfreqs = self.freq_array.size
+
+                if freq_edge_array is not None:
+                    self.freq_edge_array = freq_edge_array
+                elif self.spectral_type == "subband":
+                    warnings.warn(
+                        "freq_edge_array not set, calculating it from the freq_array."
+                    )
+                    self.freq_edge_array = _get_freq_edges_from_centers(
+                        freq_array=self.freq_array, tols=self._freq_array.tols
+                    )
             else:
-                self.Nfreqs = 1
+                if freq_edge_array is not None:
+                    self.freq_edge_array = freq_edge_array
+                    self.freq_array = _get_freq_centers_from_edges(freq_edge_array)
+                    self.Nfreqs = self.freq_array.size
+                else:
+                    self.Nfreqs = 1
 
             if reference_frequency is not None:
                 self.reference_frequency = np.atleast_1d(reference_frequency)
 
             if spectral_index is not None:
                 self.spectral_index = np.atleast_1d(spectral_index)
 
@@ -952,77 +1018,26 @@
                 self.history, self.pyradiosky_version_str
             ):
                 self.history += self.pyradiosky_version_str
 
             self.check()
 
     def __getattr__(self, name):
-        """
-        Handle references to frame coordinates (ra/dec/gl/gb, etc.).
-
-        Also Provide ra and dec for healpix objects with deprecation warnings.
-        """
-        if name == "lon":
-            warnings.warn(
-                "lon is no longer a parameter on SkyModel objects. Use "
-                "`get_lon_lat` to get the longitudinal and latidudinal values. "
-                "Starting in version 0.3.0 this call will error.",
-                category=DeprecationWarning,
-            )
-            lon, _ = self.get_lon_lat()
-            return lon
-        elif name == "lat":
-            warnings.warn(
-                "lat is no longer a parameter on SkyModel objects. Use "
-                "`get_lon_lat` to get the longitudinal and latidudinal values. "
-                "Starting in version 0.3.0 this call will error.",
-                category=DeprecationWarning,
-            )
-            _, lat = self.get_lon_lat()
-            return lat
-
-        if name == "coherency_radec":
-            warnings.warn(
-                "coherency_radec is a deprecated parameter, use frame_coherency "
-                "instead. Frame coherency is an optional parameter and is not set on "
-                "when the object is initialized. Use `calc_frame_coherency` to "
-                "calculate it and optionally save it on the object. Starting in "
-                "version 0.3.0 this call will error.",
-                category=DeprecationWarning,
-            )
-            if self.frame_coherency is None:
-                self.calc_frame_coherency()
-            return self.frame_coherency
-
+        """Handle references to frame coordinates (ra/dec/gl/gb, etc.)."""
         if name == "frame":
             if self.skycoord is not None:
                 return self.skycoord.frame.name
             else:
                 return self.hpx_frame.name
 
         if not name.startswith("__"):
             # Naming for galactic is different from astropy:
-            galactic_warning = False
-            if name == "gl":
-                galactic_warning = True
-                name = "l"
-            if name == "gb":
-                galactic_warning = True
-                name = "b"
             comp_names = self._get_lon_lat_component_names()
             if name in comp_names:
                 if self.skycoord is not None:
-                    if galactic_warning:
-                        warnings.warn(
-                            "gl and gb are no longer parameters on SkyModel objects "
-                            "in the galactic frame. Use the standard astropy labels "
-                            "l and b instead. "
-                            "Starting in version 0.3.0 this call will error.",
-                            category=DeprecationWarning,
-                        )
                     return getattr(self.skycoord, name)
                 warnings.warn(
                     "It is more efficient to use the `get_lon_lat` method to get "
                     "longitudinal and latitudinal coordinates for HEALPix maps."
                 )
                 comp_ind = np.nonzero(np.array(comp_names) == name)[0][0]
                 lon_lat = self.get_lon_lat()
@@ -1036,15 +1051,22 @@
         self.spectral_type = spectral_type
 
         if spectral_type == "spectral_index":
             self._spectral_index.required = True
             self._reference_frequency.required = True
             self._Nfreqs.acceptable_vals = [1]
             self._freq_array.required = False
-        elif spectral_type in ["full", "subband"]:
+        elif spectral_type == "subband":
+            self._freq_array.required = True
+            # TODO: make _freq_edge_array required in v0.5
+            # (and not required in other spectral types)
+            self._spectral_index.required = False
+            self._reference_frequency.required = False
+            self._Nfreqs.acceptable_vals = None
+        elif spectral_type == "full":
             self._freq_array.required = True
             self._spectral_index.required = False
             self._reference_frequency.required = False
             self._Nfreqs.acceptable_vals = None
         elif spectral_type == "flat":
             self._freq_array.required = False
             self._spectral_index.required = False
@@ -1092,14 +1114,30 @@
 
         # make sure only one of freq_array and reference_frequency is defined
         if self.freq_array is not None and self.reference_frequency is not None:
             raise ValueError(
                 "Only one of freq_array and reference_frequency can be specified, not both."
             )
 
+        if self.freq_edge_array is None and self.spectral_type == "subband":
+            msg = "freq_edge_array is not set. "
+            try:
+                self.freq_edge_array = _get_freq_edges_from_centers(
+                    freq_array=self.freq_array, tols=self._freq_array.tols
+                )
+                msg += "Calculating it from the freq_array. "
+            except ValueError:
+                msg += (
+                    "Cannot calculate it from the freq_array because freq_array "
+                    "spacing is not constant. "
+                )
+            warnings.warn(
+                msg + "This will become an error in version 0.5", DeprecationWarning
+            )
+
         # Run the basic check from UVBase
         super(SkyModel, self).check(
             check_extra=check_extra, run_check_acceptability=run_check_acceptability
         )
 
         # check units on stokes & frame_coherency
         for param in [self._stokes, self._frame_coherency]:
@@ -1141,19 +1179,18 @@
         return True
 
     def __eq__(
         self, other, check_extra=True, allowed_failures="filename", silent=False
     ):
         """Check for equality, check for future equality."""
         # Run the basic __eq__ from UVBase
-        # the filters below should be removed in version 0.3.0
+        # the filters below should be removed when we require pyuvdata>=2.3
         with warnings.catch_warnings():
             try:
-                # The `silent` parameter was added in the version *after* pyuvdata
-                # version 2.2.12
+                # The `silent` parameter was added in pyuvdata between 2.2.12 and 2.3
                 equal = super(SkyModel, self).__eq__(
                     other,
                     check_extra=check_extra,
                     allowed_failures=allowed_failures,
                     silent=silent,
                 )
             except TypeError:
@@ -1271,19 +1308,15 @@
             )
         #  quickly check the validity of the transformation using a dummy SkyCoord object.
         coords = SkyCoord(0, 0, unit="rad", frame=this.hpx_frame)
 
         # we will need the starting frame object for some interpolation later
         old_frame = coords.frame.replicate_without_data(copy=True)
 
-        # This filter can be removed when lunarsky is updated to not trigger this
-        # astropy deprecation warning.
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", message="The get_frame_attr_names")
-            coords = coords.transform_to(frame)
+        coords = coords.transform_to(frame)
 
         frame = coords.frame.replicate_without_data(copy=True)
 
         hp_obj_new = astropy_healpix.HEALPix(
             nside=this.nside, order=this.hpx_order, frame=frame
         )
         hp_obj_old = astropy_healpix.HEALPix(
@@ -1610,69 +1643,18 @@
             self.jansky_to_kelvin()
 
         if run_check:
             self.check(
                 check_extra=check_extra, run_check_acceptability=run_check_acceptability
             )
 
-    def point_to_healpix(
-        self, to_k=True, run_check=True, check_extra=True, run_check_acceptability=True
-    ):
-        """
-        Convert a point component_type object to a healpix component_type.
-
-        Deprecated. Use :meth:`assign_to_healpix` to assign point components to a healpix
-        grid. Use :meth:`_point_to_healpix` to undo a :meth:`healpix_to_point` conversion.
-
-        This method only works for objects that were originally healpix objects but
-        were converted to `point` component type using :meth:`healpix_to_point`. This
-        method undoes that conversion.
-        It does NOT assign general point components to a healpix grid.
-
-        Requires that the ``hpx_inds`` and ``nside`` parameters are set on the object.
-        Divide by the pixel area and optionally convert to K.
-        This method is provided as a convenience for users to be able to undo
-        the `healpix_to_point` method.
-
-        Parameters
-        ----------
-        to_k : bool
-            Option to convert to K compatible units.
-        run_check : bool
-            Option to check for the existence and proper shapes of parameters
-            after downselecting data on this object (the default is True,
-            meaning the check will be run).
-        check_extra : bool
-            Option to check optional parameters as well as required ones (the
-            default is True, meaning the optional parameters will be checked).
-        run_check_acceptability : bool
-            Option to check acceptable range of the values of parameters after
-            downselecting data on this object (the default is True, meaning the
-            acceptable range check will be done).
-
-        """
-        warnings.warn(
-            "This method is deprecated and will be removed in version 0.3.0. Please "
-            "use `assign_to_healpix` to assign point components to a healpix "
-            "grid. Use `_point_to_healpix` to undo a `healpix_to_point` conversion.",
-            category=DeprecationWarning,
-        )
-
-        self._point_to_healpix(
-            to_k=to_k,
-            run_check=run_check,
-            check_extra=check_extra,
-            run_check_acceptability=run_check_acceptability,
-        )
-
     def assign_to_healpix(
         self,
         nside,
         order="ring",
-        frame=None,
         to_k=True,
         full_sky=False,
         sort=True,
         inplace=False,
         run_check=True,
         check_extra=True,
         run_check_acceptability=True,
@@ -1701,20 +1683,14 @@
             Option to convert to K compatible units.
         full_sky : bool
             Option to create a full sky healpix map with zeros in the stokes array
             for pixels with no sources assigned to them. If False only pixels with
             sources mapped to them will be included in the object.
         sort : bool
             Option to sort the object in order of the healpix indicies.
-        frame : str, `BaseCoordinateFrame` class or instance
-            Deprecated. The frame of the input point source catalog.
-            Defaults to the the object's skycoord.frame attribute. Only "galactic" or
-            "icrs" are accepted through this keyword but any astropy compatible frame
-            can be used from the object's skycoord.frame attribute. Use the
-            `transform_to` method to change the skycoord frame.
         inplace : bool
             Option to do the change in place on the object rather than return a new
             object.
         run_check : bool
             Option to check for the existence and proper shapes of parameters
             after downselecting data on this object (the default is True,
             meaning the check will be run).
@@ -1743,46 +1719,22 @@
         except ImportError as e:
             raise ImportError(
                 "The astropy-healpix module must be installed to use HEALPix methods"
             ) from e
 
         sky = self if inplace else self.copy()
 
-        if frame is None:
-            frame_obj = self.skycoord.frame.replicate_without_data(copy=True)
-            sky.hpx_frame = frame_obj
-        else:
-            warnings.warn(
-                "The frame keyword is deprecated, in version 0.3.0 this method will use "
-                "the frame of this object's skycoord attribute.",
-                DeprecationWarning,
-            )
-            # easiest way to do frame checking is through making a dummy skycoord
-            coords = SkyCoord(0, 0, unit="deg", frame=frame)
-
-            frame_obj = coords.frame.replicate_without_data(copy=True)
-
-            if sky.skycoord.frame.name != coords.frame.name:
-                warnings.warn(
-                    f"Input parameter frame (value: {frame_obj.name}) differs "
-                    "from the skycoord frame on this object (value: "
-                    f"{sky.skycoord.frame.name}). "
-                    "Using input frame for coordinate calculations."
-                )
-            sky.hpx_frame = frame_obj
+        frame_obj = self.skycoord.frame.replicate_without_data(copy=True)
+        sky.hpx_frame = frame_obj
 
         # clear time & position specific parameters
         sky.clear_time_position_specific_params()
 
         hpx_obj = astropy_healpix.HEALPix(nside, order=order, frame=frame_obj)
-        # This filter can be removed when lunarsky is updated to not trigger this
-        # astropy deprecation warning.
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", message="The get_frame_attr_names")
-            hpx_inds = hpx_obj.skycoord_to_healpix(sky.skycoord)
+        hpx_inds = hpx_obj.skycoord_to_healpix(self.skycoord)
 
         sky._set_component_type_params("healpix")
         sky.nside = nside
         sky.hpx_order = order
         # now check for duplicates. If they exist, sum the flux in them
         # if other parameters have variable values, raise appropriate errors
         if hpx_inds.size > np.unique(hpx_inds).size:
@@ -1927,14 +1879,15 @@
             new_obj = SkyModel(
                 component_type="healpix",
                 frame=sky.hpx_frame,
                 nside=sky.nside,
                 hpx_order=sky.hpx_order,
                 spectral_type=sky.spectral_type,
                 freq_array=sky.freq_array,
+                freq_edge_array=sky.freq_edge_array,
                 hpx_inds=new_inds,
                 stokes=new_stokes,
                 stokes_error=new_stokes_error,
                 reference_frequency=new_reference_frequency,
                 spectral_index=new_spectral_index,
                 beam_amp=new_beam_amp,
                 extended_model_group=new_extmod,
@@ -1963,14 +1916,15 @@
             sky.check(
                 check_extra=check_extra, run_check_acceptability=run_check_acceptability
             )
 
         if not inplace:
             return sky
 
+    @units.quantity_input(freqs=units.Hz)
     def at_frequencies(
         self,
         freqs,
         inplace=True,
         freq_interp_kind="cubic",
         nan_handling="clip",
         run_check=True,
@@ -2049,14 +2003,16 @@
             )
 
             if np.sum(matches) != freqs.size:
                 raise ValueError(
                     "Some requested frequencies are not present in the current SkyModel."
                 )
             sky.stokes = self.stokes[:, matches, :]
+            if sky.freq_edge_array is not None:
+                sky.freq_edge_array = sky.freq_edge_array[:, matches]
         elif self.spectral_type == "subband":
             if np.max(freqs.to("Hz")) > np.max(self.freq_array.to("Hz")):
                 raise ValueError(
                     "A requested frequency is larger than the highest subband frequency."
                 )
             if np.min(freqs.to("Hz")) < np.min(self.freq_array.to("Hz")):
                 raise ValueError(
@@ -2238,16 +2194,18 @@
         else:
             # flat spectrum
             stokes_unit = self.stokes.unit
             sky.stokes = np.repeat(self.stokes.value, len(freqs), axis=1) * stokes_unit
 
         sky.reference_frequency = None
         sky.Nfreqs = freqs.size
-        sky.spectral_type = "full"
         sky.freq_array = freqs
+        if sky.spectral_type == "subband" and sky.freq_edge_array is not None:
+            sky.freq_edge_array = None
+        sky.spectral_type = "full"
         if sky.frame_coherency is not None:
             sky.coherency_radec = sky.calc_frame_coherency()
 
         if run_check:
             sky.check()
 
         if not inplace:
@@ -2273,16 +2231,18 @@
             Telescope location to update positions for.
         """
         if not isinstance(time, Time):
             raise ValueError(
                 "time must be an astropy Time object. value was: {t}".format(t=time)
             )
 
-        if not isinstance(telescope_location, self._telescope_location.expected_type):
-
+        if not (
+            isinstance(telescope_location, EarthLocation)
+            or (hasmoon and isinstance(telescope_location, MoonLocation))
+        ):
             errm = "telescope_location must be an :class:`astropy.EarthLocation` object"
             if hasmoon:
                 errm += " or a :class:`lunarsky.MoonLocation` object "
             errm += ". "
             raise ValueError(
                 errm + "value was: {al}".format(al=str(telescope_location))
             )
@@ -2295,26 +2255,24 @@
         self.telescope_location = telescope_location
 
         if self.component_type == "healpix":
             skycoord_use = SkyCoord(*self.get_lon_lat(), frame=self.hpx_frame)
         else:
             skycoord_use = self.skycoord
 
-        # This filter can be removed when lunarsky is updated to not trigger this
-        # astropy deprecation warning.
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", message="The get_frame_attr_names")
-            if hasmoon and isinstance(self.telescope_location, MoonLocation):
+        if isinstance(telescope_location, EarthLocation):
+            source_altaz = skycoord_use.transform_to(
+                AltAz(obstime=self.time, location=self.telescope_location)
+            )
+        else:
+            skycoord_use = LunarSkyCoord(skycoord_use)
+            if isinstance(self.telescope_location, MoonLocation):
                 source_altaz = skycoord_use.transform_to(
                     LunarTopo(obstime=self.time, location=self.telescope_location)
                 )
-            else:
-                source_altaz = skycoord_use.transform_to(
-                    AltAz(obstime=self.time, location=self.telescope_location)
-                )
 
         alt_az = np.array([source_altaz.alt.rad, source_altaz.az.rad])
 
         self.alt_az = alt_az
 
         pos_l = np.sin(alt_az[1, :]) * np.cos(alt_az[0, :])
         pos_m = np.cos(alt_az[1, :]) * np.cos(alt_az[0, :])
@@ -2361,33 +2319,41 @@
             shape (3, 3).
         """
         # unit vectors to be transformed by astropy
         x_c = np.array([1.0, 0, 0])
         y_c = np.array([0, 1.0, 0])
         z_c = np.array([0, 0, 1.0])
 
-        axes_frame = SkyCoord(
-            x=x_c,
-            y=y_c,
-            z=z_c,
-            obstime=self.time,
-            location=self.telescope_location,
-            frame=self._get_frame_obj(),
-            representation_type="cartesian",
-        )
+        if isinstance(self.telescope_location, EarthLocation):
+            axes_icrs = SkyCoord(
+                x=x_c,
+                y=y_c,
+                z=z_c,
+                obstime=self.time,
+                location=self.telescope_location,
+                frame="icrs",
+                representation_type="cartesian",
+            )
+            axes_altaz = axes_icrs.transform_to("altaz")
+        else:
+            axes_icrs = LunarSkyCoord(
+                x=x_c,
+                y=y_c,
+                z=z_c,
+                obstime=self.time,
+                location=self.telescope_location,
+                frame="icrs",
+                representation_type="cartesian",
+            )
+            axes_altaz = axes_icrs.transform_to("lunartopo")
 
-        # This filter can be removed when lunarsky is updated to not trigger this
-        # astropy deprecation warning.
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", message="The get_frame_attr_names")
-            axes_altaz = axes_frame.transform_to("altaz")
         axes_altaz.representation_type = "cartesian"
 
-        """ This transformation matrix is generally not orthogonal
-            to better than 10^-7, so let's fix that. """
+        # This transformation matrix is generally not orthogonal to better than 10^-7,
+        # so let's fix that.
 
         R_screwy = axes_altaz.cartesian.xyz
         R_really_orthogonal, _ = ortho_procr(R_screwy, np.eye(3))
 
         # Note the transpose, to be consistent with calculation in sct
         R_really_orthogonal = np.array(R_really_orthogonal).T
 
@@ -2511,21 +2477,21 @@
                 "Horizon cutoff undefined. Assuming all source components "
                 "are above the horizon."
             )
             above_horizon = np.ones(self.Ncomponents).astype(bool)
         else:
             above_horizon = self.above_horizon
 
-        if not isinstance(
-            self.telescope_location, self._telescope_location.expected_type
+        if not (
+            isinstance(self.telescope_location, EarthLocation)
+            or (hasmoon and isinstance(self.telescope_location, MoonLocation))
         ):
-
-            errm = "telescope_location must be an astropy EarthLocation object"
+            errm = "telescope_location must be an :class:`astropy.EarthLocation` object"
             if hasmoon:
-                errm += " or a lunarsky MoonLocation object "
+                errm += " or a :class:`lunarsky.MoonLocation` object "
             errm += ". "
             raise ValueError(
                 errm + "value was: {al}".format(al=str(self.telescope_location))
             )
 
         if self.frame_coherency is None:
             self.calc_frame_coherency(store=store_frame_coherency)
@@ -2544,15 +2510,14 @@
             )
 
             # Indices of polarized sources in the full Ncomponents array,
             # downselected to those that are above the horizon.
             full_pol_over_hor = [pi for pi in self._polarized if above_horizon[pi]]
 
             if len(pol_over_hor) > 0:
-
                 rotation_matrix = self._calc_coherency_rotation(full_pol_over_hor)
 
                 rotation_matrix_T = np.swapaxes(rotation_matrix, 0, 1)
                 coherency_local[:, :, :, pol_over_hor] = np.einsum(
                     "aby,bcxy,cdy->adxy",
                     rotation_matrix_T,
                     self.frame_coherency[:, :, :, full_pol_over_hor],
@@ -2636,14 +2601,16 @@
         )
 
         # Define parameters that must be the same to add objects
         compatibility_params = ["_component_type", "_spectral_type"]
 
         if this.spectral_type in ["subband", "full"]:
             compatibility_params.append("_freq_array")
+        if this.spectral_type == "subband":
+            compatibility_params.append("_freq_edge_array")
 
         if this.component_type == "healpix":
             compatibility_params.extend(["_nside", "_hpx_order"])
 
         time_pos_params = ["_" + name for name in this._time_position_params]
         if clear_time_position:
             # clear time & position specific parameters on both objects
@@ -3170,138 +3137,25 @@
             check_extra=check_extra,
             run_check_acceptability=run_check_acceptability,
         )
 
         if not inplace:
             return skyobj
 
-    def source_cuts(
-        self,
-        latitude_deg=None,
-        horizon_buffer=0.04364,
-        min_flux=None,
-        max_flux=None,
-        freq_range=None,
-        run_check=True,
-        check_extra=True,
-        run_check_acceptability=True,
-        inplace=True,
-    ):
-        """
-        Perform flux and horizon selections.
-
-        Parameters
-        ----------
-        latitude_deg : float
-            Latitude of telescope in degrees. Used to estimate rise/set lst.
-        horizon_buffer : float
-            Angle buffer for coarse horizon cut in radians.
-            Default is about 10 minutes of sky rotation. Components whose
-            calculated altitude is less than `horizon_buffer` are excluded.
-            Caution! The altitude calculation does not account for
-            precession/nutation of the Earth.
-            The buffer angle is needed to ensure that the horizon cut doesn't
-            exclude sources near but above the horizon. Since the cutoff is
-            done using lst, and the lsts are calculated with astropy, the
-            required buffer should _not_ drift with time since the J2000 epoch.
-            The default buffer has been tested around julian date 2457458.0.
-        min_flux : Quantity or float
-            Minimum stokes I flux to select. If not a Quantity, assumed to be in Jy.
-        max_flux : Quantity or float
-            Maximum stokes I flux to select. If not a Quantity, assumed to be in Jy.
-        freq_range : :class:`astropy.units.Quantity`
-            Frequency range over which the min and max flux tests should be performed.
-            Must be length 2. If None, use the range over which the object is defined.
-        run_check : bool
-            Option to check for the existence and proper shapes of parameters
-            after downselecting data on this object (the default is True,
-            meaning the check will be run).
-        check_extra : bool
-            Option to check optional parameters as well as required ones (the
-            default is True, meaning the optional parameters will be checked).
-        run_check_acceptability : bool
-            Option to check acceptable range of the values of parameters after
-            downselecting data on this object (the default is True, meaning the
-            acceptable range check will be done).
-        inplace : bool
-            Option to do the cuts on the object in place or to return a copy
-            with the cuts applied.
-
-        Returns
-        -------
-        :class:`SkyModel` object or ``None``
-            Returns ``None`` if ``inplace`` is True (the calling object is updated),
-            otherwise the modified :class:`SkyModel` object is returned.
-
-        """
-        warnings.warn(
-            "The `source_cuts` method is deprecated and will be removed in version "
-            "0.3.0. Please use the `select` method and/or the `cut_nonrising` "
-            "method as appropriate.",
-            category=DeprecationWarning,
-        )
-
-        if inplace:
-            skyobj = self
-        else:
-            skyobj = self.copy()
-
-        if freq_range is not None:
-            if not isinstance(freq_range, (Quantity,)):
-                raise ValueError("freq_range must be an astropy Quantity.")
-            if not np.atleast_1d(freq_range).size == 2:
-                raise ValueError("freq_range must have 2 elements.")
-
-        if min_flux is not None or max_flux is not None:
-            if min_flux is not None and not isinstance(min_flux, Quantity):
-                min_flux *= units.Jy
-            if max_flux is not None and not isinstance(max_flux, Quantity):
-                max_flux *= units.Jy
-            skyobj.select(
-                min_brightness=min_flux,
-                max_brightness=max_flux,
-                brightness_freq_range=freq_range,
-            )
-
-        if latitude_deg is not None:
-            skyobj.cut_nonrising(Latitude(latitude_deg, units.deg))
-            skyobj.calculate_rise_set_lsts(
-                Latitude(latitude_deg, units.deg), horizon_buffer=horizon_buffer
-            )
-
-        if run_check:
-            skyobj.check(
-                check_extra=check_extra, run_check_acceptability=run_check_acceptability
-            )
-
-        if not inplace:
-            return skyobj
-
     def _text_write_preprocess(self):
         """
         Set up a recarray to use for writing out as a text file.
 
         Returns
         -------
         catalog_table : recarray
             recarray with data for a text file.
 
         """
         self.check()
-        original_comp_type = self.component_type
-        if isinstance(self.stokes, Quantity):
-            original_units_k = self.stokes.unit.is_equivalent(
-                "K"
-            ) or self.stokes.unit.is_equivalent("K sr")
-
-        if self.component_type == "healpix":
-            self.healpix_to_point(to_jy=True)
-        else:
-            # make sure we're in Jy units
-            self.kelvin_to_jansky()
 
         max_name_len = np.max([len(name) for name in self.name])
         fieldtypes = ["U" + str(max_name_len), "f8", "f8"]
         comp_names = self._get_lon_lat_component_names()
         frame_obj = self._get_frame_obj()
         frame_desc_str = _get_frame_desc_str(frame_obj)
 
@@ -3383,191 +3237,16 @@
                 arr["spectral_index"] = self.spectral_index
 
         if hasattr(self, "_rise_lst"):
             arr["rise_lst"] = self._rise_lst
         if hasattr(self, "_set_lst"):
             arr["set_lst"] = self._set_lst
 
-        if original_comp_type == "healpix":
-            self._point_to_healpix()
-        if original_units_k:
-            self.jansky_to_kelvin()
-
         return arr
 
-    def to_recarray(self):
-        """
-        Make a recarray of source components from this object.
-
-        Deprecated, will be removed in version 0.3.0.
-
-        Returns
-        -------
-        catalog_table : recarray
-            recarray equivalent to SkyModel data.
-
-        """
-        warnings.warn(
-            "The to_recarray method is deprecated and will be removed in 0.3.0.",
-            DeprecationWarning,
-        )
-
-        return self._text_write_preprocess()
-
-    @classmethod
-    def from_recarray(
-        cls,
-        recarray_in,
-        history="",
-        run_check=True,
-        check_extra=True,
-        run_check_acceptability=True,
-    ):
-        """
-        Initialize this object from a recarray.
-
-        Deprecated, will be removed in version 0.3.0.
-
-        Parameters
-        ----------
-        recarray_in : recarray
-            recarray to turn into a SkyModel object.
-        history : str
-            History to add to object.
-        run_check : bool
-            Option to check for the existence and proper shapes of parameters
-            after downselecting data on this object (the default is True,
-            meaning the check will be run).
-        check_extra : bool
-            Option to check optional parameters as well as required ones (the
-            default is True, meaning the optional parameters will be checked).
-        run_check_acceptability : bool
-            Option to check acceptable range of the values of parameters after
-            downselecting data on this object (the default is True, meaning the
-            acceptable range check will be done).
-
-        """
-        warnings.warn(
-            "The from_recarray method is deprecated and will be removed in 0.3.0.",
-            DeprecationWarning,
-        )
-
-        fieldnames = recarray_in.dtype.names
-
-        frame_use, lon_col, lat_col = _get_frame_comp_cols(fieldnames)
-        skycoord = SkyCoord(
-            Longitude(recarray_in[lon_col], unit="deg"),
-            Latitude(recarray_in[lat_col], unit="deg"),
-            frame=frame_use,
-        )
-
-        ids = np.asarray(recarray_in["source_id"]).astype(str)
-
-        Ncomponents = ids.size
-
-        rise_lst = None
-        set_lst = None
-
-        if "reference_frequency" in fieldnames:
-            reference_frequency = Quantity(
-                np.atleast_1d(recarray_in["reference_frequency"]), "hertz"
-            )
-            if "spectral_index" in fieldnames:
-                spectral_index = np.atleast_1d(recarray_in["spectral_index"])
-                spectral_type = "spectral_index"
-            else:
-                spectral_type = "flat"
-                spectral_index = None
-            freq_array = None
-        elif "frequency" in fieldnames or "subband_frequency" in fieldnames:
-            if "frequency" in fieldnames:
-                freq_array = Quantity(np.atleast_1d(recarray_in["frequency"]), "hertz")
-            else:
-                spectral_type = "subband"
-                freq_array = Quantity(
-                    np.atleast_1d(recarray_in["subband_frequency"]), "hertz"
-                )
-            # freq_array gets copied for every component, so its zeroth axis is
-            # length Ncomponents. Just take the first one.
-            freq_array = freq_array[0, :]
-            if freq_array.size > 1:
-                if "subband_frequency" not in fieldnames:
-                    spectral_type = "full"
-            else:
-                spectral_type = "flat"
-            reference_frequency = None
-            spectral_index = None
-        else:
-            # flat spectrum, no freq info
-            spectral_type = "flat"
-            freq_array = None
-            reference_frequency = None
-            spectral_index = None
-
-        if "rise_lst" in recarray_in.dtype.names:
-            rise_lst = recarray_in["rise_lst"]
-            set_lst = recarray_in["set_lst"]
-
-        # Read Stokes parameters
-        Nfreqs = 1 if freq_array is None else freq_array.size
-        stokes = Quantity(np.zeros((4, Nfreqs, Ncomponents)), "Jy")
-        for ii, spar in enumerate(["I", "Q", "U", "V"]):
-            if spar in recarray_in.dtype.names:
-                stokes[ii] = recarray_in[spar].T * units.Jy
-
-        errors_present = False
-        for field in fieldnames:
-            if "error" in field:
-                errors_present = True
-                break
-        if errors_present:
-            stokes_error = Quantity(np.zeros((4, Nfreqs, Ncomponents)), "Jy")
-            for ii, spar in enumerate(["I_error", "Q_error", "U_error", "V_error"]):
-                if spar in recarray_in.dtype.names:
-                    stokes_error[ii] = recarray_in[spar].T * units.Jy
-        else:
-            stokes_error = None
-
-        names = ids
-
-        self = cls(
-            name=names,
-            skycoord=skycoord,
-            stokes=stokes,
-            spectral_type=spectral_type,
-            freq_array=freq_array,
-            reference_frequency=reference_frequency,
-            spectral_index=spectral_index,
-            stokes_error=stokes_error,
-            history=history,
-        )
-
-        if ids[0].startswith("nside"):
-            name_parts = ids[0].split("_")
-            self.nside = int(name_parts[0][len("nside") :])
-            self.hpx_order = name_parts[1]
-            self.hpx_inds = np.array([int(name[name.rfind("_") + 1 :]) for name in ids])
-            self._point_to_healpix(
-                run_check=run_check,
-                check_extra=check_extra,
-                run_check_acceptability=run_check_acceptability,
-            )
-
-        if rise_lst is not None:
-            self._rise_lst = rise_lst
-        if set_lst is not None:
-            self._set_lst = set_lst
-
-        if run_check:
-            self.check(
-                check_extra=check_extra, run_check_acceptability=run_check_acceptability
-            )
-
-        return self
-
     def read_skyh5(
         self, filename, run_check=True, check_extra=True, run_check_acceptability=True
     ):
         """
         Read a skyh5 file (our flavor of hdf5) into this object.
 
         Parameters
@@ -3585,47 +3264,44 @@
             Option to check acceptable range of the values of parameters after
             downselecting data on this object (the default is True, meaning the
             acceptable range check will be done).
 
         """
         with h5py.File(filename, "r") as fileobj:
             if "/Header" not in fileobj:
-                raise ValueError(
-                    "This is an old 'healvis' style healpix HDF5 file. To read it, "
-                    "use the `read_healpix_hdf5` method. Support for this file format "
-                    "is deprecated and will be removed in version 0.3.0."
-                )
+                raise ValueError("This is not a proper skyh5 file.")
 
         init_params = {"filename": os.path.basename(filename)}
 
         with h5py.File(filename, "r") as fileobj:
-
             # extract header information
             header = fileobj["/Header"]
             header_params = [
                 "_Ncomponents",
                 "_Nfreqs",
                 "_component_type",
                 "_spectral_type",
                 "_history",
                 "_name",
                 "_nside",
                 "_hpx_order",
                 "_hpx_inds",
                 "_freq_array",
+                "_freq_edge_array",
                 "_reference_frequency",
                 "_spectral_index",
                 "_stokes_error",
                 "_beam_amp",
                 "_extended_model_group",
             ]
 
             optional_params = [
                 "_hpx_order",
                 "_freq_array",
+                "_freq_edge_array",
                 "_reference_frequency",
                 "_spectral_index",
                 "_stokes_error",
                 "_beam_amp",
                 "_extended_model_group",
             ]
 
@@ -3733,14 +3409,30 @@
                 if init_params["Ncomponents"] != init_params["name"].size:
                     raise ValueError("Ncomponents is not equal to the size of 'name'.")
 
             if "freq_array" in init_params.keys():
                 if init_params["Nfreqs"] != init_params["freq_array"].size:
                     raise ValueError("Nfreqs is not equal to the size of 'freq_array'.")
 
+                if init_params["spectral_type"] == "subband":
+                    if "freq_edge_array" not in init_params.keys():
+                        try:
+                            init_params[
+                                "freq_edge_array"
+                            ] = _get_freq_edges_from_centers(
+                                init_params["freq_array"], self._freq_array.tols
+                            )
+                        except ValueError:
+                            warnings.warn(
+                                "No freq_edge_array in this file and frequencies are "
+                                "not evenly spaced, so spectral_type will be set to "
+                                "'full' rather than 'subband'."
+                            )
+                            init_params["spectral_type"] = "full"
+
             # remove parameters not needed in __init__
             init_params.pop("Ncomponents")
             init_params.pop("Nfreqs")
 
             # get stokes array
             dgrp = fileobj["/Data"]
             init_params["stokes"] = dgrp["stokes"] * units.Unit(
@@ -3806,169 +3498,31 @@
             filename,
             run_check=run_check,
             check_extra=check_extra,
             run_check_acceptability=run_check_acceptability,
         )
         return self
 
-    def read_healpix_hdf5(
-        self,
-        hdf5_filename,
-        run_check=True,
-        check_extra=True,
-        run_check_acceptability=True,
-    ):
-        """
-        Read hdf5 healpix files into this object.
-
-        Deprecated. Support for this file format will be removed in version 0.3.0.
-        Use `read_skyh5` to read our newer skyh5 file type.
-
-        Parameters
-        ----------
-        hdf5_filename : str
-            Path and name of the hdf5 file to read.
-        run_check : bool
-            Option to check for the existence and proper shapes of parameters
-            after downselecting data on this object (the default is True,
-            meaning the check will be run).
-        check_extra : bool
-            Option to check optional parameters as well as required ones (the
-            default is True, meaning the optional parameters will be checked).
-        run_check_acceptability : bool
-            Option to check acceptable range of the values of parameters after
-            downselecting data on this object (the default is True, meaning the
-            acceptable range check will be done).
-
-        Notes
-        -----
-        Currently, this function only converts a HEALPix map with a frequency axis.
-
-        """
-        with h5py.File(hdf5_filename, "r") as fileobj:
-            if "/Header" in fileobj:
-                raise ValueError(
-                    "This is a skyh5 file. To read it, use the `read_skyh5` method."
-                )
-
-        try:
-            import astropy_healpix
-        except ImportError as e:
-            raise ImportError(
-                "The astropy-healpix module must be installed to use HEALPix methods"
-            ) from e
-
-        warnings.warn(
-            "This method reads an old 'healvis' style healpix HDF5 file. Support for "
-            "this file format is deprecated and will be removed in version 0.3.0. Use "
-            "the `read_skyh5` method to read the newer skyh5 file type.",
-            category=DeprecationWarning,
-        )
-
-        with h5py.File(hdf5_filename, "r") as fileobj:
-            hpmap = fileobj["data"][0, ...]  # Remove Nskies axis.
-            indices = fileobj["indices"][()]
-            freqs = fileobj["freqs"][()]
-            history = fileobj["history"][()]
-            try:
-                history = history.decode("utf8")
-            except (UnicodeDecodeError, AttributeError):
-                history = ""
-                pass
-            try:
-                nside = int(fileobj.attrs["nside"])
-            except KeyError:
-                nside = int(astropy_healpix.npix_to_nside(hpmap.shape[-1]))
-            try:
-                hpmap_units = fileobj["units"][()]
-            except KeyError:
-                hpmap_units = "K"
-
-        freq = Quantity(freqs, "hertz")
-
-        # hmap is in K
-        stokes = Quantity(np.zeros((4, len(freq), len(indices))), hpmap_units)
-        stokes[0] = hpmap * units.Unit(hpmap_units)
-
-        self.__init__(
-            nside=nside,
-            hpx_inds=indices,
-            stokes=stokes,
-            spectral_type="full",
-            freq_array=freq,
-            history=history,
-            frame="icrs",
-            filename=os.path.basename(hdf5_filename),
-        )
-        assert self.component_type == "healpix"
-
-        if run_check:
-            self.check(
-                check_extra=check_extra, run_check_acceptability=run_check_acceptability
-            )
-        return
-
-    @classmethod
-    def from_healpix_hdf5(
-        cls,
-        hdf5_filename,
-        run_check=True,
-        check_extra=True,
-        run_check_acceptability=True,
-    ):
-        """
-        Create a new :class:`SkyModel` from a hdf5 healpix file.
-
-        Deprecated. Support for this file format will be removed in version 0.3.0.
-        Use `from_skyh5` to create a new :class:`SkyModel` from our newer skyh5 file type.
-
-        Parameters
-        ----------
-        hdf5_filename : str
-            Path and name of the hdf5 file to read.
-        run_check : bool
-            Option to check for the existence and proper shapes of parameters
-            after downselecting data on this object (the default is True,
-            meaning the check will be run).
-        check_extra : bool
-            Option to check optional parameters as well as required ones (the
-            default is True, meaning the optional parameters will be checked).
-        run_check_acceptability : bool
-            Option to check acceptable range of the values of parameters after
-            downselecting data on this object (the default is True, meaning the
-            acceptable range check will be done).
-
-        Notes
-        -----
-        Currently, this function only converts a HEALPix map with a frequency axis.
-
-        """
-        self = cls()
-        self.read_healpix_hdf5(
-            hdf5_filename,
-            run_check=run_check,
-            check_extra=check_extra,
-            run_check_acceptability=run_check_acceptability,
-        )
-        return self
-
+    @units.quantity_input(
+        freq_array=units.Hz, freq_edge_array=units.Hz, reference_frequency=units.Hz
+    )
     def read_votable_catalog(
         self,
         votable_file,
         table_name,
         id_column,
         lon_column,
         lat_column,
         flux_columns,
-        frame=None,
+        frame,
         reference_frequency=None,
         freq_array=None,
+        freq_edge_array=None,
         spectral_index_column=None,
         flux_error_columns=None,
-        source_select_kwds=None,
         history="",
         run_check=True,
         check_extra=True,
         run_check_acceptability=True,
     ):
         """
         Read a votable catalog file into this object.
@@ -3990,41 +3544,31 @@
         lat_column : str
             Part of expected latitudinal coordinate (e.g. Dec) column. Should match
             only one column in the table.
         flux_columns : str or list of str
             Part of expected Flux column(s). Each one should match only one column in the table.
         frame : str
             Name of coordinate frame of source positions (lon/lat columns).
-            Currently defaults to "icrs" to maintain backwards compatibility, in the
-            future will be a required parameter. Must be interpretable by
-            `astropy.coordinates.frame_transform_graph.lookup_name()`.
+            Must be interpretable by `astropy.coordinates.frame_transform_graph.lookup_name()`.
         reference_frequency : :class:`astropy.units.Quantity`
             Reference frequency for flux values, assumed to be the same value for all rows.
         freq_array : :class:`astropy.units.Quantity`
-            Frequencies corresponding to flux_columns (should be same length).
+            Frequency band centers corresponding to flux_columns (should be same length).
             Required for multiple flux columns.
+        freq_edge_array : :class:`astropy.units.Quantity`
+            Frequency sub-band edges for each flux_columns, shape (2, len(flux_columns)).
+            Required for multiple flux columns if `freq_array` is not regularly spaced.
+            If `freq_array` is regularly spaced and `freq_edge_array` is not passed,
+            `freq_edge_array` will be calculated from the freq_array assuming the
+            band edges are directly between the band centers.
         spectral_index_column : str
             Part of expected spectral index column. Should match only one column in the table.
         flux_error_columns : str or list of str
             Part of expected Flux error column(s). Each one should match only one
             column in the table.
-        source_select_kwds : dict, optional
-            This parameter is Deprecated, please use the `select` and/or the
-            :meth:`cut_nonrising` methods as appropriate instead.
-
-            Dictionary of keywords for source selection Valid options:
-
-            * `latitude_deg`: Latitude of telescope in degrees. Used for declination
-               coarse horizon cut.
-            * `horizon_buffer`: Angle (float, in radians) of buffer for coarse horizon
-              cut.
-              Default is about 10 minutes of sky rotation. (See caveats in
-              :func:`~skymodel.SkyModel.source_cuts` docstring)
-            * `min_flux`: Minimum stokes I flux to select [Jy]
-            * `max_flux`: Maximum stokes I flux to select [Jy]
         history : str
             History to add to object.
         run_check : bool
             Option to check for the existence and proper shapes of parameters
             after downselecting data on this object (the default is True,
             meaning the check will be run).
         check_extra : bool
@@ -4063,35 +3607,52 @@
         lon_col_use = _get_matching_fields(
             lon_column, astropy_table.colnames, exclude_start_pattern="_"
         )
         lat_col_use = _get_matching_fields(
             lat_column, astropy_table.colnames, exclude_start_pattern="_"
         )
 
-        if frame is None:
-            warnings.warn(
-                "frame parameter was not set. Defaulting to 'icrs'. This will become "
-                "an error in version 0.3",
-                DeprecationWarning,
-            )
-            frame = "icrs"
-
         if isinstance(flux_columns, (str)):
             flux_columns = [flux_columns]
         flux_cols_use = []
         for col in flux_columns:
             flux_cols_use.append(_get_matching_fields(col, astropy_table.colnames))
 
-        if len(flux_columns) > 1 and freq_array is None:
-            raise ValueError("freq_array must be provided for multiple flux columns.")
+        if len(flux_columns) > 1 and (freq_array is None and freq_edge_array is None):
+            raise ValueError(
+                "Frequency information must be provided with multiple flux columns. "
+                "Must provide either freq_edge_array or freq_array (if the "
+                "frequencies are evenly spaced), both can be provided."
+            )
+
+        if len(flux_columns) > 1:
+            if freq_edge_array is None:
+                # if get here, freq_array exists
+                try:
+                    freq_edge_array = _get_freq_edges_from_centers(
+                        freq_array=freq_array, tols=self._freq_array.tols
+                    )
+                    warnings.warn(
+                        "freq_edge_array not set, calculating it from the freq_array."
+                    )
+                except ValueError as ve:
+                    raise ValueError(
+                        "freq_edge_array must be provided for multiple flux columns if "
+                        "freq_array is not regularly spaced."
+                    ) from ve
+            elif freq_array is None:
+                warnings.warn(
+                    "freq_array not set, calculating it from the freq_edge_array."
+                )
+                freq_array = _get_freq_centers_from_edges(
+                    freq_edge_array=freq_edge_array
+                )
 
         if reference_frequency is not None or len(flux_cols_use) == 1:
             if reference_frequency is not None:
-                if not isinstance(reference_frequency, (Quantity,)):
-                    raise ValueError("reference_frequency must be an astropy Quantity.")
                 reference_frequency = (
                     np.array([reference_frequency.value] * len(astropy_table))
                     * reference_frequency.unit
                 )
             if spectral_index_column is not None:
                 spectral_type = "spectral_index"
                 spec_index_col_use = _get_matching_fields(
@@ -4166,30 +3727,22 @@
             name=astropy_table[id_col_use].data.data.astype("str"),
             lon=Longitude(astropy_table[lon_col_use].quantity),
             lat=Latitude(astropy_table[lat_col_use].quantity),
             frame=frame,
             stokes=stokes,
             spectral_type=spectral_type,
             freq_array=freq_array,
+            freq_edge_array=freq_edge_array,
             reference_frequency=reference_frequency,
             spectral_index=spectral_index,
             stokes_error=stokes_error,
             history=history,
             filename=os.path.basename(votable_file),
         )
 
-        if source_select_kwds is not None:
-            warnings.warn(
-                "The source_select_kwds parameter is deprecated, use the `select` "
-                "and/or the `cut_nonrising` methods as appropriate instead."
-                "This parameter will be removed in version 0.3.0.",
-                category=DeprecationWarning,
-            )
-            self.source_cuts(**source_select_kwds)
-
         if run_check:
             self.check(
                 check_extra=check_extra, run_check_acceptability=run_check_acceptability
             )
 
         return
 
@@ -4211,56 +3764,59 @@
         self.read_votable_catalog(votable_file, *args, **kwargs)
         return self
 
     def read_gleam_catalog(
         self,
         gleam_file,
         spectral_type="subband",
-        source_select_kwds=None,
         with_error=False,
+        use_paper_freqs=False,
         run_check=True,
         check_extra=True,
         run_check_acceptability=True,
     ):
         """
         Read the GLEAM votable catalog file into this object.
 
+        Note that the GLEAM paper specifies that the 30.72 MHz bandwidth is subdivided
+        into four 7.68 MHz sub-channels. But that clashes with the frequencies and
+        edges listed in the catalog documentation which are spaced by exactly 8MHz.
+        By default, this method uses the catalog frequency values. To use our best guess
+        of the real values (which are not specified in the paper), set
+        `use_paper_freqs=True`. This option only has an effect if
+        spectral_type="subband".
+
         Tested on: GLEAM EGC catalog, version 2
 
         Parameters
         ----------
         gleam_file : str
             Path to GLEAM votable catalog file.
         spectral_type : str
             One of 'flat', 'subband' or 'spectral_index'. If set to 'flat', the
             wide band integrated flux will be used, if set to 'spectral_index' the
             fitted flux at 200 MHz will be used for the flux column.
-        source_select_kwds : dict, optional
-            This parameter is Deprecated, please use the `select` and/or the
-            :meth:`cut_nonrising` methods as appropriate instead.
-
-            Dictionary of keywords for source selection Valid options:
-
-            * `latitude_deg`: Latitude of telescope in degrees. Used for declination coarse
-               horizon cut.
-            * `horizon_buffer`: Angle (float, in radians) of buffer for coarse horizon cut.
-              Default is about 10 minutes of sky rotation. (See caveats in
-              :func:`array_to_skymodel` docstring)
-            * `min_flux`: Minimum stokes I flux to select [Jy]
-            * `max_flux`: Maximum stokes I flux to select [Jy]
         with_error : bool
             Option to include the errors on the stokes array on the object in the
             `stokes_error` parameter. Note that the values assigned to this parameter
             are the flux fitting errors. The GLEAM paper (Hurley-Walker et al., 2019)
             specifies that flux scale errors should be added in quadrature to these
             fitting errors, but that the size of the flux scale errors depends on
             whether the comparison is between GLEAM sub-bands or with another catalog.
             Between GLEAM sub-bands, the flux scale error is 2-3% of the component flux
             (depending on declination), while flux scale errors between GLEAM and other
             catalogs is 8-80% of the component flux (depending on declination).
+        use_paper_freqs : bool
+            Use our best guess of the frequencies based on the GLEAM paper and what we
+            know about the MWA. This option exists because the GLEAM paper specifies
+            that the 30.72 MHz bandwidth is subdivided into four 7.68 MHz sub-channels.
+            But the frequencies and edges listed in the catalog documentation are spaced
+            by exactly 8MHz rather than 7.68 MHz. Our calculated band centers are
+            different from the catalog values by at most 0.6 MHz, the band edges are
+            different by at most 1.08 MHz. Only used if spectral_type="subband".
         run_check : bool
             Option to check for the existence and proper shapes of parameters
             after downselecting data on this object (the default is True,
             meaning the check will be run).
         check_extra : bool
             Option to check optional parameters as well as required ones (the
             default is True, meaning the optional parameters will be checked).
@@ -4278,38 +3834,70 @@
             )
 
         if spectral_type == "flat":
             flux_columns = "Fintwide"
             flux_error_columns = "e_Fintwide"
             reference_frequency = 200e6 * units.Hz
             freq_array = None
+            freq_edge_array = None
             spectral_index_column = None
         elif spectral_type == "spectral_index":
             flux_columns = "Fintfit200"
             flux_error_columns = "e_Fintfit200"
             reference_frequency = 200e6 * units.Hz
             spectral_index_column = "alpha"
             freq_array = None
+            freq_edge_array = None
         else:
             # fmt: off
             flux_columns = [
                 "Fint076", "Fint084", "Fint092", "Fint099", "Fint107",
                 "Fint115", "Fint122", "Fint130", "Fint143", "Fint151",
                 "Fint158", "Fint166", "Fint174", "Fint181", "Fint189",
                 "Fint197", "Fint204", "Fint212", "Fint220", "Fint227"
             ]
             flux_error_columns = [
                 "e_Fint076", "e_Fint084", "e_Fint092", "e_Fint099", "e_Fint107",
                 "e_Fint115", "e_Fint122", "e_Fint130", "e_Fint143", "e_Fint151",
                 "e_Fint158", "e_Fint166", "e_Fint174", "e_Fint181", "e_Fint189",
                 "e_Fint197", "e_Fint204", "e_Fint212", "e_Fint220", "e_Fint227"
             ]
-            freq_array = [76, 84, 92, 99, 107, 115, 122, 130, 143, 151, 158, 166,
-                          174, 181, 189, 197, 204, 212, 220, 227]
-            freq_array = np.array(freq_array) * 1e6 * units.Hz
+            # fmt: on
+            if use_paper_freqs:
+                # use the frequencies we *think* are the true ones, spaced by 7.68 MHz
+                # these are at most 0.6 MHz off of the catalog values. The edges are
+                # more different -- they differ by as much as 1.08 MHz.
+                coarse_channel_starts = np.array([57, 81, 109, 133, 157])
+                coarse_channels = np.repeat(
+                    (np.arange(24))[np.newaxis, :], 5, axis=0
+                ) + np.repeat(coarse_channel_starts[:, np.newaxis], 24, axis=1)
+                temp = np.reshape(coarse_channels, (5, 4, 6)) * 1.28 * 1e6 * units.Hz
+                freq_array = np.reshape(np.mean(temp, axis=2), 20)
+                freq_lower = np.reshape(np.min(temp, axis=2), 20)
+                freq_upper = np.reshape(np.max(temp, axis=2), 20)
+            else:
+                # use the frequencies from the catalog (default)
+                # fmt: off
+                freq_array = np.array(
+                    [76, 84, 92, 99, 107, 115, 122, 130, 143, 151, 158, 166,
+                     174, 181, 189, 197, 204, 212, 220, 227]
+                ) * 1e6 * units.Hz
+                freq_lower = np.asarray(
+                    [72, 80, 88, 95, 103, 111, 118, 126, 139, 147, 154, 162,
+                     170, 177, 185, 193, 200, 208, 216, 223]
+                ) * 1e6 * units.Hz
+                freq_upper = np.asarray(
+                    [80, 88, 95, 103, 111, 118, 126, 134, 147, 154, 162, 170,
+                     177, 185, 193, 200, 208, 216, 223, 231]
+                ) * 1e6 * units.Hz
+                # fmt: on
+
+            freq_edge_array = np.concatenate(
+                (freq_lower[np.newaxis, :], freq_upper[np.newaxis, :]), axis=0
+            )
             reference_frequency = None
             spectral_index_column = None
             # fmt: on
 
         if not with_error:
             flux_error_columns = None
 
@@ -4318,18 +3906,18 @@
             "GLEAM",
             "GLEAM",
             "RAJ2000",
             "DEJ2000",
             frame="fk5",
             flux_columns=flux_columns,
             freq_array=freq_array,
+            freq_edge_array=freq_edge_array,
             reference_frequency=reference_frequency,
             spectral_index_column=spectral_index_column,
             flux_error_columns=flux_error_columns,
-            source_select_kwds=source_select_kwds,
         )
 
         if run_check:
             self.check(
                 check_extra=check_extra, run_check_acceptability=run_check_acceptability
             )
         return
@@ -4351,15 +3939,14 @@
         self = cls()
         self.read_gleam_catalog(gleam_file, **kwargs)
         return self
 
     def read_text_catalog(
         self,
         catalog_csv,
-        source_select_kwds=None,
         run_check=True,
         check_extra=True,
         run_check_acceptability=True,
     ):
         """
         Read a text file of sources into this object.
 
@@ -4387,27 +3974,14 @@
             If flux is only specified at one reference frequency (can be different per
             component), a frequency column should be added (note: assumed to be in Hz):
             *  `Frequency`: reference frequency [Hz]
 
             Optionally a spectral index can be specified per component with:
             *  `Spectral_Index`: spectral index
 
-        source_select_kwds : dict, optional
-            This parameter is Deprecated, please use the `select` and/or the
-            :meth:`cut_nonrising` methods as appropriate.
-
-            Dictionary of keywords for source selection. Valid options:
-
-            * `latitude_deg`: Latitude of telescope in degrees. Used for declination coarse
-            *  horizon cut.
-            * `horizon_buffer`: Angle (float, in radians) of buffer for coarse horizon cut.
-              Default is about 10 minutes of sky rotation. (See caveats in
-              :func:`array_to_skymodel` docstring)
-            * `min_flux`: Minimum stokes I flux to select [Jy]
-            * `max_flux`: Maximum stokes I flux to select [Jy]
         run_check : bool
             Option to check for the existence and proper shapes of parameters
             after downselecting data on this object (the default is True,
             meaning the check will be run).
         check_extra : bool
             Option to check optional parameters as well as required ones (the
             default is True, meaning the optional parameters will be checked).
@@ -4476,21 +4050,18 @@
                 else:
                     if len(flux_fields) > 1:
                         raise ValueError(
                             "Multiple flux fields, but they do not all contain a frequency."
                         )
             if len(frequencies) > 0:
                 n_freqs = len(frequencies)
-                if "subband" in flux_fields[0]:
-                    spectral_type = "subband"
+                if len(frequencies) > 1:
+                    spectral_type = "full"
                 else:
-                    if len(frequencies) > 1:
-                        spectral_type = "full"
-                    else:
-                        spectral_type = "flat"
+                    spectral_type = "flat"
                 # This has a freq_array
                 if len(flux_error_fields) > 0:
                     for ind in range(n_freqs):
                         expected_cols.append(flux_fields_lower[ind])
                         expected_cols.append(flux_error_fields_lower[ind])
                 else:
                     expected_cols.extend(flux_fields_lower)
@@ -4563,23 +4134,14 @@
             spectral_index=spectral_index,
             stokes_error=stokes_error,
             filename=os.path.basename(catalog_csv),
         )
 
         assert type(self.stokes_error) == type(stokes_error)
 
-        if source_select_kwds is not None:
-            warnings.warn(
-                "The source_select_kwds parameter is deprecated, use the `select` "
-                "and/or the `cut_nonrising` methods as appropriate instead."
-                "This parameter will be removed in version 0.3.0.",
-                category=DeprecationWarning,
-            )
-            self.source_cuts(**source_select_kwds)
-
         if run_check:
             self.check(
                 check_extra=check_extra, run_check_acceptability=run_check_acceptability
             )
 
         return
 
@@ -4601,15 +4163,14 @@
         self.read_text_catalog(catalog_csv, **kwargs)
         return self
 
     def read_fhd_catalog(
         self,
         filename_sav,
         expand_extended=True,
-        source_select_kwds=None,
         run_check=True,
         check_extra=True,
         run_check_acceptability=True,
     ):
         """
         Read in an FHD style catalog file.
 
@@ -4618,27 +4179,14 @@
         Parameters
         ----------
         filename_sav: str
             Path to IDL .sav file.
 
         expand_extended: bool
             If True, include extended source components.
-        source_select_kwds : dict, optional
-            This parameter is Deprecated, please use the `select` and/or the
-            :meth:`cut_nonrising` methods as appropriate.
-
-            Dictionary of keywords for source selection. Valid options:
-
-            * `latitude_deg`: Latitude of telescope in degrees. Used for declination coarse
-            *  horizon cut.
-            * `horizon_buffer`: Angle (float, in radians) of buffer for coarse horizon cut.
-              Default is about 10 minutes of sky rotation. (See caveats in
-              :func:`array_to_skymodel` docstring)
-            * `min_flux`: Minimum stokes I flux to select [Jy]
-            * `max_flux`: Maximum stokes I flux to select [Jy]
         run_check : bool
             Option to check for the existence and proper shapes of parameters
             after downselecting data on this object (the default is True,
             meaning the check will be run).
         check_extra : bool
             Option to check optional parameters as well as required ones (the
             default is True, meaning the optional parameters will be checked).
@@ -4762,23 +4310,14 @@
             reference_frequency=Quantity(source_freqs, "hertz"),
             spectral_index=spectral_index,
             beam_amp=beam_amp,
             extended_model_group=extended_model_group,
             filename=os.path.basename(filename_sav),
         )
 
-        if source_select_kwds is not None:
-            warnings.warn(
-                "The source_select_kwds parameter is deprecated, use the `select` "
-                "and/or the `cut_nonrising` methods as appropriate instead."
-                "This parameter will be removed in version 0.3.0.",
-                category=DeprecationWarning,
-            )
-            self.source_cuts(**source_select_kwds)
-
         if run_check:
             self.check(
                 check_extra=check_extra, run_check_acceptability=run_check_acceptability
             )
 
         return
 
@@ -4796,37 +4335,40 @@
         sky_model : :class:`SkyModel`
             The object instantiated using the FHD catalog.
         """
         self = cls()
         self.read_fhd_catalog(filename_sav, **kwargs)
         return self
 
+    @units.quantity_input(
+        freq_array=units.Hz, freq_edge_array=units.Hz, reference_frequency=units.Hz
+    )
     def read(
         self,
         filename,
         filetype=None,
         run_check=True,
         check_extra=True,
         run_check_acceptability=True,
         # Gleam vot
         spectral_type=None,
         with_error=False,
+        use_paper_freqs=False,
         # fhd
         expand_extended=True,
         # VOTable
         table_name=None,
         id_column=None,
-        ra_column=None,
-        dec_column=None,
         lon_column=None,
         lat_column=None,
         frame=None,
         flux_columns=None,
         reference_frequency=None,
         freq_array=None,
+        freq_edge_array=None,
         spectral_index_column=None,
         flux_error_columns=None,
         history="",
     ):
         """
         Read in any file supported by :class:`SkyModel`.
 
@@ -4863,14 +4405,22 @@
             are the flux fitting errors. The GLEAM paper (Hurley-Walker et al., 2019)
             specifies that flux scale errors should be added in quadrature to these
             fitting errors, but that the size of the flux scale errors depends on
             whether the comparison is between GLEAM sub-bands or with another catalog.
             Between GLEAM sub-bands, the flux scale error is 2-3% of the component flux
             (depending on declination), while flux scale errors between GLEAM and other
             catalogs is 8-80% of the component flux (depending on declination).
+        use_paper_freqs : bool
+            Use our best guess of the frequencies based on the GLEAM paper and what we
+            know about the MWA. This option exists because the GLEAM paper specifies
+            that the 30.72 MHz bandwidth is subdivided into four 7.68 MHz sub-channels.
+            But the frequencies and edges listed in the catalog documentation are spaced
+            by exactly 8MHz rather than 7.68 MHz. Our calculated band centers are
+            different from the catalog values by at most 0.6 MHz, the band edges are
+            different by at most 1.08 MHz. Only used if spectral_type="subband".
 
         FHD
         ---
         expand_extended: bool
             If True, include the extended source components in FHD files.
 
         VOTable
@@ -4881,32 +4431,34 @@
             Part of expected VOTable ID column. Should match only one column in the file.
         lon_column : str
             Part of expected VOTable longitudinal coordinate column. Should match only
             one column in the file.
         lat_column : str
             Part of expected VOTable latitudinal coordinate column. Should match only
             one column in the file.
-        ra_column : str
-            Deprecated synonym for lon_column.
-        dec_column : str
-            Deprecated synonym for lat_column.
         flux_columns : str or list of str
             Part of expected vot Flux column(s). Each one should match only one column
             in the file. Only used for vot files.
         frame : str
             Name of coordinate frame for VOTable source positions (lon/lat columns).
             Defaults to "icrs". Must be interpretable by
             `astropy.coordinates.frame_transform_graph.lookup_name()`. Only used for
             vot files.
         reference_frequency : :class:`astropy.units.Quantity`
             Reference frequency for VOTable flux values, assumed to be the same value
             for all components.
         freq_array : :class:`astropy.units.Quantity`
             Frequencies corresponding to VOTable flux_columns (should be same length).
             Required for multiple flux columns.
+        freq_edge_array : :class:`astropy.units.Quantity`
+            Frequency sub-band edges for each flux_columns, shape (2, len(flux_columns)).
+            Required for multiple flux columns if `freq_array` is not regularly spaced.
+            If `freq_array` is regularly spaced and `freq_edge_array` is not passed,
+            `freq_edge_array` will be calculated from the freq_array assuming the
+            band edges are directly between the band centers.
         spectral_index_column : str
             Part of expected VOTable spectral index column. Should match only one
             column in the file.
         flux_error_columns : str or list of str
             Part of expected VOTable flux error column(s). Each one should match only
             one column in the file.
         history : str
@@ -4935,45 +4487,31 @@
 
         if filetype == "text":
             self.read_text_catalog(filename)
         elif filetype == "gleam":
             if spectral_type is None:
                 spectral_type = "subband"
             self.read_gleam_catalog(
-                filename, spectral_type=spectral_type, with_error=with_error
+                filename,
+                spectral_type=spectral_type,
+                with_error=with_error,
+                use_paper_freqs=use_paper_freqs,
             )
         elif filetype == "vot":
-            if ra_column is not None:
-                warnings.warn(
-                    "The `ra_column` keyword is deprecated and will be removed in "
-                    "version 0.3.0, use `lon_column` instead",
-                    DeprecationWarning,
-                )
-                if lon_column is None:
-                    lon_column = ra_column
-
-            if dec_column is not None:
-                warnings.warn(
-                    "The `dec_column` keyword is deprecated and will be removed in "
-                    "version 0.3.0, use `lat_column` instead",
-                    DeprecationWarning,
-                )
-                if lat_column is None:
-                    lat_column = dec_column
-
             self.read_votable_catalog(
                 filename,
                 table_name,
                 id_column,
                 lon_column,
                 lat_column,
                 flux_columns,
                 frame=frame,
                 reference_frequency=reference_frequency,
                 freq_array=freq_array,
+                freq_edge_array=freq_edge_array,
                 spectral_index_column=spectral_index_column,
                 flux_error_columns=flux_error_columns,
                 history=history,
                 run_check=run_check,
                 check_extra=check_extra,
                 run_check_acceptability=run_check_acceptability,
             )
@@ -4994,37 +4532,40 @@
             )
         else:
             raise ValueError(
                 "Cannot determine the file type. Please specify using the filetype parameter."
             )
 
     @classmethod
+    @units.quantity_input(
+        freq_array=units.Hz, freq_edge_array=units.Hz, reference_frequency=units.Hz
+    )
     def from_file(
         cls,
         filename,
         filetype=None,
         run_check=True,
         check_extra=True,
         run_check_acceptability=True,
         # Gleam vot
         spectral_type=None,
         with_error=False,
+        use_paper_freqs=False,
         # fhd
         expand_extended=True,
         # VOTable
         table_name=None,
         id_column=None,
         lon_column=None,
         lat_column=None,
-        ra_column=None,
-        dec_column=None,
         flux_columns=None,
         frame=None,
         reference_frequency=None,
         freq_array=None,
+        freq_edge_array=None,
         spectral_index_column=None,
         flux_error_columns=None,
         history="",
     ):
         """
         Create a :class:`SkyModel` from any file supported by SkyModel.
 
@@ -5061,14 +4602,22 @@
             are the flux fitting errors. The GLEAM paper (Hurley-Walker et al., 2019)
             specifies that flux scale errors should be added in quadrature to these
             fitting errors, but that the size of the flux scale errors depends on
             whether the comparison is between GLEAM sub-bands or with another catalog.
             Between GLEAM sub-bands, the flux scale error is 2-3% of the component flux
             (depending on declination), while flux scale errors between GLEAM and other
             catalogs is 8-80% of the component flux (depending on declination).
+        use_paper_freqs : bool
+            Use our best guess of the frequencies based on the GLEAM paper and what we
+            know about the MWA. This option exists because the GLEAM paper specifies
+            that the 30.72 MHz bandwidth is subdivided into four 7.68 MHz sub-channels.
+            But the frequencies and edges listed in the catalog documentation are spaced
+            by exactly 8MHz rather than 7.68 MHz. Our calculated band centers are
+            different from the catalog values by at most 0.6 MHz, the band edges are
+            different by at most 1.08 MHz. Only used if spectral_type="subband".
 
         FHD
         ---
         expand_extended: bool
             If True, include the extended source components in FHD files.
 
         VOTable
@@ -5079,32 +4628,34 @@
             Part of expected VOTable ID column. Should match only one column in the file.
         lon_column : str
             Part of expected VOTable longitudinal coordinate column. Should match only
             one column in the file.
         lat_column : str
             Part of expected VOTable latitudinal coordinate column. Should match only
             one column in the file.
-        ra_column : str
-            Deprecated synonym for lon_column.
-        dec_column : str
-            Deprecated synonym for lat_column.
         flux_columns : str or list of str
             Part of expected vot Flux column(s). Each one should match only one column
             in the file. Only used for vot files.
         frame : str
             Name of coordinate frame for VOTable source positions (lon/lat columns).
             Defaults to "icrs". Must be interpretable by
             `astropy.coordinates.frame_transform_graph.lookup_name()`. Only used for
             vot files.
         reference_frequency : :class:`astropy.units.Quantity`
             Reference frequency for VOTable flux values, assumed to be the same value
             for all components.
         freq_array : :class:`astropy.units.Quantity`
             Frequencies corresponding to VOTable flux_columns (should be same length).
             Required for multiple flux columns.
+        freq_edge_array : :class:`astropy.units.Quantity`
+            Frequency sub-band edges for each flux_columns, shape (2, len(flux_columns)).
+            Required for multiple flux columns if `freq_array` is not regularly spaced.
+            If `freq_array` is regularly spaced and `freq_edge_array` is not passed,
+            `freq_edge_array` will be calculated from the freq_array assuming the
+            band edges are directly between the band centers.
         spectral_index_column : str
             Part of expected VOTable spectral index column. Should match only one
             column in the file.
         flux_error_columns : str or list of str
             Part of expected VOTable flux error column(s). Each one should match only
             one column in the file.
         history : str
@@ -5117,27 +4668,27 @@
             filetype=filetype,
             run_check=run_check,
             check_extra=check_extra,
             run_check_acceptability=run_check_acceptability,
             # Gleam vot
             spectral_type=spectral_type,
             with_error=with_error,
+            use_paper_freqs=use_paper_freqs,
             # fhd
             expand_extended=expand_extended,
             # vot
             table_name=table_name,
             id_column=id_column,
             lon_column=lon_column,
             lat_column=lat_column,
-            ra_column=ra_column,
-            dec_column=dec_column,
             flux_columns=flux_columns,
             frame=frame,
             reference_frequency=reference_frequency,
             freq_array=freq_array,
+            freq_edge_array=freq_edge_array,
             spectral_index_column=spectral_index_column,
             flux_error_columns=flux_error_columns,
             history=history,
         )
         return self
 
     def write_skyh5(
@@ -5206,14 +4757,15 @@
                 "_spectral_type",
                 "_history",
                 "_name",
                 "_nside",
                 "_hpx_order",
                 "_hpx_inds",
                 "_freq_array",
+                "_freq_edge_array",
                 "_reference_frequency",
                 "_spectral_index",
                 "_stokes_error",
                 "_beam_amp",
                 "_extended_model_group",
             ]
             for par in header_params:
@@ -5266,79 +4818,14 @@
                 compression=data_compression,
                 dtype=self.stokes.dtype,
                 chunks=True,
             )
             # Use `str` to ensure this works for Composite units (e.g. Jy/sr) as well.
             dgrp["stokes"].attrs["unit"] = str(self.stokes.unit)
 
-    def write_healpix_hdf5(self, filename):
-        """
-        Write a set of HEALPix maps to an HDF5 file.
-
-        Deprecated. Support for this file format will be removed in version 0.3.0.
-        Use `write_skyh5` to read our newer skyh5 file type.
-
-        Parameters
-        ----------
-        filename: str
-            Name of file to write to.
-
-        """
-        warnings.warn(
-            "This method writes an old 'healvis' style healpix HDF5 file. Support for "
-            "this file format is deprecated and will be removed in version 0.3.0. Use "
-            "the `write_skyh5` method to write the newer skyh5 file type.",
-            category=DeprecationWarning,
-        )
-
-        if self.component_type != "healpix":
-            raise ValueError("component_type must be 'healpix' to use this method.")
-
-        self.check()
-        hpmap = self.stokes[0, :, :].to(units.K).value
-
-        history = self.history
-        if not uvutils._check_history_version(history, self.pyradiosky_version_str):
-            history += self.pyradiosky_version_str
-
-        valid_params = {
-            "Npix": self.Ncomponents,
-            "nside": self.nside,
-            "Nskies": 1,
-            "Nfreqs": self.Nfreqs,
-            "data": hpmap[None, ...],
-            "indices": self.hpx_inds,
-            "freqs": self.freq_array,
-            "units": "K",
-            "history": history,
-        }
-        dsets = {
-            "data": np.float64,
-            "indices": np.int32,
-            "freqs": np.float64,
-            "history": h5py.special_dtype(vlen=str),
-        }
-
-        with h5py.File(filename, "w") as fileobj:
-            for k in valid_params:
-                d = valid_params[k]
-                if k in dsets:
-                    if k == "history":
-                        fileobj.create_dataset(k, data=d, dtype=dsets[k])
-                    else:
-                        fileobj.create_dataset(
-                            k,
-                            data=d,
-                            dtype=dsets[k],
-                            compression="gzip",
-                            compression_opts=9,
-                        )
-                else:
-                    fileobj.attrs[k] = d
-
     def write_text_catalog(self, filename):
         """
         Write out this object to a text file.
 
         Readable with :meth:`~skymodel.SkyModel.read_text_catalog()`.
 
         Parameters
@@ -5346,14 +4833,25 @@
         filename : str
             Path to output file (string)
 
         """
         if self.component_type != "point":
             raise ValueError("component_type must be 'point' to use this method.")
 
+        if not self.stokes.unit.is_equivalent("Jy"):
+            raise ValueError(
+                "Stokes units must be equivalent to Jy to use this method."
+            )
+
+        if self.spectral_type == "subband":
+            warnings.warn(
+                "Text files do not support subband types, this will be written as a "
+                "'full' spectral type (losing the frequency edge array information)."
+            )
+
         self.check()
 
         comp_names = self._get_lon_lat_component_names()
         frame_obj = self._get_frame_obj()
         frame_desc_str = _get_frame_desc_str(frame_obj)
         comp_field = []
         for comp_name in comp_names:
@@ -5382,24 +4880,18 @@
                     freq_str = "{:g}_MHz".format(freq_hz_val * 1e-6)
                 elif freq_hz_val > 1e3:
                     freq_str = "{:g}_kHz".format(freq_hz_val * 1e-3)
                 else:
                     freq_str = "{:g}_Hz".format(freq_hz_val)
 
                 format_str += "\t{:0.8f}"
-                if self.spectral_type == "subband":
-                    header += f"\tFlux_subband_{freq_str} [Jy]"
-                    if self.stokes_error is not None:
-                        header += f"\tFlux_error_subband_{freq_str} [Jy]"
-                        format_str += "\t{:0.8f}"
-                else:
-                    header += f"\tFlux_{freq_str} [Jy]"
-                    if self.stokes_error is not None:
-                        header += f"\tFlux_error_{freq_str} [Jy]"
-                        format_str += "\t{:0.8f}"
+                header += f"\tFlux_{freq_str} [Jy]"
+                if self.stokes_error is not None:
+                    header += f"\tFlux_error_{freq_str} [Jy]"
+                    format_str += "\t{:0.8f}"
         else:
             # flat spectral response, no freq info
             header += "\tFlux [Jy]"
             format_str += "\t{:0.8f}"
             if self.stokes_error is not None:
                 header += "\tFlux_error [Jy]"
                 format_str += "\t{:0.8f}"
```

### Comparing `pyradiosky-0.2.0/pyradiosky/spherical_coords_transforms.py` & `pyradiosky-0.3.0/pyradiosky/spherical_coords_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,14 @@
 
     Returns
     -------
     array
         3x3 rotation matrix to rotate vectors by `angle` around `axis`.
     """
     if axis.shape != (3,):
-
         raise ValueError("axis must be a must be length 3 vector")
     if not is_unit_vector(axis):
         raise ValueError("axis must be a unit vector")
 
     K_matrix = np.array(
         [[0.0, -axis[2], axis[1]], [axis[2], 0.0, -axis[0]], [-axis[1], axis[0], 0.0]]
     )
@@ -288,15 +287,14 @@
 
         assert is_unit_vector(r1), "r1 is not a unit vector: " + str(r1)
         assert is_unit_vector(r2), "r2 is not a unit vector: " + str(r2)
     else:
         r1 = np.array(r1)
         r2 = np.array(r2)
         if r1.shape != (3,) or r2.shape != (3,):
-
             raise ValueError("r1 and r2 must be length 3 vectors")
         if not is_unit_vector(r1) or not is_unit_vector(r2):
             raise ValueError("r1 and r2 must be unit vectors")
 
     norm = np.cross(r1, r2)
     # Note that Psi is between 0 and pi
     sinPsi = np.sqrt(np.dot(norm, norm))
```

### Comparing `pyradiosky-0.2.0/pyradiosky/tests/conftest.py` & `pyradiosky-0.3.0/pyradiosky/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,13 +15,13 @@
     # mirror site in python 3 (but won't redownload if a current one exists).
     # If there's not a current IERS table and it can't be downloaded, turn off
     # auto downloading for the tests and turn it back on once all tests are
     # completed (done by extending auto_max_age).
     try:
         t1 = Time.now()
         t1.ut1
-    except (Exception):
+    except Exception:
         iers.conf.auto_max_age = None
 
     yield
 
     iers.conf.auto_max_age = 30
```

### Comparing `pyradiosky-0.2.0/pyradiosky/tests/test_skymodel.py` & `pyradiosky-0.3.0/pyradiosky/tests/test_skymodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,24 @@
 import os
 import re
 import warnings
 
 import h5py
 import numpy as np
 import pytest
-import pyuvdata.tests as uvtest
-import pyuvdata.utils as uvutils
+
+with warnings.catch_warnings():
+    # This filter can be removed when pyuvdata
+    # is updated to use importlib.metadata rather than pkg_resources
+    warnings.filterwarnings(
+        "ignore", "Deprecated call to `pkg_resources.declare_namespace"
+    )
+    warnings.filterwarnings("ignore", "pkg_resources is deprecated as an API")
+    import pyuvdata.tests as uvtest
+    import pyuvdata.utils as uvutils
 import scipy.io
 from astropy import units
 from astropy.coordinates import (
     AltAz,
     Angle,
     EarthLocation,
     Galactic,
@@ -43,14 +51,28 @@
 
     time = Time("2015-03-01 00:00:00", scale="utc", location=array_location)
 
     return time, array_location
 
 
 @pytest.fixture
+def moon_time_location():
+    pytest.importorskip("lunarsky")
+
+    from lunarsky import MoonLocation
+    from lunarsky import Time as LTime
+
+    array_location = MoonLocation.from_selenodetic(0.6875, 24.433, 0)
+
+    time = LTime("2015-03-01 00:00:00", scale="utc", location=array_location)
+
+    return time, array_location
+
+
+@pytest.fixture
 def zenith_skycoord(time_location):
     time, array_location = time_location
 
     source_coord = SkyCoord(
         alt=Angle(90, unit=units.deg),
         az=Angle(0, unit=units.deg),
         obstime=time,
@@ -72,33 +94,29 @@
 
 
 @pytest.fixture
 def moonsky():
     pytest.importorskip("lunarsky")
 
     from lunarsky import MoonLocation
-    from lunarsky import SkyCoord as SkyC
+    from lunarsky import SkyCoord as LunarSkyCoord
 
     # Tranquility base
     array_location = MoonLocation(lat="00d41m15s", lon="23d26m00s", height=0.0)
 
     time = Time.now()
-    zen_coord = SkyC(
+    zen_coord = LunarSkyCoord(
         alt=Angle(90, unit=units.deg),
         az=Angle(0, unit=units.deg),
         obstime=time,
         frame="lunartopo",
         location=array_location,
     )
 
-    # This filter can be removed when lunarsky is updated to not trigger this
-    # astropy deprecation warning.
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message="The get_frame_attr_names")
-        icrs_coord = zen_coord.transform_to("icrs")
+    icrs_coord = zen_coord.transform_to("icrs")
 
     names = "zen_source"
     stokes = [1.0, 0, 0, 0] * units.Jy
     zenith_source = SkyModel(
         name=names, skycoord=icrs_coord, stokes=stokes, spectral_type="flat"
     )
 
@@ -170,26 +188,31 @@
     freq_arr = np.linspace(100e6, 130e6, Nfreqs) * units.Hz
 
     # Spectrum = Power law
     alpha = -0.5
     spectrum = ((freq_arr / freq_arr[0]) ** (alpha))[None, :, None] * units.Jy
 
     def _func(stype):
-
         stokes = spectrum.repeat(4, 0).repeat(Ncomp, 2)
         filename_use = ["mock_point_" + stype]
         if stype in ["full", "subband"]:
             stokes = spectrum.repeat(4, 0).repeat(Ncomp, 2)
             stokes[1:, :, :] = 0.0  # Set unpolarized
+            freq_edge_arr = None
+            if stype == "subband":
+                freq_edge_arr = skymodel._get_freq_edges_from_centers(
+                    freq_arr, (0 * units.Hz, 10 * units.Hz)
+                )
             return SkyModel(
                 name=names,
                 skycoord=skycoord,
                 stokes=stokes,
                 spectral_type=stype,
                 freq_array=freq_arr,
+                freq_edge_array=freq_edge_arr,
                 filename=filename_use,
             )
         elif stype == "spectral_index":
             stokes = stokes[:, :1, :]
             spectral_index = np.ones(Ncomp) * alpha
             return SkyModel(
                 name=names,
@@ -210,20 +233,14 @@
                 filename=filename_use,
             )
 
     yield _func
 
 
 @pytest.fixture(scope="function")
-def healpix_disk_old():
-    pytest.importorskip("astropy_healpix")
-    return SkyModel.from_healpix_hdf5(os.path.join(SKY_DATA_PATH, "healpix_disk.hdf5"))
-
-
-@pytest.fixture(scope="function")
 def healpix_disk_new():
     pytest.importorskip("astropy_healpix")
     sky = SkyModel.from_skyh5(os.path.join(SKY_DATA_PATH, "healpix_disk.skyh5"))
 
     yield sky
 
     del sky
@@ -261,14 +278,15 @@
     sky = SkyModel(
         component_type="point",
         name=["src1", "src2"],
         skycoord=skycoord,
         stokes=stokes,
         spectral_type="subband",
         freq_array=Quantity([150], unit=units.MHz),
+        freq_edge_array=Quantity([140, 160], unit=units.MHz)[:, np.newaxis],
         stokes_error=stokes_error,
         beam_amp=beam_amp,
         extended_model_group=extended_group,
     )
 
     yield nside, pix_num, sky
 
@@ -291,22 +309,79 @@
     sky = SkyModel.from_file(os.path.join(SKY_DATA_PATH, "gsm_icrs.skyh5"))
 
     yield sky
 
     del sky
 
 
-def test_init_error(zenith_skycoord):
+@pytest.mark.filterwarnings("ignore:freq_edge_array not set, calculating it from")
+def test_init_subband(zenith_skycoord):
+    n_freqs = 5
+    freq_bottom_array = np.arange(1, (1 + n_freqs), dtype=float) * 1e8 * units.Hz
+    freq_top_array = np.arange(2, (2 + n_freqs), dtype=float) * 1e8 * units.Hz
+    freq_array = (freq_bottom_array + freq_top_array) / 2.0
+
+    stokes = np.zeros((4, n_freqs, 1), dtype=np.float64) * units.Jy
+    stokes[0, :, :] = 1 * units.Jy
+
+    refsky = SkyModel(
+        skycoord=zenith_skycoord,
+        name=["zen"],
+        stokes=stokes,
+        spectral_type="subband",
+        freq_array=freq_array,
+        freq_edge_array=np.concatenate(
+            (freq_bottom_array[np.newaxis, :], freq_top_array[np.newaxis, :]), axis=0
+        ),
+    )
 
+    sky1 = SkyModel(
+        skycoord=zenith_skycoord,
+        name=["zen"],
+        stokes=stokes,
+        spectral_type="subband",
+        freq_array=freq_array,
+    )
+    assert sky1 == refsky
+
+    sky2 = SkyModel(
+        skycoord=zenith_skycoord,
+        name=["zen"],
+        stokes=stokes,
+        spectral_type="subband",
+        freq_edge_array=np.concatenate(
+            (freq_bottom_array[np.newaxis, :], freq_top_array[np.newaxis, :]), axis=0
+        ),
+    )
+    assert sky2 == refsky
+
+
+def test_init_error(zenith_skycoord):
     with pytest.raises(ValueError, match="If initializing with values, all of"):
         SkyModel(
             skycoord=zenith_skycoord,
             stokes=[1.0, 0, 0, 0] * units.Jy,
             spectral_type="flat",
         )
+    with pytest.raises(
+        ValueError,
+        match="Cannot calculate frequency edges from frequency center array because "
+        "there is only one frequency center.",
+    ):
+        with uvtest.check_warnings(
+            UserWarning,
+            match="freq_edge_array not set, calculating it from the freq_array.",
+        ):
+            SkyModel(
+                skycoord=zenith_skycoord,
+                name=["zen"],
+                stokes=[1.0, 0, 0, 0] * units.Jy,
+                spectral_type="subband",
+                freq_array=100e6 * units.Hz,
+            )
 
     with pytest.raises(ValueError, match="component_type must be one of:"):
         SkyModel(
             name="zenith_source",
             skycoord=zenith_skycoord,
             stokes=[1.0, 0, 0, 0],
             spectral_type="flat",
@@ -362,14 +437,33 @@
     skyobj2 = skyobj.copy()
     skyobj2.freq_array = skyobj2.freq_array / units.sr
     with pytest.raises(
         ValueError, match="freq_array must have a unit that can be converted to Hz."
     ):
         skyobj2.check()
 
+    skyobj2 = skyobj.copy()
+    skyobj2.freq_edge_array = None
+    with uvtest.check_warnings(
+        DeprecationWarning,
+        match="freq_edge_array is not set. Cannot calculate it from the freq_array "
+        "because freq_array spacing is not constant. This will become an error in "
+        "version 0.5",
+    ):
+        skyobj2.check()
+
+    skyobj2.freq_array = (np.arange(skyobj2.Nfreqs) * 1e7 + 1e8) * units.Hz
+    skyobj2.freq_edge_array = None
+    with uvtest.check_warnings(
+        DeprecationWarning,
+        match="freq_edge_array is not set. Calculating it from the freq_array. This "
+        "will become an error in version 0.5",
+    ):
+        skyobj2.check()
+
     skyobj = SkyModel.from_gleam_catalog(GLEAM_vot, spectral_type="spectral_index")
     skyobj2 = skyobj.copy()
     skyobj2.reference_frequency = skyobj2.reference_frequency / units.sr
     with pytest.raises(
         ValueError,
         match="reference_frequency must have a unit that can be converted to Hz.",
     ):
@@ -423,20 +517,15 @@
 
     ras = Longitude(
         [zenith_skycoord.ra + Longitude(0.5 * ind * units.deg) for ind in range(5)]
     )
     decs = Latitude(np.zeros(5, dtype=np.float64) + icrs_coord.dec.value * units.deg)
     names = ["src_" + str(ind) for ind in range(5)]
 
-    if spec_type in ["subband", "full"]:
-        n_freqs = 3
-        freq_array = [100e6, 120e6, 140e6] * units.Hz
-    else:
-        n_freqs = 1
-        freq_array = None
+    n_freqs = 1
 
     stokes = np.zeros((4, n_freqs, 5), dtype=np.float64) * units.Jy
     stokes[0, :, :] = 1 * units.Jy
 
     if spec_type == "spectral_index":
         ref_freqs = np.zeros(5, dtype=np.float64) + 150e6 * units.Hz
         spec_index = np.zeros(5, dtype=np.float64) - 0.8
@@ -448,15 +537,14 @@
         name=names,
         ra=ras,
         dec=decs,
         frame="icrs",
         stokes=stokes,
         reference_frequency=ref_freqs,
         spectral_index=spec_index,
-        freq_array=freq_array,
         spectral_type=spec_type,
     )
 
     if param == "ra":
         ras = list(ras)
     elif param == "dec":
         decs = list(decs)
@@ -465,15 +553,14 @@
         name=names,
         ra=ras,
         dec=decs,
         frame="icrs",
         stokes=stokes,
         reference_frequency=ref_freqs,
         spectral_index=spec_index,
-        freq_array=freq_array,
         spectral_type=spec_type,
     )
 
     assert ref_model == list_model
 
 
 @pytest.mark.parametrize(
@@ -671,15 +758,14 @@
         sky.calc_frame_coherency()
         sky.frame_coherency = sky.frame_coherency.value * units.m
         sky.check()
 
 
 @pytest.mark.parametrize("spec_type", ["flat", "subband", "spectral_index"])
 def test_jansky_to_kelvin_loop(spec_type):
-
     skyobj = SkyModel.from_file(
         GLEAM_vot, spectral_type=spec_type, with_error=True, filetype="gleam"
     )
 
     stokes_expected = np.zeros_like(skyobj.stokes.value) * units.K * units.sr
     if spec_type == "subband":
         brightness_temperature_conv = units.brightness_temperature(skyobj.freq_array)
@@ -764,43 +850,43 @@
         zenith_skymodel.stokes = zenith_skymodel.stokes.value * units.K * units.sr
         zenith_skymodel.kelvin_to_jansky()
 
 
 @pytest.mark.parametrize("order", ["ring", "nested"])
 @pytest.mark.parametrize("to_jy", [True, False])
 @pytest.mark.parametrize("to_k", [True, False])
-@pytest.mark.parametrize("undo_method", ["point_to_healpix", "assign_to_healpix"])
-def test_healpix_to_point_loop(healpix_disk_new, order, to_jy, to_k, undo_method):
+def test_healpix_to_point_loop(healpix_disk_new, order, to_jy, to_k):
     skyobj = healpix_disk_new
     skyobj.calc_frame_coherency()
 
+    frame_coherency = copy.deepcopy(skyobj.frame_coherency)
+    # check strore=False
+    new_frame_coherency = skyobj.calc_frame_coherency(store=False)
+    assert np.array_equal(frame_coherency, new_frame_coherency)
+
     if order == "nested":
         skyobj.hpx_order = "nested"
 
     skyobj2 = skyobj.copy()
     skyobj2.healpix_to_point(to_jy=to_jy)
 
-    if undo_method == "point_to_healpix":
-        with uvtest.check_warnings(
-            DeprecationWarning,
-            match="This method is deprecated and will be removed in version 0.3.0.",
-        ):
-            skyobj2.point_to_healpix(to_k=to_k)
-    else:
-        skyobj2.assign_to_healpix(skyobj.nside, order=order, inplace=True, to_k=to_k)
+    skyobj2.assign_to_healpix(skyobj.nside, order=order, inplace=True, to_k=to_k)
 
     if to_jy and not to_k:
         skyobj.kelvin_to_jansky()
 
     assert skyobj == skyobj2
 
 
 def test_healpix_to_point_loop_ordering(healpix_disk_new):
     skyobj = healpix_disk_new
 
+    # add frame_coherency
+    skyobj.calc_frame_coherency()
+
     skyobj2 = skyobj.copy()
     skyobj2.hpx_order = "nested"
     skyobj2.healpix_to_point()
 
     skyobj2._point_to_healpix()
 
     assert skyobj != skyobj2
@@ -849,14 +935,15 @@
     if spectral_type != "subband":
         sky.spectral_type = "spectral_index"
         sky.reference_frequency = Quantity(
             [sky.freq_array[0], sky.freq_array[0]], unit=units.MHz
         )
         sky.spectral_index = np.array([-0.8, -0.8])
         sky.freq_array = None
+        sky.freq_edge_array = None
         sky.stokes_error = None
         sky.beam_amp = None
         sky.extended_model_group = None
 
     sky_hpx = sky.assign_to_healpix(nside, full_sky=True)
 
     hpx_area = astropy_healpix.nside_to_pixel_area(nside)
@@ -894,35 +981,14 @@
     assert sky.skycoord.frame.name == "icrs"
     assert sky.frame == "icrs"
     sky.assign_to_healpix(nside, inplace=True)
     assert sky.hpx_frame.name == "icrs"
     assert sky.frame == "icrs"
 
 
-def test_assign_healpix_frame_override_attribute(assign_hpx_data):
-    nside, _, sky = assign_hpx_data
-    sky.skycoord = sky.skycoord.transform_to("fk5")
-    assert sky.skycoord.frame.name == "fk5"
-    assert sky.frame == "fk5"
-    with uvtest.check_warnings(
-        [DeprecationWarning, UserWarning],
-        match=[
-            "The frame keyword is deprecated, in version 0.3.0 this method will use "
-            "the frame of this object's skycoord attribute.",
-            re.escape(
-                "Input parameter frame (value: icrs) differs from the skycoord "
-                "frame on this object (value: fk5)"
-            ),
-        ],
-    ):
-        sky.assign_to_healpix(nside, frame="icrs", inplace=True)
-    assert sky.hpx_frame.name == "icrs"
-    assert sky.frame == "icrs"
-
-
 def test_assign_to_healpix_errors(assign_hpx_data):
     nside, _, sky = assign_hpx_data
 
     sky2 = sky.copy()
     sky2.assign_to_healpix(nside, inplace=True)
     with pytest.raises(
         ValueError, match="This method can only be called if component_type is 'point'."
@@ -1064,21 +1130,25 @@
     )
 
     with uvtest.check_warnings(UserWarning, match="Horizon cutoff undefined"):
         with pytest.raises(ValueError, match="telescope_location must be an"):
             source.coherency_calc().squeeze()
 
 
-def test_calc_basis_rotation_matrix(time_location):
+@pytest.mark.parametrize("telescope_frame", ["itrs", "mcmf"])
+def test_calc_basis_rotation_matrix(time_location, moon_time_location, telescope_frame):
     """
     This tests whether the 3-D rotation matrix from RA/Dec to Alt/Az is
     actually a rotation matrix (R R^T = R^T R = I)
     """
 
-    time, telescope_location = time_location
+    if telescope_frame == "itrs":
+        time, telescope_location = time_location
+    else:
+        time, telescope_location = moon_time_location
 
     source = SkyModel(
         name="Test",
         skycoord=SkyCoord(
             Longitude(12.0 * units.hr), Latitude(-30.0 * units.deg), frame="icrs"
         ),
         stokes=[1.0, 0.0, 0.0, 0.0] * units.Jy,
@@ -1088,20 +1158,24 @@
 
     basis_rot_matrix = source._calc_average_rotation_matrix()
 
     assert np.allclose(np.matmul(basis_rot_matrix, basis_rot_matrix.T), np.eye(3))
     assert np.allclose(np.matmul(basis_rot_matrix.T, basis_rot_matrix), np.eye(3))
 
 
-def test_calc_vector_rotation(time_location):
+@pytest.mark.parametrize("telescope_frame", ["itrs", "mcmf"])
+def test_calc_vector_rotation(time_location, moon_time_location, telescope_frame):
     """
     This checks that the 2-D coherency rotation matrix is unit determinant.
     I suppose we could also have checked (R R^T = R^T R = I)
     """
-    time, telescope_location = time_location
+    if telescope_frame == "itrs":
+        time, telescope_location = time_location
+    else:
+        time, telescope_location = moon_time_location
 
     source = SkyModel(
         name="Test",
         ra=Longitude(12.0 * units.hr),
         dec=Latitude(-30.0 * units.deg),
         frame="icrs",
         stokes=[1.0, 0.0, 0.0, 0.0] * units.Jy,
@@ -1229,22 +1303,14 @@
         ra=Longitude(zenith_icrs.ra + raoff),
         dec=Latitude(zenith_icrs.dec + decoff),
         frame="icrs",
         stokes=stokes_radec,
         spectral_type="flat",
     )
 
-    frame_coherency = source.calc_frame_coherency(store=False)
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="coherency_radec is a deprecated parameter, use frame_coherency",
-    ):
-        assert np.array_equal(source.coherency_radec, frame_coherency)
-
     coherency_matrix_local = np.zeros([2, 2, ntimes], dtype="complex128") * units.Jy
     alts = np.zeros(ntimes)
     azs = np.zeros(ntimes)
     for ti, time in enumerate(times):
         source.update_positions(time, telescope_location=array_location)
         alt, az = source.alt_az
         assert alt == src_astropy_altaz[ti].alt.radian
@@ -1300,41 +1366,53 @@
         )
         * units.Jy
     )
 
     assert units.quantity.allclose(coherency_instr_local, expected_instr_local)
 
 
-def test_polarized_source_smooth_visibilities():
+@pytest.mark.parametrize("telescope_frame", ["itrs", "mcmf"])
+def test_polarized_source_smooth_visibilities(
+    time_location, moon_time_location, telescope_frame
+):
     """Test that visibilities change smoothly as a polarized source transits."""
-    array_location = EarthLocation(lat="-30d43m17.5s", lon="21d25m41.9s", height=1073.0)
-    time0 = Time("2015-03-01 18:00:00", scale="utc", location=array_location)
+    if telescope_frame == "itrs":
+        time0, array_location = time_location
+        altaz_frame = "altaz"
+        skycoordobj = SkyCoord
+    else:
+        pytest.importorskip("lunarsky")
+        from lunarsky import SkyCoord as LunarSkyCoord
+
+        time0, array_location = moon_time_location
+        altaz_frame = "lunartopo"
+        skycoordobj = LunarSkyCoord
 
     ha_off = 1
     ha_delta = 0.01
     time_offsets = np.arange(-ha_off, ha_off + ha_delta, ha_delta)
     zero_indx = np.argmin(np.abs(time_offsets))
     # make sure we get a true zenith time
     time_offsets[zero_indx] = 0.0
     times = time0 + time_offsets * units.hr
     ntimes = times.size
 
-    zenith = SkyCoord(
+    zenith = skycoordobj(
         alt=90.0 * units.deg,
         az=0 * units.deg,
-        frame="altaz",
+        frame=altaz_frame,
         obstime=time0,
         location=array_location,
     )
     zenith_icrs = zenith.transform_to("icrs")
 
-    src_astropy = SkyCoord(
+    src_astropy = skycoordobj(
         ra=zenith_icrs.ra, dec=zenith_icrs.dec, obstime=times, location=array_location
     )
-    src_astropy_altaz = src_astropy.transform_to("altaz")
+    src_astropy_altaz = src_astropy.transform_to(altaz_frame)
     assert np.isclose(src_astropy_altaz.alt.rad[zero_indx], np.pi / 2)
 
     stokes_radec = [1, -0.2, 0.3, 0.1] * units.Jy
 
     source = SkyModel(
         name="icrs_zen", skycoord=zenith_icrs, stokes=stokes_radec, spectral_type="flat"
     )
@@ -1713,151 +1791,14 @@
     # check it works with clear_time_position
     skyobj1.concat(skyobj2, clear_time_position=True)
     skyobj_hpx_disk.clear_time_position_specific_params()
     skyobj1.history = skyobj_hpx_disk.history
     assert skyobj1 == skyobj_hpx_disk
 
 
-@pytest.mark.filterwarnings("ignore:This method reads an old 'healvis' style healpix")
-def test_units_healpix_to_sky(healpix_data, healpix_disk_old):
-
-    healpix_filename = os.path.join(SKY_DATA_PATH, "healpix_disk.hdf5")
-    with h5py.File(healpix_filename, "r") as fileobj:
-        hpmap = fileobj["data"][0, ...]  # Remove Nskies axis.
-        freqs = fileobj["freqs"][()]
-
-    freqs = freqs * units.Hz
-
-    brightness_temperature_conv = units.brightness_temperature(
-        freqs, beam_area=healpix_data["pixel_area"]
-    )
-    stokes = (hpmap.T * units.K).to(units.Jy, brightness_temperature_conv).T
-    sky = healpix_disk_old
-    sky.healpix_to_point()
-
-    assert units.quantity.allclose(sky.stokes[0, 0], stokes[0])
-
-
-def test_healpix_recarray_loop(healpix_disk_new):
-
-    skyobj = healpix_disk_new
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="The to_recarray method is deprecated and will be removed in 0.3.0.",
-    ):
-        skyarr = skyobj.to_recarray()
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="The from_recarray method is deprecated and will be removed in 0.3.0.",
-    ):
-        skyobj2 = SkyModel.from_recarray(skyarr, history=skyobj.history)
-    assert skyobj.component_type == "healpix"
-    assert skyobj2.component_type == "healpix"
-
-    assert skyobj == skyobj2
-
-
-@pytest.mark.filterwarnings("ignore:This method reads an old 'healvis' style healpix")
-@pytest.mark.filterwarnings("ignore:This method writes an old 'healvis' style healpix")
-@pytest.mark.parametrize("change_history", [True, False, "error"])
-def test_read_write_healpix_old(tmp_path, healpix_disk_old, change_history):
-
-    test_filename = os.path.join(tmp_path, "tempfile.hdf5")
-
-    sky = healpix_disk_old
-
-    if change_history is True:
-        sky.history = ""
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method writes an old 'healvis' style healpix HDF5 file. Support for "
-        "this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        sky.write_healpix_hdf5(test_filename)
-
-    if change_history == "error":
-        with h5py.File(test_filename, "a") as h5f:
-            del h5f["/history"]
-            h5f["/history"] = sky.history.encode("ibm039")
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method reads an old 'healvis' style healpix HDF5 file. Support for "
-        "this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        sky2 = SkyModel.from_healpix_hdf5(test_filename)
-
-    if change_history:
-        assert uvutils._check_histories(sky.pyradiosky_version_str, sky2.history)
-        sky.history = sky2.history
-
-    assert sky == sky2
-
-
-@pytest.mark.filterwarnings("ignore:This method reads an old 'healvis' style healpix")
-def test_read_write_healpix_old_cut_sky(tmp_path, healpix_disk_old):
-
-    test_filename = os.path.join(tmp_path, "tempfile.hdf5")
-
-    sky = healpix_disk_old
-    sky.select(component_inds=np.arange(10))
-    sky.check()
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method writes an old 'healvis' style healpix HDF5 file. Support for "
-        "this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        sky.write_healpix_hdf5(test_filename)
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method reads an old 'healvis' style healpix HDF5 file. Support for "
-        "this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        sky2 = SkyModel.from_healpix_hdf5(test_filename)
-
-    assert sky == sky2
-
-
-@pytest.mark.filterwarnings("ignore:This method reads an old 'healvis' style healpix")
-def test_read_write_healpix_old_nover_history(tmp_path, healpix_disk_old):
-    test_filename = os.path.join(tmp_path, "tempfile.hdf5")
-
-    sky = healpix_disk_old
-    sky.history = sky.pyradiosky_version_str
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method writes an old 'healvis' style healpix HDF5 file. Support for "
-        "this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        sky.write_healpix_hdf5(test_filename)
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method reads an old 'healvis' style healpix HDF5 file. Support for "
-        "this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        sky2 = SkyModel.from_healpix_hdf5(test_filename)
-
-    assert sky == sky2
-
-
-@pytest.mark.filterwarnings("ignore:This method writes an old 'healvis' style healpix")
-def test_write_healpix_error(tmp_path):
-    skyobj = SkyModel.from_file(GLEAM_vot, with_error=True)
-    test_filename = os.path.join(tmp_path, "tempfile.hdf5")
-
-    with pytest.raises(
-        ValueError, match="component_type must be 'healpix' to use this method."
-    ):
-        skyobj.write_healpix_hdf5(test_filename)
-
-
 def test_healpix_import_err(zenith_skymodel):
     try:
         import astropy_healpix
 
         astropy_healpix.nside_to_npix(2**3)
     except ImportError:
         errstr = "The astropy-healpix module must be installed to use HEALPix methods"
@@ -1868,27 +1809,24 @@
                 hpx_inds=[0],
                 frame="icrs",
                 stokes=Quantity([1.0, 0.0, 0.0, 0.0], unit=units.K),
                 spectral_type="flat",
             )
             sm.get_lon_lat()
 
-        with pytest.raises(ImportError, match=errstr):
-            SkyModel.from_healpix_hdf5(os.path.join(SKY_DATA_PATH, "healpix_disk.hdf5"))
-
         zenith_skymodel.nside = 32
         zenith_skymodel.hpx_inds = 0
         zenith_skymodel.hpx_order = "ring"
         with pytest.raises(ImportError, match=errstr):
             zenith_skymodel._point_to_healpix()
 
         with pytest.raises(ImportError, match=errstr):
             zenith_skymodel.assign_to_healpix(32)
 
-        zenith_skymodel._set_component_type_params("healpix")
+        zenith_skymodel.component_type = "healpix"
         with pytest.raises(ImportError, match=errstr):
             zenith_skymodel.healpix_to_point()
 
 
 def test_healpix_positions(tmp_path, time_location):
     astropy_healpix = pytest.importorskip("astropy_healpix")
 
@@ -1941,21 +1879,16 @@
         hpx_inds=range(Npix),
         stokes=stokes * units.K,
         freq_array=freqs * units.Hz,
         spectral_type="full",
         frame="icrs",
     )
 
-    filename = os.path.join(tmp_path, "healpix_single.hdf5")
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method writes an old 'healvis' style healpix HDF5 file. Support "
-        "for this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        skyobj.write_healpix_hdf5(filename)
+    filename = os.path.join(tmp_path, "healpix_single.skyh5")
+    skyobj.write_skyh5(filename)
 
     time, array_location = time_location
 
     ra, dec = astropy_healpix.healpix_to_lonlat(ipix, nside)
     skycoord_use = SkyCoord(ra, dec, frame="icrs")
     source_altaz = skycoord_use.transform_to(
         AltAz(obstime=time, location=array_location)
@@ -1966,91 +1899,37 @@
     src_alt = Angle(alt_az[0], unit="deg")
     src_za = Angle("90.d") - src_alt
 
     src_l = np.sin(src_az.rad) * np.sin(src_za.rad)
     src_m = np.cos(src_az.rad) * np.sin(src_za.rad)
     src_n = np.cos(src_za.rad)
 
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="This method reads an old 'healvis' style healpix HDF5 file. Support for "
-        "this file format is deprecated and will be removed in version 0.3.0.",
-    ):
-        sky2 = SkyModel.from_healpix_hdf5(filename)
+    sky2 = SkyModel.from_file(filename)
 
     time.location = array_location
 
     sky2.update_positions(time, array_location)
     src_alt_az = sky2.alt_az
     assert np.isclose(src_alt_az[0][ipix], src_alt.rad)
     assert np.isclose(src_alt_az[1][ipix], src_az.rad)
 
     src_lmn = sky2.pos_lmn
     assert np.isclose(src_lmn[0][ipix], src_l)
     assert np.isclose(src_lmn[1][ipix], src_m)
     assert np.isclose(src_lmn[2][ipix], src_n)
 
 
-@pytest.mark.filterwarnings("ignore:The to_recarray method is deprecated")
-@pytest.mark.filterwarnings("ignore:The from_recarray method is deprecated")
-@pytest.mark.filterwarnings("ignore:recarray flux columns will no longer be labeled")
-@pytest.mark.parametrize("spec_type", ["flat", "subband", "spectral_index", "full"])
-@pytest.mark.parametrize("with_error", [False, True])
-@pytest.mark.parametrize("rise_set_lsts", [False, True])
-def test_array_to_skymodel_loop(spec_type, with_error, rise_set_lsts, time_location):
-    _, array_location = time_location
-    spectral_type = "subband" if spec_type == "full" else spec_type
-
-    sky = SkyModel.from_file(
-        GLEAM_vot, spectral_type=spectral_type, with_error=with_error
-    )
-    if spec_type == "full":
-        sky.spectral_type = "full"
-
-    if rise_set_lsts:
-        sky.calculate_rise_set_lsts(array_location.lat)
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="The to_recarray method is deprecated and will be removed in 0.3.0.",
-    ):
-        arr = sky.to_recarray()
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="The from_recarray method is deprecated and will be removed in 0.3.0.",
-    ):
-        sky2 = SkyModel.from_recarray(arr)
-
-    assert sky == sky2
-
-    if spec_type == "flat":
-        # again with no reference_frequency field
-        reference_frequency = sky.reference_frequency
-        sky.reference_frequency = None
-        arr = sky.to_recarray()
-        sky2 = SkyModel.from_recarray(arr)
-
-        assert sky == sky2
-
-        # again with flat & freq_array
-        sky.freq_array = np.atleast_1d(np.unique(reference_frequency))
-        sky2 = SkyModel.from_recarray(sky.to_recarray())
-
-        assert sky == sky2
-
-
 @pytest.mark.filterwarnings("ignore:The `source_cuts` method is deprecated")
 def test_flux_source_cuts():
     # Check that min/max flux limits in test params work.
 
     skyobj = SkyModel.from_file(GLEAM_vot, with_error=True)
 
-    skyobj2 = skyobj.source_cuts(
-        min_flux=0.2 * units.Jy, max_flux=1.5 * units.Jy, inplace=False
+    skyobj2 = skyobj.select(
+        min_brightness=0.2 * units.Jy, max_brightness=1.5 * units.Jy, inplace=False
     )
 
     for sI in skyobj2.stokes[0, 0, :]:
         assert np.all(0.2 * units.Jy < sI < 1.5 * units.Jy)
 
     components_to_keep = np.where(
         (np.min(skyobj.stokes[0, :, :], axis=0) > 0.2 * units.Jy)
@@ -2096,30 +1975,15 @@
     skyobj2 = skyobj.select(component_inds=None, inplace=False)
     assert skyobj2 == skyobj
 
     skyobj.select(component_inds=None)
     assert skyobj2 == skyobj
 
 
-def test_source_cut_healpix(healpix_disk_new, time_location):
-    skyobj = healpix_disk_new
-
-    _, array_location = time_location
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match=r"The `source_cuts` method is deprecated and will be removed in version "
-        r"0.3.0. Please use the `select` method and/or the `cut_nonrising` "
-        r"method as appropriate.",
-    ):
-        skyobj.source_cuts(latitude_deg=array_location.lat.deg)
-
-
-@pytest.mark.filterwarnings("ignore:The `source_cuts` method is deprecated")
-@pytest.mark.parametrize("function", ["select", "source_cuts"])
+@pytest.mark.filterwarnings("ignore:freq_edge_array not set, calculating it from")
 @pytest.mark.parametrize(
     "spec_type, init_kwargs, cut_kwargs",
     [
         ("flat", {}, {}),
         ("flat", {"reference_frequency": np.ones(20) * 200e6 * units.Hz}, {}),
         ("full", {"freq_array": np.array([1e8, 1.5e8]) * units.Hz}, {}),
         (
@@ -2135,15 +1999,15 @@
         (
             "flat",
             {"freq_array": np.array([1e8]) * units.Hz},
             {"freq_range": np.array([0.9e8, 2e8]) * units.Hz},
         ),
     ],
 )
-def test_flux_cuts(function, spec_type, init_kwargs, cut_kwargs):
+def test_flux_cuts(spec_type, init_kwargs, cut_kwargs):
     Nsrcs = 20
 
     minflux = 0.5
     maxflux = 3.0
 
     ids = ["src{}".format(i) for i in range(Nsrcs)]
     ras = Longitude(np.linspace(0, 360.0, Nsrcs), units.deg)
@@ -2168,47 +2032,37 @@
         stokes=stokes,
         spectral_type=spec_type,
         **init_kwargs,
     )
 
     minI_cut = 1.0
     maxI_cut = 2.3
-    if function == "select":
-        minI_cut *= units.Jy
-        maxI_cut *= units.Jy
-        if "freq_range" in cut_kwargs:
-            freq_range = cut_kwargs["freq_range"]
-        else:
-            freq_range = None
-        skyobj.select(
-            min_brightness=minI_cut,
-            max_brightness=maxI_cut,
-            brightness_freq_range=freq_range,
-        )
-    else:
-        skyobj.source_cuts(
-            latitude_deg=30.0, min_flux=minI_cut, max_flux=maxI_cut, **cut_kwargs
-        )
-
-    if function != "select":
-        minI_cut *= units.Jy
-        maxI_cut *= units.Jy
+    minI_cut *= units.Jy
+    maxI_cut *= units.Jy
+    if "freq_range" in cut_kwargs:
+        freq_range = cut_kwargs["freq_range"]
+    else:
+        freq_range = None
+    skyobj.select(
+        min_brightness=minI_cut,
+        max_brightness=maxI_cut,
+        brightness_freq_range=freq_range,
+    )
 
     if "freq_range" in cut_kwargs and np.min(
         cut_kwargs["freq_range"] > np.min(init_kwargs["freq_array"])
     ):
         assert np.all(skyobj.stokes[0] <= maxI_cut)
     else:
         assert np.all(skyobj.stokes[0] >= minI_cut)
         assert np.all(skyobj.stokes[0] <= maxI_cut)
     assert np.all(skyobj.stokes[2] == Ucomp * units.Jy)
 
 
-@pytest.mark.filterwarnings("ignore:The `source_cuts` method is deprecated")
-@pytest.mark.parametrize("function", ["select", "source_cuts"])
+@pytest.mark.filterwarnings("ignore:freq_edge_array not set, calculating it from")
 @pytest.mark.parametrize(
     "spec_type, init_kwargs, cut_kwargs, error_category, error_message",
     [
         (
             "spectral_index",
             {
                 "reference_frequency": np.ones(20) * 200e6 * units.Hz,
@@ -2238,15 +2092,15 @@
             {"freq_range": np.array([1.1e8, 1.4e8]) * units.Hz},
             ValueError,
             "No object frequencies in specified range for flux cuts.",
         ),
     ],
 )
 def test_flux_cut_error(
-    function, spec_type, init_kwargs, cut_kwargs, error_category, error_message
+    spec_type, init_kwargs, cut_kwargs, error_category, error_message
 ):
     Nsrcs = 20
 
     minflux = 0.5
     maxflux = 3.0
 
     ids = ["src{}".format(i) for i in range(Nsrcs)]
@@ -2266,45 +2120,38 @@
         dec=decs,
         frame="icrs",
         stokes=stokes,
         spectral_type=spec_type,
         **init_kwargs,
     )
 
-    if (
-        function == "select"
-        and "freq_range" in cut_kwargs
-        and not isinstance(cut_kwargs["freq_range"], Quantity)
+    if "freq_range" in cut_kwargs and not isinstance(
+        cut_kwargs["freq_range"], Quantity
     ):
         error_category = TypeError
         error_message = (
             "Argument 'brightness_freq_range' to function 'select' has no "
             "'unit' attribute. You should pass in an astropy Quantity instead."
         )
 
     with pytest.raises(error_category, match=error_message):
         minI_cut = 1.0
         maxI_cut = 2.3
 
-        if function == "select":
-            minI_cut *= units.Jy
-            maxI_cut *= units.Jy
-            if "freq_range" in cut_kwargs:
-                freq_range = cut_kwargs["freq_range"]
-            else:
-                freq_range = None
-            skyobj.select(
-                min_brightness=minI_cut,
-                max_brightness=maxI_cut,
-                brightness_freq_range=freq_range,
-            )
+        minI_cut *= units.Jy
+        maxI_cut *= units.Jy
+        if "freq_range" in cut_kwargs:
+            freq_range = cut_kwargs["freq_range"]
         else:
-            skyobj.source_cuts(
-                latitude_deg=30.0, min_flux=minI_cut, max_flux=maxI_cut, **cut_kwargs
-            )
+            freq_range = None
+        skyobj.select(
+            min_brightness=minI_cut,
+            max_brightness=maxI_cut,
+            brightness_freq_range=freq_range,
+        )
 
 
 def test_select_flux_error():
     Nsrcs = 20
 
     minflux = 0.5
     maxflux = 3.0
@@ -2330,14 +2177,15 @@
     with pytest.raises(TypeError, match="min_brightness must be a Quantity object"):
         skyobj.select(min_brightness=minI_cut)
 
     with pytest.raises(TypeError, match="max_brightness must be a Quantity object"):
         skyobj.select(max_brightness=maxI_cut)
 
 
+@pytest.mark.filterwarnings("ignore:freq_edge_array not set, calculating it from")
 @pytest.mark.parametrize(
     "spec_type, init_kwargs",
     [
         ("flat", {}),
         ("flat", {"reference_frequency": np.ones(20) * 200e6 * units.Hz}),
         ("full", {"freq_array": np.array([1e8, 1.5e8]) * units.Hz}),
         ("subband", {"freq_array": np.array([1e8, 1.5e8]) * units.Hz}),
@@ -2380,37 +2228,23 @@
     skyobj2.select(lon_range=lon_range)
     assert np.all(skyobj2.skycoord.ra >= lon_range[0])
     assert np.all(skyobj2.skycoord.ra <= lon_range[1])
 
     assert np.all(skyobj2.ra >= lon_range[0])
     assert np.all(skyobj2.ra <= lon_range[1])
 
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match=["lon is no longer a parameter on SkyModel objects."] * 2,
-    ):
-        assert np.all(skyobj2.lon >= lon_range[0])
-        assert np.all(skyobj2.lon <= lon_range[1])
-
     lat_range = Latitude([-45, 45], units.deg)
     skyobj2 = skyobj.copy()
     skyobj2.select(lat_range=lat_range)
     assert np.all(skyobj2.skycoord.dec >= lat_range[0])
     assert np.all(skyobj2.skycoord.dec <= lat_range[1])
 
     assert np.all(skyobj2.dec >= lat_range[0])
     assert np.all(skyobj2.dec <= lat_range[1])
 
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match=["lat is no longer a parameter on SkyModel objects."] * 2,
-    ):
-        assert np.all(skyobj2.lat >= lat_range[0])
-        assert np.all(skyobj2.lat <= lat_range[1])
-
     skyobj2 = skyobj.copy()
     skyobj2.select(lon_range=lon_range, lat_range=lat_range)
     assert np.all(skyobj2.skycoord.ra >= lon_range[0])
     assert np.all(skyobj2.skycoord.ra <= lon_range[1])
     assert np.all(skyobj2.skycoord.dec >= lat_range[0])
     assert np.all(skyobj2.skycoord.dec <= lat_range[1])
 
@@ -2511,14 +2345,18 @@
     stokes[0, ...] = 1.0 * units.Jy
 
     sky = SkyModel(
         name=names, ra=ra, dec=dec, frame="icrs", stokes=stokes, spectral_type="flat"
     )
 
     sky2 = sky.cut_nonrising(location.lat, inplace=False)
+    sky3 = sky.copy()
+    sky3.cut_nonrising(location.lat)
+
+    assert sky3 == sky2
 
     # Boolean array identifying nonrising sources that were removed
     nonrising = np.array([sky.name[ind] not in sky2.name for ind in range(Nsrcs)])
     sky2.calculate_rise_set_lsts(location.lat)
 
     is_below_horizon = np.zeros(Nsrcs).astype(bool)
     is_below_horizon[nonrising] = True
@@ -2657,28 +2495,27 @@
 def test_read_gleam(spec_type):
     skyobj = SkyModel.from_file(GLEAM_vot, spectral_type=spec_type, with_error=True)
 
     assert skyobj.Ncomponents == 50
     if spec_type == "subband":
         assert skyobj.Nfreqs == 20
 
-    # Check cuts
-    source_select_kwds = {"min_flux": 0.5}
-
-    msg_expected = [
-        "The source_select_kwds parameter is deprecated",
-        "The `source_cuts` method is deprecated and will be removed",
-    ]
-    with uvtest.check_warnings(DeprecationWarning, match=msg_expected):
-        cut_sky = SkyModel()
-        cut_sky.read_gleam_catalog(
-            GLEAM_vot, spectral_type=spec_type, source_select_kwds=source_select_kwds
+    if spec_type == "subband":
+        skyobj2 = SkyModel.from_file(
+            GLEAM_vot, spectral_type=spec_type, with_error=True, use_paper_freqs=True
         )
 
-    assert cut_sky.Ncomponents < skyobj.Ncomponents
+        assert skyobj2 != skyobj
+        assert skyobj2._freq_array != skyobj._freq_array
+
+        assert np.max(np.abs(skyobj2.freq_array - skyobj.freq_array)) <= 0.6 * units.MHz
+        assert (
+            np.max(np.abs(skyobj2.freq_edge_array - skyobj.freq_edge_array))
+            <= 1.08 * units.MHz
+        )
 
 
 def test_read_errors(tmpdir):
     skyobj = SkyModel()
     with pytest.raises(ValueError, match="Invalid filetype. Filetype options are"):
         skyobj.read(GLEAM_vot, filetype="foo")
 
@@ -2718,123 +2555,123 @@
         "RAJ2000",
         "DEJ2000",
         "Si",
         frame="fk5",
     )
     assert skyobj2 == skyobj
 
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match=[
-            "The `ra_column` keyword is deprecated and will be removed",
-            "The `dec_column` keyword is deprecated and will be removed",
-        ],
-    ):
-        skyobj3 = SkyModel.from_file(
-            votable_file,
-            table_name="VIII_1000_single",
-            id_column="source_id",
-            ra_column="RAJ2000",
-            dec_column="DEJ2000",
-            flux_columns="Si",
-            frame="fk5",
-        )
-    assert skyobj == skyobj3
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="frame parameter was not set. Defaulting to 'icrs'. This will become "
-        "an error in version 0.3",
-    ):
-        skyobj4 = SkyModel.from_votable_catalog(
-            votable_file, "VIII_1000_single", "source_id", "RAJ2000", "DEJ2000", "Si"
-        )
-    assert skyobj != skyobj4
-
-    new_skycoord = SkyCoord(
-        ra=skyobj4.skycoord.ra, dec=skyobj4.skycoord.dec, frame="fk5"
+    skyobj3 = SkyModel.from_file(
+        votable_file,
+        table_name="VIII_1000_single",
+        id_column="source_id",
+        lon_column="RAJ2000",
+        lat_column="DEJ2000",
+        flux_columns="Si",
+        frame="fk5",
     )
-    skyobj4.skycoord = new_skycoord
-    assert skyobj == skyobj4
+    assert skyobj == skyobj3
 
 
 def test_read_deprecated_votable():
     votable_file = os.path.join(SKY_DATA_PATH, "single_source_old.vot")
 
     skyobj = SkyModel()
     with pytest.raises(
         ValueError,
         match=re.escape(f"File {votable_file} contains tables with no name or ID."),
     ):
         skyobj.read_votable_catalog(
-            votable_file, "GLEAM", "GLEAM", "RAJ2000", "DEJ2000", "Fintwide"
+            votable_file,
+            "GLEAM",
+            "GLEAM",
+            "RAJ2000",
+            "DEJ2000",
+            "Fintwide",
+            frame="fk5",
         )
 
 
+@pytest.mark.filterwarnings("ignore:freq_edge_array not set, calculating it from")
+@pytest.mark.filterwarnings("ignore:freq_array not set, calculating it from")
 def test_read_votable_errors():
-
     # fmt: off
     flux_columns = [
         "Fint076", "Fint084", "Fint092", "Fint099", "Fint107",
         "Fint115", "Fint122", "Fint130", "Fint143", "Fint151",
         "Fint158", "Fint166", "Fint174", "Fint181", "Fint189",
         "Fint197", "Fint204", "Fint212", "Fint220", "Fint227"
     ]
     flux_error_columns = [
         "e_Fint076", "e_Fint084", "e_Fint092", "e_Fint099", "e_Fint107",
         "e_Fint115", "e_Fint122", "e_Fint130", "e_Fint143", "e_Fint151",
         "e_Fint158", "e_Fint166", "e_Fint174", "e_Fint181", "e_Fint189",
         "e_Fint197", "e_Fint204", "e_Fint212", "e_Fint220", "e_Fint227"
     ]
-    freq_array = [76, 84, 92, 99, 107, 115, 122, 130, 143, 151, 158, 166,
-                  174, 181, 189, 197, 204, 212, 220, 227]
+    freq_array = np.asarray(
+        [76, 84, 92, 99, 107, 115, 122, 130, 143, 151, 158, 166,
+         174, 181, 189, 197, 204, 212, 220, 227]
+    ) * 1e6 * units.Hz
+    freq_lower = np.asarray(
+        [72, 80, 88, 95, 103, 111, 118, 126, 139, 147, 154, 162,
+         170, 177, 185, 193, 200, 208, 216, 223]
+    ) * 1e6 * units.Hz
+    freq_upper = np.asarray(
+        [80, 88, 95, 103, 111, 118, 126, 134, 147, 154, 162, 170,
+         177, 185, 193, 200, 208, 216, 223, 231]
+    ) * 1e6 * units.Hz
+    freq_edge_array = np.concatenate(
+        (freq_lower[np.newaxis, :], freq_upper[np.newaxis, :]), axis=0,
+    )
     # fmt: on
     with pytest.raises(
-        ValueError, match="freq_array must be provided for multiple flux columns."
+        ValueError,
+        match="Frequency information must be provided with multiple flux columns.",
     ):
         SkyModel.from_file(
             GLEAM_vot,
             filetype="vot",
             table_name="GLEAM",
             id_column="GLEAM",
             lon_column="RAJ2000",
             lat_column="DEJ2000",
             frame="fk5",
             flux_columns=flux_columns,
             reference_frequency=200e6 * units.Hz,
             flux_error_columns=flux_error_columns,
         )
 
-    with pytest.raises(
-        ValueError, match="reference_frequency must be an astropy Quantity."
-    ):
+    with pytest.raises(ValueError, match="All flux columns must have compatible units"):
         SkyModel.from_file(
             GLEAM_vot,
             filetype="vot",
             table_name="GLEAM",
             id_column="GLEAM",
             lon_column="RAJ2000",
             lat_column="DEJ2000",
             frame="fk5",
-            flux_columns="Fintwide",
-            reference_frequency=200e6,
-            flux_error_columns="e_Fintwide",
+            flux_columns=["Fintwide", "Fpwide"],
+            freq_array=[150e6, 200e6] * units.Hz,
         )
 
-    with pytest.raises(ValueError, match="All flux columns must have compatible units"):
+    with pytest.raises(
+        ValueError,
+        match="freq_edge_array must be provided for multiple flux columns if "
+        "freq_array is not regularly spaced.",
+    ):
         SkyModel.from_file(
             GLEAM_vot,
             filetype="vot",
             table_name="GLEAM",
             id_column="GLEAM",
             lon_column="RAJ2000",
             lat_column="DEJ2000",
             frame="fk5",
-            flux_columns=["Fintwide", "Fpwide"],
-            freq_array=[150e6, 200e6] * units.Hz,
+            flux_columns=flux_columns,
+            flux_error_columns=flux_error_columns,
+            freq_array=freq_array,
         )
 
     flux_error_columns[0] = "e_Fp076"
     with pytest.raises(
         ValueError, match="All flux error columns must have units compatible with"
     ):
         SkyModel.from_file(
@@ -2843,15 +2680,15 @@
             table_name="GLEAM",
             id_column="GLEAM",
             lon_column="RAJ2000",
             lat_column="DEJ2000",
             frame="fk5",
             flux_columns=flux_columns,
             flux_error_columns=flux_error_columns,
-            freq_array=freq_array,
+            freq_edge_array=freq_edge_array,
         )
 
 
 def test_fhd_catalog_reader():
     catfile = os.path.join(SKY_DATA_PATH, "fhd_catalog.sav")
 
     with uvtest.check_warnings(
@@ -2860,43 +2697,14 @@
         skyobj = SkyModel.from_fhd_catalog(catfile, expand_extended=False)
 
     assert skyobj.filename == ["fhd_catalog.sav"]
     catalog = scipy.io.readsav(catfile)["catalog"]
     assert skyobj.Ncomponents == len(catalog)
 
 
-def test_fhd_catalog_reader_source_cuts():
-    catfile = os.path.join(SKY_DATA_PATH, "fhd_catalog.sav")
-
-    with uvtest.check_warnings(
-        UserWarning, match="Source IDs are not unique. Defining unique IDs."
-    ):
-        skyobj = SkyModel.from_file(catfile, expand_extended=False, filetype="fhd")
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="The `source_cuts` method is deprecated and will be removed",
-    ):
-        skyobj.source_cuts(latitude_deg=30.0)
-
-    with uvtest.check_warnings(
-        [UserWarning, DeprecationWarning, DeprecationWarning],
-        match=[
-            "Source IDs are not unique. Defining unique IDs.",
-            "The source_select_kwds parameter is deprecated",
-            "The `source_cuts` method is deprecated",
-        ],
-    ):
-        skyobj2 = SkyModel.from_fhd_catalog(
-            catfile, expand_extended=False, source_select_kwds={"latitude_deg": 30.0}
-        )
-
-    assert skyobj == skyobj2
-
-
 def test_fhd_catalog_reader_extended_sources():
     catfile = os.path.join(SKY_DATA_PATH, "fhd_catalog.sav")
     skyobj = SkyModel()
     with uvtest.check_warnings(
         UserWarning, match="Source IDs are not unique. Defining unique IDs."
     ):
         skyobj.read_fhd_catalog(catfile, expand_extended=True)
@@ -2991,28 +2799,14 @@
     assert sorted(skyobj.name) == sorted(catalog_table["source_id"])
     assert np.allclose(skyobj.skycoord.ra.deg, catalog_table["ra_j2000"])
     assert np.allclose(skyobj.skycoord.dec.deg, catalog_table["dec_j2000"])
     assert np.allclose(
         skyobj.stokes[0, :].to("Jy").value, catalog_table["flux_density"]
     )
 
-    # Check cuts
-    source_select_kwds = {"min_flux": 1.0}
-
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match=[
-            "The source_select_kwds parameter is deprecated",
-            "The `source_cuts` method is deprecated and will be removed",
-        ],
-    ):
-        skyobj2 = SkyModel()
-        skyobj2.read_text_catalog(catfile, source_select_kwds=source_select_kwds)
-    assert skyobj2.Ncomponents == 2
-
 
 @pytest.mark.filterwarnings("ignore:recarray flux columns will no longer be labeled")
 @pytest.mark.parametrize(
     "frame",
     [
         "icrs",
         "fk5",
@@ -3065,23 +2859,38 @@
     _, array_location = time_location
     spectral_type = "subband" if spec_type == "full" else spec_type
 
     skyobj = SkyModel.from_file(
         GLEAM_vot, spectral_type=spectral_type, with_error=with_error
     )
     if spec_type == "full":
-        skyobj.spectral_type = "full"
+        skyobj.at_frequencies(skyobj.freq_array)
+        skyobj.freq_edge_array = None
 
     if rise_set_lsts:
         skyobj.calculate_rise_set_lsts(array_location.lat)
 
     fname = os.path.join(tmp_path, "temp_cat.txt")
 
-    skyobj.write_text_catalog(fname)
+    if spec_type == "subband":
+        msg = (
+            "Text files do not support subband types, this will be written as a "
+            "'full' spectral type (losing the frequency edge array information)."
+        )
+        warn_type = UserWarning
+    else:
+        warn_type = None
+        msg = ""
+
+    with uvtest.check_warnings(warn_type, match=msg):
+        skyobj.write_text_catalog(fname)
     skyobj2 = SkyModel.from_file(fname)
+    if spec_type == "subband":
+        assert skyobj2.spectral_type == "full"
+        skyobj.at_frequencies(skyobj.freq_array)
 
     assert skyobj == skyobj2
 
     if spec_type == "flat":
         # again with no reference_frequency field
         reference_frequency = skyobj.reference_frequency
         skyobj.reference_frequency = None
@@ -3109,22 +2918,30 @@
     skyobj.write_text_catalog(fname)
     skyobj2 = SkyModel.from_file(fname, filetype="text")
     os.remove(fname)
 
     assert skyobj == skyobj2
 
 
-def test_write_text_catalog_healpix_error(tmp_path, healpix_disk_new):
+def test_write_text_catalog_errors(tmp_path, healpix_disk_new):
     fname = os.path.join(tmp_path, "temp_cat.txt")
 
     with pytest.raises(
         ValueError, match="component_type must be 'point' to use this method."
     ):
         healpix_disk_new.write_text_catalog(fname)
 
+    skyobj = SkyModel.from_file(GLEAM_vot)
+    skyobj.jansky_to_kelvin()
+
+    with pytest.raises(
+        ValueError, match="Stokes units must be equivalent to Jy to use this method."
+    ):
+        skyobj.write_text_catalog(fname)
+
 
 @pytest.mark.parametrize(
     ("old_str", "new_str", "err_msg"),
     [
         ("icrs", "foo", "frame not recognized from coordinate column"),
         ("ra", "foo", "Longitudinal component column not identified."),
         ("dec", "foo", "Latitudinal component column not identified."),
@@ -3165,81 +2982,57 @@
         fo.write(header)
         fo.write(str(catalog_table[0]))
 
     with pytest.raises(ValueError, match=err_msg):
         SkyModel.from_text_catalog(fname)
 
 
-@pytest.mark.filterwarnings("ignore:The reference_frequency is aliased as `frequency`")
-@pytest.mark.filterwarnings("ignore:recarray flux columns will no longer be labeled")
-@pytest.mark.parametrize("spec_type", ["flat", "subband"])
-def test_read_text_source_cuts(tmp_path, spec_type):
-
-    skyobj = SkyModel.from_file(GLEAM_vot, spectral_type=spec_type, with_error=True)
-    fname = os.path.join(tmp_path, "temp_cat.txt")
-    skyobj.write_text_catalog(fname)
-
-    source_select_kwds = {"min_flux": 0.5}
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match=[
-            "The source_select_kwds parameter is deprecated",
-            "The `source_cuts` method is deprecated",
-        ],
-    ):
-        skyobj2 = SkyModel.from_text_catalog(
-            fname, source_select_kwds=source_select_kwds
-        )
-
-    assert skyobj2.Ncomponents < skyobj.Ncomponents
-
-
 def test_pyuvsim_mock_catalog_read():
     mock_cat_file = os.path.join(SKY_DATA_PATH, "mock_hera_text_2458098.27471.txt")
 
     mock_sky = SkyModel.from_file(mock_cat_file)
     expected_names = ["src" + str(val) for val in np.arange(mock_sky.Ncomponents)]
     assert mock_sky.name.tolist() == expected_names
 
 
-@pytest.mark.filterwarnings("ignore:recarray flux columns will no longer be labeled")
 def test_read_text_errors(tmp_path):
     skyobj = SkyModel.from_file(GLEAM_vot, spectral_type="subband", with_error=True)
+    skyobj.at_frequencies(skyobj.freq_array)
 
     fname = os.path.join(tmp_path, "temp_cat.txt")
     skyobj.write_text_catalog(fname)
     with fileinput.input(files=fname, inplace=True) as infile:
         for line in infile:
-            line = line.replace("Flux_subband_76_MHz [Jy]", "Frequency [Hz]")
+            line = line.replace("Flux_76_MHz [Jy]", "Frequency [Hz]")
             print(line, end="")
 
     with pytest.raises(
         ValueError,
         match="Number of flux error fields does not match number of flux fields.",
     ):
         SkyModel.from_file(fname)
 
     skyobj2 = skyobj.copy()
     skyobj2.stokes_error = None
     skyobj2.write_text_catalog(fname)
     with fileinput.input(files=fname, inplace=True) as infile:
         for line in infile:
-            line = line.replace("Flux_subband_76_MHz [Jy]", "Frequency [Hz]")
+            line = line.replace("Flux_76_MHz [Jy]", "Frequency [Hz]")
             print(line, end="")
 
     with pytest.raises(
         ValueError,
         match="If frequency column is present, only one flux column allowed.",
     ):
         SkyModel.from_file(fname)
 
     skyobj.write_text_catalog(fname)
     with fileinput.input(files=fname, inplace=True) as infile:
         for line in infile:
-            line = line.replace("Flux_subband_76_MHz [Jy]", "Flux [Jy]")
+            line = line.replace("Flux_76_MHz [Jy]", "Flux [Jy]")
             print(line, end="")
 
     with pytest.raises(
         ValueError,
         match="Multiple flux fields, but they do not all contain a frequency.",
     ):
         SkyModel.from_file(fname)
@@ -3288,15 +3081,14 @@
     maxf = _freqs[np.argmax(np.abs(_els[_freqs > 0]) ** 2)]
     assert np.isclose(maxf, f_28d, atol=2 / ets[-1])
 
 
 @pytest.mark.parametrize("inplace", [True, False])
 @pytest.mark.parametrize("stype", ["full", "subband", "spectral_index", "flat"])
 def test_at_frequencies(mock_point_skies, inplace, stype):
-
     sind = mock_point_skies("spectral_index")
     alpha = sind.spectral_index[0]
 
     Nfreqs_fine = 50
     fine_freqs = np.linspace(100e6, 130e6, Nfreqs_fine) * units.Hz
     fine_spectrum = (fine_freqs / fine_freqs[0]) ** (alpha) * units.Jy
 
@@ -3305,14 +3097,18 @@
     old_freqs = oldsky.freq_array
     if stype == "full":
         with pytest.raises(ValueError, match="Some requested frequencies"):
             sky.at_frequencies(fine_freqs, inplace=inplace)
         new = sky.at_frequencies(old_freqs, inplace=inplace)
         if inplace:
             new = sky
+            new.freq_edge_array = skymodel._get_freq_edges_from_centers(
+                new.freq_array, new._freq_array.tols
+            )
+
         assert units.quantity.allclose(new.freq_array, old_freqs)
         new = sky.at_frequencies(old_freqs[5:10], inplace=inplace)
         if inplace:
             new = sky
         assert units.quantity.allclose(new.freq_array, old_freqs[5:10])
     else:
         # Evaluate new frequencies, and confirm the new spectrum is correct.
@@ -3323,15 +3119,14 @@
         assert new.spectral_type == "full"
 
         if stype != "flat":
             assert units.quantity.allclose(new.stokes[0, :, 0], fine_spectrum)
 
 
 def test_at_frequencies_interp_errors(mock_point_skies):
-
     sky = mock_point_skies("subband")
 
     # Check for error if interpolating outside the defined range.
     with pytest.raises(
         ValueError,
         match="A requested frequency is larger than the highest subband frequency.",
     ):
@@ -3752,29 +3547,33 @@
 @pytest.mark.parametrize(
     "param,value,errormsg",
     [
         ("name", None, "Expected parameter name is missing in file"),
         ("Ncomponents", 5, "Ncomponents is not equal to the size of 'name'."),
         ("Nfreqs", 10, "Nfreqs is not equal to the size of 'freq_array'."),
         ("skycoord", None, "No component location information found in file."),
+        ("Header", None, "This is not a proper skyh5 file."),
     ],
 )
 def test_skyh5_read_errors(mock_point_skies, param, value, errormsg, tmpdir):
     sky = mock_point_skies("full")
 
     testfile = str(tmpdir.join("testfile.skyh5"))
     sky.write_skyh5(testfile)
 
     with h5py.File(testfile, "r+") as fileobj:
-        param_loc = "/Header/" + param
-        if value is None:
-            del fileobj[param_loc]
+        if param == "Header":
+            del fileobj["Header"]
         else:
-            data = fileobj[param_loc]
-            data[...] = value
+            param_loc = "/Header/" + param
+            if value is None:
+                del fileobj[param_loc]
+            else:
+                data = fileobj[param_loc]
+                data[...] = value
 
     with pytest.raises(ValueError, match=errormsg):
         SkyModel.from_file(testfile)
 
 
 @pytest.mark.parametrize(
     "param,value,errormsg",
@@ -3798,28 +3597,14 @@
             data = fileobj[param_loc]
             data[...] = value
 
     with pytest.raises(ValueError, match=errormsg):
         SkyModel.from_file(testfile)
 
 
-def test_skyh5_read_errors_oldstyle_healpix():
-    with pytest.raises(
-        ValueError, match="This is an old 'healvis' style healpix HDF5 file"
-    ):
-        SkyModel.from_file(
-            os.path.join(SKY_DATA_PATH, "healpix_disk.hdf5"), filetype="skyh5"
-        )
-
-
-def test_healpix_hdf5_read_errors_newstyle_healpix():
-    with pytest.raises(ValueError, match="This is a skyh5 file"):
-        SkyModel.from_healpix_hdf5(os.path.join(SKY_DATA_PATH, "healpix_disk.skyh5"))
-
-
 def test_hpx_ordering():
     # Setting the hpx_order parameter
     pytest.importorskip("astropy_healpix")
     nside = 16
     npix = 12 * nside**2
     stokes = np.zeros((4, 1, npix)) * units.K
 
@@ -3881,20 +3666,33 @@
     sky.write_skyh5(testfile, clobber=True)
     sky3 = SkyModel.from_file(testfile)
 
     assert sky3 == sky
     assert sky3 != sky2
 
 
-# TODO -- Also check with healpix init
 @pytest.mark.parametrize(
     ("coord_kwds", "err_msg", "exp_frame"),
     [
-        ({"ra": Longitude("1d"), "dec": Latitude("1d")}, None, "icrs"),
-        ({"gl": Longitude("1d"), "gb": Latitude("1d")}, None, "galactic"),
+        (
+            {"ra": Longitude("1d"), "dec": Latitude("1d")},
+            "The 'frame' keyword must be set to initialize from coordinates.",
+            "icrs",
+        ),
+        (
+            {"gl": Longitude("1d"), "gb": Latitude("1d")},
+            "The 'frame' keyword must be set to initialize from coordinates.",
+            "galactic",
+        ),
+        ({"ra": Longitude("1d"), "dec": Latitude("1d"), "frame": "icrs"}, None, "icrs"),
+        (
+            {"gl": Longitude("1d"), "gb": Latitude("1d"), "frame": "galactic"},
+            None,
+            "galactic",
+        ),
         (
             {"ra": Longitude("1d"), "dec": Latitude("1d"), "frame": "galactic"},
             "ra or dec supplied but specified frame galactic does "
             "not support ra and dec coordinates.",
             None,
         ),
         (
@@ -3925,47 +3723,50 @@
             None,
         ),
         (
             {"lon": Longitude("1d"), "lat": Latitude("1d"), "frame": None},
             "The 'frame' keyword must",
             None,
         ),
-        ({"nside": 4, "hpx_inds": np.arange(1)}, None, "icrs"),
+        (
+            {"nside": 4, "hpx_inds": np.arange(1)},
+            "If initializing with values, all of ['nside', 'frame', 'hpx_inds', 'stokes', "
+            "'spectral_type'] must be set. Received: ['nside', 'hpx_inds', 'stokes', "
+            "'spectral_type']",
+            "icrs",
+        ),
+        ({"nside": 4, "hpx_inds": np.arange(1), "frame": "icrs"}, None, "icrs"),
     ],
 )
 def test_skymodel_init_with_frame(coord_kwds, err_msg, exp_frame):
     stokes = np.zeros((4, 1, 1)) * units.Jy
 
     if "nside" in coord_kwds.keys():
         pytest.importorskip("astropy_healpix")
         stokes = stokes / units.sr
     names = ["src"]
     coord_kwds["name"] = names
     coord_kwds["stokes"] = stokes
     coord_kwds["spectral_type"] = "flat"
 
     if err_msg is not None:
-        with pytest.raises(ValueError, match=err_msg):
+        with pytest.raises(ValueError, match=re.escape(err_msg)):
             SkyModel(**coord_kwds)
     else:
         msg = ""
         if "frame" not in coord_kwds.keys():
             exp_warning = DeprecationWarning
         else:
             exp_warning = None
         if "ra" in coord_kwds.keys():
             msg = (
                 "No frame was specified for RA and Dec. Defaulting to ICRS, but "
                 "this will become an error in version 0.3 and later."
             )
-        elif "gl" in coord_kwds.keys():
-            msg = (
-                "No frame was specified for gl and gb. Defaulting to galactic, but "
-                "this will become an error in version 0.3 and later."
-            )
+
         with uvtest.check_warnings(exp_warning, match=msg):
             sky = SkyModel(**coord_kwds)
         assert sky.frame == exp_frame
         lon, lat = sky.get_lon_lat()
 
         if "nside" in coord_kwds.keys():
             exp_warning = UserWarning
@@ -3982,51 +3783,33 @@
                 assert lon == sky.l
                 assert lat == sky.b
             if exp_frame == "icrs":
                 assert lon == sky.ra
                 assert lat == sky.dec
 
 
-# This filter can be removed when lunarsky is updated to not trigger this
-# astropy deprecation warning.
-@pytest.mark.filterwarnings("ignore:The get_frame_attr_names")
 def test_skymodel_tranform_frame(zenith_skymodel, zenith_skycoord):
     zenith_skymodel.transform_to("galactic")
     zenith_skycoord = zenith_skycoord.transform_to("galactic")
 
     assert zenith_skymodel.skycoord.frame.name == "galactic"
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="gl and gb are no longer parameters on SkyModel objects in the "
-        "galactic frame. Use the standard astropy labels l and b instead. Starting in "
-        "version 0.3.0 this call will error.",
-    ):
-        assert units.allclose(zenith_skymodel.gl, zenith_skycoord.l)
+    assert units.allclose(zenith_skymodel.l, zenith_skycoord.l)
 
     assert units.allclose(zenith_skymodel.b, zenith_skycoord.b)
 
 
-# This filter can be removed when lunarsky is updated to not trigger this
-# astropy deprecation warning.
-@pytest.mark.filterwarnings("ignore:The get_frame_attr_names")
 def test_skymodel_tranform_frame_roundtrip(zenith_skymodel, zenith_skycoord):
     original_sky = copy.deepcopy(zenith_skymodel)
 
     zenith_skymodel.transform_to("galactic")
     zenith_skycoord = zenith_skycoord.transform_to("galactic")
 
     assert zenith_skymodel.skycoord.frame.name == "galactic"
     assert units.allclose(zenith_skymodel.l, zenith_skycoord.l)
-    with uvtest.check_warnings(
-        DeprecationWarning,
-        match="gl and gb are no longer parameters on SkyModel objects in the "
-        "galactic frame. Use the standard astropy labels l and b instead. Starting in "
-        "version 0.3.0 this call will error.",
-    ):
-        assert units.allclose(zenith_skymodel.gb, zenith_skycoord.b)
+    assert units.allclose(zenith_skymodel.b, zenith_skycoord.b)
     zenith_skymodel.transform_to("icrs")
 
     assert zenith_skymodel == original_sky
 
 
 def test_skymodel_transform_healpix_error(healpix_disk_new):
     pytest.importorskip("astropy_healpix")
@@ -4153,11 +3936,17 @@
     # make sure we got a full sky map back
     assert healpix_disk_new.Ncomponents == hp_obj.npix
 
 
 def test_old_skyh5_reading_ra_dec():
     testfile = os.path.join(SKY_DATA_PATH, "old_skyh5_point_sources.skyh5")
     with uvtest.check_warnings(
-        UserWarning, match="Parameter skycoord not found in skyh5 file."
+        UserWarning,
+        match=[
+            "Parameter skycoord not found in skyh5 file.",
+            "No freq_edge_array in this file and frequencies are not evenly spaced",
+        ],
     ):
         sky = SkyModel.from_file(testfile)
-    assert sky.check()
+
+    sky.check()
+    assert sky.spectral_type == "full"
```

### Comparing `pyradiosky-0.2.0/pyradiosky/tests/test_spherical_coords_transforms.py` & `pyradiosky-0.3.0/pyradiosky/tests/test_spherical_coords_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from scipy.linalg import orthogonal_procrustes as ortho_procr
 
 from pyradiosky import spherical_coords_transforms as sct
 
 
 @pytest.mark.parametrize("func_name", ["r_hat", "theta_hat", "phi_hat"])
 def test_hat_errors(func_name):
-
     with pytest.raises(ValueError) as cm:
         getattr(sct, func_name)([0, 0], [0])
     assert str(cm.value).startswith("theta and phi must have the same shape")
 
 
 def test_rotate_points_3d():
     array_location = EarthLocation(lat="-30d43m17.5s", lon="21d25m41.9s", height=1073.0)
```

### Comparing `pyradiosky-0.2.0/pyradiosky/tests/test_utils.py` & `pyradiosky-0.3.0/pyradiosky/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     tee_ra = Angle(np.pi / 4.0, unit="rad")  # rad
     cirs_ra = skyutils._tee_to_cirs_ra(tee_ra, time)
     new_tee_ra = skyutils._cirs_to_tee_ra(cirs_ra, time)
     assert new_tee_ra == tee_ra
 
 
 def test_stokes_tofrom_coherency():
-
     stokesI = 4.5
     stokesQ = -0.3
     stokesU = 1.2
     stokesV = -0.15
     stokes = np.array([stokesI, stokesQ, stokesU, stokesV])
 
     expected_coherency = (
```

### Comparing `pyradiosky-0.2.0/pyradiosky/utils.py` & `pyradiosky-0.3.0/pyradiosky/utils.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/pyradiosky.egg-info/PKG-INFO` & `pyradiosky-0.3.0/pyradiosky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyradiosky
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python objects and interfaces for representing diffuse, extended and compact astrophysical radio sources
 Home-page: https://github.com/RadioAstronomySoftwareGroup/pyradiosky
 Author: Radio Astronomy Software Group
 License: BSD
 Keywords: radio astronomy
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -82,15 +82,15 @@
 * pyuvdata>=2.2.10
 * setuptools_scm>=7.0.3
 
 Optional:
 
 * astropy-healpix>=0.6 (for working with beams in HEALPix formats)
 * astroquery>=0.4.4 (for downloading GLEAM and other VizieR catalogs)
-* lunarsky>=0.1.2 (for supporting telescope locations on the moon)
+* lunarsky>=0.2.1 (for supporting telescope locations on the moon)
 
 We suggest using conda to install all the dependencies. To install
 pyuvdata, astropy-healpix and astroquery, you'll need to add conda-forge as a channel
 (```conda config --add channels conda-forge```).
 
 If you do not want to use conda, the packages are also available on PyPI.
 You can install the optional dependencies via pip by specifying an option
```

### Comparing `pyradiosky-0.2.0/pyradiosky.egg-info/SOURCES.txt` & `pyradiosky-0.3.0/pyradiosky.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 pyradiosky/data/__init__.py
 pyradiosky/data/extended_source_test.sav
 pyradiosky/data/fhd_catalog.sav
 pyradiosky/data/fhd_catalog_with_beam_values.sav
 pyradiosky/data/gleam_50srcs.vot
 pyradiosky/data/gsm_galactic.skyh5
 pyradiosky/data/gsm_icrs.skyh5
-pyradiosky/data/healpix_disk.hdf5
 pyradiosky/data/healpix_disk.skyh5
 pyradiosky/data/mock_hera_text_2458098.27471.txt
 pyradiosky/data/old_skyh5_point_sources.skyh5
 pyradiosky/data/pointsource_catalog.txt
 pyradiosky/data/simple_test.vot
 pyradiosky/data/single_source_old.vot
 pyradiosky/tests/conftest.py
```

### Comparing `pyradiosky-0.2.0/scripts/download_gleam.py` & `pyradiosky-0.3.0/scripts/download_gleam.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/scripts/make_flat_spectrum_eor.py` & `pyradiosky-0.3.0/scripts/make_flat_spectrum_eor.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.2.0/setup.py` & `pyradiosky-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,21 +37,21 @@
         "h5py>=3.1",
         "pyuvdata>=2.2.10",
         "setuptools_scm>=7.0.3",
     ],
     "extras_require": {
         "healpix": ["astropy-healpix>=0.6"],
         "astroquery": ["astroquery>=0.4.4"],
-        "lunarsky": ["lunarsky>=0.1.2"],
+        "lunarsky": ["lunarsky>=0.2.1"],
         "all": ["astropy-healpix", "astroquery"],
         "doc": ["sphinx", "pypandoc"],
         "dev": [
             "astropy-healpix",
             "astroquery",
-            "lunarsky",
+            "lunarsky>=0.2.1",
             "pytest",
             "pre-commit",
             "sphinx",
             "pypandoc",
         ],
     },
     "classifiers": [
```

