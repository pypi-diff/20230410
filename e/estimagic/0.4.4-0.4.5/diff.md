# Comparing `tmp/estimagic-0.4.4.tar.gz` & `tmp/estimagic-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimagic-0.4.4.tar", last modified: Fri Feb 17 10:59:35 2023, max compression
+gzip compressed data, was "estimagic-0.4.5.tar", last modified: Mon Apr 10 11:40:41 2023, max compression
```

## Comparing `estimagic-0.4.4.tar` & `estimagic-0.4.5.tar`

### file list

```diff
@@ -1,190 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.509184 estimagic-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.485183 estimagic-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.489183 estimagic-0.4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-17 10:59:25.000000 estimagic-0.4.4/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-17 10:59:25.000000 estimagic-0.4.4/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-17 10:59:25.000000 estimagic-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.489183 estimagic-0.4.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-02-17 10:59:25.000000 estimagic-0.4.4/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.489183 estimagic-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-02-17 10:59:25.000000 estimagic-0.4.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-17 10:59:25.000000 estimagic-0.4.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-02-17 10:59:25.000000 estimagic-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-02-17 10:59:25.000000 estimagic-0.4.4/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-17 10:59:25.000000 estimagic-0.4.4/CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-02-17 10:59:25.000000 estimagic-0.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-17 10:59:25.000000 estimagic-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-17 10:59:25.000000 estimagic-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-02-17 10:59:35.509184 estimagic-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-02-17 10:59:25.000000 estimagic-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-02-17 10:59:25.000000 estimagic-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-02-17 10:59:35.513184 estimagic-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-17 10:59:25.000000 estimagic-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.485183 estimagic-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.493183 estimagic-0.4.4/src/estimagic/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-17 10:59:35.000000 estimagic-0.4.4/src/estimagic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/batch_evaluators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.493183 estimagic-0.4.4/src/estimagic/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46600 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/benchmarking/cartis_roberts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/benchmarking/get_benchmark_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/benchmarking/more_wild.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/benchmarking/noise_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/benchmarking/process_benchmark_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/benchmarking/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.493183 estimagic-0.4.4/src/estimagic/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/dashboard_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/plot_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/run_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/dashboard/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.497183 estimagic-0.4.4/src/estimagic/differentiation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/differentiation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42814 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/differentiation/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/differentiation/finite_differences.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/differentiation/generate_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/differentiation/richardson_extrapolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.497183 estimagic-0.4.4/src/estimagic/estimation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/estimation/estimate_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/estimation/estimate_msm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/estimation/estimation_summaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/estimation/msm_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.497183 estimagic-0.4.4/src/estimagic/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/criterion_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/db1.db
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/diabetes.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/exam_points.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/logit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/numdiff_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24256 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/examples/sensitivity_probit_example_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.497183 estimagic-0.4.4/src/estimagic/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/bootstrap_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/bootstrap_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/bootstrap_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/bootstrap_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/ml_covs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/msm_covs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/inference/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.501184 estimagic-0.4.4/src/estimagic/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/logging/create_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/logging/load_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/logging/read_from_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/logging/read_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/logging/write_to_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.501184 estimagic-0.4.4/src/estimagic/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/algo_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/bhhh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/check_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/convergence_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/cyipopt_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/error_penalty.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/fides_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/get_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/history_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/internal_criterion_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/nag_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/nlopt_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/optimization_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    44426 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/optimize_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/pounders.py
--rw-r--r--   0 runner    (1001) docker     (123)    28607 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/pounders_auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/process_multistart_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/process_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    38576 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/pygmo_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/scipy_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/simopt_optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.505184 estimagic-0.4.4/src/estimagic/optimization/subsolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/_conjugate_gradient_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/_steihaug_toint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/_steihaug_toint_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/_trsbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/_trsbox_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    30881 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/bntr.py
--rw-r--r--   0 runner    (1001) docker     (123)    38900 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/bntr_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/gqtpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/gqtpar_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/subsolvers/linear_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tao_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19712 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tiktak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.505184 estimagic-0.4.4/src/estimagic/optimization/tranquilo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/adjust_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/aggregate_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/count_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/filter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/fit_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/get_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/handle_infinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/poisedness.py
--rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/sample_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/solve_subproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/thourough_subsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/tranquilo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/tranquilo_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/weighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/optimization/tranquilo/wrap_criterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.509184 estimagic-0.4.4/src/estimagic/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/block_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/check_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/consolidate_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/constraint_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/kernel_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/nonlinear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/parameter_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/parameter_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/process_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/process_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/scale_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19169 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/space_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/tree_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/parameters/tree_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/process_user_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.509184 estimagic-0.4.4/src/estimagic/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/sensitivity/msm_sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.509184 estimagic-0.4.4/src/estimagic/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/shared/check_option_dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.509184 estimagic-0.4.4/src/estimagic/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/convergence_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/derivative_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    57698 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/estimation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/history_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/lollipop_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/plotting_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/profile_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/slice_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-02-17 10:59:25.000000 estimagic-0.4.4/src/estimagic/visualization/visualize_tranquilo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:35.493183 estimagic-0.4.4/src/estimagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-02-17 10:59:35.000000 estimagic-0.4.4/src/estimagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-02-17 10:59:35.000000 estimagic-0.4.4/src/estimagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 10:59:35.000000 estimagic-0.4.4/src/estimagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-17 10:59:35.000000 estimagic-0.4.4/src/estimagic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 10:59:34.000000 estimagic-0.4.4/src/estimagic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-17 10:59:35.000000 estimagic-0.4.4/src/estimagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-17 10:59:35.000000 estimagic-0.4.4/src/estimagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.663413 estimagic-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-10 11:40:30.000000 estimagic-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-04-10 11:40:30.000000 estimagic-0.4.5/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-10 11:40:30.000000 estimagic-0.4.5/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-10 11:40:30.000000 estimagic-0.4.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 11:40:30.000000 estimagic-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-10 11:40:30.000000 estimagic-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-10 11:40:41.687413 estimagic-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-10 11:40:30.000000 estimagic-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-10 11:40:30.000000 estimagic-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-10 11:40:41.687413 estimagic-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 11:40:30.000000 estimagic-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.663413 estimagic-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/src/estimagic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/batch_evaluators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129111 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/cartis_roberts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/get_benchmark_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/more_wild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/noise_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/process_benchmark_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/dashboard_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/plot_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/run_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/differentiation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42827 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/finite_differences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/generate_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/richardson_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/estimate_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/estimate_msm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/estimation_summaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/msm_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/criterion_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/diabetes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/exam_points.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/numdiff_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24256 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/sensitivity_probit_example_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.675413 estimagic-0.4.5/src/estimagic/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/ml_covs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/msm_covs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.675413 estimagic-0.4.5/src/estimagic/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/create_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/load_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/read_from_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/read_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/write_to_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.679413 estimagic-0.4.5/src/estimagic/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/algo_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/bhhh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/check_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/convergence_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/cyipopt_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/error_penalty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/fides_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/get_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/history_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/internal_criterion_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/nag_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/nlopt_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/optimization_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44428 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/optimize_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22737 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pounders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28651 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pounders_auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pounders_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/process_multistart_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38576 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pygmo_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/scipy_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/simopt_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.679413 estimagic-0.4.5/src/estimagic/optimization/subsolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_conjugate_gradient_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_steihaug_toint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_steihaug_toint_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_trsbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_trsbox_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30929 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/bntr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39208 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/bntr_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/gqtpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/gqtpar_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/linear_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tao_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tiktak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.683413 estimagic-0.4.5/src/estimagic/optimization/tranquilo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/acceptance_decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/acceptance_sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/adjust_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/aggregate_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/estimate_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/filter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/fit_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/get_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/handle_infinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/poisedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/process_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/rho_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/sample_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/solve_subproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/tranquilo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/weighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/wrap_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/wrapped_subsolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/block_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/check_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/consolidate_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/constraint_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/kernel_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/nonlinear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/parameter_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/parameter_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/process_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/process_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/scale_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19169 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/space_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/tree_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/tree_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/process_user_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/sensitivity/msm_sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/shared/check_option_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/convergence_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/derivative_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/deviation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58619 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/estimation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/history_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/lollipop_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/plotting_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/profile_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/slice_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/visualize_tranquilo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/src/estimagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/top_level.txt
```

### Comparing `estimagic-0.4.4/.github/ISSUE_TEMPLATE/bug-report.md` & `estimagic-0.4.5/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/.github/ISSUE_TEMPLATE/enhancement.md` & `estimagic-0.4.5/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md` & `estimagic-0.4.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/.github/workflows/main.yml` & `estimagic-0.4.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/.github/workflows/publish-to-pypi.yml` & `estimagic-0.4.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/.gitignore` & `estimagic-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/CHANGES.md` & `estimagic-0.4.5/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changes
 
 This is a record of all past estimagic releases and what went into them in reverse
 chronological order. We follow [semantic versioning](https://semver.org/) and all
 releases are available on [Anaconda.org](https://anaconda.org/OpenSourceEconomics/estimagic).
 
 
+## 0.4.5
+
+- {gh}`379` Improves the estimation table ({ghuser}`ChristianZimpelmann`)
+- {gh}`445` fixes line endings in local pre-commit hook ({ghuser}`ChristianZimpelmann`)
+- {gh}`443`, {gh}`444`, {gh}`445`, {gh}`446`, {gh}`448` and {gh}`449` are a major
+  refactoring of tranquilo ({ghuser}`timmens` and {ghuser}`janosg`)
+- {gh}`441` Adds an aggregated convergence plot for benchmarks ({ghuser}`mpetrosian`)
+- {gh}`435` Completes the cartis-roberts benchmark set ({ghuser}`segsell`)
+
 ## 0.4.4
 
 - {gh}`437` removes fuzzywuzzy as dependency ({ghuser}`aidatak97`)
 - {gh}`432` makes logging compatible with sqlalchemy 2.x ({ghuser}`janosg`)
 - {gh}`430` refactors the getter functions in Tranquilo ({ghuser}`janosg`)
 - {gh}`427` improves pre-commit setup ({ghuser}`timmens` and {ghuser}`hmgaudecker`)
 - {gh}`425` improves handling of notebooks in documentation ({ghuser}`baharcos`)
```

### Comparing `estimagic-0.4.4/CITATION` & `estimagic-0.4.5/CITATION`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/CODE_OF_CONDUCT.md` & `estimagic-0.4.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/LICENSE` & `estimagic-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/MANIFEST.in` & `estimagic-0.4.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/PKG-INFO` & `estimagic-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimagic
-Version: 0.4.4
+Version: 0.4.5
 Summary: Tools to solve difficult numerical optimization problems.
 Home-page: https://github.com/OpenSourceEconomics/estimagic
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: econometrics,statistics,estimation,extremum estimation,optimization,inference,numerical differentiation,finite differences,richardson extrapolation,derivative free optimization,method of simulated moments,maximum likelihood
 Classifier: Development Status :: 4 - Beta
```

### Comparing `estimagic-0.4.4/README.md` & `estimagic-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/setup.cfg` & `estimagic-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/__init__.py` & `estimagic-0.4.5/src/estimagic/__init__.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/batch_evaluators.py` & `estimagic-0.4.5/src/estimagic/batch_evaluators.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/benchmarking/get_benchmark_problems.py` & `estimagic-0.4.5/src/estimagic/benchmarking/get_benchmark_problems.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 from functools import partial
 
 import numpy as np
 
 from estimagic.benchmarking.cartis_roberts import CARTIS_ROBERTS_PROBLEMS
 from estimagic.benchmarking.more_wild import MORE_WILD_PROBLEMS
 from estimagic.benchmarking.noise_distributions import NOISE_DISTRIBUTIONS
@@ -124,18 +123,14 @@
     return problems
 
 
 def _get_raw_problems(name):
     if name == "more_wild":
         raw_problems = MORE_WILD_PROBLEMS
     elif name == "cartis_roberts":
-        warnings.warn(
-            "Only a subset of the cartis_roberts benchmark suite is currently "
-            "implemented. Do not use this for any published work."
-        )
         raw_problems = CARTIS_ROBERTS_PROBLEMS
     elif name == "example":
         subset = {
             "rosenbrock_good_start",
             "helical_valley_good_start",
             "powell_singular_good_start",
             "freudenstein_roth_good_start",
```

### Comparing `estimagic-0.4.4/src/estimagic/benchmarking/more_wild.py` & `estimagic-0.4.5/src/estimagic/benchmarking/more_wild.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     temp_array[2] = np.exp(-x[6] * (temp - x[9]) ** 2)
     temp_array[3] = np.exp(-x[7] * (temp - x[10]) ** 2)
     fvec = y - (temp_array.T * x[:4]).T.sum(axis=0)
     return fvec
 
 
 def bdqrtic(x):
-    # the length of array x should be more then 5.
+    # the length of array x should be more than 5.
     dim_in = len(x)
     fvec = np.zeros(2 * (dim_in - 4))
     for i in range(dim_in - 4):
         fvec[i] = -4 * x[i] + 3
         fvec[dim_in - 4 + i] = (
             x[i] ** 2
             + 2 * x[i + 1] ** 2
```

### Comparing `estimagic-0.4.4/src/estimagic/benchmarking/noise_distributions.py` & `estimagic-0.4.5/src/estimagic/benchmarking/noise_distributions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/benchmarking/process_benchmark_results.py` & `estimagic-0.4.5/src/estimagic/benchmarking/process_benchmark_results.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/benchmarking/run_benchmark.py` & `estimagic-0.4.5/src/estimagic/benchmarking/run_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,19 +104,19 @@
         default_algo_options["stopping.max_iterations"] = max_evals
     if disable_convergence:
         default_algo_options["convergence.relative_criterion_tolerance"] = 1e-14
         default_algo_options["convergence.relative_params_tolerance"] = 1e-14
         default_algo_options["convergence.relative_gradient_tolerance"] = 1e-14
 
     out_options = {}
-    for name, option in dict_options.items():
-        if not isinstance(option, dict):
-            option = {"algorithm": option}
+    for name, _option in dict_options.items():
+        if not isinstance(_option, dict):
+            option = {"algorithm": _option}
         else:
-            option = option.copy()
+            option = _option.copy()
 
         algo_options = {**default_algo_options, **option.get("algo_options", {})}
         algo_options = {k.replace(".", "_"): v for k, v in algo_options.items()}
         option["algo_options"] = algo_options
         if isinstance(option.get("algo_options"), dict):
             option["algo_options"] = {**default_algo_options, **option["algo_options"]}
         else:
```

### Comparing `estimagic-0.4.4/src/estimagic/cli.py` & `estimagic-0.4.5/src/estimagic/cli.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/config.py` & `estimagic-0.4.5/src/estimagic/config.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/dashboard/callbacks.py` & `estimagic-0.4.5/src/estimagic/dashboard/callbacks.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/dashboard/colors.py` & `estimagic-0.4.5/src/estimagic/dashboard/colors.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/dashboard/dashboard_app.py` & `estimagic-0.4.5/src/estimagic/dashboard/dashboard_app.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/dashboard/plot_functions.py` & `estimagic-0.4.5/src/estimagic/dashboard/plot_functions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/dashboard/run_dashboard.py` & `estimagic-0.4.5/src/estimagic/dashboard/run_dashboard.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/decorators.py` & `estimagic-0.4.5/src/estimagic/decorators.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/differentiation/derivatives.py` & `estimagic-0.4.5/src/estimagic/differentiation/derivatives.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             according to the rule of thumb.
         f0 (numpy.ndarray): 1d numpy array with func(x), optional.
         n_cores (int): Number of processes used to parallelize the function
             evaluations. Default 1.
         error_handling (str): One of "continue" (catch errors and continue to calculate
             derivative estimates. In this case, some derivative estimates can be
             missing but no errors are raised), "raise" (catch errors and continue
-            to calculate derivative estimates at fist but raise an error if all
+            to calculate derivative estimates at first but raise an error if all
             evaluations for one parameter failed) and "raise_strict" (raise an error
             as soon as a function evaluation fails).
         batch_evaluator (str or callable): Name of a pre-implemented batch evaluator
             (currently 'joblib' and 'pathos_mp') or Callable with the same interface
             as the estimagic batch_evaluators.
         return_func_value (bool): If True, return function value at params, stored in
             output dict under "func_value". Default False. This is useful when using
@@ -356,15 +356,15 @@
             according to the rule of thumb.
         f0 (numpy.ndarray): 1d numpy array with func(x), optional.
         n_cores (int): Number of processes used to parallelize the function
             evaluations. Default 1.
         error_handling (str): One of "continue" (catch errors and continue to calculate
             derivative estimates. In this case, some derivative estimates can be
             missing but no errors are raised), "raise" (catch errors and continue
-            to calculate derivative estimates at fist but raise an error if all
+            to calculate derivative estimates at first but raise an error if all
             evaluations for one parameter failed) and "raise_strict" (raise an error
             as soon as a function evaluation fails).
         batch_evaluator (str or callable): Name of a pre-implemented batch evaluator
             (currently 'joblib' and 'pathos_mp') or Callable with the same interface
             as the estimagic batch_evaluators.
         return_func_value (bool): If True, return function value at params, stored in
             output dict under "func_value". Default False. This is useful when using
@@ -671,22 +671,22 @@
         df_steps = df_steps.melt(
             id_vars="step_number", var_name="dim_x", value_name="step"
         )
         df_steps = df_steps.sort_values("step_number")
         df_steps = df_steps.reset_index(drop=True)
         df_steps = df_steps.apply(lambda col: col.abs() if col.name == "step" else col)
 
-        eval_arr = np.transpose(eval_arr, (0, 2, 1)).reshape(-1, dim_f)
-        df_evals = pd.concat((df_steps, pd.DataFrame(eval_arr)), axis=1)
+        reshaped_eval_arr = np.transpose(eval_arr, (0, 2, 1)).reshape(-1, dim_f)
+        df_evals = pd.concat((df_steps, pd.DataFrame(reshaped_eval_arr)), axis=1)
         df_evals = df_evals.melt(
             id_vars=["step_number", "dim_x", "step"],
             var_name="dim_f",
             value_name="eval",
         )
-        df_evals = df_evals.assign(**{"sign": direction})
+        df_evals = df_evals.assign(sign=direction)
         df_evals = df_evals.set_index(["sign", "step_number", "dim_x", "dim_f"])
         df_evals = df_evals.sort_index()
 
         dfs.append(df_evals)
 
     df = pd.concat(dfs).astype({"step": float, "eval": float})
     return df
```

### Comparing `estimagic-0.4.4/src/estimagic/differentiation/finite_differences.py` & `estimagic-0.4.5/src/estimagic/differentiation/finite_differences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Finite difference formulae for jacobians and hessians.
 
-All functions in this module should not only work for the simple case
-of one positive and/or one negative step, but also for the Richardson
-Extrapolation case with several positive and/or several negative steps.
+All functions in this module should not only work for the simple case of one positive
+and/or one negative step, but also for the Richardson Extrapolation case with several
+positive and/or several negative steps.
 
 Since steps and evals contain NaNs, we have to make sure that the functions do not raise
 warnings or errors for that case.
 
 """
 from typing import NamedTuple
```

### Comparing `estimagic-0.4.4/src/estimagic/differentiation/generate_steps.py` & `estimagic-0.4.5/src/estimagic/differentiation/generate_steps.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/differentiation/richardson_extrapolation.py` & `estimagic-0.4.5/src/estimagic/differentiation/richardson_extrapolation.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/estimation/estimate_ml.py` & `estimagic-0.4.5/src/estimagic/estimation/estimate_ml.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/estimation/estimate_msm.py` & `estimagic-0.4.5/src/estimagic/estimation/estimate_msm.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/estimation/msm_weighting.py` & `estimagic-0.4.5/src/estimagic/estimation/msm_weighting.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/examples/criterion_functions.py` & `estimagic-0.4.5/src/estimagic/examples/criterion_functions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/examples/diabetes.csv` & `estimagic-0.4.5/src/estimagic/examples/diabetes.csv`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/examples/exam_points.csv` & `estimagic-0.4.5/src/estimagic/examples/exam_points.csv`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/examples/logit.py` & `estimagic-0.4.5/src/estimagic/examples/logit.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/examples/numdiff_functions.py` & `estimagic-0.4.5/src/estimagic/examples/numdiff_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Functions with known gradients, jacobians or hessians.
 
 All functions take a numpy array with parameters as their first argument.
 
-Example inputs for the binary choice functions are in binary_choice_inputs.pickle.
-They come from the statsmodels documentation:
+Example inputs for the binary choice functions are in binary_choice_inputs.pickle. They
+come from the statsmodels documentation:
+
 https://tinyurl.com/y4x67vwl
 We pickled them so we don't need statsmodels as a dependency.
 
 """
 import numpy as np
 from scipy.stats import norm
```

### Comparing `estimagic-0.4.4/src/estimagic/examples/sensitivity_probit_example_data.csv` & `estimagic-0.4.5/src/estimagic/examples/sensitivity_probit_example_data.csv`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/exceptions.py` & `estimagic-0.4.5/src/estimagic/exceptions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/bootstrap.py` & `estimagic-0.4.5/src/estimagic/inference/bootstrap.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/bootstrap_ci.py` & `estimagic-0.4.5/src/estimagic/inference/bootstrap_ci.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/bootstrap_helpers.py` & `estimagic-0.4.5/src/estimagic/inference/bootstrap_helpers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/bootstrap_outcomes.py` & `estimagic-0.4.5/src/estimagic/inference/bootstrap_outcomes.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/bootstrap_samples.py` & `estimagic-0.4.5/src/estimagic/inference/bootstrap_samples.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/ml_covs.py` & `estimagic-0.4.5/src/estimagic/inference/ml_covs.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/msm_covs.py` & `estimagic-0.4.5/src/estimagic/inference/msm_covs.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/inference/shared.py` & `estimagic-0.4.5/src/estimagic/inference/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,24 +60,24 @@
 
         sample = rng.multivariate_normal(
             mean=internal_params.values,
             cov=internal_cov,
             size=n_samples,
         )
         transformed_free = []
-        for params_vec in sample:
+        for params in sample:
             if bounds_handling == "clip":
-                params_vec = np.clip(params_vec, a_min=lower_bounds, a_max=upper_bounds)
+                x = np.clip(params, a_min=lower_bounds, a_max=upper_bounds)
             elif bounds_handling == "raise":
-                if (params_vec < lower_bounds).any() or (
-                    params_vec > upper_bounds
-                ).any():
+                if (params < lower_bounds).any() or (params > upper_bounds).any():
                     raise ValueError()
+            else:
+                x = params
 
-            transformed = _from_internal(x=params_vec, return_type="flat")
+            transformed = _from_internal(x=x, return_type="flat")
             transformed_free.append(transformed[is_free])
 
         free_cov = np.cov(
             np.array(transformed_free),
             rowvar=False,
         )
 
@@ -215,16 +215,16 @@
     return summary
 
 
 def process_pandas_arguments(**kwargs):
     """Convert pandas objects to arrays and extract names of moments and parameters.
 
     This works for any number of keyword arguments. The result is a tuple containing
-    numpy arrays in same order as the keyword arguments and a dictionary with
-    the separated index objects as last entry. This dictionary contains the entries
+    numpy arrays in same order as the keyword arguments and a dictionary with the
+    separated index objects as last entry. This dictionary contains the entries
     "moments" and "params" for the identified moment names and parameter names.
 
     The keyword arguments "jac", "hess", "weights" and "moments_cov" are used to extract
     the names. Other keyword arguments are simply converted to numpy arrays.
 
     """
     param_name_candidates = {}
```

### Comparing `estimagic-0.4.4/src/estimagic/logging/create_tables.py` & `estimagic-0.4.5/src/estimagic/logging/create_tables.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/logging/load_database.py` & `estimagic-0.4.5/src/estimagic/logging/load_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,17 @@
     return engine
 
 
 def _configure_engine(engine, fast_logging):
     """Configure the sqlite engine.
 
     The two functions that configure the emission of the begin statement are taken from
-    the sqlalchemy documentation the documentation: https://tinyurl.com/u9xea5z and are
+    the sqlalchemy documentation the documentation:
+    https://tinyurl.com/u9xea5z
+    and are
     the recommended way of working around a bug in the pysqlite driver.
 
     The other function speeds up the write process. If fast_logging is False, it does so
     using only completely safe optimizations. Of fast_logging is True, it also uses
     unsafe optimizations.
 
     """
```

### Comparing `estimagic-0.4.4/src/estimagic/logging/read_from_database.py` & `estimagic-0.4.5/src/estimagic/logging/read_from_database.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/logging/read_log.py` & `estimagic-0.4.5/src/estimagic/logging/read_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Functions to read data from the database used for logging.
 
-The functions in the module are meant for end users of estimagic.
-They do not require any knowledge of databases.
+The functions in the module are meant for end users of estimagic. They do not require
+any knowledge of databases.
 
 When using them internally (e.g. in the dashboard), make sure to supply a database to
 path_or_database. Otherwise, the functions may be very slow.
 
 """
 from dataclasses import dataclass
 from pathlib import Path
```

### Comparing `estimagic-0.4.4/src/estimagic/logging/write_to_database.py` & `estimagic-0.4.5/src/estimagic/logging/write_to_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
     Args:
         data (dict): The keys correspond to columns in the database table.
         table_name (str): Name of the database table to which the row is added.
         database (DataBase): The database to which the row is added.
 
     """
-
     stmt = database.metadata.tables[table_name].insert().values(**data)
 
     _execute_write_statement(stmt, database)
 
 
 def _execute_write_statement(statement, database):
     try:
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/__init__.py` & `estimagic-0.4.5/src/estimagic/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/algo_options.py` & `estimagic-0.4.5/src/estimagic/optimization/algo_options.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/bhhh.py` & `estimagic-0.4.5/src/estimagic/optimization/bhhh.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/check_arguments.py` & `estimagic-0.4.5/src/estimagic/optimization/check_arguments.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/convergence_report.py` & `estimagic-0.4.5/src/estimagic/optimization/convergence_report.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/cyipopt_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/cyipopt_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/error_penalty.py` & `estimagic-0.4.5/src/estimagic/optimization/error_penalty.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/fides_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/fides_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/get_algorithm.py` & `estimagic-0.4.5/src/estimagic/optimization/get_algorithm.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/history.py` & `estimagic-0.4.5/src/estimagic/optimization/pounders_history.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/history_tools.py` & `estimagic-0.4.5/src/estimagic/optimization/history_tools.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/internal_criterion_template.py` & `estimagic-0.4.5/src/estimagic/optimization/internal_criterion_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             calculates the first derivative of criterion. For most algorithm, this is
             the gradient of the scalar output (or "value" entry of the dict). However
             some algorithms (e.g. bhhh) require the jacobian of the "contributions"
             entry of the dict. You will get an error if you provide the wrong type of
             derivative.
         criterion_and_derivative (callable): Function that returns criterion
             and derivative as a tuple. This can be used to exploit synergies in the
-            evaluation of both functions. The fist element of the tuple has to be
+            evaluation of both functions. The first element of the tuple has to be
             exactly the same as the output of criterion. The second has to be exactly
             the same as the output of derivative.
         numdiff_options (dict): Keyword arguments for the calculation of numerical
             derivatives. See :ref:`first_derivative` for details. Note that the default
             method is changed to "forward" for speed reasons.
         logging (bool): Whether logging is used.
         database (DataBase): Database to which the logs are written.
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/nag_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/nag_optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,16 +377,24 @@
     processed = {
         "solution_criterion": nag_result_obj.f,
         "n_criterion_evaluations": nag_result_obj.nx,
         "message": nag_result_obj.msg,
         "success": nag_result_obj.flag == nag_result_obj.EXIT_SUCCESS,
         "reached_convergence_criterion": None,
         "diagnostic_info": nag_result_obj.diagnostic_info,
-        "n_iterations": nag_result_obj.diagnostic_info["iters_total"].iloc[-1],
     }
+    try:
+        processed["n_iterations"] = nag_result_obj.diagnostic_info["iters_total"].iloc[
+            -1
+        ]
+    except (KeyboardInterrupt, SystemExit):
+        raise
+    except Exception:
+        processed["n_iterations"] = None
+
     if hasattr(nag_result_obj, "states"):
         processed.update({"states": nag_result_obj.states})
     if hasattr(nag_result_obj, "history_params"):
         processed.update({"history_params": nag_result_obj.history_params})
     if nag_result_obj.x is not None:
         processed["solution_x"] = nag_result_obj.x
     else:
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/neldermead.py` & `estimagic-0.4.5/src/estimagic/optimization/neldermead.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/nlopt_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/nlopt_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/optimization_logging.py` & `estimagic-0.4.5/src/estimagic/optimization/optimization_logging.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/optimize.py` & `estimagic-0.4.5/src/estimagic/optimization/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             of criterion. For most algorithm, this is the gradient of the scalar
             output (or "value" entry of the dict). However some algorithms (e.g. bhhh)
             require the jacobian of the "contributions" entry of the dict. You will get
             an error if you provide the wrong type of derivative.
         derivative_kwargs (dict): Additional keyword arguments for derivative.
         criterion_and_derivative (callable): Function that returns criterion
             and derivative as a tuple. This can be used to exploit synergies in the
-            evaluation of both functions. The fist element of the tuple has to be
+            evaluation of both functions. The first element of the tuple has to be
             exactly the same as the output of criterion. The second has to be exactly
             the same as the output of derivative.
         criterion_and_derivative_kwargs (dict): Additional keyword arguments for
             criterion and derivative.
         numdiff_options (dict): Keyword arguments for the calculation of numerical
             derivatives. See :ref:`first_derivative` for details. Note that the default
             method is changed to "forward" for speed reasons.
@@ -296,15 +296,15 @@
             of criterion. For most algorithm, this is the gradient of the scalar
             output (or "value" entry of the dict). However some algorithms (e.g. bhhh)
             require the jacobian of the "contributions" entry of the dict. You will get
             an error if you provide the wrong type of derivative.
         derivative_kwargs (dict): Additional keyword arguments for derivative.
         criterion_and_derivative (callable): Function that returns criterion
             and derivative as a tuple. This can be used to exploit synergies in the
-            evaluation of both functions. The fist element of the tuple has to be
+            evaluation of both functions. The first element of the tuple has to be
             exactly the same as the output of criterion. The second has to be exactly
             the same as the output of derivative.
         criterion_and_derivative_kwargs (dict): Additional keyword arguments for
             criterion and derivative.
         numdiff_options (dict): Keyword arguments for the calculation of numerical
             derivatives. See :ref:`first_derivative` for details. Note that the default
             method is changed to "forward" for speed reasons.
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/optimize_result.py` & `estimagic-0.4.5/src/estimagic/optimization/optimize_result.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/pounders.py` & `estimagic-0.4.5/src/estimagic/optimization/pounders.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import warnings
 
 import numpy as np
 
 from estimagic.batch_evaluators import process_batch_evaluator
 from estimagic.config import DEFAULT_N_CORES
 from estimagic.decorators import mark_minimizer
-from estimagic.optimization.history import LeastSquaresHistory
+from estimagic.optimization.pounders_history import LeastSquaresHistory
 from estimagic.optimization.pounders_auxiliary import (
     add_accepted_point_to_residual_model,
     add_geomtery_points_to_make_main_model_fully_linear,
     create_initial_residual_model,
     create_main_from_residual_model,
     evaluate_residual_model,
     find_affine_points,
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/pounders_auxiliary.py` & `estimagic-0.4.5/src/estimagic/optimization/pounders_auxiliary.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,18 +286,19 @@
             "maxiter_gradient_descent": maxiter_gradient_descent,
             "gtol_abs": gtol_abs,
             "gtol_rel": gtol_rel,
             "gtol_scaled": gtol_scaled,
             "gtol_abs_conjugate_gradient": gtol_abs_conjugate_gradient,
             "gtol_rel_conjugate_gradient": gtol_rel_conjugate_gradient,
         }
-        result = bntr(main_model, lower_bounds, upper_bounds, **options)
+        result = bntr(main_model, lower_bounds, upper_bounds, x_candidate=x0, **options)
     elif solver == "gqtpar":
         result = gqtpar(
             main_model,
+            x_candidate=x0,
             k_easy=k_easy,
             k_hard=k_hard,
             maxiter=maxiter,
         )
     else:
         raise ValueError(
             "Invalid subproblem solver: {solver}. Must be one of bntr, gqtpar."
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/process_multistart_sample.py` & `estimagic-0.4.5/src/estimagic/optimization/process_multistart_sample.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/process_results.py` & `estimagic-0.4.5/src/estimagic/optimization/process_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,12 +170,12 @@
             out["contributions"] = -critval["contributions"]
     else:
         out = -critval
     return out
 
 
 def _sum_or_none(summands):
-    if any([s is None for s in summands]):
+    if any(s is None for s in summands):
         out = None
     else:
         out = int(np.sum(summands))
     return out
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/pygmo_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/pygmo_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/scipy_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/scipy_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/simopt_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/simopt_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/_conjugate_gradient.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/_conjugate_gradient_fast.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_conjugate_gradient_fast.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/_steihaug_toint.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_steihaug_toint.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/_steihaug_toint_fast.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_steihaug_toint_fast.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/_trsbox.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_trsbox.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/_trsbox_fast.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_trsbox_fast.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/bntr.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/bntr.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     inactive: Union[np.ndarray, None] = None
 
 
 def bntr(
     model,
     lower_bounds,
     upper_bounds,
+    x_candidate,
     *,
     conjugate_gradient_method,
     maxiter,
     maxiter_gradient_descent,
     gtol_abs,
     gtol_rel,
     gtol_scaled,
@@ -57,14 +58,15 @@
             main model, i.e.:
             - ``linear_terms`` (np.ndarray): 1d array of shape (n,)
             - ``square_terms`` (np.ndarray): 2d array of shape (n,n).
         lower_bounds (np.ndarray): 1d array of shape (n,) with lower bounds
             for the parameter vector x.
         upper_bounds (np.ndarray): 1d array of shape (n,) with upper bounds
             for the parameter vector x.
+        x_candidate (np.ndarray): Initial guess for the solution of the subproblem.
         conjugate_gradient_method (str): Method for computing the conjugate gradient
             step. Available conjugate gradient methods are:
                 - "cg"
                 - "steihaug_toint"
                 - "trsbox" (default)
         maxiter (int): Maximum number of iterations. If reached, terminate.
         maxiter_gradient_descent (int): Maximum number of steepest descent iterations
@@ -101,16 +103,14 @@
         "alpha4": 2.00,
         "alpha5": 4.00,
         "min_radius": 1e-10,
         "max_radius": 1e10,
         "default_radius": 100.00,
     }
 
-    x_candidate = np.zeros_like(model.linear_terms)
-
     (
         x_candidate,
         f_candidate,
         gradient_unprojected,
         hessian_bounds_inactive,
         trustregion_radius,
         active_bounds_info,
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/bntr_fast.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/bntr_fast.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 EPSILON = np.finfo(float).eps ** (2 / 3)
 
 
 def bntr_fast(
     model,
     lower_bounds,
     upper_bounds,
+    x_candidate,
     *,
     conjugate_gradient_method,
     maxiter,
     maxiter_gradient_descent,
     gtol_abs,
     gtol_rel,
     gtol_scaled,
@@ -52,14 +53,15 @@
             main model, i.e.:
             - ``linear_terms`` (np.ndarray): 1d array of shape (n,)
             - ``square_terms`` (np.ndarray): 2d array of shape (n,n).
         lower_bounds (np.ndarray): 1d array of shape (n,) with lower bounds
             for the parameter vector x.
         upper_bounds (np.ndarray): 1d array of shape (n,) with upper bounds
             for the parameter vector x.
+        x_candidate (np.ndarray): Initial guess for the solution of the subproblem.
         conjugate_gradient_method (str): Method for computing the conjugate gradient
             step. Available conjugate gradient methods are:
                 - "cg"
                 - "steihaug_toint"
                 - "trsbox" (default)
         maxiter (int): Maximum number of iterations. If reached, terminate.
         maxiter_gradient_descent (int): Maximum number of steepest descent iterations
@@ -95,14 +97,15 @@
         converged,
         convergence_reason,
     ) = _bntr_fast_jitted(
         model_gradient=model_gradient,
         model_hessian=model_hessian,
         lower_bounds=lower_bounds,
         upper_bounds=upper_bounds,
+        x_candidate=x_candidate,
         conjugate_gradient_method=conjugate_gradient_method,
         maxiter=maxiter,
         maxiter_gradient_descent=maxiter_gradient_descent,
         gtol_abs=gtol_abs,
         gtol_rel=gtol_rel,
         gtol_scaled=gtol_scaled,
         gtol_abs_conjugate_gradient=gtol_abs_conjugate_gradient,
@@ -122,14 +125,15 @@
 
 @njit
 def _bntr_fast_jitted(
     model_gradient,
     model_hessian,
     lower_bounds,
     upper_bounds,
+    x_candidate,
     conjugate_gradient_method,
     maxiter,
     maxiter_gradient_descent,
     gtol_abs,
     gtol_rel,
     gtol_scaled,
     gtol_abs_conjugate_gradient,
@@ -159,14 +163,15 @@
             surrogate model.
         model_hessian (np.ndarray): 2d array of shape (n,n) of the square terms of
             the surrogate model.
         lower_bounds (np.ndarray): 1d array of shape (n,) with lower bounds
             for the parameter vector x.
         upper_bounds (np.ndarray): 1d array of shape (n,) with upper bounds
             for the parameter vector x.
+        x_candidate (np.ndarray): Initial guess for the solution of the subproblem.
         conjugate_gradient_method (str): Method for computing the conjugate gradient
             step. Available conjugate gradient methods are:
                 - "cg"
                 - "steihaug_toint"
                 - "trsbox" (default)
         maxiter (int): Maximum number of iterations. If reached, terminate.
         maxiter_gradient_descent (int): Maximum number of steepest descent iterations
@@ -205,14 +210,15 @@
         converged,
         convergence_reason,
     ) = _take_preliminary_gradient_descent_step_and_check_for_solution(
         model_gradient,
         model_hessian,
         lower_bounds,
         upper_bounds,
+        x_candidate,
         maxiter_gradient_descent,
         gtol_abs,
         gtol_rel,
         gtol_scaled,
     )
 
     for niter in range(maxiter + 1):
@@ -337,14 +343,15 @@
 
 @njit
 def _take_preliminary_gradient_descent_step_and_check_for_solution(
     model_gradient,
     model_hessian,
     lower_bounds,
     upper_bounds,
+    x_candidate,
     maxiter_gradient_descent,
     gtol_abs,
     gtol_rel,
     gtol_scaled,
 ):
     """Take a preliminary gradient descent step and check if we found a solution.
 
@@ -353,14 +360,15 @@
             main model.
         model_hessian (np.ndarray): 2d array of shape (n,n) with square terms of
             the main model
         lower_bounds (np.ndarray): 1d array of shape (n,) with lower bounds
             for the parameter vector x.
         upper_bounds (np.ndarray): 1d array of shape (n,) with upper bounds
             for the parameter vector x.
+        x_candidate (np.ndarray): Initial guess for the solution of the subproblem.
         maxiter_gradient_descent (int): Maximum number of iterations in performing
             gradient descent step
         gtol_abs (float): Convergence tolerance for the absolute gradient norm.
         gtol_rel (float): Convergence tolerance for the relative gradient norm.
         gtol_scaled (float): Convergence tolerance for the scaled gradient norm.
 
     Returns:
@@ -380,16 +388,14 @@
     gamma2 = 0.5
     gamma3 = 2.0
     gamma4 = 5.0
 
     converged = False
     convergence_reason = 0
 
-    x_candidate = np.zeros(len(model_gradient))
-
     criterion_candidate = _evaluate_model_criterion(
         x_candidate, model_gradient, model_hessian
     )
 
     (
         active_lower_bounds,
         active_upper_bounds,
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/gqtpar.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/gqtpar.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class DampingFactors(NamedTuple):
     candidate: Union[float, None] = None
     lower_bound: Union[float, None] = None
     upper_bound: Union[float, None] = None
 
 
-def gqtpar(model, *, k_easy=0.1, k_hard=0.2, maxiter=200):
+def gqtpar(model, x_candidate, *, k_easy=0.1, k_hard=0.2, maxiter=200):
     """Solve the quadratic trust-region subproblem via nearly exact iterative method.
 
     This subproblem solver is mainly based on Conn et al. (2000) "Trust region methods"
     (:cite:`Conn2000`), pp. 169-200.
 
     But ideas from Nocedal and Wright (2006) "Numerical optimization"
     (:cite:`Nocedal2006`), pp. 83-91, who implement a similar algorithm,
@@ -46,35 +46,32 @@
     where g denotes the gradient and H the hessian of the quadratic model,
     respectively.
 
     k_easy and k_hard are stopping criteria for the iterative subproblem solver.
     See pp. 194-197 in :cite:`Conn2000` for a more detailed description.
 
     Args:
-        main_model (NamedTuple): NamedTuple containing the parameters of the
-            main model, i.e.:
+        model (NamedTuple): NamedTuple containing the parameters of the main model, i.e.
             - ``linear_terms``, a np.ndarray of shape (n,) and
             - ``square_terms``, a np.ndarray of shape (n,n).
-        trustregion_radius (float): Trustregion radius, often referred to as delta.
+        x_candidate (np.ndarray): Initial guess for the solution of the subproblem.
         k_easy (float): topping criterion for the "easy" case.
         k_hard (float): Stopping criterion for the "hard" case.
         maxiter (int): Maximum number of iterations to perform. If reached,
             terminate.
 
     Returns:
         (dict): Result dictionary containing the following keys:
             - ``x`` (np.ndarray): Solution vector of the subproblem of shape (n,)
             - ``criterion`` (float): Minimum function value associated with the
                 solution.
 
     """
     hessian_info = HessianInfo()
 
-    x_candidate = np.zeros_like(model.linear_terms)
-
     # Small floating point number signaling that for vectors smaller
     # than that backward substituition is not reliable.
     # See Golub, G. H., Van Loan, C. F. (2013), "Matrix computations", p.165.
     zero_threshold = (
         model.square_terms.shape[0]
         * np.finfo(float).eps
         * np.linalg.norm(model.square_terms, np.Inf)
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/gqtpar_fast.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/gqtpar_fast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Auxiliary functions for the quadratic GQTPAR trust-region subsolver."""
 import numpy as np
 from numba import njit
 from scipy.linalg import cho_solve, solve_triangular
 from scipy.linalg.lapack import dpotrf as compute_cholesky_factorization
 
 
-def gqtpar_fast(model, *, k_easy=0.1, k_hard=0.2, maxiter=200):
+def gqtpar_fast(model, x_candidate, *, k_easy=0.1, k_hard=0.2, maxiter=200):
     """Solve the quadratic trust-region subproblem via nearly exact iterative method.
 
     This subproblem solver is mainly based on Conn et al. (2000) "Trust region methods"
     (:cite:`Conn2000`), pp. 169-200.
 
     But ideas from Nocedal and Wright (2006) "Numerical optimization"
     (:cite:`Nocedal2006`), pp. 83-91, who implement a similar algorithm,
@@ -32,19 +32,18 @@
     where g denotes the gradient and H the hessian of the quadratic model,
     respectively.
 
     k_easy and k_hard are stopping criteria for the iterative subproblem solver.
     See pp. 194-197 in :cite:`Conn2000` for a more detailed description.
 
     Args:
-        main_model (NamedTuple): NamedTuple containing the parameters of the
-            main model, i.e.:
+        model (NamedTuple): NamedTuple containing the parameters of the main model, i.e.
             - ``linear_terms``, a np.ndarray of shape (n,) and
             - ``square_terms``, a np.ndarray of shape (n,n).
-        trustregion_radius (float): Trustregion radius, often referred to as delta.
+        x_candidate (np.ndarray): Initial guess for the solution of the subproblem.
         k_easy (float): topping criterion for the "easy" case.
         k_hard (float): Stopping criterion for the "hard" case.
         maxiter (int): Maximum number of iterations to perform. If reached,
             terminate.
 
     Returns:
         (dict): Result dictionary containing the following keys:
@@ -52,15 +51,14 @@
             - ``criterion`` (float): Minimum function value associated with the
                 solution.
 
     """
     hessian_already_factorized = False
     model_gradient = model.linear_terms
     model_hessian = model.square_terms
-    x_candidate = np.zeros(len(model_gradient))
 
     # Small floating point number signaling that for vectors smaller
     # than that backward substituition is not reliable.
     # See Golub, G. H., Van Loan, C. F. (2013), "Matrix computations", p.165.
     zero_threshold = (
         model_hessian.shape[0] * np.finfo(float).eps * _norm(model_hessian, np.Inf)
     )
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/subsolvers/linear_subsolvers.py` & `estimagic-0.4.5/src/estimagic/optimization/subsolvers/linear_subsolvers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tao_optimizers.py` & `estimagic-0.4.5/src/estimagic/optimization/tao_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tiktak.py` & `estimagic-0.4.5/src/estimagic/optimization/tiktak.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,19 @@
 <https://www.nber.org/system/files/working_papers/w26340/w26340.pdf>`_)
 
 
 
 
 
 
+is an algorithm for solving global optimization problems. It performs local searches
+from a set of carefully-selected points in the parameter space.
 
+First implemented in Python by Alisdair McKay (
 
-
-
-
-is an algorithm for solving global optimization problems. It performs local
-searches from a set of carefully-selected points in the parameter space.
-
-First implemented in Python by Alisdair McKay
-(
 `GitHub Repository <https://github.com/amckay/TikTak>`_)
 
 """
 import warnings
 from functools import partial
 
 import numpy as np
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/adjust_radius.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/adjust_radius.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-def adjust_radius(radius, rho, step, options):
+def adjust_radius(radius, rho, step_length, options):
     """Adjust the trustregion radius based on relative improvement and stepsize.
 
     This is just a slight generalization of the pounders radius adjustment. With default
     options it yields the same result.
 
     Noise handling is not built-in here. It will be achieved by calling the
     function with a noise-adjusted rho.
@@ -17,15 +17,14 @@
         step (np.ndarray): The step between the last two accepted parameter vectors.
         options (NamedTuple): Options for radius management.
 
     Returns:
         float: The updated radius.
 
     """
-    step_length = np.linalg.norm(step)
     is_large_step = step_length / radius >= options.large_step
 
     if rho >= options.rho_increase and is_large_step:
         new_radius = radius * options.expansion_factor
     elif rho >= options.rho_decrease:
         new_radius = radius
     else:
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/aggregate_models.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/aggregate_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,39 @@
 from functools import partial
 
 import numpy as np
 
 from estimagic.optimization.tranquilo.models import ScalarModel
 
 
-def get_aggregator(aggregator, functype, model_info):
+def get_aggregator(aggregator):
     """Get a function that aggregates a VectorModel into a ScalarModel.
 
     Args:
-        aggregator (str or callable): Name of an aggregator or aggregator function.
-            The function must take as argument:
-            - vector_model (VectorModel): A fitted vector model.
-        functype (str): One of "scalar", "least_squares" and "likelihood".
-        model_info (ModelInfo): Information that describes the functional form of
-            the model.
+        aggregator (str): Name of an aggregator.
 
     Returns:
         callable: The partialled aggregator that only depends on vector_model.
 
     """
     built_in_aggregators = {
         "identity": aggregator_identity,
         "sum": aggregator_sum,
         "information_equality_linear": aggregator_information_equality_linear,
         "least_squares_linear": aggregator_least_squares_linear,
     }
 
-    if isinstance(aggregator, str) and aggregator in built_in_aggregators:
+    if aggregator in built_in_aggregators:
         _aggregator = built_in_aggregators[aggregator]
-        _aggregator_name = aggregator
-        _using_built_in_aggregator = True
-    elif callable(aggregator):
-        _aggregator = aggregator
-        _aggregator_name = getattr(aggregator, "__name__", "your aggregator")
-        _using_built_in_aggregator = False
     else:
         raise ValueError(
-            "Invalid aggregator: {aggregator}. Must be one of "
+            f"Invalid aggregator: {aggregator}. Must be one of "
             f"{list(built_in_aggregators)} or a callable."
         )
 
-    # determine if aggregator is compatible with functype and model_info
-    aggregator_compatible_with_functype = {
-        "scalar": ("identity", "sum"),
-        "least_squares": ("least_squares_linear",),
-        "likelihood": (
-            "sum",
-            "information_equality_linear",
-        ),
-    }
-
-    aggregator_compatible_with_model_info = {
-        # keys are names of aggregators and values are functions of model_info that
-        # return False in case of incompatibility
-        "identity": lambda x: True,  # noqa: ARG005
-        "sum": _is_second_order_model,
-        "information_equality_linear": lambda model_info: not _is_second_order_model(
-            model_info
-        ),
-        "least_squares_linear": lambda model_info: not _is_second_order_model(
-            model_info
-        ),
-    }
-
-    if _using_built_in_aggregator:
-        # compatibility errors
-        if _aggregator_name not in aggregator_compatible_with_functype[functype]:
-            raise ValueError(
-                f"Aggregator {_aggregator_name} is not compatible with functype "
-                f"{functype}. It would not produce a quadratic main model."
-            )
-        if not aggregator_compatible_with_model_info[_aggregator_name](model_info):
-            raise ValueError(
-                f"ModelInfo {model_info} is not compatible with aggregator "
-                f"{_aggregator_name}. Depending on the aggregator this may be because "
-                "it would not produce a quadratic main model or that the aggregator "
-                "requires a different residual model for theoretical reasons."
-            )
-
-    # create aggregator
     out = partial(_aggregate_models_template, aggregator=_aggregator)
     return out
 
 
 def _aggregate_models_template(vector_model, aggregator):
     """Aggregate a VectorModel into a ScalarModel.
 
@@ -93,52 +43,57 @@
 
     Returns:
         ScalarModel: The aggregated model
 
     """
     intercept, linear_terms, square_terms = aggregator(vector_model)
     scalar_model = ScalarModel(
-        intercept=intercept, linear_terms=linear_terms, square_terms=square_terms
+        intercept=intercept,
+        linear_terms=linear_terms,
+        square_terms=square_terms,
+        shift=vector_model.shift,
+        scale=vector_model.scale,
     )
     return scalar_model
 
 
 def aggregator_identity(vector_model):
     """Aggregate quadratic VectorModel using identity function.
 
     This aggregation is useful if the underlying maximization problem is a scalar
     problem. To get a second-order main model vector_model must be second-order model.
 
     Assumptions
     -----------
     1. functype: scalar
-    2. ModelInfo: has squares or interactions
+    2. model_type: quadratic
 
     """
+    n_params = vector_model.linear_terms.size
     intercept = float(vector_model.intercepts)
-    linear_terms = np.squeeze(vector_model.linear_terms)
+    linear_terms = vector_model.linear_terms.flatten()
     if vector_model.square_terms is None:
-        square_terms = np.zeros((len(linear_terms), len(linear_terms)))
+        square_terms = np.zeros((n_params, n_params))
     else:
-        square_terms = np.squeeze(vector_model.square_terms)
+        square_terms = vector_model.square_terms.reshape(n_params, n_params)
     return intercept, linear_terms, square_terms
 
 
 def aggregator_sum(vector_model):
     """Aggregate quadratic VectorModel using sum function.
 
     This aggregation is useful if the underlying maximization problem is a likelihood
     problem. That is, the criterion is the sum of residuals, which allows us to sum
     up the coefficients of the residual model to get the main model. The main model will
     only be a second-order model if the residual model is a second-order model.
 
     Assumptions
     -----------
     1. functype: likelihood
-    2. ModelInfo: has squares or interactions
+    2. model_type: quadratic
 
     """
     vm_intercepts = vector_model.intercepts
     intercept = vm_intercepts.sum(axis=0)
     linear_terms = vector_model.linear_terms.sum(axis=0)
     square_terms = vector_model.square_terms.sum(axis=0)
     return intercept, linear_terms, square_terms
@@ -150,15 +105,15 @@
     This aggregation is useful if the underlying maximization problem is a least-squares
     problem. We can then simply plug-in a linear model for the residuals into the
     least-squares formulae to get a second-order main model.
 
     Assumptions
     -----------
     1. functype: least_squares
-    2. ModelInfo: has intercept but no squares and no interaction
+    2. model_type: linear
 
     References
     ----------
     See section 2.1 of :cite:`Cartis2018` for further information.
 
     """
     vm_linear_terms = vector_model.linear_terms
@@ -178,24 +133,20 @@
     problem. Given a linear model for the likelihood contributions we get an estimate of
     the scores. Using the Fisher-Information-Equality we estimate the average Hessian
     using the scores.
 
     Assumptions
     -----------
     1. functype: likelihood
-    2. ModelInfo: has no squares and no interaction
+    2. model_type: linear
 
     """
     vm_linear_terms = vector_model.linear_terms
     vm_intercepts = vector_model.intercepts
 
     fisher_information = vm_linear_terms.T @ vm_linear_terms
 
     intercept = vm_intercepts.sum(axis=0)
     linear_terms = vm_linear_terms.sum(axis=0)
     square_terms = -fisher_information / 2
 
     return intercept, linear_terms, square_terms
-
-
-def _is_second_order_model(model_info):
-    return model_info.has_squares or model_info.has_interactions
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/clustering.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/clustering.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/fit_models.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/fit_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,154 +1,178 @@
 from functools import partial
 
 import numpy as np
 from numba import njit
 from scipy.linalg import qr_multiply
 
 from estimagic.optimization.tranquilo.get_component import get_component
+from estimagic.optimization.tranquilo.handle_infinity import get_infinity_handler
+from estimagic.optimization.tranquilo.options import FitterOptions
 from estimagic.optimization.tranquilo.models import (
-    ModelInfo,
     VectorModel,
-    n_interactions,
+    add_models,
+    move_model,
     n_second_order_terms,
 )
 
 
-def get_fitter(fitter, user_options=None, model_info=None):
+def get_fitter(
+    fitter,
+    fitter_options=None,
+    model_type=None,
+    residualize=None,
+    infinity_handling=None,
+):
     """Get a fit-function with partialled options.
 
     Args:
-        fitter (str or callable): Name of a fit method or a fit method. The first
-            argument of any fit method needs to be ``x``, second ``y`` and third
-            ``model_info``.
+        fitter (str or callable): Name of a fit method or a fit method. Arguments need
+            to be, in order,
+            - x (np.ndarray): Data points.
+            - y (np.ndarray): Corresponding function evaluations at data points.
+            - weighs (np.ndarray): Weights for the data points.
+            - model_type (str): Type of model to be fitted.
 
-        user_options (dict): Options for the fit method. The following are supported:
+        fitter_options (dict): Options for the fit method. The following are supported:
             - l2_penalty_linear (float): Penalty that is applied to all linear terms.
             - l2_penalty_square (float): Penalty that is applied to all square terms,
             that is the quadratic and interaction terms.
 
-        model_info (ModelInfo): Information that describes the functional form of
-            the model. Has entries:
-            - has_squares (bool): Whether to use quadratic terms as features in the
-            regression.
-            - has_interactions (bool): Whether to use interaction terms as features
-            in the regression.
+        model_type (str): Type of the model that is fitted. The following are supported:
+            - "linear": Only linear effects and intercept.
+            - "quadratic": Fully quadratic model.
+
+        residualize (bool): If True, the model is fitted to the residuals of the old
+            model. This introduces momentum when the coefficients are penalized.
+
+        infinity_handling (str): How to handle infinite values in the data. Currently
+            supported: {"relative"}. See `handle_infinty.py`.
 
     Returns:
         callable: The partialled fit method that only depends on x and y.
 
     """
-    if model_info is None:
-        model_info = ModelInfo()
-
     built_in_fitters = {
         "ols": fit_ols,
         "ridge": fit_ridge,
         "powell": fit_powell,
+        "tranquilo": fit_tranquilo,
     }
 
-    default_options = {
-        "l2_penalty_linear": 0,
-        "l2_penalty_square": 0.1,
-        "model_info": model_info,
-    }
-
-    mandatory_arguments = ["x", "y", "model_info"]
+    mandatory_arguments = ["x", "y", "model_type"]
 
     _raw_fitter = get_component(
         name_or_func=fitter,
         component_name="fitter",
         func_dict=built_in_fitters,
-        default_options=default_options,
-        user_options=user_options,
+        default_options=FitterOptions(),
+        user_options=fitter_options,
         mandatory_signature=mandatory_arguments,
     )
 
+    clip_infinite_values = get_infinity_handler(infinity_handling)
+
     fitter = partial(
         _fitter_template,
         fitter=_raw_fitter,
-        model_info=model_info,
+        model_type=model_type,
+        clip_infinite_values=clip_infinite_values,
+        residualize=residualize,
     )
 
     return fitter
 
 
 def _fitter_template(
     x,
     y,
+    region,
+    old_model,
     weights=None,
     fitter=None,
-    model_info=None,
+    model_type=None,
+    clip_infinite_values=None,
+    residualize=False,
 ):
     """Fit a model to data.
 
     Args:
         x (np.ndarray): Array of shape (n_samples, n_params) of x-values,
             rescaled such that the trust region becomes a hypercube from -1 to 1.
         y (np.ndarray): Array of shape (n_samples, n_residuals) with function
             evaluations that have been centered around the function value at the
             trust region center.
         fitter (callable): Fit method. The first argument of any fit method needs to be
-            ``x``, second ``y`` and third ``model_info``.
-        model_info (ModelInfo): Information that describes the functional form of
-            the model.
+            ``x``, second ``y`` and third ``model_type``.
+        model_type (str): Type of the model that is fitted. The following are supported:
+            - "linear": Only linear effects and intercept.
+            - "quadratic": Fully quadratic model.
 
     Returns:
         VectorModel or ScalarModel: Results container.
 
     """
-    n_samples, n_params = x.shape
+    _, n_params = x.shape
     n_residuals = y.shape[1]
 
-    # weight the data in order to get weighted fitting from fitters that do not support
-    # weights. Inspired by: https://stackoverflow.com/a/52452833
-    if weights is not None:
-        _root_weights = np.sqrt(weights).reshape(n_samples, 1)
-        y = y * _root_weights
-        x = x * _root_weights
+    y_clipped = clip_infinite_values(y)
+    x_unit = region.map_to_unit(x)
 
-    coef = fitter(x, y)
+    if residualize:
+        old_model_moved = move_model(old_model, region)
+        y_clipped = y_clipped - old_model_moved.predict(x_unit).reshape(y_clipped.shape)
+
+    coef = fitter(x=x_unit, y=y_clipped, weights=weights, model_type=model_type)
 
     # results processing
     intercepts, linear_terms, square_terms = np.split(coef, (1, n_params + 1), axis=1)
     intercepts = intercepts.flatten()
 
     # construct final square terms
-    if model_info.has_interactions:
+    if model_type == "quadratic":
         square_terms = _reshape_square_terms_to_hess(
-            square_terms, n_params, n_residuals, model_info.has_squares
+            square_terms, n_params, n_residuals
         )
-    elif model_info.has_squares:
-        square_terms = 2 * np.stack([np.diag(a) for a in square_terms])
     else:
         square_terms = None
 
-    results = VectorModel(intercepts, linear_terms, square_terms)
+    results = VectorModel(
+        intercepts,
+        linear_terms,
+        square_terms,
+        shift=region.effective_center,
+        scale=region.effective_radius,
+    )
+
+    if residualize:
+        results = add_models(results, old_model_moved)
 
     return results
 
 
-def fit_ols(x, y, model_info):
+def fit_ols(x, y, weights, model_type):
     """Fit a linear model using ordinary least squares.
 
     Args:
         x (np.ndarray): Array of shape (n_samples, n_params) of x-values,
             rescaled such that the trust region becomes a hypercube from -1 to 1.
         y (np.ndarray): Array of shape (n_samples, n_residuals) with function
             evaluations that have been centered around the function value at the
             trust region center.
-        model_info (ModelInfo): Information that describes the functional form of the
-            model.
+        model_type (str): Type of the model that is fitted. The following are supported:
+            - "linear": Only linear effects and intercept.
+            - "quadratic": Fully quadratic model.
 
     Returns:
         np.ndarray: The model coefficients.
 
     """
-    features = _build_feature_matrix(x, model_info)
-    coef = _fit_ols(features, y)
+    features = _build_feature_matrix(x, model_type)
+    features_w, y_w = _add_weighting(features, y, weights)
+    coef = _fit_ols(features_w, y_w)
 
     return coef
 
 
 def _fit_ols(x, y):
     """Fit a linear model using least-squares.
 
@@ -162,51 +186,93 @@
     """
     coef, *_ = np.linalg.lstsq(x, y, rcond=None)
     coef = coef.T
 
     return coef
 
 
+def fit_tranquilo(x, y, weights, model_type, p_intercept, p_linear, p_square):
+    """Fit a linear model using ordinary least squares.
+
+    The difference to fit_ols is that the linear terms are penalized less strongly
+    when the system is underdetermined.
+
+    Args:
+        x (np.ndarray): Array of shape (n_samples, n_params) of x-values,
+            rescaled such that the trust region becomes a hypercube from -1 to 1.
+        y (np.ndarray): Array of shape (n_samples, n_residuals) with function
+            evaluations that have been centered around the function value at the
+            trust region center.
+        model_type (str): Type of the model that is fitted. The following are supported:
+            - "linear": Only linear effects and intercept.
+            - "quadratic": Fully quadratic model.
+
+    Returns:
+        np.ndarray: The model coefficients.
+
+    """
+    features = _build_feature_matrix(x, model_type)
+    features_w, y_w = _add_weighting(features, y, weights)
+
+    n_params = x.shape[1]
+    n_features = features.shape[1]
+
+    factor = np.array(
+        [1 / p_intercept]
+        + [1 / p_linear] * n_params
+        + [1 / p_square] * (n_features - 1 - n_params)
+    )
+
+    coef_raw = _fit_ols(features_w * factor, y_w)
+    coef = coef_raw * factor
+
+    return coef
+
+
 def fit_ridge(
     x,
     y,
-    model_info,
+    weights,
+    model_type,
     l2_penalty_linear,
     l2_penalty_square,
 ):
     """Fit a linear model using Ridge regression.
 
     Args:
         x (np.ndarray): Array of shape (n_samples, n_params) of x-values, rescaled such
             that the trust region becomes a hypercube from -1 to 1.
         y (np.ndarray): Array of shape (n_samples, n_residuals) with function
             evaluations that have been centered around the function value at the trust
             region center.
-        model_info (ModelInfo): Information that describes the functional form of the
-            model.
+        model_type (str): Type of the model that is fitted. The following are supported:
+            - "linear": Only linear effects and intercept.
+            - "quadratic": Fully quadratic model.
         l2_penalty_linear (float): Penalty that is applied to all linear terms.
         l2_penalty_square (float): Penalty that is applied to all square terms, that is
             the quadratic and interaction terms.
 
     Returns:
         np.ndarray: The model coefficients.
 
     """
-    features = _build_feature_matrix(x, model_info)
+    features = _build_feature_matrix(x, model_type)
+
+    features_w, y_w = _add_weighting(features, y, weights)
 
     # create penalty array
     n_params = x.shape[1]
     cutoffs = (1, n_params + 1)
 
     penalty = np.zeros(features.shape[1])
     penalty[: cutoffs[0]] = 0
     penalty[cutoffs[0] : cutoffs[1]] = l2_penalty_linear
     penalty[cutoffs[1] :] = l2_penalty_square
 
-    coef = _fit_ridge(features, y, penalty)
+    coef = _fit_ridge(features_w, y_w, penalty)
 
     return coef
 
 
 def _fit_ridge(x, y, penalty):
     """Fit a linear model using ridge regression.
 
@@ -224,15 +290,15 @@
 
     coef, *_ = np.linalg.lstsq(a + np.diag(penalty), b, rcond=None)
     coef = coef.T
 
     return coef
 
 
-def fit_powell(x, y, model_info):
+def fit_powell(x, y, model_type):
     """Fit a model, switching between penalized and unpenalized fitting.
 
     For:
     - n + 1 points: Fit ols with linear feature matrix.
     - n + 2 <= n + 0.5 * n * (n + 1) points, i.e. until one less than a
         just identified quadratic model: Fit pounders.
     - else: Fit ols with quadratic feature matrix.
@@ -240,46 +306,44 @@
 
     Args:
         x (np.ndarray): Array of shape (n_samples, n_params) of x-values,
             rescaled such that the trust region becomes a hypercube from -1 to 1.
         y (np.ndarray): Array of shape (n_samples, n_residuals) with function
             evaluations that have been centered around the function value at the
             trust region center.
-        model_info (ModelInfo): Information that describes the functional form of the
-            model.
+        model_type (str): Type of the model that is fitted. The following are supported:
+            - "linear": Only linear effects and intercept.
+            - "quadratic": Fully quadratic model.
 
     Returns:
         np.ndarray: The model coefficients.
 
     """
     n_samples, n_params = x.shape
 
     _switch_to_linear = n_samples <= n_params + 1
 
     _n_just_identified = n_params + 1
-    if model_info.has_squares:
-        _n_just_identified += n_params
-    if model_info.has_interactions:
-        _n_just_identified += int(0.5 * n_params * (n_params - 1))
+    if model_type == "quadratic":
+        _n_just_identified += n_second_order_terms(n_params)
 
     if _switch_to_linear:
-        model_info = model_info._replace(has_squares=False, has_interactions=False)
-        coef = fit_ols(x, y, model_info)
+        coef = fit_ols(x, y, weights=None, model_type="linear")
         n_resid, n_present = coef.shape
         padding = np.zeros((n_resid, _n_just_identified - n_present))
         coef = np.hstack([coef, padding])
     elif n_samples >= _n_just_identified:
-        coef = fit_ols(x, y, model_info)
+        coef = fit_ols(x, y, weights=None, model_type=model_type)
     else:
-        coef = _fit_minimal_frobenius_norm_of_hessian(x, y, model_info)
+        coef = _fit_minimal_frobenius_norm_of_hessian(x, y)
 
     return coef
 
 
-def _fit_minimal_frobenius_norm_of_hessian(x, y, model_info):
+def _fit_minimal_frobenius_norm_of_hessian(x, y):
     """Fit a quadraitc model using the powell fitting method.
 
     The solution represents the quadratic whose Hessian matrix is of
     minimum Frobenius norm. This has been popularized by Powell and is used in
     many optimizers, e.g. bobyqa and pounders.
 
     For a mathematical exposition, see :cite:`Wild2008`, p. 3-5.
@@ -291,16 +355,14 @@
 
     Args:
         x (np.ndarray): Array of shape (n_samples, n_params) of x-values,
             rescaled such that the trust region becomes a hypercube from -1 to 1.
         y (np.ndarray): Array of shape (n_samples, n_residuals) with function
             evaluations that have been centered around the function value at the
             trust region center.
-        model_info (ModelInfo): Information that describes the functional form of the
-            model.
 
     Returns:
         np.ndarray: The model coefficients.
 
     """
     n_samples, n_params = x.shape
 
@@ -308,27 +370,22 @@
     _n_too_many = n_params + n_params * (n_params + 1) // 2 + 1
 
     if n_samples <= _n_too_few:
         raise ValueError("Too few points for minimum frobenius fitting.")
     if n_samples >= _n_too_many:
         raise ValueError("Too may points for minimum frobenius fitting")
 
-    has_squares = model_info.has_squares
-
-    if has_squares:
-        n_poly_features = n_params * (n_params + 1) // 2
-    else:
-        n_poly_features = n_params * (n_params - 1) // 2
+    n_poly_features = n_second_order_terms(n_params)
 
     (
         m_mat,
         n_mat,
         z_mat,
         n_z_mat,
-    ) = _get_feature_matrices_minimal_frobenius_norm_of_hessian(x, model_info)
+    ) = _get_feature_matrices_minimal_frobenius_norm_of_hessian(x)
 
     coef = _get_current_fit_minimal_frobenius_norm_of_hessian(
         y=y,
         m_mat=m_mat,
         n_mat=n_mat,
         z_mat=z_mat,
         n_z_mat=n_z_mat,
@@ -372,19 +429,19 @@
         coeffs_square[k] = coeffs_second_stage
 
     coef = np.concatenate((coeffs_linear, coeffs_square), axis=1)
 
     return np.atleast_2d(coef)
 
 
-def _get_feature_matrices_minimal_frobenius_norm_of_hessian(x, model_info):
+def _get_feature_matrices_minimal_frobenius_norm_of_hessian(x):
     n_samples, n_params = x.shape
-    has_squares = model_info.has_squares
 
-    features = _polynomial_features(x, has_squares)
+    intercept = np.ones((n_samples, 1))
+    features = np.concatenate((intercept, _quadratic_features(x)), axis=1)
     m_mat, n_mat = np.split(features, (n_params + 1,), axis=1)
 
     m_mat_pad = np.zeros((n_samples, n_samples))
     m_mat_pad[:, : n_params + 1] = m_mat
 
     n_z_mat, _ = qr_multiply(
         m_mat_pad,
@@ -400,51 +457,51 @@
         m_mat[: n_params + 1, : n_params + 1],
         n_mat,
         z_mat[:, n_params + 1 : n_samples],
         n_z_mat[:, n_params + 1 : n_samples],
     )
 
 
-def _build_feature_matrix(x, model_info):
-    if model_info.has_interactions:
-        features = _polynomial_features(x, model_info.has_squares)
-    else:
-        data = (np.ones(len(x)), x)
-        data = (*data, x**2) if model_info.has_squares else data
-        features = np.column_stack(data)
-
+def _build_feature_matrix(x, model_type):
+    raw = x if model_type == "linear" else _quadratic_features(x)
+    intercept = np.ones((len(x), 1))
+    features = np.concatenate((intercept, raw), axis=1)
     return features
 
 
-def _reshape_square_terms_to_hess(square_terms, n_params, n_residuals, has_squares):
-    offset = 0 if has_squares else 1
-    idx1, idx2 = np.triu_indices(n_params, k=offset)
+def _reshape_square_terms_to_hess(square_terms, n_params, n_residuals):
+    idx1, idx2 = np.triu_indices(n_params)
     hess = np.zeros((n_residuals, n_params, n_params), dtype=np.float64)
     hess[:, idx1, idx2] = square_terms
     hess = hess + np.triu(hess).transpose(0, 2, 1)
 
     return hess
 
 
 @njit
-def _polynomial_features(x, has_squares):
+def _quadratic_features(x):
+    # Create fully quadratic features without intercept
     n_samples, n_params = x.shape
-
-    if has_squares:
-        n_poly_terms = n_second_order_terms(n_params)
-    else:
-        n_poly_terms = n_interactions(n_params)
+    n_poly_terms = n_second_order_terms(n_params)
 
     poly_terms = np.empty((n_poly_terms, n_samples), np.float64)
     xt = x.T
 
     idx = 0
     for i in range(n_params):
-        j_start = i if has_squares else i + 1
+        j_start = i
         for j in range(j_start, n_params):
             poly_terms[idx] = xt[i] * xt[j]
             idx += 1
+    out = np.concatenate((xt, poly_terms), axis=0)
+    return out.T
 
-    intercept = np.ones((1, n_samples), x.dtype)
-    out = np.concatenate((intercept, xt, poly_terms), axis=0)
 
-    return out.T
+def _add_weighting(x, y, weights=None):
+    # weight the data in order to get weighted fitting from fitters that do not support
+    # weights. Inspired by: https://stackoverflow.com/a/52452833
+    n_samples = len(x)
+    if weights is not None:
+        _root_weights = np.sqrt(weights).reshape(n_samples, 1)
+        y = y * _root_weights
+        x = x * _root_weights
+    return x, y
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/get_component.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/get_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import functools
 import inspect
 import warnings
 from functools import partial
 
 from estimagic.utilities import propose_alternatives
+from estimagic.optimization.tranquilo.options import update_option_bundle
 
 
 def get_component(
     name_or_func,
     component_name,
     func_dict=None,
     default_options=None,
@@ -23,18 +24,18 @@
     partial all static options into the function.
 
     Args:
         name_or_func (str or callable): Name of a function or function.
         component_name (str): Name of the component. Used in error messages. Examples
             would be "subsolver" or "model".
         func_dict (dict): Dict with function names as keys and functions as values.
-        default_options (dict): Default options for the function. Those will be
-            partialled into the function unless overridden by user_options.
-        user_options (dict): Options for the function. Those will be partialled into
-            the function.
+        default_options (NamedTuple): Default options as a dict or NamedTuple. The
+            default options will be updated by the user options.
+        user_options (NamedTuple, Dict or None): User options as a dict or NamedTuple.
+            The default options will be updated by the user options.
         redundant_option_handling (str): How to handle redundant options. Can be
             "warn", "raise" or "ignore". Default "ignore".
         redundant_argument_handling (str): How to handle redundant arguments passed
             to the processed function at runtime. Can be "warn", "raise" or "ignore".
             Default "ignore".
         mandatory_signature (list): List or tuple of arguments that must be in the
             signature of all functions in `func_dict`. These can be options or
@@ -124,30 +125,30 @@
     name,
     component_name,
     redundant_option_handling,
 ):
     """Get the options that are valid for the function.
 
     Args:
-        default_options (dict): Default options for the function.
-        user_options (dict): Options for the function.
+        default_options (NamedTuple): Default options as a dict or NamedTuple. The
+            default options will be updated by the user options.
+        user_options (NamedTuple, Dict or None): User options as a dict or NamedTuple.
+            The default options will be updated by the user options.
         signature (list): List of arguments that are present in the signature.
         name (str): Name of the function.
         component_name (str): Name of the component. Used in error messages. Examples
             would be "subsolver" or "model".
         redundant_option_handling (str): How to handle redundant options. Can be
 
     Returns:
         dict: Valid options.
 
     """
-    _default_options = {} if default_options is None else default_options
-    _user_options = {} if user_options is None else user_options
-
-    _options = {**_default_options, **_user_options}
+    _options = update_option_bundle(default_options, user_options=user_options)
+    _options = _options._asdict()
 
     _valid_options = {k: v for k, v in _options.items() if k in signature}
     _redundant_options = {k: v for k, v in _options.items() if k not in signature}
 
     if redundant_option_handling == "warn" and _redundant_options:
         msg = (
             f"The following options are not supported by the {component_name} {name} "
@@ -192,16 +193,14 @@
     if _missing:
         msg = (
             f"The following mandatory arguments are missing in the signature of the "
             f"{component_name} {name}: {_missing}."
         )
         raise ValueError(msg)
 
-    return None
-
 
 def _add_redundant_argument_handling(func, signature, warn):
     """Allow func to be called with arguments that are not in the signature.
 
     Args:
         func (callable): The function to be wrapped.
         signature (list): List of arguments that are supported by func.
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/handle_infinity.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/handle_infinity.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/poisedness.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/poisedness.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/sample_points.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/sample_points.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,243 +2,211 @@
 
 import numpy as np
 from scipy.spatial.distance import pdist
 from scipy.special import gammainc, logsumexp
 
 import estimagic as em
 from estimagic.optimization.tranquilo.get_component import get_component
-from estimagic.optimization.tranquilo.options import Bounds
+from estimagic.optimization.tranquilo.options import SamplerOptions
 
 
-def get_sampler(
-    sampler, bounds, model_info=None, radius_factors=None, user_options=None
-):
+def get_sampler(sampler, user_options=None):
     """Get sampling function partialled options.
 
     Args:
         sampler (str or callable): Name of a sampling method or sampling function.
             The arguments of sampling functions need to be: ``trustregion``,
             ``n_points``, ``rng``, ``existing_xs`` and ``bounds``.
             Sampling functions need to return a dictionary with the entry "points"
             (and arbitrary additional information). See ``reference_sampler`` for
             details.
-        bounds (Bounds): A NamedTuple with attributes ``lower`` and ``upper``
         user_options (dict): Additional keyword arguments for the sampler. Options that
             are not used by the sampler are ignored with a warning. If sampler is
             'hull_sampler' or 'optimal_hull_sampler' the user options must contain the
             argument 'order', which is a positive integer.
 
     Returns:
         callable: Function that depends on trustregion, n_points, existing_xs and
-            existing_fvals, model_info and  and returns a new sample.
+            returns a new sample.
 
     """
-
     built_in_samplers = {
-        "box": _box_sampler,
-        "ball": _ball_sampler,
-        "hull_sampler": _hull_sampler,
-        "optimal_hull_sampler": _optimal_hull_sampler,
-        "cube": partial(_hull_sampler, order=np.inf),
-        "sphere": partial(_hull_sampler, order=2),
-        "optimal_cube": partial(_optimal_hull_sampler, order=np.inf),
-        "optimal_sphere": partial(_optimal_hull_sampler, order=2),
-    }
-
-    if (
-        isinstance(sampler, str)
-        and "hull_sampler" in sampler
-        and "order" not in user_options
-    ):
-        msg = (
-            "The hull_sampler and optimal_hull_sampler require the argument 'order' to "
-            "be prespecfied in the user_options dictionary. Order is a positive "
-            "integer. For order = 2 the hull_sampler equals the sphere_sampler, and "
-            "for order = np.inf it equals the cube_sampler."
-        )
-        raise ValueError(msg)
-
-    default_options = {
-        "bounds": bounds,
-        "model_info": model_info,
-        "radius_factors": radius_factors,
+        "random_interior": _interior_sampler,
+        "random_hull": _hull_sampler,
+        "optimal_hull": _optimal_hull_sampler,
     }
 
     mandatory_args = [
-        "bounds",
         "trustregion",
         "n_points",
         "existing_xs",
         "rng",
     ]
 
     out = get_component(
         name_or_func=sampler,
         component_name="sampler",
         func_dict=built_in_samplers,
-        default_options=default_options,
         user_options=user_options,
+        default_options=SamplerOptions(),
         mandatory_signature=mandatory_args,
     )
 
     return out
 
 
-def _box_sampler(
+def _interior_sampler(
     trustregion,
     n_points,
     rng,
     existing_xs=None,  # noqa: ARG001
-    bounds=None,
 ):
-    """Naive random generation of trustregion points inside a box.
+    """Random generation of trustregion points inside a ball or box.
+
+    Args:
+        trustregion (Region): Trustregion. See module region.py.
+        n_points (int): how many new points to sample
+        rng (numpy.random.Generator): Random number generator.
+        existing_xs (np.ndarray or None): 2d numpy array in which each row is an
+            x vector at which the criterion function has already been evaluated, that
+            satisfies lower_bounds <= existing_xs <= upper_bounds.
+
+    """
+    if trustregion.shape == "sphere":
+        _sampler = _ball_sampler
+    else:
+        _sampler = _box_sampler
+
+    out = _sampler(
+        trustregion=trustregion,
+        n_points=n_points,
+        rng=rng,
+    )
+    return out
+
 
-    This is just a reference implementation to illustrate the interface of trustregion
-    samplers. Mathematically it samples uniformaly from inside the cube defined by the
-    intersection of the trustregion and the bounds.
-
-    All arguments but seed are mandatory, even if not used.
-
-    Samplers should not make unnecessary checks on input compatibility (e.g. that the
-    shapes of existing_xs and existing_fvals match). This will be done automatically
-    outside of the sampler.
+def _box_sampler(
+    trustregion,
+    n_points,
+    rng,
+):
+    """Naive random generation of trustregion points inside a box.
 
     Args:
-        trustregion (TrustRegion): NamedTuple with attributes center and radius.
+        trustregion (Region): Trustregion. See module region.py.
         n_points (int): how many new points to sample
         rng (numpy.random.Generator): Random number generator.
         existing_xs (np.ndarray or None): 2d numpy array in which each row is an
             x vector at which the criterion function has already been evaluated, that
             satisfies lower_bounds <= existing_xs <= upper_bounds.
-        bounds (Bounds or None): NamedTuple.
 
     """
     n_params = len(trustregion.center)
-    effective_bounds = _get_effective_bounds(trustregion, bounds=bounds)
-
+    bounds = trustregion.cube_bounds
     points = rng.uniform(
-        low=effective_bounds.lower,
-        high=effective_bounds.upper,
+        low=bounds.lower,
+        high=bounds.upper,
         size=(n_points, n_params),
     )
     return points
 
 
 def _ball_sampler(
-    trustregion, n_points, rng, existing_xs=None, bounds=None  # noqa: ARG001
+    trustregion,
+    n_points,
+    rng,
 ):
     """Naive random generation of trustregion points inside a ball.
 
-    Mathematically it samples uniformaly from inside the ball defined by the
-    intersection of the trustregion and the bounds.
-
     Code is adapted from https://tinyurl.com/y3p2dz6b.
 
     Args:
-        trustregion (TrustRegion): NamedTuple with attributes center and radius.
+        trustregion (Region): Trustregion. See module region.py.
         n_points (int): how many new points to sample
         rng (numpy.random.Generator): Random number generator.
         existing_xs (np.ndarray or None): 2d numpy array in which each row is an
             x vector at which the criterion function has already been evaluated, that
             satisfies lower_bounds <= existing_xs <= upper_bounds.
-        bounds (Bounds or None): NamedTuple.
 
     """
     n_params = len(trustregion.center)
-    effective_bounds = _get_effective_bounds(trustregion, bounds=bounds)
-
     raw = rng.normal(size=(n_points, n_params))
     norm = np.linalg.norm(raw, axis=1, ord=2)
     scale = gammainc(n_params / 2, norm**2 / 2) ** (1 / n_params) / norm
     points = raw * scale.reshape(-1, 1)
-
-    out = _map_into_feasible_trustregion(points, bounds=effective_bounds)
+    out = trustregion.map_from_unit(points)
     return out
 
 
 def _hull_sampler(
     trustregion,
     n_points,
     rng,
-    order,
-    distribution=None,
+    distribution,
     existing_xs=None,  # noqa: ARG001
-    bounds=None,
 ):
     """Random generation of trustregion points on the hull of general sphere / cube.
 
-    Points are sampled randomly on a hull (of a sphere for order=2 and of a cube for
-    order=np.inf). These points are then mapped into the feasible region, which is
-    defined by the intersection of the trustregion and the bounds.
+    Points are sampled randomly on a hull of a sphere or cube. These points are then
+    mapped into the feasible region, which is defined by the intersection of the
+    trustregion and the bounds.
 
     Args:
-        trustregion (TrustRegion): NamedTuple with attributes center and radius.
+        trustregion (Region): Trustregion. See module region.py.
         n_points (int): how many new points to sample
         rng (numpy.random.Generator): Random number generator.
-        order (int): Type of norm to use when scaling the sampled points. For 2 it will
-            result in sphere sampling, for np.inf in cube sampling.
         distribution (str): Distribution to use for initial sample before points are
             projected onto unit hull. Must be in {'normal', 'uniform'}.
         existing_xs (np.ndarray or None): 2d numpy array in which each row is an
             x vector at which the criterion function has already been evaluated, that
             satisfies lower_bounds <= existing_xs <= upper_bounds.
-        bounds (Bounds or None): NamedTuple.
 
     """
     n_params = len(trustregion.center)
-    effective_bounds = _get_effective_bounds(trustregion, bounds=bounds)
 
     if distribution is None:
-        distribution = "normal" if order <= 3 else "uniform"
-    points = _draw_from_distribution(distribution, rng=rng, size=(n_points, n_params))
-    points = _project_onto_unit_hull(points, order=order)
-    points = _map_into_feasible_trustregion(points, bounds=effective_bounds)
-    return points
+        distribution = "normal" if trustregion.shape == "sphere" else "uniform"
+    raw = _draw_from_distribution(distribution, rng=rng, size=(n_points, n_params))
+    points = _project_onto_unit_hull(raw, trustregion_shape=trustregion.shape)
+    out = trustregion.map_from_unit(points)
+    return out
 
 
 def _optimal_hull_sampler(
     trustregion,
     n_points,
     rng,
-    model_info,  # noqa: ARG001
-    radius_factors,
-    order,
-    distribution=None,
-    hardness=1,
+    distribution,
+    hardness,
+    algorithm,
+    algo_options,
+    criterion,
+    n_points_randomsearch,
+    return_info,
     existing_xs=None,
-    bounds=None,
-    algorithm="scipy_lbfgsb",
-    algo_options=None,
-    criterion=None,
 ):
     """Optimal generation of trustregion points on the hull of general sphere / cube.
 
-    Points are sampled optimally on a hull (of a sphere for order=2 and of a cube for
-    order=np.inf), where the criterion that is maximized is the minimum distance of all
-    pairs of points, except for pairs of existing points. These points are then mapped
-    into the feasible region, which is defined by the intersection of the trustregion
-    and the bounds. Instead of using a hard minimum we return the soft minimum, whose
-    accuracy we govern by the hardness factor. For more information on the soft-minimum,
-    seek: https://tinyurl.com/mrythbk4.
+    Points are sampled optimally on a hull of a sphere or cube, where the criterion that
+    is maximized is the minimum distance of all pairs of points, except for pairs of
+    existing points. These points are then mapped into the feasible region, which is
+    defined by the intersection of the trustregion and the bounds. Instead of using a
+    hard minimum we return the soft minimum, whose accuracy we govern by the hardness
+    factor. For more information on the soft-minimum, seek:
+    https://tinyurl.com/mrythbk4.
 
     Args:
-        trustregion (TrustRegion): NamedTuple with attributes center and radius.
+        trustregion (Region): Trustregion. See module region.py.
         n_points (int): how many new points to sample
         rng (numpy.random.Generator): Random number generator.
-        order (int): Type of norm to use when scaling the sampled points. For 2 it will
-            result in sphere sampling, for np.inf in cube sampling.
         distribution (str): Distribution to use for initial sample before points are
             projected onto unit hull. Must be in {'normal', 'uniform'}.
         hardness (float): Positive scaling factor. As hardness tends to infinity the
             soft minimum (logsumexp) approaches the hard minimum. Default is 1. A
             detailed explanation is given in the docstring.
-        existing_xs (np.ndarray or None): 2d numpy array in which each row is an
-            x vector at which the criterion function has already been evaluated, that
-            satisfies lower_bounds <= existing_xs <= upper_bounds.
-        bounds (Bounds or None): NamedTuple.
         algorithm (str): Optimization algorithm.
         algo_options (dict): Algorithm specific configuration of the optimization. See
             :ref:`list_of_algorithms` for supported options of each algorithm. Default
             sets ``stopping_max_iterations=n_params``.
         criterion (str or None): "distance", "determinant" or None.
             - "distance": maximize the minimal distance between points, excluding
               distances between existing points. This is a fast and relatively simple
@@ -247,136 +215,167 @@
             - "determinant": maximize the determinant of the x'x where x is the matrix
               of points. This is known as d-optimality in the optimal design literature
               and as fekete points in the function approximation literature. This
               criterion has the best theoretical properties but is very hard to
               optimize. Thus the practical performance can be bad.
             - None: Use the "determinant" criterion if only one point is added and the
               "distance" criterion if multiple points are added.
+        n_points_randomsearch (int): Number of random points to from which to select
+            the best in terms of the Fekete criterion before starting the optimization.
+            Default is 1.
+        existing_xs (np.ndarray or None): 2d numpy array in which each row is an
+            x vector at which the criterion function has already been evaluated, that
+            satisfies lower_bounds <= existing_xs <= upper_bounds.
 
     Returns:
-        np.ndarray: Generated points. Has shape (n_points, len(trustregion.center)).
+        - np.ndarray: Generated points. Has shape (n_points, len(trustregion.center)).
+        - dict: Information about the optimization. Only returned if ``return_info`` is
+        True.
 
     """
     n_params = len(trustregion.center)
 
     if n_points <= 0:
         return np.array([])
 
     if criterion is None:
-        if n_points == 1:
-            criterion = "determinant"
-        else:
-            criterion = "distance"
+        criterion = "determinant" if n_points == 1 else "distance"
 
     algo_options = {} if algo_options is None else algo_options
     if "stopping_max_iterations" not in algo_options:
         algo_options["stopping_max_iterations"] = 2 * n_params + 5
 
-    effective_bounds = _get_effective_bounds(trustregion, bounds=bounds)
-
     if existing_xs is not None:
         # map existing points into unit space for easier optimization
-        existing_xs_unit = _map_from_feasible_trustregion(existing_xs, effective_bounds)
+
+        existing_xs_unit = trustregion.map_to_unit(existing_xs)
 
         if criterion == "distance":
             dist_to_center = np.linalg.norm(existing_xs_unit, axis=1)
-            not_centric = dist_to_center >= radius_factors.centric
+            not_centric = dist_to_center >= 0.1
             if not_centric.any():
                 existing_xs_unit = existing_xs_unit[not_centric]
             else:
                 existing_xs_unit = None
 
     else:
         existing_xs_unit = None
 
-    # start params
+    # Define criterion functions. "determinant" is the Fekete criterion and "distance"
+    # corresponds to an approximation of the Fekete criterion.
+    criterion_kwargs = {
+        "existing_xs": existing_xs_unit,
+        "trustregion_shape": trustregion.shape,
+        "n_params": n_params,
+    }
+
+    func_dict = {
+        "determinant": partial(_determinant_on_hull, **criterion_kwargs),
+        "distance": partial(
+            _minimal_pairwise_distance_on_hull,
+            **criterion_kwargs,
+            hardness=hardness,
+        ),
+    }
+
+    # Select start params through random search
     if distribution is None:
-        distribution = "normal" if order <= 3 else "uniform"
-    x0 = _draw_from_distribution(distribution, rng=rng, size=(n_points, n_params))
-    x0 = _project_onto_unit_hull(x0, order=order)
+        distribution = "normal" if trustregion.shape == "sphere" else "uniform"
+
+    candidates = _draw_from_distribution(
+        distribution, rng=rng, size=(n_points_randomsearch, n_points, n_params)
+    )
+    candidates = [
+        _project_onto_unit_hull(_x, trustregion_shape=trustregion.shape)
+        for _x in candidates
+    ]
+
+    if n_points_randomsearch == 1:
+        x0 = candidates[0]
+    else:
+        _fekete_criterion = [func_dict["determinant"](_x) for _x in candidates]
+        x0 = candidates[np.argmax(_fekete_criterion)]
+
     x0 = x0.flatten()  # flatten so that em.maximize uses fast path
 
     # This would raise an error because there are zero pairs to calculate the
     # pairwise distance
     if existing_xs_unit is None and n_points == 1:
         opt_params = x0
     else:
-        criterion_kwargs = {
-            "existing_xs": existing_xs_unit,
-            "order": order,
-            "n_params": n_params,
-        }
-
-        func_dict = {
-            "determinant": partial(_determinant_on_hull, **criterion_kwargs),
-            "distance": partial(
-                _minimal_pairwise_distance_on_hull,
-                **criterion_kwargs,
-                hardness=hardness,
-            ),
-        }
-
         res = em.maximize(
             criterion=func_dict[criterion],
             params=x0,
             algorithm=algorithm,
             lower_bounds=-np.ones_like(x0),
             upper_bounds=np.ones_like(x0),
             algo_options=algo_options,
         )
-
         opt_params = res.params
 
     # Make sure the optimal sampling is actually better than the initial one with
     # respect to the fekete criterion. This could be violated if the surrogate
     # criterion is not a good approximation or if the optimization fails.
     start_fekete = func_dict["determinant"](x0)
     end_fekete = func_dict["determinant"](opt_params)
 
     if start_fekete >= end_fekete:
         opt_params = x0
 
-    points = _project_onto_unit_hull(opt_params.reshape(-1, n_params), order=order)
-    points = _map_into_feasible_trustregion(points, bounds=effective_bounds)
-    return points
+    points = _project_onto_unit_hull(
+        opt_params.reshape(-1, n_params), trustregion_shape=trustregion.shape
+    )
+    points = trustregion.map_from_unit(points)
+
+    # Collect additional information. Mostly used for testing.
+    info = {
+        "start_params": x0,
+        "opt_params": opt_params,
+        "start_fekete": start_fekete,
+        "opt_fekete": end_fekete,
+    }
+
+    out = (points, info) if return_info else points
+    return out
 
 
 # ======================================================================================
 # Helper functions
 # ======================================================================================
 
 
-def _minimal_pairwise_distance_on_hull(x, existing_xs, order, hardness, n_params):
+def _minimal_pairwise_distance_on_hull(
+    x, existing_xs, trustregion_shape, hardness, n_params
+):
     """Compute minimal pairwise distance of new and existing points.
 
     Instead of optimizing the distance of points in the feasible trustregion, this
     criterion function leads to the maximization of the minimum distance of the points
     in the unit space. These can then be mapped into the feasible trustregion. We do not
     consider the distances between existing points. Instead of using a hard minimum we
     return the soft minimum, whose accuracy we govern by the hardness factor. For more
     information on the soft-minimum, seek: https://tinyurl.com/mrythbk4.
 
     Args:
         x (np.ndarray): Flattened 1d array of internal points. Each value is in [-1, 1].
         existing_xs (np.ndarray or None): 2d numpy array in which each row is an
             x vector at which the criterion function has already been evaluated, that
             satisfies -1 <= existing_xs <= 1.
-        order (int): Type of norm to use when scaling the sampled points. For 2 we
-            project onto the hull of a sphere, for np.inf onto the hull of a cube.
+        trustregion_shape (str): Shape of the trustregion. Either "cube" or "sphere".
         hardness (float): Positive scaling factor. As hardness tends to infinity the
             soft minimum (logsumexp) approaches the hard minimum. Default is 1. A
             detailed explanation is given in the docstring.
         n_params (int): Dimensionality of the problem.
 
     Returns:
         float: The criterion value.
 
     """
     x = x.reshape(-1, n_params)
-    x = _project_onto_unit_hull(x, order=order)
+    x = _project_onto_unit_hull(x, trustregion_shape=trustregion_shape)
 
     if existing_xs is not None:
         sample = np.row_stack([x, existing_xs])
         n_existing_pairs = len(existing_xs) * (len(existing_xs) - 1) // 2
         slc = slice(0, -n_existing_pairs) if n_existing_pairs else slice(None)
     else:
         sample = x
@@ -388,38 +387,37 @@
     dist = dist[slc]
 
     # soft minimum
     crit_value = -logsumexp(-hardness * dist)
     return crit_value
 
 
-def _determinant_on_hull(x, existing_xs, order, n_params):
+def _determinant_on_hull(x, existing_xs, trustregion_shape, n_params):
     """Compute d-optimality criterion of new and existing points.
 
     Instead of optimizing the distance of points in the feasible trustregion, this
     criterion function leads to the maximization of the minimum distance of the points
     in the unit space.
 
     Args:
         x (np.ndarray): Flattened 1d array of internal points. Each value is in [-1, 1].
         existing_xs (np.ndarray or None): 2d numpy array in which each row is an
             x vector at which the criterion function has already been evaluated, that
             satisfies -1 <= existing_xs <= 1.
-        order (int): Type of norm to use when scaling the sampled points. For 2 we
-            project onto the hull of a sphere, for np.inf onto the hull of a cube.
+        trustregion_shape (str): Shape of the trustregion. Either "cube" or "sphere".
         n_params (int): Dimensionality of the problem.
 
     Returns:
         float: The criterion value.
 
     """
     x = x.reshape(-1, n_params)
     n_samples = len(x)
 
-    x = _project_onto_unit_hull(x, order=order)
+    x = _project_onto_unit_hull(x, trustregion_shape=trustregion_shape)
 
     if existing_xs is not None:
         sample = np.row_stack([x, existing_xs])
     else:
         sample = x
 
     crit_value = np.linalg.det(sample.T @ sample / n_samples)
@@ -447,67 +445,22 @@
     else:
         raise ValueError(
             f"distribution is {distribution}, but needs to be in ('normal', 'uniform')."
         )
     return draw
 
 
-def _map_into_feasible_trustregion(points, bounds):
-    """Map points from the unit space into trustregion defined by bounds.
-
-    Args:
-        points (np.ndarray): 2d array of points to be mapped. Each value is in [-1, 1].
-        bounds (Bounds): A NamedTuple with attributes ``lower`` and ``upper``, where
-            lower and upper define the rectangle that is the feasible trustregion.
-
-    Returns:
-        np.ndarray: Points in trustregion.
-
-    """
-    out = (bounds.upper - bounds.lower) * (points + 1) / 2 + bounds.lower
-    return out
-
-
-def _map_from_feasible_trustregion(points, bounds):
-    """Map points from a feasible trustregion definde by bounds into unit space.
-
-    Args:
-        points (np.ndarray): 2d array of points to be mapped. Each value is in [-1, 1].
-        bounds (Bounds): A NamedTuple with attributes ``lower`` and ``upper``, where
-            lower and upper define the rectangle that is the feasible trustregion.
-
-    Returns:
-        np.ndarray: Points in unit space.
-
-    """
-    out = 2 * (points - bounds.lower) / (bounds.upper - bounds.lower) - 1
-    return out
-
-
-def _project_onto_unit_hull(x, order):
+def _project_onto_unit_hull(x, trustregion_shape):
     """Project points from the unit space onto the hull of a geometric figure.
 
     Args:
         x (np.ndarray): 2d array of points to be projects. Each value is in [-1, 1].
-        order (int): Type of norm to use when scaling the sampled points. For 2 we
-            project onto the hull of a sphere, for np.inf onto the hull of a cube.
+        trustregion_shape (str): Shape of the trustregion: {'sphere', 'cube'}.
 
     Returns:
         np.ndarray: The projected points.
 
     """
+    order = 2 if trustregion_shape == "sphere" else np.inf
     norm = np.linalg.norm(x, axis=1, ord=order).reshape(-1, 1)
     projected = x / norm
     return projected
-
-
-def _get_effective_bounds(trustregion, bounds):
-    lower_bounds = trustregion.center - trustregion.radius
-    upper_bounds = trustregion.center + trustregion.radius
-
-    if bounds is not None and bounds.lower is not None:
-        lower_bounds = np.clip(lower_bounds, bounds.lower, np.inf)
-
-    if bounds is not None and bounds.upper is not None:
-        upper_bounds = np.clip(upper_bounds, -np.inf, bounds.upper)
-
-    return Bounds(lower=lower_bounds, upper=upper_bounds)
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/tranquilo.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/tranquilo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,439 +1,420 @@
-import numbers
-import warnings
+import functools
 from functools import partial
 from typing import NamedTuple
 
 import numpy as np
 
 from estimagic.decorators import mark_minimizer
 from estimagic.optimization.tranquilo.adjust_radius import adjust_radius
-from estimagic.optimization.tranquilo.aggregate_models import get_aggregator
-from estimagic.optimization.tranquilo.count_points import get_counter
-from estimagic.optimization.tranquilo.filter_points import get_sample_filter
-from estimagic.optimization.tranquilo.fit_models import get_fitter
-from estimagic.optimization.tranquilo.handle_infinity import get_infinity_handler
+from estimagic.optimization.tranquilo.filter_points import (
+    drop_worst_points,
+)
 from estimagic.optimization.tranquilo.models import (
-    ModelInfo,
     ScalarModel,
-    n_free_params,
-)
-from estimagic.optimization.tranquilo.options import (
-    Bounds,
-    ConvOptions,
-    HistorySearchOptions,
-    RadiusFactors,
-    RadiusOptions,
-    TrustRegion,
+    VectorModel,
 )
-from estimagic.optimization.tranquilo.sample_points import get_sampler
-from estimagic.optimization.tranquilo.solve_subproblem import get_subsolver
-from estimagic.optimization.tranquilo.tranquilo_history import History
-from estimagic.optimization.tranquilo.weighting import get_sample_weighter
-from estimagic.optimization.tranquilo.wrap_criterion import get_wrapped_criterion
-
-
-def _tranquilo(
-    criterion,
-    x,
-    functype,
-    lower_bounds=None,
-    upper_bounds=None,
-    disable_convergence=False,
-    stopping_max_iterations=200,
-    random_seed=925408,
-    sampler=None,
-    sample_filter=None,
-    filter_options=None,
-    fitter=None,
-    subsolver=None,
-    sample_size=None,
-    surrogate_model=None,
-    radius_options=None,
-    radius_factors=None,
-    sampler_options=None,
-    counter="count_all",
-    weighter="no_weights",
-    fit_options=None,
-    solver_options=None,
-    conv_options=None,
-    batch_evaluator="joblib",
-    n_cores=1,
-    silence_experimental_warning=False,
-    infinity_handling="relative",
-    history_search_options=None,
-):
-    """Find the local minimum to a noisy optimization problem.
-
-    Args:
-        criterion (callable): Function that return values of the objective function.
-        x (np.ndarray): Initial guess for the parameter vector.
-        functype (str): String indicating whether the criterion is a scalar, a
-            likelihood function or a least-square type of function. Valid arguments
-            are:
-            - "scalar"
-            - "likelihood"
-            - "least_squares"
-        lower_bounds (np.ndarray or NoneTeyp): 1d array of shape (n,) with lower bounds
-            for the parameter vector x.
-        upper_bounds (np.ndarray or NoneTeyp): 1d array of shape (n,) with upper bounds
-            for the parameter vector x.
-        disable_convergence (bool): If True, check for convergence criterion and stop
-            the iterations.
-        stopping_max_iterations (int): Maximum number of iterations to run.
-        random_seed (int): The seed used in random number generation.
-        sample_filter (str): The method used to filter points in the current trust
-            region.
-        sampler (str): The sampling method used to sample points from the current
-            trust region.
-        fitter (str): The method used to fit the surrogate model.
-        subsolver (str): The algorithm used for solving the nested surrogate model.
-        sample_size (str): Target sample size. One of:
-            - "linear": n + 1
-            - "powell": 2 * n + 1
-            - "quadratic: 0.5 * n * (n + 1) + n + 1
-        surrogate_model (str): Type of surrogate model to fit. Both a "linear" and
-            "quadratic" surrogate model are supported.
-        radius_options (NemdTuple or NoneType): Options for trust-region radius
-            management.
-        sampler_options (dict or NoneType): Additional keyword arguments passed to the
-            sampler function.
-        fit_options (dict or NoneType): Additional keyword arguments passed to the
-            fitter function.
-        solver_options (dict or NoneType): Additional keyword arguments passed to the
-            sub-solver function.
-        conv_options (NamedTuple or NoneType): Criteria for successful convergence.
-        batch_evaluator (str or callabler)
-        n_cores (int): Number of cores.
-
-    Returns:
-        (dict): Results dictionary with the following items:
-            - solution_x (np.ndarray): Solution vector of shape (n,).
-            - solution_criterion (np.ndarray): Values of the criterion function at the
-                solution vector. Shape (n_obs,).
-            - states (list): The history of optimization as a list of the State objects.
-            - message (str or NoneType): Message stating which convergence criterion,
-                if any has been reached at the end of optimization
-
-    """
-    # ==================================================================================
-    # experimental warning
-    # ==================================================================================
-    if not silence_experimental_warning:
-        warnings.warn(
-            "Tranquilo is extremely experimental. algo_options and results will change "
-            "frequently and without notice. Do not use."
-        )
-
-    # ==================================================================================
-    # set default values for optional arguments
-    # ==================================================================================
-    sampling_rng = np.random.default_rng(random_seed)
-
-    if sample_filter is None:
-        sample_filter = "clustering" if functype == "scalar" else "keep_all"
-
-    if radius_options is None:
-        radius_options = RadiusOptions()
-    if radius_factors is None:
-        radius_factors = RadiusFactors()
-    if sampler_options is None:
-        sampler_options = {}
-    if fit_options is None:
-        fit_options = {}
-    if solver_options is None:
-        solver_options = {}
-
-    model_info = _process_surrogate_model(
-        surrogate_model=surrogate_model,
-        functype=functype,
-    )
+from estimagic.optimization.tranquilo.process_arguments import process_arguments
+from estimagic.optimization.tranquilo.region import Region
 
-    if _has_bounds(lower_bounds, upper_bounds):
-        if sampler is None:
-            sampler = "optimal_cube"
-        if subsolver is None:
-            subsolver = "bntr_fast"
-    else:
-        if sampler is None:
-            sampler = "optimal_sphere"
-        if subsolver is None:
-            subsolver = "gqtpar_fast"
-
-    target_sample_size = _process_sample_size(
-        user_sample_size=sample_size,
-        model_info=model_info,
-        x=x,
-    )
 
-    if fitter is None:
-        fitter = "ols"
+# wrapping gives us the signature and docstring of process arguments
+@functools.wraps(process_arguments)
+def _tranquilo(*args, **kwargs):
+    internal_kwargs = process_arguments(*args, **kwargs)
+    return _internal_tranquilo(**internal_kwargs)
 
-    if functype == "scalar":
-        aggregator = "identity"
-    elif functype == "likelihood":
-        aggregator = "information_equality_linear"
-    elif functype == "least_squares":
-        aggregator = "least_squares_linear"
-    else:
-        raise ValueError(f"Invalid functype: {functype}")
 
-    if conv_options is None:
-        conv_options = ConvOptions()
-
-    if history_search_options is None:
-        if functype == "scalar":
-            history_search_options = HistorySearchOptions(radius_factor=1.0)
-        else:
-            history_search_options = HistorySearchOptions()
-
-    # ==================================================================================
-    # initialize compoments for the solver
-    # ==================================================================================
-
-    history = History(functype=functype)
-
-    wrapped_criterion = get_wrapped_criterion(
-        criterion=criterion,
-        batch_evaluator=batch_evaluator,
-        n_cores=n_cores,
-        history=history,
-    )
-
-    bounds = Bounds(lower=lower_bounds, upper=upper_bounds)
-    sample_points = get_sampler(
-        sampler,
-        bounds=bounds,
-        model_info=model_info,
-        radius_factors=radius_factors,
-        user_options=sampler_options,
-    )
-    filter_points = get_sample_filter(sample_filter, user_options=filter_options)
+def _internal_tranquilo(
+    evaluate_criterion,
+    x,
+    noisy,
+    conv_options,
+    stop_options,
+    radius_options,
+    batch_size,
+    target_sample_size,
+    stagnation_options,
+    search_radius_factor,
+    n_evals_per_point,
+    n_evals_at_start,
+    trustregion,
+    sampling_rng,
+    history,
+    sample_points,
+    solve_subproblem,
+    filter_points,
+    fit_model,
+    aggregate_model,
+    estimate_variance,
+    accept_candidate,
+):
+    eval_info = {0: n_evals_at_start}
 
-    aggregate_vector_model = get_aggregator(
-        aggregator=aggregator,
-        functype=functype,
-        model_info=model_info,
-    )
+    evaluate_criterion(eval_info)
 
-    fit_model = get_fitter(
-        fitter=fitter,
-        user_options=fit_options,
-        model_info=model_info,
-    )
+    _init_fvec = history.get_fvecs(0).mean(axis=0)
 
-    solve_subproblem = get_subsolver(
-        solver=subsolver,
-        user_options=solver_options,
-        bounds=bounds,
+    _init_vector_model = VectorModel(
+        intercepts=_init_fvec,
+        linear_terms=np.zeros((len(_init_fvec), len(x))),
+        square_terms=np.zeros((len(_init_fvec), len(x), len(x))),
+        shift=trustregion.center,
+        scale=trustregion.radius,
     )
 
-    count_points = get_counter(counter, bounds=bounds)
-
-    calculate_weights = get_sample_weighter(weighter, bounds=bounds)
-
-    clip_infinite_values = get_infinity_handler(infinity_handling)
-
-    _, _first_fval, _first_indices = wrapped_criterion(x)
+    _init_model = aggregate_model(_init_vector_model)
 
     state = State(
-        safety=False,
-        trustregion=TrustRegion(center=x, radius=radius_options.initial_radius),
-        model_indices=_first_indices,
-        model=None,
+        trustregion=trustregion,
+        model_indices=[0],
+        model=_init_model,
+        vector_model=_init_vector_model,
         index=0,
         x=x,
-        fval=_first_fval,
+        fval=np.mean(history.get_fvals(0)),
         rho=np.nan,
         accepted=True,
-        new_indices=_first_indices,
-        old_indices_discarded=_first_indices,
-        old_indices_used=_first_indices,
+        new_indices=[0],
+        old_indices_discarded=[],
+        old_indices_used=[],
+        candidate_index=0,
+        candidate_x=x,
     )
 
     states = [state]
 
     # ==================================================================================
     # main optimization loop
     # ==================================================================================
     converged, msg = False, None
-    for _ in range(stopping_max_iterations):
+    for _ in range(stop_options.max_iter):
         # ==============================================================================
         # find, filter and count points
         # ==============================================================================
-        old_indices = history.get_indices_in_trustregion(
-            state.trustregion,
-            search_options=history_search_options,
+
+        search_region = state.trustregion._replace(
+            radius=search_radius_factor * state.trustregion.radius
         )
+
+        old_indices = history.get_x_indices_in_region(search_region)
+
         old_xs = history.get_xs(old_indices)
 
-        filtered_xs, filtered_indices = filter_points(
+        model_xs, model_indices = filter_points(
             xs=old_xs,
             indices=old_indices,
             state=state,
             target_size=target_sample_size,
         )
 
-        n_effective_points = count_points(filtered_xs, trustregion=state.trustregion)
-
-        # ==============================================================================
-        # sample new points
-        # ==============================================================================
-        n_to_sample = max(0, target_sample_size - n_effective_points)
-
+        # ==========================================================================
+        # sample points if necessary and do simple iteration
+        # ==========================================================================
         new_xs = sample_points(
             trustregion=state.trustregion,
-            n_points=n_to_sample,
-            existing_xs=filtered_xs,
+            n_points=max(0, target_sample_size - len(model_xs)),
+            existing_xs=model_xs,
             rng=sampling_rng,
         )
 
-        # ==============================================================================
-        # criterion evaluations
-        # ==============================================================================
-
-        _, _, new_indices = wrapped_criterion(new_xs)
-        model_indices = np.hstack([filtered_indices, new_indices])
-        model_xs = history.get_xs(model_indices)
-        model_fvecs = history.get_fvecs(model_indices)
+        new_indices = history.add_xs(new_xs)
 
-        # ==============================================================================
-        # build surrogate and optimize it
-        # ==============================================================================
+        eval_info = {i: n_evals_per_point for i in new_indices}
 
-        weights = calculate_weights(model_xs, trustregion=state.trustregion)
+        evaluate_criterion(eval_info)
 
-        centered_xs = (model_xs - state.trustregion.center) / state.trustregion.radius
+        model_indices = _concatenate_indices(model_indices, new_indices)
 
-        clipped_fvecs = clip_infinite_values(model_fvecs)
+        model_xs = history.get_xs(model_indices)
+        model_data = history.get_model_data(
+            x_indices=model_indices,
+            average=True,
+        )
 
-        vector_model = fit_model(centered_xs, clipped_fvecs, weights=weights)
+        vector_model = fit_model(
+            *model_data,
+            region=state.trustregion,
+            old_model=state.vector_model,
+            weights=None,
+        )
 
-        scalar_model = aggregate_vector_model(
+        scalar_model = aggregate_model(
             vector_model=vector_model,
         )
 
         sub_sol = solve_subproblem(model=scalar_model, trustregion=state.trustregion)
 
+        _relative_step_length = (
+            np.linalg.norm(sub_sol.x - state.x) / state.trustregion.radius
+        )
+
+        # ==========================================================================
+        # If we have enough points, drop points until the relative step length
+        # becomes large enough
+        # ==========================================================================
+
+        if len(model_xs) > target_sample_size:
+            while (
+                _relative_step_length < stagnation_options.min_relative_step_keep
+                and len(model_xs) > target_sample_size
+            ):
+                model_xs, model_indices = drop_worst_points(
+                    xs=model_xs,
+                    indices=model_indices,
+                    state=state,
+                    n_to_drop=1,
+                )
+
+                model_data = history.get_model_data(
+                    x_indices=model_indices,
+                    average=True,
+                )
+
+                vector_model = fit_model(
+                    *model_data,
+                    region=state.trustregion,
+                    old_model=state.vector_model,
+                    weights=None,
+                )
+
+                scalar_model = aggregate_model(
+                    vector_model=vector_model,
+                )
+
+                sub_sol = solve_subproblem(
+                    model=scalar_model, trustregion=state.trustregion
+                )
+
+                _relative_step_length = (
+                    np.linalg.norm(sub_sol.x - state.x) / state.trustregion.radius
+                )
+
+        # ==========================================================================
+        # If step length is still too small, replace the worst point with a new one
+        # ==========================================================================
+
+        sample_counter = 0
+        while _relative_step_length < stagnation_options.min_relative_step:
+            if stagnation_options.drop:
+                model_xs, model_indices = drop_worst_points(
+                    xs=model_xs,
+                    indices=model_indices,
+                    state=state,
+                    n_to_drop=stagnation_options.sample_increment,
+                )
+
+            new_xs = sample_points(
+                trustregion=state.trustregion,
+                n_points=stagnation_options.sample_increment,
+                existing_xs=model_xs,
+                rng=sampling_rng,
+            )
+
+            new_indices = history.add_xs(new_xs)
+
+            eval_info = {i: n_evals_per_point for i in new_indices}
+
+            evaluate_criterion(eval_info)
+
+            model_indices = _concatenate_indices(model_indices, new_indices)
+            model_xs = history.get_xs(model_indices)
+            model_data = history.get_model_data(
+                x_indices=model_indices,
+                average=True,
+            )
+
+            vector_model = fit_model(
+                *model_data,
+                region=state.trustregion,
+                old_model=state.vector_model,
+                weights=None,
+            )
+
+            scalar_model = aggregate_model(
+                vector_model=vector_model,
+            )
+
+            sub_sol = solve_subproblem(
+                model=scalar_model, trustregion=state.trustregion
+            )
+
+            _relative_step_length = (
+                np.linalg.norm(sub_sol.x - state.x) / state.trustregion.radius
+            )
+
+            sample_counter += 1
+            if sample_counter >= stagnation_options.max_trials:
+                break
+
         # ==============================================================================
-        # acceptance decision
+        # fit noise model based on previous acceptance samples
         # ==============================================================================
 
-        candidate_x = sub_sol["x"]
+        if noisy:
+            scalar_noise_variance = estimate_variance(
+                trustregion=state.trustregion,
+                history=history,
+                model_type="scalar",
+            )
+        else:
+            scalar_noise_variance = None
 
-        _, candidate_fval, candidate_index = wrapped_criterion(candidate_x)
-        actual_improvement = -(candidate_fval - state.fval)
+        # ==============================================================================
+        # acceptance decision
+        # ==============================================================================
 
-        rho = _calculate_rho(
-            actual_improvement=actual_improvement,
-            expected_improvement=sub_sol["expected_improvement"],
+        acceptance_result = accept_candidate(
+            subproblem_solution=sub_sol,
+            state=state,
+            wrapped_criterion=evaluate_criterion,
+            noise_variance=scalar_noise_variance,
+            history=history,
         )
 
-        is_accepted = actual_improvement > 0
-
         # ==============================================================================
         # update state with information on this iteration
         # ==============================================================================
 
         state = state._replace(
             model_indices=model_indices,
             model=scalar_model,
-            rho=rho,
-            accepted=is_accepted,
-            new_indices=new_indices,
-            old_indices_used=filtered_indices,
-            old_indices_discarded=np.setdiff1d(old_indices, filtered_indices),
+            new_indices=np.setdiff1d(model_indices, old_indices),
+            old_indices_used=np.intersect1d(model_indices, old_indices),
+            old_indices_discarded=np.setdiff1d(old_indices, model_indices),
+            **acceptance_result._asdict(),
         )
 
-        if is_accepted:
-            state = state._replace(
-                index=candidate_index,
-                x=candidate_x,
-                fval=candidate_fval,
-            )
-
         states.append(state)
 
         # ==============================================================================
         # update state for beginning of next iteration
         # ==============================================================================
 
         new_radius = adjust_radius(
             radius=state.trustregion.radius,
-            rho=rho,
-            step=candidate_x - state.trustregion.center,
+            rho=acceptance_result.rho,
+            step_length=acceptance_result.step_length,
             options=radius_options,
         )
 
-        if is_accepted:
-            new_trustregion = state.trustregion._replace(
-                center=candidate_x, radius=new_radius
-            )
-        else:
-            new_trustregion = state.trustregion._replace(radius=new_radius)
+        new_trustregion = state.trustregion._replace(
+            center=acceptance_result.x, radius=new_radius
+        )
 
         state = state._replace(trustregion=new_trustregion)
 
         # ==============================================================================
         # convergence check
         # ==============================================================================
 
-        if actual_improvement >= 0 and not disable_convergence:
+        if acceptance_result.accepted and not conv_options.disable:
             converged, msg = _is_converged(states=states, options=conv_options)
             if converged:
                 break
 
+        if history.get_n_fun() >= stop_options.max_eval:
+            converged = False
+            msg = "Maximum number of criterion evaluations reached."
+            break
+
     # ==================================================================================
     # results processing
     # ==================================================================================
     res = {
         "solution_x": state.x,
         "solution_criterion": state.fval,
         "states": states,
         "message": msg,
         "tranquilo_history": history,
     }
 
     return res
 
 
-def _calculate_rho(actual_improvement, expected_improvement):
-    if expected_improvement == 0 and actual_improvement > 0:
-        rho = np.inf
-    elif expected_improvement == 0:
-        rho = -np.inf
-    else:
-        rho = actual_improvement / expected_improvement
-    return rho
-
-
 class State(NamedTuple):
-    # Whether this is a safety iteration
-    safety: bool
-
-    # the trustregion at the beginning of the iteration
-    trustregion: TrustRegion
+    trustregion: Region
+    """The trustregion at the beginning of the iteration."""
 
     # Information about the model used to make the acceptance decision in the iteration
     model_indices: np.ndarray
+    """The indices of points used to build the current surrogate model `State.model`.
+
+    The points can be retrieved through calling `history.get_xs(model_indices)`.
+
+    """
+
     model: ScalarModel
+    """The current surrogate model.
+
+    The solution to the subproblem with this model as the criterion is stored as
+    `State.candidate_x`.
+
+    """
+
+    vector_model: VectorModel
+
+    # candidate information
+    candidate_index: int
+    """The index of the candidate point in the history.
+
+    This corresponds to the index of the point in the history that solved the
+    subproblem.
+
+    """
+
+    candidate_x: np.ndarray
+    """The candidate point.
+
+    Is the same as `history.get_xs(candidate_index)`.
+
+    """
 
     # accepted parameters and function values at the end of the iteration
     index: int
+    """The index of the accepted point in the history."""
+
     x: np.ndarray
+    """The accepted point.
+
+    Is the same as  `history.get_xs(index)`.
+
+    """
+
     fval: np.ndarray  # this is an estimate for noisy functions
+    """The function value at the accepted point.
+
+    If `noisy=False` this is the same as `history.get_fval(index)`. Otherwise, this is
+    an average.
+
+    """
 
-    # success Information
+    # success information
     rho: float
+    """The calculated rho in the current iteration."""
+
     accepted: bool
+    """Whether the candidate point was accepted."""
 
     # information on existing and new points
     new_indices: np.ndarray
+    """The indices of new points generated for the model fitting in this iteration."""
+
     old_indices_used: np.ndarray
+    """The indices of existing points used to build the model in this iteration."""
+
     old_indices_discarded: np.ndarray
+    """The indices of existing points not used to build the model in this iteration."""
+
+    # information on step length
+    step_length: float = None
+    """The euclidian distance between `State.x` and `State.trustregion.center`."""
+
+    relative_step_length: float = None
+    """The step_length divided by the radius of the trustregion."""
 
 
 def _is_converged(states, options):
     old, new = states[-2:]
 
     f_change_abs = np.abs(old.fval - new.fval)
     f_change_rel = f_change_abs / max(np.abs(old.fval), 1)
@@ -458,63 +439,14 @@
     else:
         converged = False
         msg = None
 
     return converged, msg
 
 
-def _process_surrogate_model(surrogate_model, functype):
-    if surrogate_model is None:
-        if functype == "scalar":
-            surrogate_model = "quadratic"
-        else:
-            surrogate_model = "linear"
-
-    if isinstance(surrogate_model, ModelInfo):
-        out = surrogate_model
-    elif isinstance(surrogate_model, str):
-        if surrogate_model == "linear":
-            out = ModelInfo(has_squares=False, has_interactions=False)
-        elif surrogate_model == "diagonal":
-            out = ModelInfo(has_squares=True, has_interactions=False)
-        elif surrogate_model == "quadratic":
-            out = ModelInfo(has_squares=True, has_interactions=True)
-        else:
-            raise ValueError(f"Invalid surrogate model: {surrogate_model}")
-
-    else:
-        raise TypeError(f"Invalid surrogate model: {surrogate_model}")
-    return out
-
-
-def _process_sample_size(user_sample_size, model_info, x):
-    if user_sample_size is None:
-        if model_info.has_squares or model_info.has_interactions:
-            out = 2 * len(x) + 1
-        else:
-            out = len(x) + 1
-
-    elif isinstance(user_sample_size, str):
-        user_sample_size = user_sample_size.replace(" ", "")
-        if user_sample_size in ["linear", "n+1"]:
-            out = n_free_params(dim=len(x), info_or_name="linear")
-        elif user_sample_size in ["powell", "2n+1", "2*n+1"]:
-            out = 2 * len(x) + 1
-        elif user_sample_size == "quadratic":
-            out = n_free_params(dim=len(x), info_or_name="quadratic")
-        else:
-            raise ValueError(f"Invalid sample size: {user_sample_size}")
-
-    elif isinstance(user_sample_size, numbers.Number):
-        out = int(user_sample_size)
-    else:
-        raise TypeError(f"invalid sample size: {user_sample_size}")
-    return out
-
-
 tranquilo = mark_minimizer(
     func=partial(_tranquilo, functype="scalar"),
     name="tranquilo",
     primary_criterion_entry="value",
     needs_scaling=True,
     is_available=True,
     is_global=False,
@@ -526,14 +458,11 @@
     name="tranquilo_ls",
     needs_scaling=True,
     is_available=True,
     is_global=False,
 )
 
 
-def _has_bounds(lb, ub):
-    out = False
-    if lb is not None and np.isfinite(lb).any():
-        out = True
-    if ub is not None and np.isfinite(ub).any():
-        out = True
-    return out
+def _concatenate_indices(first, second):
+    first = np.atleast_1d(first).astype(int)
+    second = np.atleast_1d(second).astype(int)
+    return np.hstack((first, second))
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/volume.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,36 @@
 
 
 def get_radius_after_volume_scaling(radius, dim, scaling_factor):
     out = radius * scaling_factor ** (1 / dim)
     return out
 
 
-def get_radius_of_sphere_with_volume_of_cube(cube_radius, dim, scaling_factor):
+def get_radius_of_sphere_with_volume_of_cube(cube_radius, dim, scaling_factor=None):
     log_radius = (
         loggamma(dim / 2 + 1) / dim
         - np.log(np.pi) / 2
         + np.log(2)
         + np.log(cube_radius)
-        + np.log(scaling_factor) / dim
     )
+    if scaling_factor is not None:
+        log_radius += np.log(scaling_factor) / dim
     out = np.exp(log_radius)
     return out
 
 
-def get_radius_of_cube_with_volume_of_sphere(sphere_radius, dim, scaling_factor):
+def get_radius_of_cube_with_volume_of_sphere(sphere_radius, dim, scaling_factor=None):
     log_radius = (
-        np.log(scaling_factor) / dim
-        + np.log(np.pi) / 2
+        np.log(np.pi) / 2
         + np.log(sphere_radius)
         - np.log(2)
         - loggamma(dim / 2 + 1) / dim
     )
+    if scaling_factor is not None:
+        log_radius += np.log(scaling_factor) / dim
     out = np.exp(log_radius)
     return out
 
 
 def get_volume(radius, dim, shape):
     if shape == "sphere":
         out = _sphere_volume(radius, dim)
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/weighting.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/weighting.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def get_sample_weighter(weighter, bounds):
     """Get a function that calculates weights for points in a sample.
 
     The resulting function takes the following arguments:
     - xs (np.ndarray): A 2d numpy array containing a sample.
-    - trustregion (TrustRegion): The current trustregion.
+    - trustregion (Region): Trustregion. See module region.py.
 
     Args:
         weighter (str)
         bounds (Bounds)
 
     """
     if isinstance(weighter, str):
```

### Comparing `estimagic-0.4.4/src/estimagic/optimization/tranquilo/wrap_criterion.py` & `estimagic-0.4.5/src/estimagic/optimization/tranquilo/wrap_criterion.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,47 +2,55 @@
 
 import numpy as np
 
 from estimagic.batch_evaluators import process_batch_evaluator
 
 
 def get_wrapped_criterion(criterion, batch_evaluator, n_cores, history):
+    """Wrap the criterion function to do get parallelization and history handling.
+
+    The wrapped criterion function takes a dict mapping x_indices to required numbers of
+    evaluations as only argument. It evaluates the criterion function in parallel and
+    saves the resulting function evaluations in the history.
+
+    The wrapped criterion function does not return anything.
+
+    """
     batch_evaluator = process_batch_evaluator(batch_evaluator)
 
     @functools.wraps(criterion)
-    def wrapper_criterion(params):
-        if np.array(params).size == 0:
-            return (np.array([]), np.array([]), np.array([]).astype(int))
+    def wrapper_criterion(eval_info):
+        if not isinstance(eval_info, dict):
+            raise ValueError("eval_info must be a dict.")
+
+        if len(eval_info) == 0:
+            return
 
-        _is_just_one = np.array(params).ndim == 1
+        x_indices = list(eval_info)
+        repetitions = list(eval_info.values())
 
-        _parlist = list(np.atleast_2d(params))
+        xs = history.get_xs(x_indices)
+        xs = np.repeat(xs, repetitions, axis=0)
 
-        _effective_n_cores = min(n_cores, len(_parlist))
+        arguments = list(xs)
 
-        _raw_evals = batch_evaluator(
+        effective_n_cores = min(n_cores, len(arguments))
+
+        raw_evals = batch_evaluator(
             criterion,
-            arguments=_parlist,
-            n_cores=_effective_n_cores,
+            arguments=arguments,
+            n_cores=effective_n_cores,
         )
 
         # replace NaNs but keep infinite values. NaNs would be problematic in many
-        # places, infs are only a problem in the model fitting and will thus be handled
-        # there
-        _clipped_evals = [
+        # places, infs are only a problem in model fitting and will be handled there
+        clipped_evals = [
             np.nan_to_num(critval, nan=np.inf, posinf=np.inf, neginf=-np.inf)
-            for critval in _raw_evals
+            for critval in raw_evals
         ]
 
-        indices = np.arange(history.get_n_fun(), history.get_n_fun() + len(_parlist))
-        history.add_entries(_parlist, _clipped_evals)
-        fvecs = history.get_fvecs(indices)
-        fvals = history.get_fvals(indices)
-
-        if _is_just_one:
-            out = (fvecs[0], fvals[0], indices[0])
-        else:
-            out = (fvecs, fvals, indices)
-
-        return out
+        history.add_evals(
+            x_indices=np.repeat(x_indices, repetitions),
+            evals=clipped_evals,
+        )
 
     return wrapper_criterion
```

### Comparing `estimagic-0.4.4/src/estimagic/parameters/block_trees.py` & `estimagic-0.4.5/src/estimagic/parameters/block_trees.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         for leaf_outer, s1, submat in zip(
             flat_p, shapes_p, np.split(subarr, block_bounds_p, axis=1)
         ):
             row = []
             for leaf_inner, s2, block_values in zip(
                 flat_p, shapes_p, np.split(submat, block_bounds_p, axis=2)
             ):
-                raw_block = block_values.reshape((*s0, *s1, *s2))
-                raw_block = np.squeeze(raw_block)
+                _shape = [k for k in (*s0, *s1, *s2) if k != 1]
+                raw_block = block_values.reshape(_shape)
                 block = _convert_raw_block_to_pandas(raw_block, leaf_outer, leaf_inner)
                 row.append(block)
             blocks.append(row)
         block_tree = tree_unflatten(
             treedef_p, [tree_unflatten(treedef_p, row) for row in blocks]
         )
         sub_block_trees.append(block_tree)
@@ -332,21 +332,27 @@
 
 def _check_dimensions_hessian(hessian, f_tree, params_tree):
     extended_registry = get_registry(extended=True)
     flat_f = tree_leaves(f_tree, registry=extended_registry)
     flat_p = tree_leaves(params_tree, registry=extended_registry)
 
     if len(flat_f) == 1:
-        if np.squeeze(hessian).ndim == 0:
-            if len(flat_p) != 1:
-                raise ValueError("Hessian dimension does not match those of params.")
-        elif np.squeeze(hessian).ndim == 2:
-            if np.squeeze(hessian).shape != (len(flat_p), len(flat_p)):
+        # consider only dimensions with non trivial size (larger than 1)
+        relevant_hessian_shape = tuple(k for k in hessian.shape if k != 1)
+
+        if len(relevant_hessian_shape) == 0 and len(flat_p) != 1:
+            # scalar f and scalar params -> scalar hessian
+            raise ValueError("Hessian dimension does not match those of params.")
+
+        if len(relevant_hessian_shape) == 2:
+            # scalar f and vector params -> matrix hessian
+            if relevant_hessian_shape != (len(flat_p), len(flat_p)):
                 raise ValueError("Hessian dimension does not match those of params.")
-        else:
+
+        if len(relevant_hessian_shape) > 2:
             raise ValueError("Hessian must be 0- or 2-d if f is scalar-valued.")
     else:
         if hessian.ndim != 3:
             raise ValueError("Hessian must be 3d if f is multidimensional.")
         if hessian.shape[0] != len(flat_f):
             raise ValueError("First Hessian dimension does not match that of f.")
         if hessian.shape[1:] != (len(flat_p), len(flat_p)):
```

### Comparing `estimagic-0.4.4/src/estimagic/parameters/check_constraints.py` & `estimagic-0.4.5/src/estimagic/parameters/check_constraints.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/consolidate_constraints.py` & `estimagic-0.4.5/src/estimagic/parameters/consolidate_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Functions to consolidate user provided constraints.
 
-Consolidation means that redundant constraints are dropped
-and other constraints are collected in meaningful bundles.
+Consolidation means that redundant constraints are dropped and other constraints are
+collected in meaningful bundles.
 
 Check the module docstring of process_constraints for naming conventions.
 
 """
 import numpy as np
 import pandas as pd
```

### Comparing `estimagic-0.4.4/src/estimagic/parameters/constraint_tools.py` & `estimagic-0.4.5/src/estimagic/parameters/constraint_tools.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/conversion.py` & `estimagic-0.4.5/src/estimagic/parameters/conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/kernel_transformations.py` & `estimagic-0.4.5/src/estimagic/parameters/kernel_transformations.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/nonlinear_constraints.py` & `estimagic-0.4.5/src/estimagic/parameters/nonlinear_constraints.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/parameter_bounds.py` & `estimagic-0.4.5/src/estimagic/parameters/parameter_bounds.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/parameter_groups.py` & `estimagic-0.4.5/src/estimagic/parameters/parameter_groups.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/process_constraints.py` & `estimagic-0.4.5/src/estimagic/parameters/process_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Process the user provided pc for use during the optimization.
 
-The main purpose of this module is to convert the user provided constraints into
-inputs for fast reparametrization functions. In the process, the constraints are
-checked and consolidated. Consolidation means that redundant constraints are dropped
-and other constraints are collected in meaningful bundles.
+The main purpose of this module is to convert the user provided constraints into inputs
+for fast reparametrization functions. In the process, the constraints are checked and
+consolidated. Consolidation means that redundant constraints are dropped and other
+constraints are collected in meaningful bundles.
 
 To improve readability, the actual code for checking and consolidation are in separate
 modules.
 
-Calls to functions doing checking are scattered across the module.
-This is in order to perform each check as soon as it becomes possible, which allows
-errors to be raised at a point where constraints still look similar to
-what users wrote. However, some checks can only be done
-after consolidation.
+Calls to functions doing checking are scattered across the module. This is in order to
+perform each check as soon as it becomes possible, which allows errors to be raised at a
+point where constraints still look similar to what users wrote. However, some checks can
+only be done after consolidation.
 
 """
 import numpy as np
 import pandas as pd
 
 from estimagic.parameters.check_constraints import (
     check_constraints_are_satisfied,
```

### Comparing `estimagic-0.4.4/src/estimagic/parameters/process_selectors.py` & `estimagic-0.4.5/src/estimagic/parameters/process_selectors.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/scale_conversion.py` & `estimagic-0.4.5/src/estimagic/parameters/scale_conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/space_conversion.py` & `estimagic-0.4.5/src/estimagic/parameters/space_conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/tree_conversion.py` & `estimagic-0.4.5/src/estimagic/parameters/tree_conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/parameters/tree_registry.py` & `estimagic-0.4.5/src/estimagic/parameters/tree_registry.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/process_user_function.py` & `estimagic-0.4.5/src/estimagic/process_user_function.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/sensitivity/msm_sensitivity.py` & `estimagic-0.4.5/src/estimagic/sensitivity/msm_sensitivity.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/shared/check_option_dicts.py` & `estimagic-0.4.5/src/estimagic/shared/check_option_dicts.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/utilities.py` & `estimagic-0.4.5/src/estimagic/utilities.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/visualization/convergence_plot.py` & `estimagic-0.4.5/src/estimagic/visualization/convergence_plot.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/visualization/derivative_plot.py` & `estimagic-0.4.5/src/estimagic/visualization/derivative_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     func_value = derivative_result["func_value"]
     func_evals = derivative_result["func_evals"]
     derivative_candidates = derivative_result["derivative_candidates"]
 
     # remove index from main data for plotting
     df = func_evals.reset_index()
-    df = df.assign(**{"step": df.step * df.sign})
+    df = df.assign(step=df.step * df.sign)
     func_evals = df.set_index(["sign", "step_number", "dim_x", "dim_f"])
 
     # prepare derivative data
     df_der = _select_derivative_with_minimal_error(derivative_candidates)
     df_der_method = _select_derivative_with_minimal_error(
         derivative_candidates, given_method=True
     )
```

### Comparing `estimagic-0.4.4/src/estimagic/visualization/estimation_table.py` & `estimagic-0.4.5/src/estimagic/visualization/estimation_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from pathlib import Path
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 
 
+suppress_performance_warnings = np.testing.suppress_warnings()
+suppress_performance_warnings.filter(category=pd.errors.PerformanceWarning)
+
+
+@suppress_performance_warnings
 def estimation_table(
     models,
     *,
     return_type="dataframe",
     render_options=None,
     show_col_names=True,
     show_col_groups=None,
@@ -103,29 +108,29 @@
             index levels of the parameters. This is mostly relevant when working with
             estimagic style params DataFrames with a MultiIndex and only used if
             "index_names" is set to True in the render_options. Default None.
         custom_notes (list): A list of strings for additional notes. Default is None.
         confidence_intervals (bool): If True, display confidence intervals as inference
             values. Display standard errors otherwise. Default False.
         significance_levels (list): a list of floats for p value's significance cut-off
-            values.This is used to generate the significance stars. Default is
+            values. This is used to generate the significance stars. Default is
             [0.1,0.05,0.01].
         append_notes (bool): A boolean variable for printing p value cutoff explanation
             and additional notes, if applicable. Default is True.
         notes_label (str): A sting to print as the title of the notes section, if
             applicable. Default is 'Notes'
         stats_options (dict): A dictionary that determines which statistics (e.g.
             R-Squared, No. of Observations) are displayed and how they are labeled.
             The keys are the names of the statistics inside the model['info'] dictionary
             or attribute names of a statsmodels results object. The values are the new
             labels to be displayed for those statistics, i.e. the set of the values is
             used as row names in the table.
         number_format (int, str, iterable or callable): A callable, iterable, integer
             or string that is used to apply string formatter(s) to floats in the
-            table. Defualt ("{0:.3g}", "{0:.5f}", "{0:.4g}").
+            table. Default ("{0:.3g}", "{0:.5f}", "{0:.4g}").
         add_trailing_zeros (bool): If True, format floats such that they have same
             number of digits after the decimal point. Default True.
         siunitx_warning (bool): If True, print warning about LaTex preamble to add for
             proper compilation of  when working with siunitx package. Default True.
         escape_special_characters (bool): If True, replaces special characters
             in parameter and model names with LaTeX or HTML safe sequences.
     Returns:
@@ -257,15 +262,15 @@
         append_notes (bool): A boolean variable for printing p value cutoff explanation
             and additional notes, if applicable. Default is True.
         notes_label (str): A sting to print as the title of the notes section, if
             applicable. Default is 'Notes'
         significance_levels (list or tuple): a list of floats for p value's significance
             cutt-off values. Default is [0.1,0.05,0.01].
         custom_notes (list): A list of strings for additional notes. Default is None.
-        siunitx_watning (bool): If True, print warning about LaTex preamble to add for
+        siunitx_warning (bool): If True, print warning about LaTex preamble to add for
             proper compilation of  when working with siunitx package. Default True.
         show_index_names (bool): If True, display index names in the table.
         show_col_names (bool): If True, the column names are displayed.
         show_col_groups (bool): If True, the column groups are displayed.
         escape_special_characters (bool): If True, replaces the characters &, %,
             $, #, _, {, }, ~, ^, and \ in parameter and model names with
             LaTeX-safe sequences.
@@ -344,16 +349,15 @@
             + "\\\\"
             + temp_str
             + latex_str.split("\\\\", 1)[1]
         )
     latex_str = latex_str.split("\\bottomrule")[0]
     if show_footer:
         footer = footer.copy(deep=True)
-        for _, r in footer.iterrows():
-            r = _center_align_integers(r)
+        footer = footer.apply(_center_align_integers_and_non_numeric_strings, axis=1)
         footer_styler = footer.style
         stats_str = footer_styler.to_latex(**default_options)
         if "\\midrule" in stats_str:
             stats_str = (
                 "\\midrule" + stats_str.split("\\midrule")[1].split("\\bottomrule")[0]
             )
         else:
@@ -540,15 +544,15 @@
         show_inference(bool): If True, inference (standard errors or confidence
             intervals) below param values.
         confidence_intervals (bool): If True, display confidence intervals as inference
             values.
         number_format (int, str, iterable or callable): A callable, iterable, integer
             or callable that is used to apply string formatter(s) to floats in the
             table.
-        add_trailing_zeros (bool): If True, format floats such that they haave same
+        add_trailing_zeros (bool): If True, format floats such that they have same
             number of digits after the decimal point.
 
     Returns:
         body (DataFrame): DataFrame data frame with formatted strings of parameter
             and inference values and significance stars to display in estimation table.
         footer (DataFrame): DataFrame with formatted strings of summary statistics to
             display at the bottom of estimation table.
@@ -620,15 +624,15 @@
         show_inference(bool): If True, inference (standard errors or confidence
             intervals) below param values.
         confidence_intervals (bool): If True, display confidence intervals as inference
             values.
         number_format (int, str, iterable or callable): A callable, iterable, integer
             or callable that is used to apply string formatter(s) to floats in the
             table.
-        add_trailing_zeros (bool): If True, format floats such that they haave same
+        add_trailing_zeros (bool): If True, format floats such that they have same
             number of digits after the decimal point.
 
     Returns:
         body (DataFrame): DataFrame data frame with formatted strings of parameter
             and inference values and significance stars to display in estimation table.
         max_trail (int): Integer that shows the maximum number of digits after a decimal
             point in the parameters DataFrame. Is passed to
@@ -715,16 +719,14 @@
             number_format,
             add_trailing_zeros,
             max_trail,
         )
         for mod in models
     ]
     stats = pd.concat(to_concat, axis=1)
-    for _, r in stats.iterrows():
-        r = _unformat_integers(r)
     return stats
 
 
 def _reindex_and_float_format_params(
     models, show_inference, confidence_intervals, number_format, add_trailing_zeros
 ):
     """Reindex all params DataFrames with a common index and apply number formatting."""
@@ -766,18 +768,25 @@
         else:
             cols.append("standard_error")
     return cols
 
 
 def _apply_number_formatting_frames(dfs, columns, number_format, add_trailing_zeros):
     """Apply string formatter to specific columns of a list of DataFrames."""
-    raw_formatted = [_apply_number_format(df[columns], number_format) for df in dfs]
+
+    raw_formatted = [
+        _apply_number_format(df[columns], number_format, format_integers=False)
+        for df in dfs
+    ]
     max_trail = int(max([_get_digits_after_decimal(df) for df in raw_formatted]))
     if add_trailing_zeros:
-        formatted = [_apply_number_format(df, max_trail) for df in raw_formatted]
+        formatted = [
+            _apply_number_format(df, max_trail, format_integers=True)
+            for df in raw_formatted
+        ]
     else:
         formatted = raw_formatted
     return formatted, max_trail
 
 
 def _update_show_col_groups(show_col_groups, column_groups):
     """Set the value of show_col_groups to False or True given column_groups.
@@ -978,15 +987,15 @@
 ):
     """Return processed value series with significance stars and inference information.
 
     Args:
 
         df (DataFrame): params DataFrame of the model
         significance_levels (list): see main docstring
-        number_format (int): see main docstring
+        number_format (int, str, iterable or callable): see main docstring
         show_inference (bool): see main docstring
         confidence_intervals (bool): see main docstring
         show_stars (bool): see main docstring
 
     Returns:
         sr (pd.Series): string series with values and inferences.
 
@@ -1072,34 +1081,42 @@
     """Process statistics values, return string series.
 
     Args:
         model (estimation result): see main docstring
         stats_options (dict): see main docstring
         significance_levels (list): see main docstring
         show_stars (bool): see main docstring
-        number_format (int): see main focstring
+        number_format (int, str, iterable or callable): see main docstring
+        add_trailing_zeros (bool): If True, format floats such that they haave same
+            number of digits after the decimal point.
+        max_trail (int): If add_trailing_zeros is True, add corresponding number of
+            trailing zeros to floats in the stats DataFrame to have number of digits
+            after a decimal point equal to max_trail for each float.
 
     Returns:
         series: string series with summary statistics values and additional info
             if applicable.
 
     """
     stats_values = {}
     stats_options = deepcopy(stats_options)
     if "show_dof" in stats_options:
         show_dof = stats_options.pop("show_dof")
     else:
         show_dof = None
     for k in stats_options:
         stats_values[stats_options[k]] = model["info"].get(k, np.nan)
+
     raw_formatted = _apply_number_format(
-        pd.DataFrame(pd.Series(stats_values)), number_format
+        pd.DataFrame(pd.Series(stats_values)), number_format, format_integers=False
     )
     if add_trailing_zeros:
-        formatted = _apply_number_format(raw_formatted, max_trail)
+        formatted = _apply_number_format(
+            raw_formatted, max_trail, format_integers=False
+        )
     else:
         formatted = raw_formatted
     stats_values = formatted.to_dict()[0]
     if "fvalue" in model["info"] and "F Statistic" in stats_values:
         if show_stars and "f_pvalue" in model["info"]:
             sig_bins = [-1, *sorted(significance_levels)] + [2]
             sig_icon_fstat = "*" * (
@@ -1120,15 +1137,15 @@
     if "resid_std_err" in model["info"] and "Residual Std. Error" in stats_values:
         if show_dof:
             rse_str = "{{{}(df={})}}"
             stats_values["Residual Std. Error"] = rse_str.format(
                 stats_values["Residual Std. Error"], int(model["info"]["df_resid"])
             )
     stat_sr = pd.Series(stats_values)
-    # the follwing is to make sure statistics dataframe has as many levels of
+    # the following is to make sure statistics dataframe has as many levels of
     # indices as the parameters dataframe.
     stat_ind = np.empty((len(stat_sr), model["params"].index.nlevels - 1), dtype=str)
     stat_ind = np.concatenate(
         [stat_sr.index.values.reshape(len(stat_sr), 1), stat_ind], axis=1
     ).T
     stat_sr.index = pd.MultiIndex.from_arrays(stat_ind)
     return stat_sr.astype("str").replace("nan", "")
@@ -1342,40 +1359,49 @@
         info[kv] = getattr(model, kv)
     info["name"] = model.model.endog_names
     info["resid_std_err"] = np.sqrt(model.scale)
     info["n_obs"] = model.df_model + model.df_resid + 1
     return info
 
 
-def _apply_number_format(df, number_format):
+def _apply_number_format(df_raw, number_format, format_integers):
     """Apply string format to DataFrame cells.
 
     Args:
-        df (DataFrame): The DataFrame with float values to format.
-        number_format(str, list, tuple, callable or int): User defined number format
+        df_raw (DataFrame): The DataFrame with float values to format.
+        number_format (str, list, tuple, callable or int): User defined number format
             to apply to the DataFrame.
+        format_integers (bool): Apply number format also to integers
 
     Returns:
         df_formatted (DataFrame): Formatted DataFrame.
 
     """
     processed_format = _process_number_format(number_format)
+    df_raw = df_raw.copy(deep=True)
     if isinstance(processed_format, (list, tuple)):
-        df_formatted = df.copy(deep=True).astype("float")
+        df_formatted = df_raw.copy(deep=True).astype("float")
         for formatter in processed_format[:-1]:
             df_formatted = df_formatted.applymap(formatter.format).astype("float")
         df_formatted = df_formatted.astype("float").applymap(
             processed_format[-1].format
         )
     elif isinstance(processed_format, str):
-        df_formatted = df.astype("str").applymap(
+        df_formatted = df_raw.astype("str").applymap(
             partial(_format_non_scientific_numbers, format_string=processed_format)
         )
     elif callable(processed_format):
-        df_formatted = df.applymap(processed_format)
+        df_formatted = df_raw.applymap(processed_format)
+
+    # Don't format integers: set to original value
+    if not format_integers:
+        integer_locs = df_raw.applymap(_is_integer)
+        df_formatted[integer_locs] = (
+            df_raw[integer_locs].astype(float).applymap("{:.0f}".format)
+        )
     return df_formatted
 
 
 def _format_non_scientific_numbers(number_string, format_string):
     """Apply number format if the number string is not in scientific format."""
     if "e" in number_string:
         out = number_string
@@ -1423,39 +1449,24 @@
         except KeyError:
             trail_length = 0
         if trail_length > max_trail:
             max_trail = trail_length
     return max_trail
 
 
-def _center_align_integers(sr):
-    """Align integer numbers at the center of model column."""
-    for i in sr.index:
-        res_numeric = re.findall(
-            r"[-+]?[.]?[\d]+(?:,\d\d\d)*[\.]?\d*(?:[eE][-+]?\d+)?", sr[i]
-        )
-        if res_numeric:
-            num = res_numeric[0]
-            char = sr[i].split(num)[1]
-            if int(float(num)) == float(num):
-                sr[i] = f"\\multicolumn{{1}}{{c}}{{{str(int(float(num)))+char}}}"
-    return sr
-
-
-def _unformat_integers(sr):
-    """Remove trailing zeros from integer numbers."""
+def _center_align_integers_and_non_numeric_strings(sr):
+    """Align integer numbers and strings at the center of model column."""
+    sr = deepcopy(sr)
     for i in sr.index:
-        res_numeric = re.findall(
-            r"[-+]?[.]?[\d]+(?:,\d\d\d)*[\.]?\d*(?:[eE][-+]?\d+)?", sr[i]
-        )
-        if res_numeric:
-            num = res_numeric[0]
-            char = sr[i].split(num)[1]
-            if int(float(num)) == float(num):
-                sr[i] = str(int(float(num))) + char
+        if _is_integer(sr[i]):
+            sr[i] = f"\\multicolumn{{1}}{{c}}{{{str(int(float(sr[i])))}}}"
+        else:
+            string_without_stars = sr[i].split("$", 1)[0]
+            if not string_without_stars.replace(".", "").isnumeric():
+                sr[i] = f"\\multicolumn{{1}}{{c}}{{{sr[i]}}}"
     return sr
 
 
 def _get_updated_styler(
     df, show_index_names, show_col_names, show_col_groups, escape_special_characters
 ):
     """Return pandas.Styler object based ont the data and styling options."""
@@ -1465,7 +1476,16 @@
     if not show_col_names:
         styler = styler.hide(axis=1)
     if not show_col_groups:
         styler = styler.hide(axis=1, level=0)
     for ax in [0, 1]:
         styler = styler.format_index(escape=escape_special_characters, axis=ax)
     return styler
+
+
+def _is_integer(num):
+    """Check if number is an integer (including a float with only zeros as digits)"""
+    try:
+        out = int(float(num)) == float(num)
+    except ValueError:
+        out = False
+    return out
```

### Comparing `estimagic-0.4.4/src/estimagic/visualization/history_plots.py` & `estimagic-0.4.5/src/estimagic/visualization/history_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,19 +246,21 @@
         helper = tree_unflatten(treedef, list(range(len(flat))), registry=registry)
         selected = np.array(tree_just_flatten(selector(helper), registry=registry))
         names = [names[i] for i in selected]
         hist_arr = hist_arr[selected]
 
     for name, data in zip(names, hist_arr):
         if max_evaluations is not None and len(data) > max_evaluations:
-            data = data[:max_evaluations]
+            plot_data = data[:max_evaluations]
+        else:
+            plot_data = data
 
         trace = go.Scatter(
-            x=np.arange(len(data)),
-            y=data,
+            x=np.arange(len(plot_data)),
+            y=plot_data,
             mode="lines",
             name=name,
         )
         fig.add_trace(trace)
 
     fig.update_layout(
         template=template,
```

### Comparing `estimagic-0.4.4/src/estimagic/visualization/lollipop_plot.py` & `estimagic-0.4.5/src/estimagic/visualization/lollipop_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 
 
 def _harmonize_data(data):
     if not isinstance(data, list):
         data = [data]
 
     to_concat = []
-    for i, df in enumerate(data):
-        df = df.copy()
+    for i, _df in enumerate(data):
+        df = _df.copy()
         df.columns = _make_string_index(df.columns)
         df.index = _make_string_index(df.index)
         df["__name__"] = df.index
         df["__hue__"] = i
         to_concat.append(df)
 
     combined = pd.concat(to_concat)
```

### Comparing `estimagic-0.4.4/src/estimagic/visualization/plotting_utilities.py` & `estimagic-0.4.5/src/estimagic/visualization/plotting_utilities.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/visualization/profile_plot.py` & `estimagic-0.4.5/src/estimagic/visualization/profile_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,20 +102,23 @@
         names=["alpha"],
     )
     performance_profiles = for_each_alpha.groupby("alpha").mean().stack().reset_index()
 
     fig = px.line(performance_profiles, x="alpha", y=0, color="algorithm")
 
     xlabels = {
-        ("n_evaluations", True): "Multiple of Minimal Number of Function Evaluations\n"
+        (
+            "n_evaluations",
+            True,
+        ): "Multiple of Minimal Number of Function Evaluations<br>"
         "Needed to Solve the Problem",
         (
             "walltime",
             True,
-        ): "Multiple of Minimal Wall Time\nNeeded to Solve the Problem",
+        ): "Multiple of Minimal Wall Time<br>Needed to Solve the Problem",
         ("n_evaluations", False): "Number of Function Evaluations",
         ("walltime", False): "Wall Time Needed to Solve the Problem",
     }
 
     fig.update_layout(
         xaxis_title=xlabels[(runtime_measure, normalize_runtime)],
         yaxis_title="Share of Problems Solved",
```

### Comparing `estimagic-0.4.4/src/estimagic/visualization/slice_plot.py` & `estimagic-0.4.5/src/estimagic/visualization/slice_plot.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.4/src/estimagic/visualization/visualize_tranquilo.py` & `estimagic-0.4.5/src/estimagic/visualization/visualize_tranquilo.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from plotly import figure_factory as ff
 from plotly import graph_objects as go
 from plotly.subplots import make_subplots
 
 from estimagic.optimization.optimize_result import OptimizeResult
 from estimagic.optimization.tranquilo.clustering import cluster
 from estimagic.optimization.tranquilo.geometry import log_d_quality_calculator
-from estimagic.optimization.tranquilo.options import Bounds
 from estimagic.optimization.tranquilo.volume import get_radius_after_volume_scaling
 
 
 def visualize_tranquilo(results, iterations):
     """Plot diagnostic information of optimization result in given iteration(s).
 
     Generates plots with sample points (trustregion or heatmap), criterion evaluations,
@@ -420,21 +419,19 @@
     )
     return fig
 
 
 def _get_fekete_criterion(res):
     states = res.algorithm_output["states"][1:]
     history = np.array(res.history["params"])
-    bounds = Bounds(lower=-np.inf, upper=np.inf)
 
     out = [np.nan] + [
         log_d_quality_calculator(
             sample=history[state.model_indices],
             trustregion=state.trustregion,
-            bounds=bounds,
         )
         for state in states
     ]
     return out
 
 
 def _get_sample_points(state, history):
```

### Comparing `estimagic-0.4.4/src/estimagic.egg-info/PKG-INFO` & `estimagic-0.4.5/src/estimagic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimagic
-Version: 0.4.4
+Version: 0.4.5
 Summary: Tools to solve difficult numerical optimization problems.
 Home-page: https://github.com/OpenSourceEconomics/estimagic
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: econometrics,statistics,estimation,extremum estimation,optimization,inference,numerical differentiation,finite differences,richardson extrapolation,derivative free optimization,method of simulated moments,maximum likelihood
 Classifier: Development Status :: 4 - Beta
```

### Comparing `estimagic-0.4.4/src/estimagic.egg-info/SOURCES.txt` & `estimagic-0.4.5/src/estimagic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 src/estimagic/estimation/__init__.py
 src/estimagic/estimation/estimate_ml.py
 src/estimagic/estimation/estimate_msm.py
 src/estimagic/estimation/estimation_summaries.py
 src/estimagic/estimation/msm_weighting.py
 src/estimagic/examples/__init__.py
 src/estimagic/examples/criterion_functions.py
-src/estimagic/examples/db1.db
 src/estimagic/examples/diabetes.csv
 src/estimagic/examples/exam_points.csv
 src/estimagic/examples/logit.py
 src/estimagic/examples/numdiff_functions.py
 src/estimagic/examples/sensitivity_probit_example_data.csv
 src/estimagic/inference/__init__.py
 src/estimagic/inference/bootstrap.py
@@ -83,25 +82,25 @@
 src/estimagic/optimization/bhhh.py
 src/estimagic/optimization/check_arguments.py
 src/estimagic/optimization/convergence_report.py
 src/estimagic/optimization/cyipopt_optimizers.py
 src/estimagic/optimization/error_penalty.py
 src/estimagic/optimization/fides_optimizers.py
 src/estimagic/optimization/get_algorithm.py
-src/estimagic/optimization/history.py
 src/estimagic/optimization/history_tools.py
 src/estimagic/optimization/internal_criterion_template.py
 src/estimagic/optimization/nag_optimizers.py
 src/estimagic/optimization/neldermead.py
 src/estimagic/optimization/nlopt_optimizers.py
 src/estimagic/optimization/optimization_logging.py
 src/estimagic/optimization/optimize.py
 src/estimagic/optimization/optimize_result.py
 src/estimagic/optimization/pounders.py
 src/estimagic/optimization/pounders_auxiliary.py
+src/estimagic/optimization/pounders_history.py
 src/estimagic/optimization/process_multistart_sample.py
 src/estimagic/optimization/process_results.py
 src/estimagic/optimization/pygmo_optimizers.py
 src/estimagic/optimization/scipy_optimizers.py
 src/estimagic/optimization/simopt_optimizers.py
 src/estimagic/optimization/tao_optimizers.py
 src/estimagic/optimization/tiktak.py
@@ -113,34 +112,40 @@
 src/estimagic/optimization/subsolvers/_trsbox_fast.py
 src/estimagic/optimization/subsolvers/bntr.py
 src/estimagic/optimization/subsolvers/bntr_fast.py
 src/estimagic/optimization/subsolvers/gqtpar.py
 src/estimagic/optimization/subsolvers/gqtpar_fast.py
 src/estimagic/optimization/subsolvers/linear_subsolvers.py
 src/estimagic/optimization/tranquilo/__init__.py
+src/estimagic/optimization/tranquilo/acceptance_decision.py
+src/estimagic/optimization/tranquilo/acceptance_sample_size.py
 src/estimagic/optimization/tranquilo/adjust_radius.py
 src/estimagic/optimization/tranquilo/aggregate_models.py
+src/estimagic/optimization/tranquilo/bounds.py
 src/estimagic/optimization/tranquilo/clustering.py
-src/estimagic/optimization/tranquilo/count_points.py
+src/estimagic/optimization/tranquilo/estimate_variance.py
 src/estimagic/optimization/tranquilo/filter_points.py
 src/estimagic/optimization/tranquilo/fit_models.py
 src/estimagic/optimization/tranquilo/geometry.py
 src/estimagic/optimization/tranquilo/get_component.py
 src/estimagic/optimization/tranquilo/handle_infinity.py
+src/estimagic/optimization/tranquilo/history.py
 src/estimagic/optimization/tranquilo/models.py
 src/estimagic/optimization/tranquilo/options.py
 src/estimagic/optimization/tranquilo/poisedness.py
+src/estimagic/optimization/tranquilo/process_arguments.py
+src/estimagic/optimization/tranquilo/region.py
+src/estimagic/optimization/tranquilo/rho_noise.py
 src/estimagic/optimization/tranquilo/sample_points.py
 src/estimagic/optimization/tranquilo/solve_subproblem.py
-src/estimagic/optimization/tranquilo/thourough_subsolver.py
 src/estimagic/optimization/tranquilo/tranquilo.py
-src/estimagic/optimization/tranquilo/tranquilo_history.py
 src/estimagic/optimization/tranquilo/volume.py
 src/estimagic/optimization/tranquilo/weighting.py
 src/estimagic/optimization/tranquilo/wrap_criterion.py
+src/estimagic/optimization/tranquilo/wrapped_subsolvers.py
 src/estimagic/parameters/__init__.py
 src/estimagic/parameters/block_trees.py
 src/estimagic/parameters/check_constraints.py
 src/estimagic/parameters/consolidate_constraints.py
 src/estimagic/parameters/constraint_tools.py
 src/estimagic/parameters/conversion.py
 src/estimagic/parameters/kernel_transformations.py
@@ -154,14 +159,15 @@
 src/estimagic/parameters/tree_conversion.py
 src/estimagic/parameters/tree_registry.py
 src/estimagic/sensitivity/msm_sensitivity.py
 src/estimagic/shared/check_option_dicts.py
 src/estimagic/visualization/__init__.py
 src/estimagic/visualization/convergence_plot.py
 src/estimagic/visualization/derivative_plot.py
+src/estimagic/visualization/deviation_plot.py
 src/estimagic/visualization/estimation_table.py
 src/estimagic/visualization/history_plots.py
 src/estimagic/visualization/lollipop_plot.py
 src/estimagic/visualization/plotting_utilities.py
 src/estimagic/visualization/profile_plot.py
 src/estimagic/visualization/slice_plot.py
 src/estimagic/visualization/visualize_tranquilo.py
```

