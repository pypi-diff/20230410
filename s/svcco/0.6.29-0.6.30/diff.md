# Comparing `tmp/svcco-0.6.29.tar.gz` & `tmp/svcco-0.6.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svcco-0.6.29.tar", last modified: Thu Apr  6 19:16:55 2023, max compression
+gzip compressed data, was "svcco-0.6.30.tar", last modified: Mon Apr 10 20:02:11 2023, max compression
```

## Comparing `svcco-0.6.29.tar` & `svcco-0.6.30.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.516540 svcco-0.6.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-06 19:16:44.000000 svcco-0.6.29/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-06 19:16:55.516540 svcco-0.6.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-06 19:16:44.000000 svcco-0.6.29/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 19:16:55.516540 svcco-0.6.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-06 19:16:45.000000 svcco-0.6.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.480538 svcco-0.6.29/svcco/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.488539 svcco-0.6.29/svcco/branch_addition/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_bifurcation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_branches_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28983 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_branches_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/add_geodesic_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/calculate_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/calculate_radii.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/close.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/geodesic.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/get_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/get_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/local_func_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/local_func_v6.py
--rw-r--r--   0 runner    (1001) docker     (123)    25855 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/local_func_v7.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/sample_triad.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/set_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/set_root_homogeneous_nonconvex.py
--rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/branch_addition/update_geodesic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.492539 svcco-0.6.29/svcco/collision/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/collision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25794 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/collision/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/collision/obb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/collision/obb_unit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/collision/sphere_proximity.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/collision/sphere_proximity_unit_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.492539 svcco-0.6.29/svcco/forest_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/compete_add.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/connect_collision.py
--rw-r--r--   0 runner    (1001) docker     (123)    30103 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/optimize_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/optimize_connection_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/optimize_connection_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/optimize_connection_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/optimize_connection_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/forest_utils/smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.492539 svcco-0.6.29/svcco/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.496539 svcco-0.6.29/svcco/implicit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/core/a_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/core/h_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/core/m_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/core/n_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    58198 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)    52523 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/implicit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.496539 svcco-0.6.29/svcco/implicit/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/kernel/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.496539 svcco-0.6.29/svcco/implicit/kernel/kernel_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/kernel/kernel_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/kernel/kernel_functions/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/kernel/kernel_functions/grad.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/kernel/kernel_functions/hess.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.496539 svcco-0.6.29/svcco/implicit/solver/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/solver/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.496539 svcco-0.6.29/svcco/implicit/solver/solver_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/solver/solver_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/solver/solver_functions/init_normals_given.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/solver/solver_functions/init_normals_not_given.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.496539 svcco-0.6.29/svcco/implicit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/tests/bumpy_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/tests/heart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.496539 svcco-0.6.29/svcco/implicit/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27404 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/visualize/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/implicit/weingarten_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.500539 svcco-0.6.29/svcco/sv_interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.508539 svcco-0.6.29/svcco/sv_interface/Post/
--rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/1D_to_3D_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/asymptotic_pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/bc_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/check_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18067 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/compare_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/compare_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/compare_centerline_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/create_db_from_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_faceid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_surf_discr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_surf_displacement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_surf_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_surf_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_surf_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/fix_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_bc_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_bcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_branches_bifurcations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)    35969 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_mean_flow_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_rom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_statistics_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_statistics_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_statistics_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_sv_meshes.py
--rw-r--r--   0 runner    (1001) docker     (123)    37033 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/get_sv_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/inflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/lift_laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/paper_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/plot_pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/post_process_1d_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/postproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/project_1d_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/simulation_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/sv_get_path_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/vtk_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/Post/vtk_to_xdmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.512539 svcco-0.6.29/svcco/sv_interface/ROM/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/centerlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    25287 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/generate_1d_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/io_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/io_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/io_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/ROM/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/build_0d_run_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/build_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/build_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/export_3d_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    47588 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/get_sv_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/locate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/loft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    22017 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/presolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/rom.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/solid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/sv_install_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/view_0d_result_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    27999 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/sv_interface/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/test_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)   161493 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.512539 svcco-0.6.29/svcco/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.512539 svcco-0.6.29/svcco/utils/fluid_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/fluid_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/fluid_analysis/reynolds.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/fluid_analysis/wss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.512539 svcco-0.6.29/svcco/utils/gcode/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/gcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/gcode/gcode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.512539 svcco-0.6.29/svcco/utils/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/gui/gui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/gui/spline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.512539 svcco-0.6.29/svcco/utils/perfusion/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/perfusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/perfusion/fast_geodesic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.516540 svcco-0.6.29/svcco/utils/remeshing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.516540 svcco-0.6.29/svcco/utils/remeshing/Linux/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/remeshing/Linux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.516540 svcco-0.6.29/svcco/utils/remeshing/Mac/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/remeshing/Mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.516540 svcco-0.6.29/svcco/utils/remeshing/Windows/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/remeshing/Windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/remeshing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-06 19:16:45.000000 svcco-0.6.29/svcco/utils/remeshing/remesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:16:55.484539 svcco-0.6.29/svcco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-06 19:16:55.000000 svcco-0.6.29/svcco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-06 19:16:55.000000 svcco-0.6.29/svcco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:55.000000 svcco-0.6.29/svcco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:16:55.000000 svcco-0.6.29/svcco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-06 19:16:55.000000 svcco-0.6.29/svcco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 19:16:55.000000 svcco-0.6.29/svcco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.393683 svcco-0.6.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-10 20:02:03.000000 svcco-0.6.30/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-10 20:02:11.393683 svcco-0.6.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-10 20:02:03.000000 svcco-0.6.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 20:02:11.393683 svcco-0.6.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-10 20:02:03.000000 svcco-0.6.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.365683 svcco-0.6.30/svcco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.373683 svcco-0.6.30/svcco/branch_addition/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_bifurcation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_branches_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28983 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_branches_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/add_geodesic_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/calculate_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/calculate_radii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/get_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/get_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/local_func_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/local_func_v6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25855 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/local_func_v7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/sample_triad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/set_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/set_root_homogeneous_nonconvex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/branch_addition/update_geodesic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.373683 svcco-0.6.30/svcco/collision/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/collision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25794 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/collision/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/collision/obb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/collision/obb_unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/collision/sphere_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/collision/sphere_proximity_unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.377683 svcco-0.6.30/svcco/forest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/compete_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/connect_collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30103 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/optimize_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/optimize_connection_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/optimize_connection_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/optimize_connection_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34225 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/optimize_connection_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/forest_utils/smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.377683 svcco-0.6.30/svcco/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/implicit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/core/a_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/core/h_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/core/m_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/core/n_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58198 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52523 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/implicit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/implicit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/kernel/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/implicit/kernel/kernel_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/kernel/kernel_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/kernel/kernel_functions/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/kernel/kernel_functions/grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/kernel/kernel_functions/hess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/implicit/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/solver/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/implicit/solver/solver_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/solver/solver_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/solver/solver_functions/init_normals_given.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/solver/solver_functions/init_normals_not_given.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/implicit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/tests/bumpy_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/tests/heart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/implicit/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27404 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/visualize/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/implicit/weingarten_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.381683 svcco-0.6.30/svcco/sv_interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.385683 svcco-0.6.30/svcco/sv_interface/Post/
+-rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/1D_to_3D_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/asymptotic_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/bc_0d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/check_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18067 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/compare_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/compare_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/compare_centerline_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/create_db_from_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_faceid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_surf_discr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_surf_displacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_surf_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_surf_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_surf_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/fix_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_bc_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_bcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_branches_bifurcations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35969 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_mean_flow_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_rom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_statistics_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_statistics_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_statistics_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_sv_meshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37033 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/get_sv_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/inflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/lift_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/paper_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/plot_pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/post_process_1d_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/project_1d_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/simulation_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/sv_get_path_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/vtk_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/Post/vtk_to_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.385683 svcco-0.6.30/svcco/sv_interface/ROM/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/centerlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25287 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/generate_1d_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/io_0d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/io_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/io_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/ROM/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/build_0d_run_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/build_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/build_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/export_3d_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47588 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/get_sv_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/locate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/loft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22017 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/presolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/rom.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/solid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/sv_install_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/view_0d_result_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27999 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/sv_interface/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/test_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161493 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.389683 svcco-0.6.30/svcco/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.389683 svcco-0.6.30/svcco/utils/fluid_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/fluid_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/fluid_analysis/reynolds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/fluid_analysis/wss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.389683 svcco-0.6.30/svcco/utils/gcode/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/gcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/gcode/gcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.389683 svcco-0.6.30/svcco/utils/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/gui/gui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/gui/spline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.389683 svcco-0.6.30/svcco/utils/perfusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/perfusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/perfusion/fast_geodesic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.393683 svcco-0.6.30/svcco/utils/remeshing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.393683 svcco-0.6.30/svcco/utils/remeshing/Linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/remeshing/Linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.393683 svcco-0.6.30/svcco/utils/remeshing/Mac/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/remeshing/Mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.393683 svcco-0.6.30/svcco/utils/remeshing/Windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/remeshing/Windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/remeshing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-10 20:02:03.000000 svcco-0.6.30/svcco/utils/remeshing/remesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:02:11.365683 svcco-0.6.30/svcco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-10 20:02:11.000000 svcco-0.6.30/svcco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-10 20:02:11.000000 svcco-0.6.30/svcco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:11.000000 svcco-0.6.30/svcco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:02:11.000000 svcco-0.6.30/svcco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-10 20:02:11.000000 svcco-0.6.30/svcco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 20:02:11.000000 svcco-0.6.30/svcco.egg-info/top_level.txt
```

### Comparing `svcco-0.6.29/LICENSE.txt` & `svcco-0.6.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/PKG-INFO` & `svcco-0.6.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svcco
-Version: 0.6.29
+Version: 0.6.30
 Summary: Automated Vascular Generation and CFD Simulation
 Home-page: https://zasexton.github.io/svcco/
 Author: Zachary Sexton
 Author-email: zsexton@stanford.edu
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `svcco-0.6.29/README.md` & `svcco-0.6.30/README.md`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/setup.py` & `svcco-0.6.30/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 long_description = (here / "README.md").read_text("utf8")
 
 #VERSION = re.search(
 #    r'__version__ = "(.+?)"', (here / "svcco" / "__init__.py").read_text("utf8")
 #).group(1)
 
-VERSION = '0.6.29'
+VERSION = '0.6.30'
 
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'License :: OSI Approved :: MIT License',
                'Programming Language :: Python',
                'Programming Language :: Python :: 3.7',
                'Programming Language :: Python :: 3.8',
                'Programming Language :: Python :: 3.9',
```

### Comparing `svcco-0.6.29/svcco/__init__.py` & `svcco-0.6.30/svcco/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ```bash
 pip install svcco
 ```
 '''
 #from __future__ import annotations
 
-__version__ = "0.6.29"
+__version__ = "0.6.30"
 
 import traceback
 import warnings
 from pathlib import Path
 from typing import overload
 
 #from svcco import implicit, collision, branch_addition, sv_interface, forest_utils, utils
```

### Comparing `svcco-0.6.29/svcco/branch_addition/add_bifurcation.py` & `svcco-0.6.30/svcco/branch_addition/add_bifurcation.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/add_branches.py` & `svcco-0.6.30/svcco/branch_addition/add_branches.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/add_branches_v2.py` & `svcco-0.6.30/svcco/branch_addition/add_branches_v2.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/add_branches_v3.py` & `svcco-0.6.30/svcco/branch_addition/add_branches_v3.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/add_depths.py` & `svcco-0.6.30/svcco/branch_addition/add_depths.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/add_edge.py` & `svcco-0.6.30/svcco/branch_addition/add_edge.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/add_geodesic_path.py` & `svcco-0.6.30/svcco/branch_addition/add_geodesic_path.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/basis.py` & `svcco-0.6.30/svcco/branch_addition/basis.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/calculate_radii.py` & `svcco-0.6.30/svcco/branch_addition/calculate_radii.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/check.py` & `svcco-0.6.30/svcco/branch_addition/check.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/close.py` & `svcco-0.6.30/svcco/branch_addition/close.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/finite_difference.py` & `svcco-0.6.30/svcco/branch_addition/finite_difference.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/geodesic.py` & `svcco-0.6.30/svcco/branch_addition/geodesic.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/get_point.py` & `svcco-0.6.30/svcco/branch_addition/get_point.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/local_func_v5.py` & `svcco-0.6.30/svcco/branch_addition/local_func_v5.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/local_func_v6.py` & `svcco-0.6.30/svcco/branch_addition/local_func_v6.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/local_func_v7.py` & `svcco-0.6.30/svcco/branch_addition/local_func_v7.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/sample_triad.py` & `svcco-0.6.30/svcco/branch_addition/sample_triad.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/set_root.py` & `svcco-0.6.30/svcco/branch_addition/set_root.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/triangle.py` & `svcco-0.6.30/svcco/branch_addition/triangle.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/branch_addition/update.py` & `svcco-0.6.30/svcco/branch_addition/update.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/collision/collision.py` & `svcco-0.6.30/svcco/collision/collision.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/collision/obb.py` & `svcco-0.6.30/svcco/collision/obb.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/collision/obb_unit_tests.py` & `svcco-0.6.30/svcco/collision/obb_unit_tests.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/collision/sphere_proximity.py` & `svcco-0.6.30/svcco/collision/sphere_proximity.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/collision/sphere_proximity_unit_tests.py` & `svcco-0.6.30/svcco/collision/sphere_proximity_unit_tests.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/compete_add.py` & `svcco-0.6.30/svcco/forest_utils/compete_add.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/connect.py` & `svcco-0.6.30/svcco/forest_utils/connect.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/connect_collision.py` & `svcco-0.6.30/svcco/forest_utils/connect_collision.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/optimize_connection.py` & `svcco-0.6.30/svcco/forest_utils/optimize_connection.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/optimize_connection_v2.py` & `svcco-0.6.30/svcco/forest_utils/optimize_connection_v2.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/optimize_connection_v3.py` & `svcco-0.6.30/svcco/forest_utils/optimize_connection_v3.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/optimize_connection_v4.py` & `svcco-0.6.30/svcco/forest_utils/optimize_connection_v4.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/forest_utils/optimize_connection_v5.py` & `svcco-0.6.30/svcco/forest_utils/optimize_connection_v5.py`

 * *Files 14% similar despite different names*

```diff
@@ -253,45 +253,65 @@
         filter_1_y = np.argwhere(collision_vessels[:, 1] != self.P1[1]).flatten().tolist()
         filter_1_z = np.argwhere(collision_vessels[:, 2] != self.P1[2]).flatten().tolist()
         filter_1 = []
         filter_1.extend(filter_1_x)
         filter_1.extend(filter_1_y)
         filter_1.extend(filter_1_z)
         filter_1 = np.array(list(set(filter_1)))
+        if len(filter_1) == 0:
+            self.collision_vessels = None
+            self.collision_centers = None
+            self.collision_lengths = None
+            return
         collision_vessels = collision_vessels[filter_1,:]
         filter_2_x = np.argwhere(collision_vessels[:, 0] != self.P3[0]).flatten().tolist()
         filter_2_y = np.argwhere(collision_vessels[:, 1] != self.P3[1]).flatten().tolist()
         filter_2_z = np.argwhere(collision_vessels[:, 2] != self.P3[2]).flatten().tolist()
         filter_2 = []
         filter_2.extend(filter_2_x)
         filter_2.extend(filter_2_y)
         filter_2.extend(filter_2_z)
         filter_2 = np.array(list(set(filter_2)))
+        if len(filter_2) == 0:
+            self.collision_vessels = None
+            self.collision_centers = None
+            self.collision_lengths = None
+            return
         collision_vessels = collision_vessels[filter_2,:]
         filter_3_x = np.argwhere(collision_vessels[:, 3] != self.P1[0]).flatten().tolist()
         filter_3_y = np.argwhere(collision_vessels[:, 4] != self.P1[1]).flatten().tolist()
         filter_3_z = np.argwhere(collision_vessels[:, 5] != self.P1[2]).flatten().tolist()
         filter_3 = []
         filter_3.extend(filter_3_x)
         filter_3.extend(filter_3_y)
         filter_3.extend(filter_3_z)
         filter_3 = np.array(list(set(filter_3)))
+        if len(filter_3) == 0:
+            self.collision_vessels = None
+            self.collision_centers = None
+            self.collision_lengths = None
+            return
         collision_vessels = collision_vessels[filter_3,:]
         filter_4_x = np.argwhere(collision_vessels[:, 3] != self.P3[0]).flatten().tolist()
         filter_4_y = np.argwhere(collision_vessels[:, 4] != self.P3[1]).flatten().tolist()
         filter_4_z = np.argwhere(collision_vessels[:, 5] != self.P3[2]).flatten().tolist()
         filter_4 = []
         filter_4.extend(filter_4_x)
         filter_4.extend(filter_4_y)
         filter_4.extend(filter_4_z)
         filter_4 = np.array(list(set(filter_4)))
-        collision_vessels = collision_vessels[filter_4,:]
-        self.collision_vessels = collision_vessels
-        self.collision_centers = (collision_vessels[:,0:3]+collision_vessels[:,3:6])/2
-        self.collision_lengths = np.linalg.norm(collision_vessels[:,3:6]-collision_vessels[:,0:3],axis=1)
+        if len(filter_4) == 0:
+            self.collision_vessels = None
+            self.collision_centers = None
+            self.collision_lengths = None
+        else:
+            collision_vessels = collision_vessels[filter_4,:]
+            self.collision_vessels = collision_vessels
+            self.collision_centers = (collision_vessels[:,0:3]+collision_vessels[:,3:6])/2
+            self.collision_lengths = np.linalg.norm(collision_vessels[:,3:6]-collision_vessels[:,0:3],axis=1)
         return
     def solve(self,*args,clamp_first=True,clamp_second=True,sample_size=20,radius_buffer=0.01):
         start = perf_counter()
         if len(args) == 0:
             number_free_points = 2
         else:
             number_free_points = args[0]
@@ -530,20 +550,27 @@
             tmp_connection.clamp_first = clamp_first
             tmp_connection.clamp_second = clamp_second
             tmp_connection.seperate = seperate
             tmp_connection.set_solver()
             for j in range(len(connection_solutions)):
                 if connection_solutions[j].seperate:
                     collision_vessels = tmp_connection.conn.collision_vessels
-                    collision_vessels = np.vstack((collision_vessels,connection_solutions[j].vessels_1,
-                                                   connection_solutions[j].vessels_2))
+                    if collision_vessels is None or collision_vessels.shape[0] == 0:
+                        collision_vessels = np.vstack((connection_solutions[j].vessels_1,
+                                                       connection_solutions[j].vessels_2))
+                    else:
+                        collision_vessels = np.vstack((collision_vessels,connection_solutions[j].vessels_1,
+                                                       connection_solutions[j].vessels_2))
                     tmp_connection.conn.set_collision_vessels(collision_vessels)
                 else:
                     collision_vessels = tmp_connection.conn.collision_vessels
-                    collision_vessels = np.vstack((collision_vessels,connection_solutions[j].vessels_1))
+                    if collision_vessels is None or collision_vessels.shape[0] == 0:
+                        collision_vessels = connection_solutions[j].vessels_1
+                    else:
+                        collision_vessels = np.vstack((collision_vessels,connection_solutions[j].vessels_1))
                     tmp_connection.conn.set_collision_vessels(collision_vessels)
             if self.extra_collision_vessels is not None:
                 collision_vessels = tmp_connection.conn.collision_vessels
                 collision_vessels = np.vstack((collision_vessels,self.extra_collision_vessels))
                 tmp_connection.conn.set_collision_vessels(collision_vessels)
             tmp_connection.solve(num_ctrl_points)
             if tmp_connection.res.fun > 0:
```

### Comparing `svcco-0.6.29/svcco/forest_utils/smooth.py` & `svcco-0.6.30/svcco/forest_utils/smooth.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/core/a_matrix.py` & `svcco-0.6.30/svcco/implicit/core/a_matrix.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/core/m_matrix.py` & `svcco-0.6.30/svcco/implicit/core/m_matrix.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/derivative.py` & `svcco-0.6.30/svcco/implicit/derivative.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/implicit.py` & `svcco-0.6.30/svcco/implicit/implicit.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/kernel/kernel.py` & `svcco-0.6.30/svcco/implicit/kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/kernel/kernel_functions/grad.py` & `svcco-0.6.30/svcco/implicit/kernel/kernel_functions/grad.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/kernel/kernel_functions/hess.py` & `svcco-0.6.30/svcco/implicit/kernel/kernel_functions/hess.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/load.py` & `svcco-0.6.30/svcco/implicit/load.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/sampling.py` & `svcco-0.6.30/svcco/implicit/sampling.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/solver/solver.py` & `svcco-0.6.30/svcco/implicit/solver/solver.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/solver/solver_functions/init_normals_given.py` & `svcco-0.6.30/svcco/implicit/solver/solver_functions/init_normals_given.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/solver/solver_functions/init_normals_not_given.py` & `svcco-0.6.30/svcco/implicit/solver/solver_functions/init_normals_not_given.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/tests/bumpy_sphere.py` & `svcco-0.6.30/svcco/implicit/tests/bumpy_sphere.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/visualize/visualize.py` & `svcco-0.6.30/svcco/implicit/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/implicit/weingarten_map.py` & `svcco-0.6.30/svcco/implicit/weingarten_map.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/1D_to_3D_projection.py` & `svcco-0.6.30/svcco/sv_interface/Post/1D_to_3D_projection.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/asymptotic_pressure.py` & `svcco-0.6.30/svcco/sv_interface/Post/asymptotic_pressure.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/bc_0d.py` & `svcco-0.6.30/svcco/sv_interface/Post/bc_0d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/check_bc.py` & `svcco-0.6.30/svcco/sv_interface/Post/check_bc.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/common.py` & `svcco-0.6.30/svcco/sv_interface/Post/common.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/compare_1d.py` & `svcco-0.6.30/svcco/sv_interface/Post/compare_1d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/compare_3d.py` & `svcco-0.6.30/svcco/sv_interface/Post/compare_3d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/compare_centerline_path.py` & `svcco-0.6.30/svcco/sv_interface/Post/compare_centerline_path.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/cover.py` & `svcco-0.6.30/svcco/sv_interface/Post/cover.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/create_db_from_local.py` & `svcco-0.6.30/svcco/sv_interface/Post/create_db_from_local.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_faceid.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_faceid.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_scale.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_scale.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_surf_discr.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_surf_discr.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_surf_displacement.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_surf_displacement.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_surf_id.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_surf_id.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_surf_mesh.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_surf_mesh.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_surf_orientation.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_surf_orientation.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/fix_time.py` & `svcco-0.6.30/svcco/sv_interface/Post/fix_time.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_3d.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_3d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_bc_integrals.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_bc_integrals.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_bcs.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_bcs.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_branches_bifurcations.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_branches_bifurcations.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_centerline.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_centerline.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_database.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_database.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_inventory.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_inventory.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_mean_flow_3d.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_mean_flow_3d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_rom.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_rom.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_statistics_1d.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_statistics_1d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_statistics_3d.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_statistics_3d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_statistics_bc.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_statistics_bc.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_sv_meshes.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_sv_meshes.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/get_sv_project.py` & `svcco-0.6.30/svcco/sv_interface/Post/get_sv_project.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/inflow.py` & `svcco-0.6.30/svcco/sv_interface/Post/inflow.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/lift_laplace.py` & `svcco-0.6.30/svcco/sv_interface/Post/lift_laplace.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/paper_plots.py` & `svcco-0.6.30/svcco/sv_interface/Post/paper_plots.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/plot_pod.py` & `svcco-0.6.30/svcco/sv_interface/Post/plot_pod.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/post_process_1d_simulation.py` & `svcco-0.6.30/svcco/sv_interface/Post/post_process_1d_simulation.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/postproc.py` & `svcco-0.6.30/svcco/sv_interface/Post/postproc.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/project_1d_3d.py` & `svcco-0.6.30/svcco/sv_interface/Post/project_1d_3d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/simulation_io.py` & `svcco-0.6.30/svcco/sv_interface/Post/simulation_io.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/sv_get_path_segmentation.py` & `svcco-0.6.30/svcco/sv_interface/Post/sv_get_path_segmentation.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/vtk_functions.py` & `svcco-0.6.30/svcco/sv_interface/Post/vtk_functions.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/Post/vtk_to_xdmf.py` & `svcco-0.6.30/svcco/sv_interface/Post/vtk_to_xdmf.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/centerlines.py` & `svcco-0.6.30/svcco/sv_interface/ROM/centerlines.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/generate_1d_mesh.py` & `svcco-0.6.30/svcco/sv_interface/ROM/generate_1d_mesh.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/io_0d.py` & `svcco-0.6.30/svcco/sv_interface/ROM/io_0d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/io_1d.py` & `svcco-0.6.30/svcco/sv_interface/ROM/io_1d.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/io_headers.py` & `svcco-0.6.30/svcco/sv_interface/ROM/io_headers.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/manage.py` & `svcco-0.6.30/svcco/sv_interface/ROM/manage.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/mesh.py` & `svcco-0.6.30/svcco/sv_interface/ROM/mesh.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/models.py` & `svcco-0.6.30/svcco/sv_interface/ROM/models.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/parameters.py` & `svcco-0.6.30/svcco/sv_interface/ROM/parameters.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/ROM/utils.py` & `svcco-0.6.30/svcco/sv_interface/ROM/utils.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/build_files.py` & `svcco-0.6.30/svcco/sv_interface/build_files.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/build_results.py` & `svcco-0.6.30/svcco/sv_interface/build_results.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/centerline.py` & `svcco-0.6.30/svcco/sv_interface/centerline.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/export_3d_only.py` & `svcco-0.6.30/svcco/sv_interface/export_3d_only.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/flow.py` & `svcco-0.6.30/svcco/sv_interface/flow.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/get_sv_data.py` & `svcco-0.6.30/svcco/sv_interface/get_sv_data.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/locate.py` & `svcco-0.6.30/svcco/sv_interface/locate.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/loft.py` & `svcco-0.6.30/svcco/sv_interface/loft.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/mesh.py` & `svcco-0.6.30/svcco/sv_interface/mesh.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/options.py` & `svcco-0.6.30/svcco/sv_interface/options.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/presolver.py` & `svcco-0.6.30/svcco/sv_interface/presolver.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/rom.py` & `svcco-0.6.30/svcco/sv_interface/rom.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/solid.py` & `svcco-0.6.30/svcco/sv_interface/solid.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/solver.py` & `svcco-0.6.30/svcco/sv_interface/solver.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/sv_install_function.py` & `svcco-0.6.30/svcco/sv_interface/sv_install_function.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/view_0d_result_plots.py` & `svcco-0.6.30/svcco/sv_interface/view_0d_result_plots.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/sv_interface/waveform.py` & `svcco-0.6.30/svcco/sv_interface/waveform.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/test_rotation.py` & `svcco-0.6.30/svcco/test_rotation.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/tree.py` & `svcco-0.6.30/svcco/tree.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/utils/fluid_analysis/wss.py` & `svcco-0.6.30/svcco/utils/fluid_analysis/wss.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/utils/gcode/gcode.py` & `svcco-0.6.30/svcco/utils/gcode/gcode.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/utils/gui/gui_helper.py` & `svcco-0.6.30/svcco/utils/gui/gui_helper.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/utils/gui/spline_helper.py` & `svcco-0.6.30/svcco/utils/gui/spline_helper.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/utils/perfusion/fast_geodesic.py` & `svcco-0.6.30/svcco/utils/perfusion/fast_geodesic.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco/utils/remeshing/remesh.py` & `svcco-0.6.30/svcco/utils/remeshing/remesh.py`

 * *Files identical despite different names*

### Comparing `svcco-0.6.29/svcco.egg-info/PKG-INFO` & `svcco-0.6.30/svcco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svcco
-Version: 0.6.29
+Version: 0.6.30
 Summary: Automated Vascular Generation and CFD Simulation
 Home-page: https://zasexton.github.io/svcco/
 Author: Zachary Sexton
 Author-email: zsexton@stanford.edu
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `svcco-0.6.29/svcco.egg-info/SOURCES.txt` & `svcco-0.6.30/svcco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

