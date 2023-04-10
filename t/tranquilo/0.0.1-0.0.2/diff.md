# Comparing `tmp/tranquilo-0.0.1.tar.gz` & `tmp/tranquilo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tranquilo-0.0.1.tar", last modified: Sun Apr  9 17:45:05 2023, max compression
+gzip compressed data, was "tranquilo-0.0.2.tar", last modified: Mon Apr 10 09:14:49 2023, max compression
```

## Comparing `tranquilo-0.0.1.tar` & `tranquilo-0.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.460150 tranquilo-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.440149 tranquilo-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.444149 tranquilo-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-09 17:44:54.000000 tranquilo-0.0.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-09 17:44:54.000000 tranquilo-0.0.1/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-09 17:44:54.000000 tranquilo-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.444149 tranquilo-0.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-09 17:44:54.000000 tranquilo-0.0.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.444149 tranquilo-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 17:44:54.000000 tranquilo-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-09 17:44:54.000000 tranquilo-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-09 17:44:54.000000 tranquilo-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 17:44:54.000000 tranquilo-0.0.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-09 17:44:54.000000 tranquilo-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-09 17:44:54.000000 tranquilo-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-09 17:44:54.000000 tranquilo-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-09 17:45:05.460150 tranquilo-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-09 17:44:54.000000 tranquilo-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-09 17:44:54.000000 tranquilo-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-09 17:45:05.460150 tranquilo-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-09 17:44:54.000000 tranquilo-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.440149 tranquilo-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.452149 tranquilo-0.0.1/src/tranquilo/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 17:45:05.000000 tranquilo-0.0.1/src/tranquilo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/acceptance_decision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/acceptance_sample_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/adjust_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/aggregate_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/estimate_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/exploration_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/filter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/fit_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/get_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/handle_infinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/poisedness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/process_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/rho_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/sample_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/solve_subproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.460150 tranquilo-0.0.1/src/tranquilo/subsolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/_conjugate_gradient_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/_steihaug_toint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/_steihaug_toint_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/_trsbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/_trsbox_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    30890 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/bntr.py
--rw-r--r--   0 runner    (1001) docker     (123)    39169 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/bntr_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/gqtpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/gqtpar_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/linear_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/subsolvers/wrapped_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/tranquilo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19526 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/weighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-09 17:44:54.000000 tranquilo-0.0.1/src/tranquilo/wrap_criterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:45:05.456150 tranquilo-0.0.1/src/tranquilo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-09 17:45:05.000000 tranquilo-0.0.1/src/tranquilo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-09 17:45:05.000000 tranquilo-0.0.1/src/tranquilo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:45:05.000000 tranquilo-0.0.1/src/tranquilo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:45:05.000000 tranquilo-0.0.1/src/tranquilo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-09 17:45:05.000000 tranquilo-0.0.1/src/tranquilo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 17:45:05.000000 tranquilo-0.0.1/src/tranquilo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.650888 tranquilo-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.638887 tranquilo-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.642887 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.642887 tranquilo-0.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.642887 tranquilo-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-10 09:14:35.000000 tranquilo-0.0.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-10 09:14:35.000000 tranquilo-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 09:14:35.000000 tranquilo-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-10 09:14:35.000000 tranquilo-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 09:14:49.650888 tranquilo-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-10 09:14:35.000000 tranquilo-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-10 09:14:35.000000 tranquilo-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-10 09:14:49.650888 tranquilo-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 09:14:35.000000 tranquilo-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.638887 tranquilo-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.646888 tranquilo-0.0.2/src/tranquilo/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/acceptance_decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/acceptance_sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/adjust_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/aggregate_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/estimate_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/exploration_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/filter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/fit_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/get_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/handle_infinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/poisedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/process_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/rho_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/sample_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/solve_subproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.646888 tranquilo-0.0.2/src/tranquilo/subsolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30890 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/bntr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39169 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/bntr_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/linear_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/wrapped_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/tranquilo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19526 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/weighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/wrap_criterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.646888 tranquilo-0.0.2/src/tranquilo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/top_level.txt
```

### Comparing `tranquilo-0.0.1/.github/ISSUE_TEMPLATE/bug-report.md` & `tranquilo-0.0.2/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/.github/ISSUE_TEMPLATE/enhancement.md` & `tranquilo-0.0.2/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `tranquilo-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/.github/workflows/main.yml` & `tranquilo-0.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/.github/workflows/publish-to-pypi.yml` & `tranquilo-0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/.gitignore` & `tranquilo-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/CODE_OF_CONDUCT.md` & `tranquilo-0.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/LICENSE` & `tranquilo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/MANIFEST.in` & `tranquilo-0.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/PKG-INFO` & `tranquilo-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tranquilo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Trust-region optimizer for scalar, least-square and noisy problems
 Home-page: https://github.com/OpenSourceEconomics/tranquilo
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
-Keywords: econometrics,statistics,estimation,extremum estimation,optimization,inference,numerical differentiation,finite differences,richardson extrapolation,derivative free optimization,method of simulated moments,maximum likelihood
-Classifier: Development Status :: 4 - Beta
+Keywords: optimization,dfo,derivative free optimization,noisy optimization,parallel optimization,numerical optimization
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `tranquilo-0.0.1/README.md` & `tranquilo-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/pyproject.toml` & `tranquilo-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/setup.cfg` & `tranquilo-0.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -5,43 +5,39 @@
 long_description_content_type = text/markdown
 url = https://github.com/OpenSourceEconomics/tranquilo
 author = Janos Gabler
 author_email = janos.gabler@gmail.com
 license = MIT
 license_file = LICENSE
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Scientific/Engineering
 keywords = 
-	econometrics
-	statistics
-	estimation
-	extremum estimation
 	optimization
-	inference
-	numerical differentiation
-	finite differences
-	richardson extrapolation
+	dfo
 	derivative free optimization
-	method of simulated moments
-	maximum likelihood
+	noisy optimization
+	parallel optimization
+	numerical optimization
 
 [options]
 packages = find:
 install_requires = 
+	estimagic>=0.4.2
 	numba
 	numpy>=1.17.0
 	pandas
+	plotly
 	scipy>=1.2.1
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
```

### Comparing `tranquilo-0.0.1/src/tranquilo/acceptance_decision.py` & `tranquilo-0.0.2/src/tranquilo/acceptance_decision.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/acceptance_sample_size.py` & `tranquilo-0.0.2/src/tranquilo/acceptance_sample_size.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/adjust_radius.py` & `tranquilo-0.0.2/src/tranquilo/adjust_radius.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/aggregate_models.py` & `tranquilo-0.0.2/src/tranquilo/aggregate_models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/bounds.py` & `tranquilo-0.0.2/src/tranquilo/bounds.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/clustering.py` & `tranquilo-0.0.2/src/tranquilo/clustering.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/config.py` & `tranquilo-0.0.2/src/tranquilo/config.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/estimate_variance.py` & `tranquilo-0.0.2/src/tranquilo/estimate_variance.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/exploration_sample.py` & `tranquilo-0.0.2/src/tranquilo/exploration_sample.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/filter_points.py` & `tranquilo-0.0.2/src/tranquilo/filter_points.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/fit_models.py` & `tranquilo-0.0.2/src/tranquilo/fit_models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/geometry.py` & `tranquilo-0.0.2/src/tranquilo/geometry.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/get_component.py` & `tranquilo-0.0.2/src/tranquilo/get_component.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/handle_infinity.py` & `tranquilo-0.0.2/src/tranquilo/handle_infinity.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/history.py` & `tranquilo-0.0.2/src/tranquilo/history.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/models.py` & `tranquilo-0.0.2/src/tranquilo/models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/options.py` & `tranquilo-0.0.2/src/tranquilo/options.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/poisedness.py` & `tranquilo-0.0.2/src/tranquilo/poisedness.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/process_arguments.py` & `tranquilo-0.0.2/src/tranquilo/process_arguments.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/region.py` & `tranquilo-0.0.2/src/tranquilo/region.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/rho_noise.py` & `tranquilo-0.0.2/src/tranquilo/rho_noise.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/sample_points.py` & `tranquilo-0.0.2/src/tranquilo/sample_points.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/solve_subproblem.py` & `tranquilo-0.0.2/src/tranquilo/solve_subproblem.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/_conjugate_gradient.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/_conjugate_gradient_fast.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/_steihaug_toint.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/_steihaug_toint_fast.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/_trsbox.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/_trsbox_fast.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/bntr.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/bntr.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/bntr_fast.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/bntr_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/gqtpar.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/gqtpar_fast.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/linear_subsolvers.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/linear_subsolvers.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/subsolvers/wrapped_subsolvers.py` & `tranquilo-0.0.2/src/tranquilo/subsolvers/wrapped_subsolvers.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/tranquilo.py` & `tranquilo-0.0.2/src/tranquilo/tranquilo.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/utilities.py` & `tranquilo-0.0.2/src/tranquilo/utilities.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/visualize.py` & `tranquilo-0.0.2/src/tranquilo/visualize.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/volume.py` & `tranquilo-0.0.2/src/tranquilo/volume.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/weighting.py` & `tranquilo-0.0.2/src/tranquilo/weighting.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo/wrap_criterion.py` & `tranquilo-0.0.2/src/tranquilo/wrap_criterion.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.1/src/tranquilo.egg-info/PKG-INFO` & `tranquilo-0.0.2/src/tranquilo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tranquilo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Trust-region optimizer for scalar, least-square and noisy problems
 Home-page: https://github.com/OpenSourceEconomics/tranquilo
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
-Keywords: econometrics,statistics,estimation,extremum estimation,optimization,inference,numerical differentiation,finite differences,richardson extrapolation,derivative free optimization,method of simulated moments,maximum likelihood
-Classifier: Development Status :: 4 - Beta
+Keywords: optimization,dfo,derivative free optimization,noisy optimization,parallel optimization,numerical optimization
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `tranquilo-0.0.1/src/tranquilo.egg-info/SOURCES.txt` & `tranquilo-0.0.2/src/tranquilo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

