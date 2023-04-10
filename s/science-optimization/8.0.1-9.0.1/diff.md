# Comparing `tmp/science_optimization-8.0.1.tar.gz` & `tmp/science_optimization-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "science_optimization-8.0.1.tar", max compression
+gzip compressed data, was "science_optimization-9.0.1.tar", max compression
```

## Comparing `science_optimization-8.0.1.tar` & `science_optimization-9.0.1.tar`

### file list

```diff
@@ -1,105 +1,104 @@
--rw-r--r--   0        0        0      250 2023-03-24 16:09:36.347720 science_optimization-8.0.1/LICENSE
--rw-r--r--   0        0        0    11780 2023-03-24 16:09:36.347720 science_optimization-8.0.1/README.md
--rw-r--r--   0        0        0     3137 2023-03-24 16:09:36.347720 science_optimization-8.0.1/build.py
--rw-r--r--   0        0        0     1072 2023-03-24 16:09:36.347720 science_optimization-8.0.1/pyproject.toml
--rw-r--r--   0        0        0      193 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/__init__.py
--rw-r--r--   0        0        0      272 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/algorithms/__init__.py
--rw-r--r--   0        0        0      901 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/algorithms/base_algorithms.py
--rw-r--r--   0        0        0       85 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/algorithms/cutting_plane/__init__.py
--rw-r--r--   0        0        0     6028 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/algorithms/cutting_plane/ellipsoid_method.py
--rw-r--r--   0        0        0       89 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/algorithms/decomposition/__init__.py
--rw-r--r--   0        0        0     7106 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/algorithms/decomposition/dual_decomposition.py
--rw-r--r--   0        0        0       77 2023-03-24 16:09:36.347720 science_optimization-8.0.1/science_optimization/algorithms/derivative_free/__init__.py
--rw-r--r--   0        0        0    17247 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/derivative_free/nelder_mead.py
--rw-r--r--   0        0        0       88 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/lagrange/__init__.py
--rw-r--r--   0        0        0     5177 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/lagrange/augmented_lagrangian.py
--rw-r--r--   0        0        0      233 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/linear_programming/__init__.py
--rw-r--r--   0        0        0     4543 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/linear_programming/glop.py
--rw-r--r--   0        0        0     3347 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/linear_programming/scipy_base_linear.py
--rw-r--r--   0        0        0      429 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/linear_programming/scipy_interior_point_method.py
--rw-r--r--   0        0        0      395 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/linear_programming/scipy_simplex_method.py
--rw-r--r--   0        0        0      231 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/search_direction/__init__.py
--rw-r--r--   0        0        0     9608 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/search_direction/base_search_direction.py
--rw-r--r--   0        0        0      731 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/search_direction/gradient_algorithm.py
--rw-r--r--   0        0        0      589 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/search_direction/newton_algorithm.py
--rw-r--r--   0        0        0     3121 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/search_direction/quasi_newton.py
--rw-r--r--   0        0        0      197 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/unidimensional/__init__.py
--rw-r--r--   0        0        0     1824 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/unidimensional/base_unidimensional.py
--rw-r--r--   0        0        0     1305 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/unidimensional/golden_section.py
--rw-r--r--   0        0        0     5579 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/unidimensional/multimodal_golden_section.py
--rw-r--r--   0        0        0       63 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/utils/__init__.py
--rw-r--r--   0        0        0     4684 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/algorithms/utils/algorithms_utils.py
--rw-r--r--   0        0        0      255 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/builder/__init__.py
--rw-r--r--   0        0        0      504 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/builder/__init__.pyc
--rw-r--r--   0        0        0      446 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/builder/builder_optimization_problem.py
--rw-r--r--   0        0        0     4766 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/builder/constraint.py
--rw-r--r--   0        0        0     1823 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/builder/objective.py
--rw-r--r--   0        0        0    15936 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/builder/optimization_problem.py
--rw-r--r--   0        0        0     3292 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/builder/variable.py
--rw-r--r--   0        0        0      599 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/__init__.py
--rw-r--r--   0        0        0     2002 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/decomposition_example.py
--rw-r--r--   0        0        0     1323 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/diet_example.py
--rw-r--r--   0        0        0     1542 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/ellipsoid_example.py
--rw-r--r--   0        0        0     1213 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/generic_function_example.py
--rw-r--r--   0        0        0      660 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/kleeminty_example.py
--rw-r--r--   0        0        0      909 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/lp_sampling.py
--rw-r--r--   0        0        0     1236 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/mgs_rastringin.py
--rw-r--r--   0        0        0     2003 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/multiobjective_example.py
--rw-r--r--   0        0        0     4106 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/neldermead_article_example.py
--rw-r--r--   0        0        0    10402 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/neldermead_example.py
--rw-r--r--   0        0        0     3144 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs0.py
--rw-r--r--   0        0        0     3295 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs1.py
--rw-r--r--   0        0        0     1655 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs2.py
--rw-r--r--   0        0        0     1956 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs3.py
--rw-r--r--   0        0        0     1622 2023-03-24 16:09:36.351720 science_optimization-8.0.1/science_optimization/examples/plot_example.py
--rw-r--r--   0        0        0     1530 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/examples/quadratic_example.py
--rw-r--r--   0        0        0      318 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/__init__.py
--rw-r--r--   0        0        0    10400 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/base_function.py
--rw-r--r--   0        0        0     7807 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/functions_composite.py
--rw-r--r--   0        0        0     2486 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/generic_function.py
--rw-r--r--   0        0        0     5421 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/lagrange_function.py
--rw-r--r--   0        0        0     3173 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/linear_function.py
--rw-r--r--   0        0        0     8303 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/polynomial_function.py
--rw-r--r--   0        0        0     2821 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/function/quadratic_function.py
--rw-r--r--   0        0        0      297 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/__init__.py
--rw-r--r--   0        0        0     2964 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/diet.py
--rw-r--r--   0        0        0     2694 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/generic.py
--rw-r--r--   0        0        0     2333 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/klee_minty.py
--rw-r--r--   0        0        0     4853 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/mip.py
--rw-r--r--   0        0        0     2416 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/quadratic.py
--rw-r--r--   0        0        0     5971 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/rosen_suzuki.py
--rw-r--r--   0        0        0     3145 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/problems/separable_resource_allocation.py
--rw-r--r--   0        0        0       67 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/profiling/__init__.py
--rw-r--r--   0        0        0     2164 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/profiling/profiling.py
--rw-r--r--   0        0        0      150 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/__init__.py
--rw-r--r--   0        0        0     2824 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/optimization_results.py
--rw-r--r--   0        0        0     2616 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/optimizer.py
--rw-r--r--   0        0        0      310 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/__init__.py
--rw-r--r--   0        0        0     5804 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py
--rw-r--r--   0        0        0     8087 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/epsilon_sampler.py
--rw-r--r--   0        0        0     3270 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/lambda_sampler.py
--rw-r--r--   0        0        0     3845 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/mu_sampler.py
--rw-r--r--   0        0        0     3786 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/nondominated_sampler.py
--rw-r--r--   0        0        0     2202 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/random_sampler.py
--rw-r--r--   0        0        0      403 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/test/__init__.py
--rw-r--r--   0        0        0     4286 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/test/test_algorithm_utils.py
--rw-r--r--   0        0        0     3386 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/test/test_base_linear.py
--rw-r--r--   0        0        0     8060 2023-03-24 16:09:36.355721 science_optimization-8.0.1/science_optimization/test/test_builder_package.py
--rw-r--r--   0        0        0    39169 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/test_constraint_algorithms.py
--rw-r--r--   0        0        0    35781 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/test_functions.py
--rw-r--r--   0        0        0     4511 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/test_glop.py
--rw-r--r--   0        0        0     8156 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/test_pareto_sampler.py
--rw-r--r--   0        0        0     6502 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/test_problems.py
--rw-r--r--   0        0        0     4403 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/test_search_direction.py
--rw-r--r--   0        0        0     2912 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/test_unidimensional.py
--rw-r--r--   0        0        0    13229 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/valueslinear.pickle
--rw-r--r--   0        0        0    13262 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/valuesquad.pickle
--rw-r--r--   0        0        0    13262 2023-03-24 16:09:36.359721 science_optimization-8.0.1/science_optimization/test/valuessparse.pickle
--rw-r--r--   0        0        0        0 2023-03-24 16:09:36.359721 science_optimization-8.0.1/src/__init__.py
--rw-r--r--   0        0        0     9974 2023-03-24 16:09:36.359721 science_optimization-8.0.1/src/algorithms.h
--rw-r--r--   0        0        0    26683 2023-03-24 16:09:36.359721 science_optimization-8.0.1/src/matrix.h
--rw-r--r--   0        0        0     4064 2023-03-24 16:09:36.359721 science_optimization-8.0.1/src/nlpalg.cpp
--rw-r--r--   0        0        0   163623 2023-03-24 16:09:36.363721 science_optimization-8.0.1/src/nlpalg.pdf
--rw-r--r--   0        0        0     7608 2023-03-24 16:09:36.367722 science_optimization-8.0.1/src/pybind.vcxproj
--rw-r--r--   0        0        0    14018 1970-01-01 00:00:00.000000 science_optimization-8.0.1/setup.py
--rw-r--r--   0        0        0    12978 1970-01-01 00:00:00.000000 science_optimization-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0      250 2022-11-08 13:42:14.460435 science_optimization-9.0.1/LICENSE
+-rw-r--r--   0        0        0    11780 2022-11-08 13:53:18.706299 science_optimization-9.0.1/README.md
+-rw-r--r--   0        0        0     3137 2023-03-23 19:11:45.733736 science_optimization-9.0.1/build.py
+-rw-r--r--   0        0        0     1058 2023-04-10 17:53:18.176530 science_optimization-9.0.1/pyproject.toml
+-rw-r--r--   0        0        0      193 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/__init__.py
+-rw-r--r--   0        0        0      272 2023-03-23 19:11:41.489780 science_optimization-9.0.1/science_optimization/algorithms/__init__.py
+-rw-r--r--   0        0        0      901 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/base_algorithms.py
+-rw-r--r--   0        0        0       85 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/cutting_plane/__init__.py
+-rw-r--r--   0        0        0     6028 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/cutting_plane/ellipsoid_method.py
+-rw-r--r--   0        0        0       89 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/decomposition/__init__.py
+-rw-r--r--   0        0        0     7106 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/decomposition/dual_decomposition.py
+-rw-r--r--   0        0        0       77 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/derivative_free/__init__.py
+-rw-r--r--   0        0        0    17247 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/derivative_free/nelder_mead.py
+-rw-r--r--   0        0        0       88 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/lagrange/__init__.py
+-rw-r--r--   0        0        0     5177 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/lagrange/augmented_lagrangian.py
+-rw-r--r--   0        0        0      233 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/__init__.py
+-rw-r--r--   0        0        0     4543 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/glop.py
+-rw-r--r--   0        0        0     3347 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_base_linear.py
+-rw-r--r--   0        0        0      429 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_interior_point_method.py
+-rw-r--r--   0        0        0      395 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_simplex_method.py
+-rw-r--r--   0        0        0      231 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/__init__.py
+-rw-r--r--   0        0        0     9608 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/base_search_direction.py
+-rw-r--r--   0        0        0      731 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/gradient_algorithm.py
+-rw-r--r--   0        0        0      589 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/newton_algorithm.py
+-rw-r--r--   0        0        0     3121 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/quasi_newton.py
+-rw-r--r--   0        0        0      197 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/__init__.py
+-rw-r--r--   0        0        0     1824 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/base_unidimensional.py
+-rw-r--r--   0        0        0     1305 2023-04-10 17:48:13.277434 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/golden_section.py
+-rw-r--r--   0        0        0     5579 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/multimodal_golden_section.py
+-rw-r--r--   0        0        0       63 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/utils/__init__.py
+-rw-r--r--   0        0        0     4684 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/utils/algorithms_utils.py
+-rw-r--r--   0        0        0      255 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/__init__.py
+-rw-r--r--   0        0        0      504 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/__init__.pyc
+-rw-r--r--   0        0        0      446 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/builder_optimization_problem.py
+-rw-r--r--   0        0        0     4766 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/constraint.py
+-rw-r--r--   0        0        0     1823 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/objective.py
+-rw-r--r--   0        0        0    15936 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/optimization_problem.py
+-rw-r--r--   0        0        0     3292 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/variable.py
+-rw-r--r--   0        0        0      599 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/__init__.py
+-rw-r--r--   0        0        0     2002 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/decomposition_example.py
+-rw-r--r--   0        0        0     1323 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/diet_example.py
+-rw-r--r--   0        0        0     1542 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/ellipsoid_example.py
+-rw-r--r--   0        0        0     1213 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/generic_function_example.py
+-rw-r--r--   0        0        0      660 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/kleeminty_example.py
+-rw-r--r--   0        0        0      909 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/lp_sampling.py
+-rw-r--r--   0        0        0     1236 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/mgs_rastringin.py
+-rw-r--r--   0        0        0     2003 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/multiobjective_example.py
+-rw-r--r--   0        0        0     4106 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/neldermead_article_example.py
+-rw-r--r--   0        0        0    10402 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/neldermead_example.py
+-rw-r--r--   0        0        0     3144 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs0.py
+-rw-r--r--   0        0        0     3295 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs1.py
+-rw-r--r--   0        0        0     1655 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs2.py
+-rw-r--r--   0        0        0     1956 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs3.py
+-rw-r--r--   0        0        0     1622 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/plot_example.py
+-rw-r--r--   0        0        0     1530 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/quadratic_example.py
+-rw-r--r--   0        0        0      318 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/__init__.py
+-rw-r--r--   0        0        0    10400 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/base_function.py
+-rw-r--r--   0        0        0     7807 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/functions_composite.py
+-rw-r--r--   0        0        0     2486 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/generic_function.py
+-rw-r--r--   0        0        0     5421 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/lagrange_function.py
+-rw-r--r--   0        0        0     3173 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/linear_function.py
+-rw-r--r--   0        0        0     8303 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/polynomial_function.py
+-rw-r--r--   0        0        0     2821 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/quadratic_function.py
+-rw-r--r--   0        0        0      297 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/__init__.py
+-rw-r--r--   0        0        0     2964 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/diet.py
+-rw-r--r--   0        0        0     2694 2022-11-08 13:53:18.706299 science_optimization-9.0.1/science_optimization/problems/generic.py
+-rw-r--r--   0        0        0     2333 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/klee_minty.py
+-rw-r--r--   0        0        0     4853 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/mip.py
+-rw-r--r--   0        0        0     2416 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/quadratic.py
+-rw-r--r--   0        0        0     5971 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/rosen_suzuki.py
+-rw-r--r--   0        0        0     3145 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/separable_resource_allocation.py
+-rw-r--r--   0        0        0       67 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/profiling/__init__.py
+-rw-r--r--   0        0        0     2164 2022-11-08 13:53:18.706299 science_optimization-9.0.1/science_optimization/profiling/profiling.py
+-rw-r--r--   0        0        0      150 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/__init__.py
+-rw-r--r--   0        0        0     2824 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/solvers/optimization_results.py
+-rw-r--r--   0        0        0     2616 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/optimizer.py
+-rw-r--r--   0        0        0      310 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/__init__.py
+-rw-r--r--   0        0        0     5804 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py
+-rw-r--r--   0        0        0     8087 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/epsilon_sampler.py
+-rw-r--r--   0        0        0     3270 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/lambda_sampler.py
+-rw-r--r--   0        0        0     3845 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/mu_sampler.py
+-rw-r--r--   0        0        0     3786 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/nondominated_sampler.py
+-rw-r--r--   0        0        0     2202 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/random_sampler.py
+-rw-r--r--   0        0        0      403 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/test/__init__.py
+-rw-r--r--   0        0        0     4286 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_algorithm_utils.py
+-rw-r--r--   0        0        0     3386 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_base_linear.py
+-rw-r--r--   0        0        0     8060 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_builder_package.py
+-rw-r--r--   0        0        0    39169 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_constraint_algorithms.py
+-rw-r--r--   0        0        0    35781 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_functions.py
+-rw-r--r--   0        0        0     4511 2022-11-08 13:53:18.706299 science_optimization-9.0.1/science_optimization/test/test_glop.py
+-rw-r--r--   0        0        0     8156 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_pareto_sampler.py
+-rw-r--r--   0        0        0     6502 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_problems.py
+-rw-r--r--   0        0        0     4403 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_search_direction.py
+-rw-r--r--   0        0        0     2912 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_unidimensional.py
+-rw-r--r--   0        0        0    13229 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/valueslinear.pickle
+-rw-r--r--   0        0        0    13262 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/valuesquad.pickle
+-rw-r--r--   0        0        0    13262 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/valuessparse.pickle
+-rw-r--r--   0        0        0        0 2023-03-23 19:11:45.733736 science_optimization-9.0.1/src/__init__.py
+-rw-r--r--   0        0        0     9974 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/algorithms.h
+-rw-r--r--   0        0        0    26683 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/matrix.h
+-rw-r--r--   0        0        0     4064 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/nlpalg.cpp
+-rw-r--r--   0        0        0   163623 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/nlpalg.pdf
+-rw-r--r--   0        0        0     7608 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/pybind.vcxproj
+-rw-r--r--   0        0        0    12983 1970-01-01 00:00:00.000000 science_optimization-9.0.1/PKG-INFO
```

### Comparing `science_optimization-8.0.1/README.md` & `science_optimization-9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/build.py` & `science_optimization-9.0.1/build.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/base_algorithms.py` & `science_optimization-9.0.1/science_optimization/algorithms/base_algorithms.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/cutting_plane/ellipsoid_method.py` & `science_optimization-9.0.1/science_optimization/algorithms/cutting_plane/ellipsoid_method.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/decomposition/dual_decomposition.py` & `science_optimization-9.0.1/science_optimization/algorithms/decomposition/dual_decomposition.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/derivative_free/nelder_mead.py` & `science_optimization-9.0.1/science_optimization/algorithms/derivative_free/nelder_mead.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/lagrange/augmented_lagrangian.py` & `science_optimization-9.0.1/science_optimization/algorithms/lagrange/augmented_lagrangian.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/linear_programming/glop.py` & `science_optimization-9.0.1/science_optimization/algorithms/linear_programming/glop.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/linear_programming/scipy_base_linear.py` & `science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_base_linear.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/search_direction/base_search_direction.py` & `science_optimization-9.0.1/science_optimization/algorithms/search_direction/base_search_direction.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/search_direction/gradient_algorithm.py` & `science_optimization-9.0.1/science_optimization/algorithms/search_direction/gradient_algorithm.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/search_direction/newton_algorithm.py` & `science_optimization-9.0.1/science_optimization/algorithms/search_direction/newton_algorithm.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/search_direction/quasi_newton.py` & `science_optimization-9.0.1/science_optimization/algorithms/search_direction/quasi_newton.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/unidimensional/base_unidimensional.py` & `science_optimization-9.0.1/science_optimization/algorithms/unidimensional/base_unidimensional.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/unidimensional/golden_section.py` & `science_optimization-9.0.1/science_optimization/algorithms/unidimensional/golden_section.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/unidimensional/multimodal_golden_section.py` & `science_optimization-9.0.1/science_optimization/algorithms/unidimensional/multimodal_golden_section.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/algorithms/utils/algorithms_utils.py` & `science_optimization-9.0.1/science_optimization/algorithms/utils/algorithms_utils.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/builder/constraint.py` & `science_optimization-9.0.1/science_optimization/builder/constraint.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/builder/objective.py` & `science_optimization-9.0.1/science_optimization/builder/objective.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/builder/optimization_problem.py` & `science_optimization-9.0.1/science_optimization/builder/optimization_problem.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/builder/variable.py` & `science_optimization-9.0.1/science_optimization/builder/variable.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/__init__.py` & `science_optimization-9.0.1/science_optimization/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/decomposition_example.py` & `science_optimization-9.0.1/science_optimization/examples/decomposition_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/diet_example.py` & `science_optimization-9.0.1/science_optimization/examples/diet_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/ellipsoid_example.py` & `science_optimization-9.0.1/science_optimization/examples/ellipsoid_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/generic_function_example.py` & `science_optimization-9.0.1/science_optimization/examples/generic_function_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/kleeminty_example.py` & `science_optimization-9.0.1/science_optimization/examples/kleeminty_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/lp_sampling.py` & `science_optimization-9.0.1/science_optimization/examples/lp_sampling.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/mgs_rastringin.py` & `science_optimization-9.0.1/science_optimization/examples/mgs_rastringin.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/multiobjective_example.py` & `science_optimization-9.0.1/science_optimization/examples/multiobjective_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/neldermead_article_example.py` & `science_optimization-9.0.1/science_optimization/examples/neldermead_article_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/neldermead_example.py` & `science_optimization-9.0.1/science_optimization/examples/neldermead_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs0.py` & `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs0.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs1.py` & `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs1.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs2.py` & `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs2.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/pareto_sampling_cs3.py` & `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs3.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/plot_example.py` & `science_optimization-9.0.1/science_optimization/examples/plot_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/examples/quadratic_example.py` & `science_optimization-9.0.1/science_optimization/examples/quadratic_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/function/base_function.py` & `science_optimization-9.0.1/science_optimization/function/base_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/function/functions_composite.py` & `science_optimization-9.0.1/science_optimization/function/functions_composite.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/function/generic_function.py` & `science_optimization-9.0.1/science_optimization/function/generic_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/function/lagrange_function.py` & `science_optimization-9.0.1/science_optimization/function/lagrange_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/function/linear_function.py` & `science_optimization-9.0.1/science_optimization/function/linear_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/function/polynomial_function.py` & `science_optimization-9.0.1/science_optimization/function/polynomial_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/function/quadratic_function.py` & `science_optimization-9.0.1/science_optimization/function/quadratic_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/problems/diet.py` & `science_optimization-9.0.1/science_optimization/problems/diet.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/problems/generic.py` & `science_optimization-9.0.1/science_optimization/problems/generic.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/problems/klee_minty.py` & `science_optimization-9.0.1/science_optimization/problems/klee_minty.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/problems/mip.py` & `science_optimization-9.0.1/science_optimization/problems/mip.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/problems/quadratic.py` & `science_optimization-9.0.1/science_optimization/problems/quadratic.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/problems/rosen_suzuki.py` & `science_optimization-9.0.1/science_optimization/problems/rosen_suzuki.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/problems/separable_resource_allocation.py` & `science_optimization-9.0.1/science_optimization/problems/separable_resource_allocation.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/profiling/profiling.py` & `science_optimization-9.0.1/science_optimization/profiling/profiling.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/optimization_results.py` & `science_optimization-9.0.1/science_optimization/solvers/optimization_results.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/optimizer.py` & `science_optimization-9.0.1/science_optimization/solvers/optimizer.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py` & `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/epsilon_sampler.py` & `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/epsilon_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/lambda_sampler.py` & `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/lambda_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/mu_sampler.py` & `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/mu_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/nondominated_sampler.py` & `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/nondominated_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/solvers/pareto_samplers/random_sampler.py` & `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_algorithm_utils.py` & `science_optimization-9.0.1/science_optimization/test/test_algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_base_linear.py` & `science_optimization-9.0.1/science_optimization/test/test_base_linear.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_builder_package.py` & `science_optimization-9.0.1/science_optimization/test/test_builder_package.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_constraint_algorithms.py` & `science_optimization-9.0.1/science_optimization/test/test_constraint_algorithms.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_functions.py` & `science_optimization-9.0.1/science_optimization/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_glop.py` & `science_optimization-9.0.1/science_optimization/test/test_glop.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_pareto_sampler.py` & `science_optimization-9.0.1/science_optimization/test/test_pareto_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_problems.py` & `science_optimization-9.0.1/science_optimization/test/test_problems.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_search_direction.py` & `science_optimization-9.0.1/science_optimization/test/test_search_direction.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/test_unidimensional.py` & `science_optimization-9.0.1/science_optimization/test/test_unidimensional.py`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/valueslinear.pickle` & `science_optimization-9.0.1/science_optimization/test/valueslinear.pickle`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/valuesquad.pickle` & `science_optimization-9.0.1/science_optimization/test/valuesquad.pickle`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/science_optimization/test/valuessparse.pickle` & `science_optimization-9.0.1/science_optimization/test/valuessparse.pickle`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/src/algorithms.h` & `science_optimization-9.0.1/src/algorithms.h`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/src/matrix.h` & `science_optimization-9.0.1/src/matrix.h`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/src/nlpalg.cpp` & `science_optimization-9.0.1/src/nlpalg.cpp`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/src/nlpalg.pdf` & `science_optimization-9.0.1/src/nlpalg.pdf`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/src/pybind.vcxproj` & `science_optimization-9.0.1/src/pybind.vcxproj`

 * *Files identical despite different names*

### Comparing `science_optimization-8.0.1/setup.py` & `science_optimization-9.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,416 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: science-optimization
+Version: 9.0.1
+Summary: A framework for optimization.
+Author: Matheus Mendonça
+Author-email: matheus.mendonca@enacom.com.br
+Requires-Python: >=3.8,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cycler (>=0.11,<1.0)
+Requires-Dist: decorator (>=5.1,<6.0)
+Requires-Dist: joblib (>=1.1,<2.0)
+Requires-Dist: kiwisolver (>=1.3,<2.0)
+Requires-Dist: matplotlib (>=3.4,<4.0)
+Requires-Dist: networkx (>=2.6,<3.0)
+Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: ortools (>=9.6,<10.0)
+Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: pillow (>=9.3,<10.0)
+Requires-Dist: protobuf (>=4.22,<5.0)
+Requires-Dist: pybind11 (>=2.10.4,<3.0.0)
+Requires-Dist: pyparsing (>=3.0,<4.0)
+Requires-Dist: python-dateutil (>=2.8,<3.0)
+Requires-Dist: pytz (>=2021.3,<2022.0)
+Requires-Dist: pywavelets (>=1.1,<2.0)
+Requires-Dist: scipy (>=1.10,<2.0)
+Requires-Dist: six (>=1.16,<2.0)
+Requires-Dist: xlrd (>=2.0,<3.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['science_optimization',
- 'science_optimization.algorithms',
- 'science_optimization.algorithms.cutting_plane',
- 'science_optimization.algorithms.decomposition',
- 'science_optimization.algorithms.derivative_free',
- 'science_optimization.algorithms.lagrange',
- 'science_optimization.algorithms.linear_programming',
- 'science_optimization.algorithms.search_direction',
- 'science_optimization.algorithms.unidimensional',
- 'science_optimization.algorithms.utils',
- 'science_optimization.builder',
- 'science_optimization.examples',
- 'science_optimization.function',
- 'science_optimization.problems',
- 'science_optimization.profiling',
- 'science_optimization.solvers',
- 'science_optimization.solvers.pareto_samplers',
- 'science_optimization.test',
- 'src']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cycler>=0.11,<1.0',
- 'decorator>=5.1,<6.0',
- 'joblib>=1.1,<2.0',
- 'kiwisolver>=1.3,<2.0',
- 'matplotlib>=3.4,<4.0',
- 'networkx>=2.6,<3.0',
- 'numpy>=1.21,<2.0',
- 'ortools>=9.1,<10.0',
- 'pandas>=1.3,<2.0',
- 'pillow>=8.4,<9.0',
- 'protobuf>=3.19,<4.0',
- 'pybind11>=2.10.3,<3.0.0',
- 'pyparsing>=3.0,<4.0',
- 'python-dateutil>=2.8,<3.0',
- 'pytz>=2021.3,<2022.0',
- 'pywavelets>=1.1,<2.0',
- 'scipy>=1.7,<2.0',
- 'six>=1.16,<2.0',
- 'xlrd>=2.0,<3.0']
-
-setup_kwargs = {
-    'name': 'science-optimization',
-    'version': '8.0.1',
-    'description': 'A framework for optimization.',
-    'long_description': '# Optimization Framework \n\nThis is a framework for linear and non-linear optimization developed by ENACOM Group.\n\nIt solves a problem in the form:\n\n```\nmin  f(x)\n\ns.t. g(x) <= 0\n     h(x)  = 0\n     x_min <= x <= x_max\n```\n\nwhere `x` is an n-dimensional vector, `f(x)` maps the n-dimensional space to the o-dimensional space,\nwith `o` being the number of objectives. \n## Prerequisites\n\nWhat you need to be able to run:\n\n* Python 3.6 +\n\nAll requirements are in the file `requirements.txt`.\nTo install all packages at once: \n```shell\n$ pip install -r requirements.txt\n```\n\n## Installing science-optimization\n\nBuilding science-optimization requires the following software installed:\n\n1. Python 3\n    - Make sure that distutils is installed before continuing. For example in Debian GNU/Linux, disutils is included in the python3-dev package.\n2. PyBind11\n    - Note  that this is PyBind11, not PyBind.\n3. GNU C Compiler version >= 5.0\n\nTo install the package in any environment:\n\n- clone this repo\n- `$ pip install ./science-optimization`\n\n## Conventions\n\n### Development\n\n- In Python programming, it is a common practice to initialize "private" methods/attributes with an underscore \n(e.g. _private_method(), _private_attribute). This framework follows this convention\n\n- Attributes sets and gets are implemented using the native \n[`@property`](https://www.programiz.com/python-programming/property) decorator\n\n- An abstract base class inherits from `abc.ABCMeta`\n\n- Google is the default Docstring format\n\n- A package must contain an `__init__.py` file with the package initialization\n\n- PyCharm 2017+ is highly recommended\n\nA detailed explanation of code development can be found [here](https://github.com/LucasSubli/EnacomPythonExample) and \n[here](https://sourcemaking.com/design_patterns).\n\nTutorials on Python programming can be found \n[here](https://www.digitalocean.com/community/tutorial_series/object-oriented-programming-in-python-3).\n\n### Optimization\n\nGiven that `n` is the problem dimension and `m` is the number of points:\n\n- A single point is a `nx1` matrix\n\n- Multiple points are a `nxm` matrix\n\n- Gradient is a `nxm` matrix\n\n- Hessian is a `nxnxm` matrix\n\n## Packages\n\n### Builder\n\nThis package is responsible for building an optimization problem. It was built based on the \n[Builder Design Pattern](https://sourcemaking.com/design_patterns/builder) and it has the following classes.\n\n1. `OptimizationProblem()`: the base class of every optimization problem.\n\n    - Attributes:\n\n        * `objective`: `Objective()` instance\n    \n        * `constraints`: `Contraints()` instance\n    \n        * `variables`: `Variables()` instance\n    \n    - Methods:\n\n        * `_build_problem(builder)`: receives a `BuilderOptimizationProblem()` instance, checks problem\n    consistency and sets attributes\n    \n        * `_check_consistency(variables, objectives, constraints)`: receives attributes and check problem\n    consistency\n    \n        * `info()`: prints to user the assembled problem\n        \n        * `__call__()`: overloaded method that turns an `OptimizationProblem` instance a callable function, that\n        evaluates `f, g, h, df, dg, dh, hf, hg, hh` for a given point `x`\n\n2. `BuilderOptimizationProblem()`: abstract class responsible for defining the builder\'s methods of the \noptimization problem.\n\n    - Abstract methods:\n    \n        * `build_objectives()`: abstract method responsible for building the problem\'s objectives\n        \n        * `build_constraints()`: abstract method responsible for building the problem\'s constraints\n        \n        * `build_variables()`: abstract method responsible for building the problem\'s variables\n\n3. `Objective()`: container class of objectives functions.\n\n    - Attributes:\n    \n        * `objective_functions`: a list with all functions of the problem. Each function\n        is a `FunctionComposite()` instance.\n        \n    - Methods:\n    \n        * `C()`: return the matrix C of linear objectives coefficients\n        \n        * `d()`: return the vector d of linear objectives constants\n\n4. `Contraints()`: container class of constraints functions.\n\n    - Attributes:\n    \n        * `equality_contraints`: a list with equality constraints functions. Each function\n        is a `FunctionComposite()` instance.\n        \n        * `inequality_contraints`: a list with inequality constraints functions. Each function\n        is a `FunctionComposite()` instance.\n        \n    - Methods:\n    \n        * `equality_contraints_feasibility(x)`: evaluates the feasibility of `x` on these constraints\n        \n        * `inequality_contraints_feasibility(x)`: evaluates the feasibility of `x` on these constraints\n        \n        * `A()`: returns the matrix `A` of linear inequality constraints coefficients\n        \n        * `b()`: returns the vector `b` of linear inequality constraints bounds\n        \n        * `Aeq()`: returns the matrix `Aeq` of linear equality constraints coefficients\n        \n        * `beq()`: returns the vector `beq` of linear equality constraints bounds\n\n5. `Variables()`: container class of the problem variables.\n\n    - Attributes:\n        \n        * `x_min`: variables\' lower bounds\n        \n        * `x_max`: variables\' upper bounds\n        \n        * `x_type`: list with variables\' type (\'c\': continuous or \'d\': discrete)\n        \n\n### Function\n\nThis package has the definitions of a function. Is was base on the \n[Composite](https://sourcemaking.com/design_patterns/composite) design pattern and \ncontains the following classes:\n\n1. `BaseFunction()`: base class of every other class inside this package.\n\n    - Attributes:\n    \n        * `parameters`: abstract attribute for functions parameters (e.g. coefficients)\n        \n        * `eps`: precision for numerical calculations\n        \n    - Methods:\n    \n        * `eval(x)`: abstract method for the evaluation of `x`\n        \n        * `gradient(x)`: numerical calculation of the Gradient of `x`\n        \n        * `hessian(x)`: numerical calculation of the Hessian of `x`\n        \n        * `dimension()`: function dimension `n`\n\n2. `FunctionsComposite()`: container class of `BaseFunction()`\'s children.\n\n    - Attributes:\n    \n        * `functions`: a list of functions\n        \n    - Methods:\n    \n        * `eval(x)`: abstract method for the evaluation of `x` in `functions`\n        \n        * `gradient(x)`: numerical calculation of the Gradient of `x` in `functions`\n        \n        * `hessian(x)`: numerical calculation of the Hessian of `x` in `functions`\n        \n        * `add(f)`: adds function `f` to `functions`\n        \n        * `remove(idx)`: removes element `functions[idx]`\n        \n        * `clear()`: removes all functions from list\n        \n         \n3. `LinearFunction()`: implements a function in the form `f(x) = c\'x + d`\n\n    - Attributes:\n    \n        * `parameters`: dictionary with `c` and `d` keys\n        \n    - Methods:\n        \n        * `eval(x)`: method for the evaluation of `x`\n        \n        * `gradient(x)`: analytical calculation of the Gradient of `x`\n        \n        * `hessian(x)`: analytical calculation of the Hessian of `x`    \n\n4. `QuadraticFunction()`: implements a function in the form `f(x) = x\'Qx + c\'x + d`\n\n    - Attributes:\n    \n        * `parameters`: dictionary with `Q`, `c` and `d` keys\n        \n    - Methods:\n        \n        * `eval(x)`: method for the evaluation of `x`\n        \n        * `gradient(x)`: analytical calculation of the Gradient of `x`\n        \n        * `hessian(x)`: analytical calculation of the Hessian of `x`\n\n5. `PolynomialFunction()`: implements a polynomial function\n\n    - Attributes:\n    \n        * `parameters`: dictionary with exponents `e` and `c` coefficients\n        \n    - Methods:\n        \n        * `eval(x)`: method for the evaluation of `x`\n        \n        * `gradient(x)`: analytical calculation of the Gradient of `x`\n        \n        * `hessian(x)`: analytical calculation of the Hessian of `x`\n\n### Problems\n\nThis package is responsible for creating the interface of `BuilderOptimizationProblem()` for each optimization problem\ninstance. The classes must follow the format:\n\n1. `Problem(BuilderOptimizationProblem)`: inherits from BuilderOptimizationProblem\n\n    - Attributes: necessary problem attributes\n    \n    - Methods:\n    \n        * `build_objectives()`: concrete method responsible for building the problem\'s objectives\n        \n        * `build_constraints()`: concrete method responsible for building the problem\'s constraints\n        \n        * `build_variables()`: concrete method responsible for building the problem\'s variables\n\nThe class `Generic(BuilderOptimizationProblem)` builds a generic optimization problem in the canonical\nformat defined at the beginning of this document. However, it also possible to implement customized \noptimization problems inheriting from `BuilderOptimizationProblem` class, such as `Diet` and `KleeMinty`.\n\nFor linear programming, the problem `MIP` is a straightforward abstraction of a problem in the format:\n\n```\n    min  c\'  @ x\n    s.t. A   @ x <= b\n         Aeq @ x == beq\n         x_min  <= x <=  x_max\n```\n\n### Algorithms\n\nThis package contains the implementations of the optimization algorithms. It is organized in sub-packages according\nto algorithm\'s families. Each sub-package contains one abstract implementation of the algorithm\'s family, it is named\n`BaseAlgorithmFamily()`\n\n1. `BaseAlgorithms()`: base class for every `BaseAlgorithmFamily()`\n\n    - Attributes:\n    \n        * `eps`: algorithms\' numerical precision\n        \n    - Methods:\n    \n        * `optimize()`: abstract method for the implementation core\n        \nThis framework currently supports the following optimization algorithms:\n\n* Cutting-plane family:\n    * Ellipsoidal (Multiobjective)\n\n* Decomposition :\n    * Nonlinear dual decomposition\n    \n* Derivative-free :\n    * Nelder-Mead simplex (constrained)\n\n* Lagrange (constrained):\n    * Augmented lagrangian method (using Quasi Newton)\n\n* Linear programming:\n    * Scipy simplex and interior-point\n    * GLOP for LP\n    * CBC for MIP\n\n* Unidimensional search:\n    * Enhanced golden section\n    * Multimodal golden section\n\n* Search direction family (unconstrained):\n    * Gradient method\n    * Modified Newton method\n    * Quasi Newton method\n    \n\n### Solvers\n\nThis package contains the interface to optimization solvers implemented in the framework.\n\n1. `Optimizer()`: optimization for built-in methods, i.e. `algorithms`.\n\n    - Attributes\n    \n        * `optimization_problem`: `OptimizationProblem()` instance\n        \n        * `algorithm`: a concrete algorithm implementation instance (e.g. `GradientAlgorithm()`)\n        \n    - Methods\n    \n        * `solve`: implements `algorithm.optimize()`\n\n2. `OptimizationResults()`: container for optimization results\n\n    - Attributes\n    \n        * `x`: the solution of the optimization\n        \n        * `fx`: function value at solution point\n        \n        * `sucess`: whether or not the solvers exited successfully\n        \n        * `message`: description of the cause of termination\n        \n        * `n_iterations`: number of iterations\n        \n        * `n_function_evaluations`: number of function evaluations\n    \n    - Methods\n    \n        * `info()`: displays optimization results info.\n\n3. `pareto_samplers package`: used to find the pareto border of a multiobjective problem, the implemented\n                              sampling strategies are:\n\n    - Lambda sampler\n    - Epsilon sampler\n    - Nondominated sampler\n    - Mu sampler\n\n### Examples\n\nThis package contains modules implementing examples of building and solving an optimization problem. It can also\nbe used for profiling via `@profiling` decorator.\n\n### Profiling\n\nImplementation of the `@profiling` decorator.\n',
-    'author': 'Matheus Mendonça',
-    'author_email': 'matheus.mendonca@enacom.com.br',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4',
-}
-from build import *
-build(setup_kwargs)
+# Optimization Framework 
+
+This is a framework for linear and non-linear optimization developed by ENACOM Group.
+
+It solves a problem in the form:
+
+```
+min  f(x)
+
+s.t. g(x) <= 0
+     h(x)  = 0
+     x_min <= x <= x_max
+```
+
+where `x` is an n-dimensional vector, `f(x)` maps the n-dimensional space to the o-dimensional space,
+with `o` being the number of objectives. 
+## Prerequisites
+
+What you need to be able to run:
+
+* Python 3.6 +
+
+All requirements are in the file `requirements.txt`.
+To install all packages at once: 
+```shell
+$ pip install -r requirements.txt
+```
+
+## Installing science-optimization
+
+Building science-optimization requires the following software installed:
+
+1. Python 3
+    - Make sure that distutils is installed before continuing. For example in Debian GNU/Linux, disutils is included in the python3-dev package.
+2. PyBind11
+    - Note  that this is PyBind11, not PyBind.
+3. GNU C Compiler version >= 5.0
+
+To install the package in any environment:
+
+- clone this repo
+- `$ pip install ./science-optimization`
+
+## Conventions
+
+### Development
+
+- In Python programming, it is a common practice to initialize "private" methods/attributes with an underscore 
+(e.g. _private_method(), _private_attribute). This framework follows this convention
+
+- Attributes sets and gets are implemented using the native 
+[`@property`](https://www.programiz.com/python-programming/property) decorator
+
+- An abstract base class inherits from `abc.ABCMeta`
+
+- Google is the default Docstring format
+
+- A package must contain an `__init__.py` file with the package initialization
+
+- PyCharm 2017+ is highly recommended
+
+A detailed explanation of code development can be found [here](https://github.com/LucasSubli/EnacomPythonExample) and 
+[here](https://sourcemaking.com/design_patterns).
+
+Tutorials on Python programming can be found 
+[here](https://www.digitalocean.com/community/tutorial_series/object-oriented-programming-in-python-3).
+
+### Optimization
+
+Given that `n` is the problem dimension and `m` is the number of points:
+
+- A single point is a `nx1` matrix
+
+- Multiple points are a `nxm` matrix
+
+- Gradient is a `nxm` matrix
+
+- Hessian is a `nxnxm` matrix
+
+## Packages
+
+### Builder
+
+This package is responsible for building an optimization problem. It was built based on the 
+[Builder Design Pattern](https://sourcemaking.com/design_patterns/builder) and it has the following classes.
+
+1. `OptimizationProblem()`: the base class of every optimization problem.
+
+    - Attributes:
+
+        * `objective`: `Objective()` instance
+    
+        * `constraints`: `Contraints()` instance
+    
+        * `variables`: `Variables()` instance
+    
+    - Methods:
+
+        * `_build_problem(builder)`: receives a `BuilderOptimizationProblem()` instance, checks problem
+    consistency and sets attributes
+    
+        * `_check_consistency(variables, objectives, constraints)`: receives attributes and check problem
+    consistency
+    
+        * `info()`: prints to user the assembled problem
+        
+        * `__call__()`: overloaded method that turns an `OptimizationProblem` instance a callable function, that
+        evaluates `f, g, h, df, dg, dh, hf, hg, hh` for a given point `x`
+
+2. `BuilderOptimizationProblem()`: abstract class responsible for defining the builder's methods of the 
+optimization problem.
+
+    - Abstract methods:
+    
+        * `build_objectives()`: abstract method responsible for building the problem's objectives
+        
+        * `build_constraints()`: abstract method responsible for building the problem's constraints
+        
+        * `build_variables()`: abstract method responsible for building the problem's variables
+
+3. `Objective()`: container class of objectives functions.
+
+    - Attributes:
+    
+        * `objective_functions`: a list with all functions of the problem. Each function
+        is a `FunctionComposite()` instance.
+        
+    - Methods:
+    
+        * `C()`: return the matrix C of linear objectives coefficients
+        
+        * `d()`: return the vector d of linear objectives constants
+
+4. `Contraints()`: container class of constraints functions.
+
+    - Attributes:
+    
+        * `equality_contraints`: a list with equality constraints functions. Each function
+        is a `FunctionComposite()` instance.
+        
+        * `inequality_contraints`: a list with inequality constraints functions. Each function
+        is a `FunctionComposite()` instance.
+        
+    - Methods:
+    
+        * `equality_contraints_feasibility(x)`: evaluates the feasibility of `x` on these constraints
+        
+        * `inequality_contraints_feasibility(x)`: evaluates the feasibility of `x` on these constraints
+        
+        * `A()`: returns the matrix `A` of linear inequality constraints coefficients
+        
+        * `b()`: returns the vector `b` of linear inequality constraints bounds
+        
+        * `Aeq()`: returns the matrix `Aeq` of linear equality constraints coefficients
+        
+        * `beq()`: returns the vector `beq` of linear equality constraints bounds
+
+5. `Variables()`: container class of the problem variables.
+
+    - Attributes:
+        
+        * `x_min`: variables' lower bounds
+        
+        * `x_max`: variables' upper bounds
+        
+        * `x_type`: list with variables' type ('c': continuous or 'd': discrete)
+        
+
+### Function
+
+This package has the definitions of a function. Is was base on the 
+[Composite](https://sourcemaking.com/design_patterns/composite) design pattern and 
+contains the following classes:
+
+1. `BaseFunction()`: base class of every other class inside this package.
+
+    - Attributes:
+    
+        * `parameters`: abstract attribute for functions parameters (e.g. coefficients)
+        
+        * `eps`: precision for numerical calculations
+        
+    - Methods:
+    
+        * `eval(x)`: abstract method for the evaluation of `x`
+        
+        * `gradient(x)`: numerical calculation of the Gradient of `x`
+        
+        * `hessian(x)`: numerical calculation of the Hessian of `x`
+        
+        * `dimension()`: function dimension `n`
+
+2. `FunctionsComposite()`: container class of `BaseFunction()`'s children.
+
+    - Attributes:
+    
+        * `functions`: a list of functions
+        
+    - Methods:
+    
+        * `eval(x)`: abstract method for the evaluation of `x` in `functions`
+        
+        * `gradient(x)`: numerical calculation of the Gradient of `x` in `functions`
+        
+        * `hessian(x)`: numerical calculation of the Hessian of `x` in `functions`
+        
+        * `add(f)`: adds function `f` to `functions`
+        
+        * `remove(idx)`: removes element `functions[idx]`
+        
+        * `clear()`: removes all functions from list
+        
+         
+3. `LinearFunction()`: implements a function in the form `f(x) = c'x + d`
+
+    - Attributes:
+    
+        * `parameters`: dictionary with `c` and `d` keys
+        
+    - Methods:
+        
+        * `eval(x)`: method for the evaluation of `x`
+        
+        * `gradient(x)`: analytical calculation of the Gradient of `x`
+        
+        * `hessian(x)`: analytical calculation of the Hessian of `x`    
+
+4. `QuadraticFunction()`: implements a function in the form `f(x) = x'Qx + c'x + d`
+
+    - Attributes:
+    
+        * `parameters`: dictionary with `Q`, `c` and `d` keys
+        
+    - Methods:
+        
+        * `eval(x)`: method for the evaluation of `x`
+        
+        * `gradient(x)`: analytical calculation of the Gradient of `x`
+        
+        * `hessian(x)`: analytical calculation of the Hessian of `x`
+
+5. `PolynomialFunction()`: implements a polynomial function
+
+    - Attributes:
+    
+        * `parameters`: dictionary with exponents `e` and `c` coefficients
+        
+    - Methods:
+        
+        * `eval(x)`: method for the evaluation of `x`
+        
+        * `gradient(x)`: analytical calculation of the Gradient of `x`
+        
+        * `hessian(x)`: analytical calculation of the Hessian of `x`
+
+### Problems
+
+This package is responsible for creating the interface of `BuilderOptimizationProblem()` for each optimization problem
+instance. The classes must follow the format:
+
+1. `Problem(BuilderOptimizationProblem)`: inherits from BuilderOptimizationProblem
+
+    - Attributes: necessary problem attributes
+    
+    - Methods:
+    
+        * `build_objectives()`: concrete method responsible for building the problem's objectives
+        
+        * `build_constraints()`: concrete method responsible for building the problem's constraints
+        
+        * `build_variables()`: concrete method responsible for building the problem's variables
+
+The class `Generic(BuilderOptimizationProblem)` builds a generic optimization problem in the canonical
+format defined at the beginning of this document. However, it also possible to implement customized 
+optimization problems inheriting from `BuilderOptimizationProblem` class, such as `Diet` and `KleeMinty`.
+
+For linear programming, the problem `MIP` is a straightforward abstraction of a problem in the format:
+
+```
+    min  c'  @ x
+    s.t. A   @ x <= b
+         Aeq @ x == beq
+         x_min  <= x <=  x_max
+```
+
+### Algorithms
+
+This package contains the implementations of the optimization algorithms. It is organized in sub-packages according
+to algorithm's families. Each sub-package contains one abstract implementation of the algorithm's family, it is named
+`BaseAlgorithmFamily()`
+
+1. `BaseAlgorithms()`: base class for every `BaseAlgorithmFamily()`
+
+    - Attributes:
+    
+        * `eps`: algorithms' numerical precision
+        
+    - Methods:
+    
+        * `optimize()`: abstract method for the implementation core
+        
+This framework currently supports the following optimization algorithms:
+
+* Cutting-plane family:
+    * Ellipsoidal (Multiobjective)
+
+* Decomposition :
+    * Nonlinear dual decomposition
+    
+* Derivative-free :
+    * Nelder-Mead simplex (constrained)
+
+* Lagrange (constrained):
+    * Augmented lagrangian method (using Quasi Newton)
+
+* Linear programming:
+    * Scipy simplex and interior-point
+    * GLOP for LP
+    * CBC for MIP
+
+* Unidimensional search:
+    * Enhanced golden section
+    * Multimodal golden section
+
+* Search direction family (unconstrained):
+    * Gradient method
+    * Modified Newton method
+    * Quasi Newton method
+    
+
+### Solvers
+
+This package contains the interface to optimization solvers implemented in the framework.
+
+1. `Optimizer()`: optimization for built-in methods, i.e. `algorithms`.
+
+    - Attributes
+    
+        * `optimization_problem`: `OptimizationProblem()` instance
+        
+        * `algorithm`: a concrete algorithm implementation instance (e.g. `GradientAlgorithm()`)
+        
+    - Methods
+    
+        * `solve`: implements `algorithm.optimize()`
+
+2. `OptimizationResults()`: container for optimization results
+
+    - Attributes
+    
+        * `x`: the solution of the optimization
+        
+        * `fx`: function value at solution point
+        
+        * `sucess`: whether or not the solvers exited successfully
+        
+        * `message`: description of the cause of termination
+        
+        * `n_iterations`: number of iterations
+        
+        * `n_function_evaluations`: number of function evaluations
+    
+    - Methods
+    
+        * `info()`: displays optimization results info.
+
+3. `pareto_samplers package`: used to find the pareto border of a multiobjective problem, the implemented
+                              sampling strategies are:
+
+    - Lambda sampler
+    - Epsilon sampler
+    - Nondominated sampler
+    - Mu sampler
+
+### Examples
+
+This package contains modules implementing examples of building and solving an optimization problem. It can also
+be used for profiling via `@profiling` decorator.
+
+### Profiling
+
+Implementation of the `@profiling` decorator.
 
-setup(**setup_kwargs)
```

