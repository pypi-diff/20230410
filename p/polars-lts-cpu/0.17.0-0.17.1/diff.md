# Comparing `tmp/polars_lts_cpu-0.17.0.tar.gz` & `tmp/polars_lts_cpu-0.17.1.tar.gz`

## Comparing `polars_lts_cpu-0.17.0.tar` & `polars_lts_cpu-0.17.1.tar`

### file list

```diff
@@ -1,1072 +1,1076 @@
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123     8985 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13678 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123     4012 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123     8059 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/cli.rs
--rw-r--r--   0     1001      123    13201 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    15996 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123    27124 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123      342 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/main.rs
--rw-r--r--   0     1001      123    13197 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     3386 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0        0        0    10379 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3271 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8778 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20401 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       32 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17826 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      189 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123     6258 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    10844 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30146 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7044 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      988 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      702 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10815 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1064 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10121 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1655 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5381 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4476 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6441 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123      552 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123     2645 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123      514 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/hash.rs
--rw-r--r--   0     1001      123     2709 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      583 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      353 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     1792 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1114 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0     5945 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123     1796 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4359 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     4505 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     4674 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2831 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9288 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    47120 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     3440 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123      764 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1284 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3908 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     3577 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13592 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4335 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     6058 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     7074 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2986 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4184 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1211 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     1922 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     3702 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1284 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    22402 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    17171 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    18847 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     3153 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     2003 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5804 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     3670 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    20940 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     3929 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    11541 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14345 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31804 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2044 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      419 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    27332 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    18867 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9563 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123    20901 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
--rw-r--r--   0     1001      123      219 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     3333 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14987 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7031 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12749 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4207 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4293 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    14819 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6799 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3158 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47889 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     8358 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2953 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1033 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123     7265 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123    19606 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      123     8679 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1179 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     1556 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    19936 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8845 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1382 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2263 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    13129 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    48300 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123     9463 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     5150 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    38411 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1395 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2986 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7001 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     2802 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19456 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10220 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6453 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     3567 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2549 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    13166 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23438 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4826 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2517 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32120 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123     9946 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2875 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123     9391 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2365 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    27269 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6295 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123     6264 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    24977 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8339 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     5308 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     4436 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    16465 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123    22261 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     2585 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     1539 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10234 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     6151 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5467 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7430 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    30762 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    20472 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     6630 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123     1859 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5041 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6064 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123    11229 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     7755 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1959 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2489 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    12191 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      533 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     1592 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    29283 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7689 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2701 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42068 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    11442 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5532 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     7644 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      433 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    37711 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     7874 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    33715 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6561 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5179 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16609 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    16518 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     7643 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    47350 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123      218 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    12291 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14048 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39434 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10535 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    17027 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123    18264 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22392 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    16303 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     2953 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6076 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4247 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    11583 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123   124249 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    19811 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     3732 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5950 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     8778 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2149 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10935 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      453 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2707 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17653 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1903 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15766 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2411 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123     8247 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     6551 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    17338 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28511 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    13187 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    24117 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     9318 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10951 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    13039 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18120 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15344 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     5718 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    14668 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14348 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6308 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18430 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5191 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7851 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11097 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9836 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4062 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6297 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    36305 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      673 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5204 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1355 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4247 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5072 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18378 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2840 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     8117 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123    32703 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1181 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13773 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123       98 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      229 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      548 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3247 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     2324 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6501 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    10473 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4555 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123    24282 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs
--rw-r--r--   0     1001      123     2150 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4666 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     3906 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20859 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23521 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     7893 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5485 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2002 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      567 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     3808 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     6295 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3801 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      600 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5076 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      376 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     3387 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      430 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    19550 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    13982 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1237 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      234 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1679 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2452 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    21989 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     5269 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      489 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9380 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8251 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123     2486 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18025 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13483 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      217 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     7231 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3680 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     3413 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     2779 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123      952 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123     2383 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3604 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    27794 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1898 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19430 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    21349 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10817 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13909 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    31233 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    24032 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    12866 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7580 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9245 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8282 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123     9974 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      123     4892 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7155 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ndjson_core/buffer.rs
--rw-r--r--   0     1001      123       39 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ndjson_core/mod.rs
--rw-r--r--   0     1001      123    12177 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
--rw-r--r--   0     1001      123      273 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7354 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4790 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9629 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10106 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      633 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4467 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123     3565 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    10476 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     7368 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     4125 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    11297 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    19622 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     3783 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123     9585 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     2958 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    31306 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      535 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123      320 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1568 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     4028 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12448 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1630 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7059 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2567 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2491 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    23642 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    20089 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    24202 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11624 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123     1975 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     3160 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     2986 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     7757 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123     1125 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     1807 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      232 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123       56 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123    24907 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123     1042 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      915 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4740 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1015 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1895 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9731 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3703 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2022 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    18684 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3924 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11659 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5504 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     8683 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1749 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14367 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123     9070 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11609 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4698 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8335 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     4292 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/take_agg.rs
--rw-r--r--   0     1001      123     3898 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      434 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      762 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2716 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2533 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5020 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123    17253 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     6950 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123      935 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      969 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123     9323 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123    13163 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123      753 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123     1431 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1366 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123      344 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123    13120 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123     1668 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     1364 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123      190 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/is_in.rs
--rw-r--r--   0     1001      123     8119 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123    16613 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123     2051 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      200 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    12568 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    18206 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     2627 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123    38368 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/functions.rs
--rw-r--r--   0     1001      123    10197 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     2181 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    70400 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2094 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123    14993 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      156 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     6819 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11189 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25701 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    25056 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29650 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15193 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    12019 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123     9746 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10463 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     7271 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15287 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     3260 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3210 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14494 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6715 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    27950 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15130 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15747 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26507 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     2692 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27236 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13850 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     3161 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    19767 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10197 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    15273 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     4535 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13048 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      809 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11955 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123     6297 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/LICENSE
--rw-r--r--   0     1001      123     2425 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/Makefile
--rw-r--r--   0     1001      123    10846 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/README.md
--rw-r--r--   0     1001      123      651 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/build.rs
--rw-r--r--   0     1001      123       32 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      450 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1567 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7304 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1339 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1513 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      663 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      388 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      309 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1023 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1072 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      461 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      695 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      374 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      125 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      860 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123      968 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      692 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      392 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1269 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      252 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123      988 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123      339 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      256 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1086 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      722 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      428 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      749 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123      922 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      396 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1118 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      302 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123      647 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     5941 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/__init__.py
--rw-r--r--   0     1001      123    13331 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/api.py
--rw-r--r--   0     1001      123    24553 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/config.py
--rw-r--r--   0     1001      123    25409 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5057 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   301438 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    33240 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2524 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    11189 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1356 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4430 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    14468 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7049 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/dependencies.py
--rw-r--r--   0     1001      123     2954 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/__init__.py
--rw-r--r--   0     1001      123     2730 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/binary.py
--rw-r--r--   0     1001      123     1708 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/categorical.py
--rw-r--r--   0     1001      123    65759 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/datetime.py
--rw-r--r--   0     1001      123   249803 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/expr.py
--rw-r--r--   0     1001      123    22899 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/list.py
--rw-r--r--   0     1001      123     2059 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/meta.py
--rw-r--r--   0     1001      123    44150 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/string.py
--rw-r--r--   0     1001      123     5436 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/expr/struct.py
--rw-r--r--   0     1001      123     1941 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/functions/__init__.py
--rw-r--r--   0     1001      123    29135 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/functions/eager.py
--rw-r--r--   0     1001      123    88753 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/functions/lazy.py
--rw-r--r--   0     1001      123     6293 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      280 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/internals.py
--rw-r--r--   0     1001      123      978 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/_utils.py
--rw-r--r--   0     1001      123      878 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1082 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4691 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35581 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     8590 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/database.py
--rw-r--r--   0     1001      123    10988 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18459 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     5309 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1193 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5840 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      519 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/json.py
--rw-r--r--   0     1001      123     2257 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1215 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7212 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2331 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3546 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   165907 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24010 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/py.typed
--rw-r--r--   0     1001      123       69 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/__init__.py
--rw-r--r--   0     1001      123     1579 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/_numpy.py
--rw-r--r--   0     1001      123     1920 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/binary.py
--rw-r--r--   0     1001      123     1699 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/categorical.py
--rw-r--r--   0     1001      123    43693 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/datetime.py
--rw-r--r--   0     1001      123    12385 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/list.py
--rw-r--r--   0     1001      123   160434 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/series.py
--rw-r--r--   0     1001      123    26584 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/string.py
--rw-r--r--   0     1001      123     2287 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/struct.py
--rw-r--r--   0     1001      123     5375 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/series/utils.py
--rw-r--r--   0     1001      123     7638 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/sql/__init__.py
--rw-r--r--   0     1001      123     1351 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/sql/context.py
--rw-r--r--   0     1001      123     4698 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/testing/__init__.py
--rw-r--r--   0     1001      123    23938 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/testing/_parametric.py
--rw-r--r--   0     1001      123      929 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/testing/_private.py
--rw-r--r--   0     1001      123    13264 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/testing/asserts.py
--rw-r--r--   0     1001      123      551 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/testing/parametric.py
--rw-r--r--   0     1001      123     5681 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/type_aliases.py
--rw-r--r--   0     1001      123     1035 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/__init__.py
--rw-r--r--   0     1001      123    47849 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/_construction.py
--rw-r--r--   0     1001      123     2782 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      721 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/_scan.py
--rw-r--r--   0     1001      123      687 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8948 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/convert.py
--rw-r--r--   0     1001      123     5889 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1594 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2118 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    10839 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/polars/utils/various.py
--rw-r--r--   0     1001      123     5279 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/pyproject.toml
--rw-r--r--   0     1001      123      690 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/requirements-lint.txt
--rw-r--r--   0     1001      123     2500 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/scripts/check_decorators_stacklevels.py
--rw-r--r--   0     1001      123    10959 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     8388 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/apply/mod.rs
--rw-r--r--   0     1001      123    71436 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3906 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5214 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/batched_csv.rs
--rw-r--r--   0     1001      123    47903 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/conversion.rs
--rw-r--r--   0     1001      123    45496 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/dataframe.rs
--rw-r--r--   0     1001      123     3799 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/error.rs
--rw-r--r--   0     1001      123     9482 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/file.rs
--rw-r--r--   0     1001      123     7468 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/lazy/apply.rs
--rw-r--r--   0     1001      123    32612 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/lazy/dataframe.rs
--rw-r--r--   0     1001      123    62172 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/lazy/dsl.rs
--rw-r--r--   0     1001      123     1082 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/lazy/meta.rs
--rw-r--r--   0     1001      123      727 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/lazy/mod.rs
--rw-r--r--   0     1001      123      212 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/lazy/utils.rs
--rw-r--r--   0     1001      123    20790 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/lib.rs
--rw-r--r--   0     1001      123     4050 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/list_construction.rs
--rw-r--r--   0     1001      123     7902 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/npy.rs
--rw-r--r--   0     1001      123     1022 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/object.rs
--rw-r--r--   0     1001      123      122 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/py_modules.rs
--rw-r--r--   0     1001      123    54555 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/series.rs
--rw-r--r--   0     1001      123     3478 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/set.rs
--rw-r--r--   0     1001      123      889 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7945 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     4978 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4478 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123     3707 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     5709 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     7584 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/__init__.py
--rw-r--r--   0     1001      123     2695 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      351 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    11514 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     2552 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123    14169 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2486 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    27073 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    88066 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      218 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1907 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    38071 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     7127 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     3456 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11067 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5849 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3361 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     6828 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2851 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    12087 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13684 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3319 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123     3218 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    13569 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    12741 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1748 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23100 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    13247 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     4637 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123     9412 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     3952 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123      956 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     2906 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     7840 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3881 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    22696 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123    16263 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    10467 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      513 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    18639 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123    19137 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     3517 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     3327 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      551 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123     9325 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     4775 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19916 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    32466 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     3497 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   118730 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_df.py
--rw-r--r--   0     1001      123     1009 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    15408 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2387 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    31861 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3305 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123    10759 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_functions.py
--rw-r--r--   0     1001      123     3763 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    32596 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    48110 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2369 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4008 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     6995 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11550 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     3960 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    10825 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     2226 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83249 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_series.py
--rw-r--r--   0     1001      123     2561 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    13877 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_streaming.py
--rw-r--r--   0     1001      123    10344 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123      247 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     4307 2023-04-07 15:49:12.000000 polars_lts_cpu-0.17.0/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    63097 2023-04-07 15:50:05.000000 polars_lts_cpu-0.17.0/Cargo.lock
--rw-r--r--   0        0        0    13384 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123     3565 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    10476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     7368 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     4125 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    15873 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    20048 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     5808 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123     9585 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     2960 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    31306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      535 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123      320 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1568 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     4028 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12448 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1630 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7059 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2008 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    23538 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    20089 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    24202 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11624 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      234 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1679 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2452 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    21989 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     5269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      489 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9380 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8251 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123     2486 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18025 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13483 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      217 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     7231 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3680 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     3413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     2779 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123      952 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123     6297 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123     8985 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13678 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123     4012 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/README.md
+-rw-r--r--   0     1001      123     9096 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/assets/SQL.sublime-syntax
+-rw-r--r--   0     1001      123    21158 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/assets/theme
+-rw-r--r--   0     1001      123     1450 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/highlighter.rs
+-rw-r--r--   0     1001      123     5052 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/mod.rs
+-rw-r--r--   0     1001      123     1043 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/cli/prompt.rs
+-rw-r--r--   0     1001      123    13598 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    16415 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123    26866 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123      342 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/main.rs
+-rw-r--r--   0     1001      123    13264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     3386 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0        0        0     5945 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123     1796 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4359 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     4505 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     4674 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2831 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9288 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    47120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     3440 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123      764 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1284 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3908 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     3577 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13592 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4335 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     6058 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     7074 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2986 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4184 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1211 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     1922 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     3702 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1284 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    22402 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    17171 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    18847 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     3153 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     2003 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5804 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     3670 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    20940 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     3929 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    11541 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14345 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31804 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2044 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      419 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    27332 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    18867 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9563 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123    20901 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
+-rw-r--r--   0     1001      123      219 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     3333 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14987 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7031 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12749 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4207 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4293 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    14819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3158 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47889 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     8358 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2953 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1033 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123     2383 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3604 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28016 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1898 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    21349 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10817 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13909 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    31233 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    25209 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    12866 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7580 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9245 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8282 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123     9974 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      123     4892 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7215 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/buffer.rs
+-rw-r--r--   0     1001      123       39 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/mod.rs
+-rw-r--r--   0     1001      123    12177 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
+-rw-r--r--   0     1001      123      273 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7354 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4790 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9629 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10106 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      633 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123     7265 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123     2645 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123      514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/hash.rs
+-rw-r--r--   0     1001      123     2709 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      583 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      353 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     1792 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1114 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0    10379 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3271 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8778 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20419 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       32 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17826 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123     6258 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    10844 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30146 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7044 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      988 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      702 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10815 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1064 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10121 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1655 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5381 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6441 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123      552 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123    19606 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      123     8679 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1179 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     1556 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    19936 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8845 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1382 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2263 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    13129 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    48300 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123     9463 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     5150 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    38411 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1395 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2986 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7001 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     2802 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19456 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10220 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6453 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     3567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2549 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    13166 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23438 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4826 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2517 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123     9946 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2875 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123     9391 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2365 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    27269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6295 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123     6264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    24977 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     5308 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     4436 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    16465 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123    22261 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     2585 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     1539 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10234 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     6151 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    30762 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    20472 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     6630 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123     1859 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5041 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6064 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123    11229 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     7755 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1959 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2489 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    11559 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     1592 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    29283 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7689 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2701 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42068 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    11442 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5532 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     7644 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      433 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    37711 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     7874 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    33715 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6561 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5179 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16609 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    16518 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     7643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    47350 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123      218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    12291 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14048 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39434 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10535 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    17027 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123    18264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22392 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    16303 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     2953 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6076 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    11583 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123   124249 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    19811 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     3732 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5950 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     8778 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2149 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10935 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      453 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2707 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17653 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1903 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15766 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2411 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123     8247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     6551 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    17338 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28511 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    13187 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    24117 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     9318 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10951 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    13039 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15344 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     5718 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    14668 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14348 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6308 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5191 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     7851 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11097 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9836 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4062 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6297 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    36305 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      673 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5204 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1355 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5072 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18378 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2840 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     8117 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123    32703 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1181 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13773 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123     1975 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     3160 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     2986 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     7757 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123     1125 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     1807 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      232 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123       56 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123    24907 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123     1042 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      915 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4740 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1015 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1895 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9731 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3703 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2022 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    18684 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3924 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11659 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5504 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     8683 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1749 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14367 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123     9070 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11609 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4698 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8335 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     4292 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/take_agg.rs
+-rw-r--r--   0     1001      123     3897 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      434 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      762 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2716 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5020 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123       98 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      229 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      548 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     2324 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6501 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    10473 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4555 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123    24282 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs
+-rw-r--r--   0     1001      123     2150 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4666 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     3906 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20859 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23521 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     7893 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5485 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2002 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     3808 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     6295 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3801 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      600 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5076 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      376 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     3387 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    19550 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    13982 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1237 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123    17253 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     6950 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123      935 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      969 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123     9323 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123    13163 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123      753 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123     1431 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1366 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123      344 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123    13120 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123     1668 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     1364 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123      190 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/is_in.rs
+-rw-r--r--   0     1001      123     8119 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123    16613 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123     2051 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      200 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    12568 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    18280 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     2627 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123    38368 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/functions.rs
+-rw-r--r--   0     1001      123    10197 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2181 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    70400 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2094 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123    14993 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      156 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     6819 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11390 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25701 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    25056 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29650 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15193 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    12019 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123     9746 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10463 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8148 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15287 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     3260 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3210 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14494 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6715 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    27950 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15130 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15747 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26507 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2692 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27236 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13850 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     3161 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    19767 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10197 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    15273 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     4535 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13048 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      809 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11955 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/Makefile
+-rw-r--r--   0     1001      123    10846 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/README.md
+-rw-r--r--   0     1001      123      651 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/build.rs
+-rw-r--r--   0     1001      123       32 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      450 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1567 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7304 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     1339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1513 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      663 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      388 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      309 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1023 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1072 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      461 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      695 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      374 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      125 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      860 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123      968 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      692 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      392 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1269 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      252 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123      988 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123      339 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      256 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1086 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      722 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      428 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      749 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123      922 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      396 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1118 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      302 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123      647 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     5941 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/__init__.py
+-rw-r--r--   0     1001      123    13396 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/api.py
+-rw-r--r--   0     1001      123    24553 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/config.py
+-rw-r--r--   0     1001      123    25409 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5057 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   301533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    33240 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2524 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    11189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1356 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4430 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    14468 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7049 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/dependencies.py
+-rw-r--r--   0     1001      123     2954 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     2730 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1708 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    65759 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   249864 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/expr.py
+-rw-r--r--   0     1001      123    22899 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/list.py
+-rw-r--r--   0     1001      123     2059 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/meta.py
+-rw-r--r--   0     1001      123    44215 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/string.py
+-rw-r--r--   0     1001      123     5436 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/expr/struct.py
+-rw-r--r--   0     1001      123     1941 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    29688 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/eager.py
+-rw-r--r--   0     1001      123    88870 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/lazy.py
+-rw-r--r--   0     1001      123     6293 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      280 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/internals.py
+-rw-r--r--   0     1001      123      978 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/_utils.py
+-rw-r--r--   0     1001      123      878 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1082 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4691 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35533 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     8655 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/database.py
+-rw-r--r--   0     1001      123    10988 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18459 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     5309 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1271 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5840 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      519 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/json.py
+-rw-r--r--   0     1001      123     2257 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7212 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2331 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3611 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   165937 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24010 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/py.typed
+-rw-r--r--   0     1001      123       69 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1579 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     1920 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/binary.py
+-rw-r--r--   0     1001      123     1699 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/categorical.py
+-rw-r--r--   0     1001      123    43693 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/datetime.py
+-rw-r--r--   0     1001      123    12385 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/list.py
+-rw-r--r--   0     1001      123   160561 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/series.py
+-rw-r--r--   0     1001      123    26584 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/string.py
+-rw-r--r--   0     1001      123     2287 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/struct.py
+-rw-r--r--   0     1001      123     5375 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/series/utils.py
+-rw-r--r--   0     1001      123     7638 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/sql/__init__.py
+-rw-r--r--   0     1001      123     1351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/sql/context.py
+-rw-r--r--   0     1001      123     4764 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/__init__.py
+-rw-r--r--   0     1001      123    23938 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/_parametric.py
+-rw-r--r--   0     1001      123      929 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/_private.py
+-rw-r--r--   0     1001      123    13264 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      551 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/testing/parametric.py
+-rw-r--r--   0     1001      123     5681 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1035 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    47827 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     2782 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      721 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      687 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8948 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/convert.py
+-rw-r--r--   0     1001      123     5789 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2226 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    11592 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/polars/utils/various.py
+-rw-r--r--   0     1001      123     5299 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/pyproject.toml
+-rw-r--r--   0     1001      123      690 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/requirements-lint.txt
+-rw-r--r--   0     1001      123     1610 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    10959 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     8388 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/apply/mod.rs
+-rw-r--r--   0     1001      123    71436 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3906 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5214 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/batched_csv.rs
+-rw-r--r--   0     1001      123    47903 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/conversion.rs
+-rw-r--r--   0     1001      123    45496 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/dataframe.rs
+-rw-r--r--   0     1001      123     3799 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/error.rs
+-rw-r--r--   0     1001      123     9482 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/file.rs
+-rw-r--r--   0     1001      123     7468 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/apply.rs
+-rw-r--r--   0     1001      123    32612 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      123    62204 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/dsl.rs
+-rw-r--r--   0     1001      123     1082 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/meta.rs
+-rw-r--r--   0     1001      123      727 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/mod.rs
+-rw-r--r--   0     1001      123      212 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lazy/utils.rs
+-rw-r--r--   0     1001      123    20790 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/lib.rs
+-rw-r--r--   0     1001      123     4050 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/list_construction.rs
+-rw-r--r--   0     1001      123     7902 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/npy.rs
+-rw-r--r--   0     1001      123     1022 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/py_modules.rs
+-rw-r--r--   0     1001      123    54555 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/series.rs
+-rw-r--r--   0     1001      123     3478 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/set.rs
+-rw-r--r--   0     1001      123      843 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7945 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     5018 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123     3707 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     5709 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     7584 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3394 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    11514 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     2552 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123    14169 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2486 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    27073 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    89703 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1907 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    38972 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     7127 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     3456 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11067 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5916 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3361 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     6828 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2851 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11918 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13357 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3229 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123     3218 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    13569 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    12741 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1748 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23698 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    15640 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     4637 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123     9412 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     3952 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123      956 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     2906 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     7840 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3881 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    22696 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123    16263 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    10467 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    18639 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123    19137 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     3643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     3631 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123     9805 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     4775 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    19916 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    32466 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     3497 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   118730 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     1009 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    15408 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2387 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    32643 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3305 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123    10759 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_functions.py
+-rw-r--r--   0     1001      123     3763 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    32596 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    48110 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2369 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4008 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     6995 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11550 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     3960 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    10976 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     2226 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    83327 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_series.py
+-rw-r--r--   0     1001      123     2561 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    13877 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_streaming.py
+-rw-r--r--   0     1001      123    10344 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123      247 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     4307 2023-04-10 19:13:00.000000 polars_lts_cpu-0.17.1/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    63097 2023-04-10 19:13:55.000000 polars_lts_cpu-0.17.1/Cargo.lock
+-rw-r--r--   0        0        0    13384 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.1/PKG-INFO
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/pola-rs/polars"
 description = "Lazy query engine for the Polars DataFrame library"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
-cli = ["csv", "polars-lazy/fmt", "atty", "rustyline", "jemallocator"]
+cli = ["csv", "polars-lazy/fmt", "atty", "reedline", "jemallocator"]
+highlight = ["syntect", "nu-ansi-term"]
 csv = ["polars-lazy/csv-file"]
 default = []
 ipc = ["polars-lazy/ipc"]
 parquet = ["polars-lazy/parquet"]
 
 [dependencies]
 atty = { version = "0.2", optional = true }
+nu-ansi-term = { version = "0.47.0", optional = true }
 polars-arrow = { version = "0.28.0", path = "../polars-arrow", features = ["like"] }
 polars-core = { version = "0.28.0", path = "../polars-core", features = [] }
 polars-lazy = { version = "0.28.0", path = "../polars-lazy", features = ["compile", "strings", "cross_join", "trigonometry", "abs", "round_series", "log", "regex", "is_in", "meta"] }
 polars-plan = { version = "0.28.0", path = "../polars-plan", features = ["compile"] }
-rustyline = { version = "11.0.0", optional = true }
+reedline = { version = "0.18.0", optional = true }
 serde = "1"
 serde_json = { version = "1" }
 sqlparser = { version = "0.30" }
+syntect = { version = "5.0.0", features = ["dump-load"], optional = true }
 
 [target.'cfg(target_os = "linux")'.dependencies]
 jemallocator = { version = "0.5", features = ["disable_initial_exec_tls"], optional = true }
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/README.md` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/context.rs`

 * *Files 7% similar despite different names*

```diff
@@ -14,58 +14,57 @@
 use sqlparser::parser::Parser;
 
 use crate::sql_expr::{parse_sql_expr, process_join_constraint};
 use crate::table_functions::PolarsTableFunctions;
 
 thread_local! {pub(crate) static TABLES: RefCell<Vec<String>> = RefCell::new(vec![])}
 
+/// The SQLContext is the main entry point for executing SQL queries.
 #[derive(Default, Clone)]
 pub struct SQLContext {
-    pub table_map: PlHashMap<String, LazyFrame>,
+    pub(crate) table_map: PlHashMap<String, LazyFrame>,
+    pub(crate) tables: Vec<String>,
 }
 
 impl SQLContext {
-    pub fn try_new() -> PolarsResult<Self> {
-        TABLES.with(|cell| {
-            polars_ensure!(
-                cell.borrow().is_empty(),
-                ComputeError: "only one sql-context per thread allowed",
-            );
-            Ok(())
-        })?;
-        Ok(Self {
+    /// Create a new SQLContext
+    pub fn new() -> Self {
+        Self {
             table_map: PlHashMap::new(),
-        })
+            tables: vec![],
+        }
     }
-
+    /// Register a DataFrame as a table in the SQLContext.
     pub fn register(&mut self, name: &str, lf: LazyFrame) {
-        TABLES.with(|cell| cell.borrow_mut().push(name.to_owned()));
+        self.tables.push(name.to_owned());
         self.table_map.insert(name.to_owned(), lf);
     }
 }
 
 impl SQLContext {
+    /// Execute a sql query and return the result as a LazyFrame.
     pub fn execute(&mut self, query: &str) -> PolarsResult<LazyFrame> {
         let ast = Parser::parse_sql(&GenericDialect::default(), query).map_err(to_compute_err)?;
         polars_ensure!(ast.len() == 1, ComputeError: "One and only one statement at a time please");
         self.execute_statement(ast.get(0).unwrap())
     }
 
-    pub fn execute_statement(&mut self, stmt: &Statement) -> PolarsResult<LazyFrame> {
+    pub(crate) fn execute_statement(&mut self, stmt: &Statement) -> PolarsResult<LazyFrame> {
         let ast = stmt;
         Ok(match ast {
             Statement::Query(query) => self.execute_query(query)?,
+            stmt @ Statement::ShowTables { .. } => self.execute_show_tables(stmt)?,
             stmt @ Statement::CreateTable { .. } => self.execute_create_table(stmt)?,
             _ => polars_bail!(
                 ComputeError: "SQL statement type {:?} is not supported", ast,
             ),
         })
     }
 
-    pub fn execute_query(&mut self, query: &Query) -> PolarsResult<LazyFrame> {
+    pub(crate) fn execute_query(&mut self, query: &Query) -> PolarsResult<LazyFrame> {
         let mut lf = match &query.body.as_ref() {
             SetExpr::Select(select_stmt) => self.execute_select(select_stmt)?,
             _ => polars_bail!(ComputeError: "INSERT, UPDATE is not supported"),
         };
         if !query.order_by.is_empty() {
             lf = self.process_order_by(lf, &query.order_by)?;
         }
@@ -79,14 +78,20 @@
             None => Ok(lf),
             _ => polars_bail!(
                 ComputeError: "non-number arguments to LIMIT clause are not supported",
             ),
         }
     }
 
+    fn execute_show_tables(&mut self, _: &Statement) -> PolarsResult<LazyFrame> {
+        let tables = Series::new("name", self.tables.clone());
+        let df = DataFrame::new(vec![tables])?;
+        Ok(df.lazy())
+    }
+
     /// execute the 'FROM' part of the query
     fn execute_from_statement(&mut self, tbl_expr: &TableWithJoins) -> PolarsResult<LazyFrame> {
         let (tbl_name, mut lf) = self.get_table(&tbl_expr.relation)?;
         if !tbl_expr.joins.is_empty() {
             for tbl in &tbl_expr.joins {
                 let (join_tbl_name, join_tbl) = self.get_table(&tbl.relation)?;
                 match &tbl.join_operator {
@@ -130,28 +135,28 @@
 
         let lf = self.execute_from_statement(sql_tbl)?;
         let mut contains_wildcard = false;
 
         // Filter Expression
         let lf = match select_stmt.selection.as_ref() {
             Some(expr) => {
-                let filter_expression = parse_sql_expr(expr)?;
+                let filter_expression = parse_sql_expr(expr, self)?;
                 lf.filter(filter_expression)
             }
             None => lf,
         };
         // Column Projections
         let projections: Vec<_> = select_stmt
             .projection
             .iter()
             .map(|select_item| {
                 Ok(match select_item {
-                    SelectItem::UnnamedExpr(expr) => parse_sql_expr(expr)?,
+                    SelectItem::UnnamedExpr(expr) => parse_sql_expr(expr, self)?,
                     SelectItem::ExprWithAlias { expr, alias } => {
-                        let expr = parse_sql_expr(expr)?;
+                        let expr = parse_sql_expr(expr, self)?;
                         expr.alias(&alias.value)
                     }
                     SelectItem::QualifiedWildcard { .. } | SelectItem::Wildcard { .. } => {
                         contains_wildcard = true;
                         col("*")
                     }
                 })
@@ -175,15 +180,15 @@
                     }?;
                     Ok(projections[idx].clone())
                 }
                 SqlExpr::Value(_) => Err(polars_err!(
                     ComputeError:
                     "groupby error: a positive number or an expression expected",
                 )),
-                _ => parse_sql_expr(e),
+                _ => parse_sql_expr(e, self),
             })
             .collect::<PolarsResult<_>>()?;
 
         if groupby_keys.is_empty() {
             Ok(lf.select(projections))
         } else {
             self.process_groupby(lf, contains_wildcard, &groupby_keys, &projections)
@@ -257,24 +262,26 @@
 
         let read_fn = tbl_fn.parse::<PolarsTableFunctions>()?;
         let (tbl_name, lf) = read_fn.execute(args)?;
         let tbl_name = alias
             .as_ref()
             .map(|a| a.name.value.clone())
             .unwrap_or_else(|| tbl_name);
-        self.register(&tbl_name, lf.clone());
+
+        self.table_map.insert(tbl_name.clone(), lf.clone());
+
         Ok((tbl_name, lf))
     }
 
     fn process_order_by(&mut self, lf: LazyFrame, ob: &[OrderByExpr]) -> PolarsResult<LazyFrame> {
         let mut by = Vec::with_capacity(ob.len());
         let mut descending = Vec::with_capacity(ob.len());
 
         for ob in ob {
-            by.push(parse_sql_expr(&ob.expr)?);
+            by.push(parse_sql_expr(&ob.expr, self)?);
             if let Some(false) = ob.asc {
                 descending.push(true)
             } else {
                 descending.push(false)
             }
             polars_ensure!(
                 ob.nulls_first.is_none(),
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/functions.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 use polars_lazy::dsl::{lit, Expr};
 use sqlparser::ast::{
     Expr as SqlExpr, Function as SQLFunction, FunctionArg, FunctionArgExpr, Value as SqlValue,
     WindowSpec,
 };
 
 use crate::sql_expr::parse_sql_expr;
+use crate::SQLContext;
 
-pub(crate) struct SqlFunctionVisitor<'a>(pub(crate) &'a SQLFunction);
+pub(crate) struct SqlFunctionVisitor<'a> {
+    pub(crate) func: &'a SQLFunction,
+    pub(crate) ctx: &'a SQLContext,
+}
 
 /// SQL functions that are supported by Polars
 pub(crate) enum PolarsSqlFunctions {
     // ----
     // Math functions
     // ----
     /// SQL 'abs' function
@@ -281,15 +285,15 @@
             other => polars_bail!(InvalidOperation: "unsupported SQL function: {}", other),
         })
     }
 }
 
 impl SqlFunctionVisitor<'_> {
     pub(crate) fn visit_function(&self) -> PolarsResult<Expr> {
-        let function = self.0;
+        let function = self.func;
 
         let function_name: PolarsSqlFunctions = function.try_into()?;
         use PolarsSqlFunctions::*;
         match function_name {
             // ----
             // Math functions
             // ----
@@ -353,91 +357,97 @@
             Explode => self.visit_unary(|e| e.explode()),
             ArrayContains => self.visit_binary::<Expr>(|e, s| e.arr().contains(s)),
             ArrayGet => self.visit_binary(|e, i| e.arr().get(i)),
         }
     }
 
     fn visit_unary(&self, f: impl Fn(Expr) -> Expr) -> PolarsResult<Expr> {
-        let function = self.0;
+        let function = self.func;
         let args = extract_args(function);
         if let FunctionArgExpr::Expr(sql_expr) = args[0] {
             // parse the inner sql expr -- e.g. SUM(a) -> a
-            let expr = parse_sql_expr(sql_expr)?;
+            let expr = parse_sql_expr(sql_expr, self.ctx)?;
             // apply the function on the inner expr -- e.g. SUM(a) -> SUM
             let expr = f(expr);
             // apply the window spec if present
-            apply_window_spec(expr, &function.over)
+            self.apply_window_spec(expr, &function.over)
         } else {
             not_supported_error(function.name.0[0].value.as_str(), &args)
         }
     }
 
     fn visit_binary<Arg: FromSqlExpr>(&self, f: impl Fn(Expr, Arg) -> Expr) -> PolarsResult<Expr> {
-        let function = self.0;
+        let function = self.func;
         let args = extract_args(function);
         if let FunctionArgExpr::Expr(sql_expr) = args[0] {
-            let expr = apply_window_spec(parse_sql_expr(sql_expr)?, &function.over)?;
+            let expr =
+                self.apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &function.over)?;
             if let FunctionArgExpr::Expr(sql_expr) = args[1] {
-                let expr2 = Arg::from_sql_expr(sql_expr)?;
+                let expr2 = Arg::from_sql_expr(sql_expr, self.ctx)?;
                 Ok(f(expr, expr2))
             } else {
                 not_supported_error(function.name.0[0].value.as_str(), &args)
             }
         } else {
             not_supported_error(function.name.0[0].value.as_str(), &args)
         }
     }
 
     fn visit_count(&self) -> PolarsResult<Expr> {
-        let args = extract_args(self.0);
-        Ok(match (args.len(), self.0.distinct) {
+        let args = extract_args(self.func);
+        Ok(match (args.len(), self.func.distinct) {
             // count()
             (0, false) => lit(1i32).count(),
             // count(distinct)
             (0, true) => return not_supported_error("count", &args),
             (1, false) => match args[0] {
                 // count(col)
                 FunctionArgExpr::Expr(sql_expr) => {
-                    let expr = apply_window_spec(parse_sql_expr(sql_expr)?, &self.0.over)?;
+                    let expr = self
+                        .apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &self.func.over)?;
                     expr.count()
                 }
                 // count(*)
                 FunctionArgExpr::Wildcard => lit(1i32).count(),
                 // count(tbl.*) is not supported
                 _ => return not_supported_error("count", &args),
             },
             (1, true) => {
                 // count(distinct col)
                 if let FunctionArgExpr::Expr(sql_expr) = args[0] {
-                    let expr = apply_window_spec(parse_sql_expr(sql_expr)?, &self.0.over)?;
+                    let expr = self
+                        .apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &self.func.over)?;
                     expr.n_unique()
                 } else {
                     // count(distinct *) or count(distinct tbl.*) is not supported
                     return not_supported_error("count", &args);
                 }
             }
             _ => return not_supported_error("count", &args),
         })
     }
-}
-
-fn apply_window_spec(expr: Expr, window_spec: &Option<WindowSpec>) -> PolarsResult<Expr> {
-    Ok(match &window_spec {
-        Some(window_spec) => {
-            // Process for simple window specification, partition by first
-            let partition_by = window_spec
-                .partition_by
-                .iter()
-                .map(parse_sql_expr)
-                .collect::<PolarsResult<Vec<_>>>()?;
-            expr.over(partition_by)
-            // Order by and Row range may not be supported at the moment
-        }
-        None => expr,
-    })
+    fn apply_window_spec(
+        &self,
+        expr: Expr,
+        window_spec: &Option<WindowSpec>,
+    ) -> PolarsResult<Expr> {
+        Ok(match &window_spec {
+            Some(window_spec) => {
+                // Process for simple window specification, partition by first
+                let partition_by = window_spec
+                    .partition_by
+                    .iter()
+                    .map(|p| parse_sql_expr(p, self.ctx))
+                    .collect::<PolarsResult<Vec<_>>>()?;
+                expr.over(partition_by)
+                // Order by and Row range may not be supported at the moment
+            }
+            None => expr,
+        })
+    }
 }
 
 fn not_supported_error(function_name: &str, args: &Vec<&FunctionArgExpr>) -> PolarsResult<Expr> {
     polars_bail!(
         InvalidOperation:
         "function `{}` with args {:?} is not supported in polars-sql",
         function_name, args
@@ -452,21 +462,21 @@
             FunctionArg::Named { arg, .. } => arg,
             FunctionArg::Unnamed(arg) => arg,
         })
         .collect()
 }
 
 pub(crate) trait FromSqlExpr {
-    fn from_sql_expr(expr: &SqlExpr) -> PolarsResult<Self>
+    fn from_sql_expr(expr: &SqlExpr, ctx: &SQLContext) -> PolarsResult<Self>
     where
         Self: Sized;
 }
 
 impl FromSqlExpr for f64 {
-    fn from_sql_expr(expr: &SqlExpr) -> PolarsResult<Self>
+    fn from_sql_expr(expr: &SqlExpr, _ctx: &SQLContext) -> PolarsResult<Self>
     where
         Self: Sized,
     {
         match expr {
             SqlExpr::Value(v) => match v {
                 SqlValue::Number(s, _) => s
                     .parse()
@@ -475,29 +485,29 @@
             },
             _ => polars_bail!(ComputeError: "can't parse literal {:?}", expr),
         }
     }
 }
 
 impl FromSqlExpr for String {
-    fn from_sql_expr(expr: &SqlExpr) -> PolarsResult<Self>
+    fn from_sql_expr(expr: &SqlExpr, _: &SQLContext) -> PolarsResult<Self>
     where
         Self: Sized,
     {
         match expr {
             SqlExpr::Value(v) => match v {
                 SqlValue::SingleQuotedString(s) => Ok(s.clone()),
                 _ => polars_bail!(ComputeError: "can't parse literal {:?}", v),
             },
             _ => polars_bail!(ComputeError: "can't parse literal {:?}", expr),
         }
     }
 }
 
 impl FromSqlExpr for Expr {
-    fn from_sql_expr(expr: &SqlExpr) -> PolarsResult<Self>
+    fn from_sql_expr(expr: &SqlExpr, ctx: &SQLContext) -> PolarsResult<Self>
     where
         Self: Sized,
     {
-        parse_sql_expr(expr)
+        parse_sql_expr(expr, ctx)
     }
 }
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+//! # Polars SQL
+#![deny(missing_docs)]
 mod context;
 mod functions;
 mod sql_expr;
 mod table_functions;
 pub use context::SQLContext;
 
 #[cfg(test)]
@@ -17,15 +19,15 @@
         let b = Series::new("b", 1..10000i64);
         DataFrame::new(vec![a, b])
     }
 
     #[test]
     fn test_simple_select() -> PolarsResult<()> {
         let df = create_sample_df()?;
-        let mut context = SQLContext::try_new()?;
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let df_sql = context
             .execute(
                 r#"
             SELECT a, b, a + b as c
             FROM df
             where a > 10 and a < 20
@@ -42,28 +44,28 @@
         assert_eq!(df_sql, df_pl);
         Ok(())
     }
 
     #[test]
     fn test_nested_expr() -> PolarsResult<()> {
         let df = create_sample_df()?;
-        let mut context = SQLContext::try_new()?;
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let df_sql = context
             .execute(r#"SELECT * FROM df WHERE (a > 3)"#)?
             .collect()?;
         let df_pl = df.lazy().filter(col("a").gt(lit(3))).collect()?;
         assert_eq!(df_sql, df_pl);
         Ok(())
     }
 
     #[test]
     fn test_groupby_simple() -> PolarsResult<()> {
         let df = create_sample_df()?;
-        let mut context = SQLContext::try_new()?;
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let df_sql = context
             .execute(
                 r#"
             SELECT a, sum(b) as b , sum(a + b) as c, count(a) as total_count
             FROM df
             GROUP BY a
@@ -100,15 +102,15 @@
         assert_eq!(df_sql, df_pl);
         Ok(())
     }
 
     #[test]
     fn test_cast_exprs() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 cast(a as FLOAT) as floats, 
                 cast(a as INT) as ints, 
                 cast(a as BIGINT) as bigints, 
                 cast(a as STRING) as strings
@@ -126,15 +128,15 @@
             .unwrap();
         assert!(df_sql.frame_equal(&df_pl));
     }
 
     #[test]
     fn test_literal_exprs() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 1 as int_lit, 
                 1.0 as float_lit, 
                 'foo' as string_lit,
                 true as bool_lit,
@@ -154,15 +156,15 @@
             .unwrap();
         assert!(df_sql.frame_equal_missing(&df_pl));
     }
 
     #[test]
     fn test_prefixed_column_names() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 df.a as a, 
                 df.b as b
             FROM df"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
@@ -173,15 +175,15 @@
             .unwrap();
         assert!(df_sql.frame_equal(&df_pl));
     }
 
     #[test]
     fn test_prefixed_column_names_2() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 "df"."a" as a, 
                 "df"."b" as b
             FROM df"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
@@ -191,15 +193,15 @@
             .collect()
             .unwrap();
         assert!(df_sql.frame_equal(&df_pl));
     }
     #[test]
     fn test_binary_functions() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 a, 
                 b, 
                 a + b as add, 
                 a - b as sub, 
@@ -240,15 +242,15 @@
         let df_pl = df_pl.collect().unwrap();
         assert_eq!(df_sql, df_pl);
     }
 
     #[test]
     fn test_null_exprs() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 a, 
                 b,
                 a is null as isnull_a, 
                 b is null as isnull_b, 
@@ -275,15 +277,15 @@
     fn test_null_exprs_in_where() {
         let df = df! {
             "a" => &[Some(1), None, Some(3)],
             "b" => &[Some(1), Some(2), None]
         }
         .unwrap();
 
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 a, 
                 b
             FROM df
             WHERE a is null and b is not null"#;
@@ -299,15 +301,15 @@
 
     #[test]
     fn test_math_functions() {
         let df = df! {
             "a" => [1.0]
         }
         .unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 a, 
                 ABS(a) AS abs,
                 ACOS(a) AS acos,
                 ASIN(a) AS asin,
@@ -348,15 +350,15 @@
     fn test_iss_7440() {
         let df = df! {
             "a" => [2.0, -2.5]
         }
         .unwrap()
         .lazy();
         let sql = r#"SELECT a, FLOOR(a) AS floor, CEIL(a) AS ceil FROM df"#;
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone());
 
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
 
         let df_pl = df
             .select(&[
                 col("a"),
@@ -369,15 +371,15 @@
     }
     #[test]
     fn test_string_functions() {
         let df = df! {
             "a" => &["foo", "xxxbarxxx", "---bazyyy"]
         }
         .unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 a, 
                 lower('LITERAL') as lower_literal,
                 lower(a) as lower_a,
                 lower("a") as lower_a2,
@@ -444,15 +446,15 @@
             .collect()
             .unwrap();
         assert!(df_sql.frame_equal_missing(&df_pl));
     }
     #[test]
     fn test_agg_functions() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             SELECT 
                 sum(a) as sum_a,
                 first(a) as first_a,
                 last(a) as last_a,
                 avg(a) as avg_a,
@@ -485,15 +487,15 @@
             .collect()
             .unwrap();
         assert!(df_sql.frame_equal(&df_pl));
     }
     #[test]
     fn create_table() {
         let df = create_sample_df().unwrap();
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"
             CREATE TABLE df2 AS
             SELECT a
             FROM df"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let create_tbl_res = df! {
@@ -513,15 +515,15 @@
     #[test]
     fn test_unary_minus_0() {
         let df = df! {
             "value" => [-5, -3, 0, 3, 5],
         }
         .unwrap();
 
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"SELECT * FROM df WHERE value < -1"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let df_pl = df
             .lazy()
             .filter(col("value").lt(lit(-1)))
             .collect()
@@ -531,25 +533,25 @@
     #[test]
     fn test_unary_minus_1() {
         let df = df! {
             "value" => [-5, -3, 0, 3, 5],
         }
         .unwrap();
 
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let sql = r#"SELECT * FROM df WHERE -value < 1"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let neg_value = lit(0) - col("value");
         let df_pl = df.lazy().filter(neg_value.lt(lit(1))).collect().unwrap();
         assert!(df_sql.frame_equal(&df_pl));
     }
 
     fn assert_sql_to_polars(df: &DataFrame, sql: &str, f: impl FnOnce(LazyFrame) -> LazyFrame) {
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         context.register("df", df.clone().lazy());
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let df_pl = f(df.clone().lazy()).collect().unwrap();
         assert!(df_sql.frame_equal(&df_pl));
     }
 
     #[test]
@@ -592,15 +594,15 @@
             assert_sql_to_polars(&df, sql, |df| df.select(&expr));
         }
     }
 
     #[test]
     #[cfg(feature = "csv")]
     fn read_csv_tbl_func() {
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         let sql = r#"
             CREATE TABLE foods1 AS
             SELECT *
             FROM read_csv('../../examples/datasets/foods1.csv')"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let create_tbl_res = df! {
             "Response" => ["Create Table"]
@@ -614,15 +616,15 @@
             .unwrap();
         assert_eq!(df_2.height(), 27);
         assert_eq!(df_2.width(), 4);
     }
     #[test]
     #[cfg(feature = "csv")]
     fn read_csv_tbl_func_inline() {
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         let sql = r#"
             SELECT foods1.category
             FROM read_csv('../../examples/datasets/foods1.csv') as foods1"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
 
         let expected = LazyCsvReader::new("../../examples/datasets/foods1.csv")
             .finish()
@@ -631,15 +633,15 @@
             .collect()
             .unwrap();
         assert!(df_sql.frame_equal(&expected));
     }
     #[test]
     #[cfg(feature = "csv")]
     fn read_csv_tbl_func_inline_2() {
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         let sql = r#"
             SELECT category
             FROM read_csv('../../examples/datasets/foods1.csv')"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
 
         let expected = LazyCsvReader::new("../../examples/datasets/foods1.csv")
             .finish()
@@ -649,15 +651,15 @@
             .unwrap();
         assert!(df_sql.frame_equal(&expected));
     }
 
     #[test]
     #[cfg(feature = "parquet")]
     fn read_parquet_tbl() {
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         let sql = r#"
             CREATE TABLE foods1 AS
             SELECT *
             FROM read_parquet('../../examples/datasets/foods1.parquet')"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let create_tbl_res = df! {
             "Response" => ["Create Table"]
@@ -671,15 +673,15 @@
             .unwrap();
         assert_eq!(df_2.height(), 27);
         assert_eq!(df_2.width(), 4);
     }
     #[test]
     #[cfg(feature = "ipc")]
     fn read_ipc_tbl() {
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         let sql = r#"
             CREATE TABLE foods1 AS
             SELECT *
             FROM read_ipc('../../examples/datasets/foods1.ipc')"#;
         let df_sql = context.execute(sql).unwrap().collect().unwrap();
         let create_tbl_res = df! {
             "Response" => ["Create Table"]
@@ -694,15 +696,15 @@
         assert_eq!(df_2.height(), 27);
         assert_eq!(df_2.width(), 4);
     }
 
     #[test]
     #[cfg(feature = "csv")]
     fn iss_7436() {
-        let mut context = SQLContext::try_new().unwrap();
+        let mut context = SQLContext::new();
         let sql = r#"
             CREATE TABLE foods AS
             SELECT *
             FROM read_csv('../../examples/datasets/foods1.csv')"#;
         context.execute(sql).unwrap().collect().unwrap();
         let df_sql = context
             .execute(
@@ -732,15 +734,15 @@
             .unwrap();
         assert!(df_sql.frame_equal(&expected));
     }
 
     #[test]
     #[cfg(feature = "csv")]
     fn iss_7437() -> PolarsResult<()> {
-        let mut context = SQLContext::try_new()?;
+        let mut context = SQLContext::new();
         let sql = r#"
             CREATE TABLE foods AS
             SELECT *
             FROM read_csv('../../examples/datasets/foods1.csv')"#;
         context.execute(sql)?.collect()?;
 
         let df_sql = context
@@ -763,15 +765,15 @@
 
         assert!(df_sql.frame_equal(&expected));
         Ok(())
     }
     #[test]
     #[cfg(feature = "ipc")]
     fn test_groupby_2() -> PolarsResult<()> {
-        let mut context = SQLContext::try_new()?;
+        let mut context = SQLContext::new();
         let sql = r#"
         CREATE TABLE foods AS
         SELECT *
         FROM read_ipc('../../examples/datasets/foods1.ipc')"#;
 
         context.execute(sql)?.collect()?;
         let sql = r#"
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 use polars_lazy::prelude::*;
 use sqlparser::ast::{
     ArrayAgg, BinaryOperator as SQLBinaryOperator, BinaryOperator, DataType as SQLDataType,
     Expr as SqlExpr, Function as SQLFunction, JoinConstraint, OrderByExpr, TrimWhereField,
     UnaryOperator, Value as SqlValue,
 };
 
-use crate::context::TABLES;
 use crate::functions::SqlFunctionVisitor;
+use crate::SQLContext;
 
 pub(crate) fn map_sql_polars_datatype(data_type: &SQLDataType) -> PolarsResult<DataType> {
     Ok(match data_type {
         SQLDataType::Char(_)
         | SQLDataType::Varchar(_)
         | SQLDataType::Uuid
         | SQLDataType::Clob(_)
@@ -38,17 +38,19 @@
             DataType::List(Box::new(map_sql_polars_datatype(inner_type)?))
         }
         _ => polars_bail!(ComputeError: "SQL datatype {:?} is not yet supported", data_type),
     })
 }
 
 /// Recursively walks a SQL Expr to create a polars Expr
-pub(crate) struct SqlExprVisitor {}
+pub(crate) struct SqlExprVisitor<'a> {
+    ctx: &'a SQLContext,
+}
 
-impl SqlExprVisitor {
+impl SqlExprVisitor<'_> {
     fn visit_expr(&self, expr: &SqlExpr) -> PolarsResult<Expr> {
         match expr {
             SqlExpr::CompoundIdentifier(idents) => self.visit_compound_identifier(idents),
             SqlExpr::Identifier(ident) => self.visit_identifier(ident),
             SqlExpr::BinaryOp { left, op, right } => self.visit_binary_op(left, op, right),
             SqlExpr::Function(function) => self.visit_function(function),
             SqlExpr::Cast { expr, data_type } => self.visit_cast(expr, data_type),
@@ -86,18 +88,16 @@
     /// e.g. df.column or "df"."column"
     fn visit_compound_identifier(&self, idents: &[sqlparser::ast::Ident]) -> PolarsResult<Expr> {
         polars_ensure!(
             idents.len() == 2,
             ComputeError: "compound identifier {:?} is not yet supported", idents,
         );
         let tbl_name = &idents[0].value;
-        let refers_main_table = TABLES.with(|cell| {
-            let tables = cell.borrow();
-            tables.len() == 1 && tables.contains(tbl_name)
-        });
+        let refers_main_table =
+            { self.ctx.tables.len() == 1 && self.ctx.tables.contains(&tbl_name) };
         polars_ensure!(
             refers_main_table, ComputeError:
             "compound identifier {:?} is not yet supported if multiple tables are registered",
             idents
         );
         Ok(col(&idents[1].value))
     }
@@ -153,15 +153,18 @@
 
     /// Visit a SQL function
     ///
     /// e.g. SUM(column) or COUNT(*)
     ///
     /// See [SqlFunctionVisitor] for more details
     fn visit_function(&self, function: &SQLFunction) -> PolarsResult<Expr> {
-        let visitor = SqlFunctionVisitor(function);
+        let visitor = SqlFunctionVisitor {
+            func: function,
+            ctx: self.ctx,
+        };
         visitor.visit_function()
     }
 
     /// Visit a SQL CAST
     ///
     /// e.g. `CAST(column AS INT)` or `column::INT`
     fn visit_cast(&self, expr: &SqlExpr, data_type: &SQLDataType) -> PolarsResult<Expr> {
@@ -279,16 +282,16 @@
     }
 
     fn err(&self, expr: &Expr) -> PolarsResult<Expr> {
         polars_bail!(ComputeError: "SQL expression {:?} is not yet supported", expr);
     }
 }
 
-pub(crate) fn parse_sql_expr(expr: &SqlExpr) -> PolarsResult<Expr> {
-    let visitor = SqlExprVisitor {};
+pub(crate) fn parse_sql_expr<'a>(expr: &SqlExpr, ctx: &'a SQLContext) -> PolarsResult<Expr> {
+    let visitor = SqlExprVisitor { ctx };
     visitor.visit_expr(expr)
 }
 
 pub(super) fn process_join_constraint(
     constraint: &JoinConstraint,
     left_name: &str,
     right_name: &str,
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.17.1/local_dependencies/polars/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 //! * `POLARS_FMT_TABLE_HIDE_COLUMN_NAMES` -> hide table column names.
 //! * `POLARS_FMT_TABLE_HIDE_COLUMN_DATA_TYPES` -> hide data types for columns.
 //! * `POLARS_FMT_TABLE_HIDE_COLUMN_SEPARATOR` -> hide separator that separates column names from rows.
 //! * `POLARS_FMT_TABLE_HIDE_DATAFRAME_SHAPE_INFORMATION"` -> omit table shape information.
 //! * `POLARS_FMT_TABLE_INLINE_COLUMN_DATA_TYPE` -> put column data type on the same line as the column name.
 //! * `POLARS_FMT_TABLE_ROUNDED_CORNERS` -> apply rounded corners to UTF8-styled tables.
 //! * `POLARS_FMT_MAX_COLS` -> maximum number of columns shown when formatting DataFrames.
-//! * `POLARS_FMT_MAX_ROWS` -> maximum number of rows shown when formatting DataFrames.
+//! * `POLARS_FMT_MAX_ROWS` -> maximum number of rows shown when formatting DataFrames, `-1` to show all.
 //! * `POLARS_FMT_STR_LEN` -> maximum number of characters printed per string value.
 //! * `POLARS_TABLE_WIDTH` -> width of the tables used during DataFrame formatting.
 //! * `POLARS_MAX_THREADS` -> maximum number of threads used to initialize thread pool (on startup).
 //! * `POLARS_VERBOSE` -> print logging info to stderr.
 //! * `POLARS_NO_PARTITION` -> polars may choose to partition the groupby operation, based on data
 //!                            cardinality. Setting this env var will turn partitioned groupby's off.
 //! * `POLARS_PARTITION_SAMPLE_FRAC` -> how large chunk of the dataset to sample to determine cardinality,
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars/tests/it/schema.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/hash.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 #[cfg(feature = "timezones")]
 fn validate_time_zone(tz: TimeZone) -> PolarsResult<()> {
     match parse_offset(&tz) {
         Ok(_) => Ok(()),
         Err(_) => match tz.parse::<Tz>() {
             Ok(_) => Ok(()),
-            Err(_) => polars_bail!(ComputeError: "unable to parse timezone: '{}'", tz),
+            Err(_) => polars_bail!(ComputeError: "unable to parse time zone: '{}'", tz),
         },
     }
 }
 
 fn apply_datefmt_f<'a>(
     arr: &PrimitiveArray<i64>,
     fmted: &'a str,
@@ -120,52 +120,31 @@
 
     #[cfg(feature = "timezones")]
     pub fn replace_time_zone(&self, time_zone: Option<&str>) -> PolarsResult<DatetimeChunked> {
         match (self.time_zone(), time_zone) {
             (Some(from), Some(to)) => {
                 let chunks = self
                     .downcast_iter()
-                    .map(|arr| {
-                        replace_timezone(
-                            arr,
-                            self.time_unit().to_arrow(),
-                            to.to_string(),
-                            from.to_string(),
-                        )
-                    })
+                    .map(|arr| replace_timezone(arr, self.time_unit().to_arrow(), to, from))
                     .collect::<PolarsResult<_>>()?;
                 let out = unsafe { ChunkedArray::from_chunks(self.name(), chunks) };
                 Ok(out.into_datetime(self.time_unit(), Some(to.to_string())))
             }
             (Some(from), None) => {
                 let chunks = self
                     .downcast_iter()
-                    .map(|arr| {
-                        replace_timezone(
-                            arr,
-                            self.time_unit().to_arrow(),
-                            "UTC".to_string(),
-                            from.to_string(),
-                        )
-                    })
+                    .map(|arr| replace_timezone(arr, self.time_unit().to_arrow(), "UTC", from))
                     .collect::<PolarsResult<_>>()?;
                 let out = unsafe { ChunkedArray::from_chunks(self.name(), chunks) };
                 Ok(out.into_datetime(self.time_unit(), None))
             }
             (None, Some(to)) => {
                 let chunks = self
                     .downcast_iter()
-                    .map(|arr| {
-                        replace_timezone(
-                            arr,
-                            self.time_unit().to_arrow(),
-                            to.to_string(),
-                            "UTC".to_string(),
-                        )
-                    })
+                    .map(|arr| replace_timezone(arr, self.time_unit().to_arrow(), to, "UTC"))
                     .collect::<PolarsResult<_>>()?;
                 let out = unsafe { ChunkedArray::from_chunks(self.name(), chunks) };
                 Ok(out.into_datetime(self.time_unit(), Some(to.to_string())))
             }
             (None, None) => Ok(self.clone()),
         }
     }
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/schema.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -424,26 +424,28 @@
     };
 
     match infer_pattern_single(val) {
         None => {
             buf.builder.append_null();
             Ok(())
         }
-        Some(pattern) => match DatetimeInfer::<T::Native>::try_from(pattern) {
-            Ok(mut infer) => {
-                let parsed = infer.parse(val);
-                buf.compiled = Some(infer);
-                buf.builder.append_option(parsed);
-                Ok(())
-            }
-            Err(_) => {
-                buf.builder.append_null();
-                Ok(())
+        Some(pattern_with_offset) => {
+            match DatetimeInfer::<T::Native>::try_from(pattern_with_offset.pattern) {
+                Ok(mut infer) => {
+                    let parsed = infer.parse(val, pattern_with_offset.offset);
+                    buf.compiled = Some(infer);
+                    buf.builder.append_option(parsed);
+                    Ok(())
+                }
+                Err(_) => {
+                    buf.builder.append_null();
+                    Ok(())
+                }
             }
-        },
+        }
     }
 }
 
 #[cfg(any(feature = "dtype-datetime", feature = "dtype-date"))]
 impl<T> ParsedBuffer for DatetimeField<T>
 where
     T: PolarsNumericType,
@@ -516,17 +518,18 @@
                     capacity,
                     str_capacity,
                     quote_char,
                     encoding,
                     ignore_errors,
                 )),
                 #[cfg(feature = "dtype-datetime")]
-                &DataType::Datetime(tu, _) => Buffer::Datetime {
+                DataType::Datetime(tu, offset) => Buffer::Datetime {
                     buf: DatetimeField::new(name, capacity),
-                    tu,
+                    tu: *tu,
+                    offset: offset.clone(),
                 },
                 #[cfg(feature = "dtype-date")]
                 &DataType::Date => Buffer::Date(DatetimeField::new(name, capacity)),
                 #[cfg(feature = "dtype-categorical")]
                 &DataType::Categorical(_) => {
                     Buffer::Categorical(CategoricalField::new(name, capacity, quote_char))
                 }
@@ -550,14 +553,15 @@
     Float64(PrimitiveChunkedBuilder<Float64Type>),
     /// Stores the Utf8 fields and the total string length seen for that column
     Utf8(Utf8Field),
     #[cfg(feature = "dtype-datetime")]
     Datetime {
         buf: DatetimeField<Int64Type>,
         tu: TimeUnit,
+        offset: Option<String>,
     },
     #[cfg(feature = "dtype-date")]
     Date(DatetimeField<Int32Type>),
     #[allow(dead_code)]
     Categorical(CategoricalField<'a>),
 }
 
@@ -568,19 +572,19 @@
             Buffer::Int32(v) => v.finish().into_series(),
             Buffer::Int64(v) => v.finish().into_series(),
             Buffer::UInt32(v) => v.finish().into_series(),
             Buffer::UInt64(v) => v.finish().into_series(),
             Buffer::Float32(v) => v.finish().into_series(),
             Buffer::Float64(v) => v.finish().into_series(),
             #[cfg(feature = "dtype-datetime")]
-            Buffer::Datetime { buf, tu } => buf
+            Buffer::Datetime { buf, tu, offset } => buf
                 .builder
                 .finish()
                 .into_series()
-                .cast(&DataType::Datetime(tu, None))
+                .cast(&DataType::Datetime(tu, offset))
                 .unwrap(),
             #[cfg(feature = "dtype-date")]
             Buffer::Date(v) => v
                 .builder
                 .finish()
                 .into_series()
                 .cast(&DataType::Date)
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use std::mem::MaybeUninit;
 
 use once_cell::sync::Lazy;
 use polars_core::datatypes::PlHashSet;
 use polars_core::prelude::*;
 #[cfg(feature = "polars-time")]
 use polars_time::chunkedarray::utf8::infer as date_infer;
+use polars_time::chunkedarray::utf8::PatternWithOffset;
 #[cfg(feature = "polars-time")]
 use polars_time::prelude::utf8::Pattern;
 use regex::{Regex, RegexBuilder};
 
 #[cfg(any(feature = "decompress", feature = "decompress-fast"))]
 use crate::csv::parser::next_line_position_naive;
 use crate::csv::parser::{next_line_position, skip_bom, skip_line_ending, SplitLines};
@@ -106,18 +107,31 @@
     // when quoting is enabled in the reader, these quotes aren't escaped, we default to
     // Utf8 for them
     if string.starts_with('"') {
         if try_parse_dates {
             #[cfg(feature = "polars-time")]
             {
                 match date_infer::infer_pattern_single(&string[1..string.len() - 1]) {
-                    Some(Pattern::DatetimeYMD | Pattern::DatetimeDMY) => {
-                        DataType::Datetime(TimeUnit::Microseconds, None)
-                    }
-                    Some(Pattern::DateYMD | Pattern::DateDMY) => DataType::Date,
+                    Some(pattern_with_offset) => match pattern_with_offset {
+                        PatternWithOffset {
+                            pattern: Pattern::DatetimeYMD | Pattern::DatetimeDMY,
+                            offset: _,
+                        } => DataType::Datetime(TimeUnit::Microseconds, None),
+                        PatternWithOffset {
+                            pattern: Pattern::DateYMD | Pattern::DateDMY,
+                            offset: _,
+                        } => DataType::Date,
+                        PatternWithOffset {
+                            pattern: Pattern::DatetimeYMDZ,
+                            offset,
+                        } => DataType::Datetime(
+                            TimeUnit::Microseconds,
+                            offset.map(|x| x.to_string()),
+                        ),
+                    },
                     None => DataType::Utf8,
                 }
             }
             #[cfg(not(feature = "polars-time"))]
             {
                 panic!("activate one of {{'dtype-date', 'dtype-datetime', dtype-time'}} features")
             }
@@ -132,18 +146,28 @@
         DataType::Float64
     } else if INTEGER_RE.is_match(string) {
         DataType::Int64
     } else if try_parse_dates {
         #[cfg(feature = "polars-time")]
         {
             match date_infer::infer_pattern_single(string) {
-                Some(Pattern::DatetimeYMD | Pattern::DatetimeDMY) => {
-                    DataType::Datetime(TimeUnit::Microseconds, None)
-                }
-                Some(Pattern::DateYMD | Pattern::DateDMY) => DataType::Date,
+                Some(pattern_with_offset) => match pattern_with_offset {
+                    PatternWithOffset {
+                        pattern: Pattern::DatetimeYMD | Pattern::DatetimeDMY,
+                        offset: _,
+                    } => DataType::Datetime(TimeUnit::Microseconds, None),
+                    PatternWithOffset {
+                        pattern: Pattern::DateYMD | Pattern::DateDMY,
+                        offset: _,
+                    } => DataType::Date,
+                    PatternWithOffset {
+                        pattern: Pattern::DatetimeYMDZ,
+                        offset,
+                    } => DataType::Datetime(TimeUnit::Microseconds, offset.map(|x| x.to_string())),
+                },
                 None => DataType::Utf8,
             }
         }
         #[cfg(not(feature = "polars-time"))]
         {
             panic!("activate one of {{'dtype-date', 'dtype-datetime', dtype-time'}} features")
         }
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/json.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ndjson_core/buffer.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/buffer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -150,17 +150,17 @@
     T: PolarsNumericType,
     DatetimeInfer<T::Native>: TryFrom<Pattern>,
 {
     let val = match value {
         Value::String(s) => s,
         _ => return None,
     };
-    infer_pattern_single(val).and_then(|pattern| {
-        match DatetimeInfer::<T::Native>::try_from(pattern) {
-            Ok(mut infer) => infer.parse(val),
+    infer_pattern_single(val).and_then(|pattern_with_offset| {
+        match DatetimeInfer::<T::Native>::try_from(pattern_with_offset.pattern) {
+            Ok(mut infer) => infer.parse(val, pattern_with_offset.offset),
             Err(_) => None,
         }
     })
 }
 
 fn deserialize_all<'a>(json: &Value, dtype: &DataType) -> PolarsResult<AnyValue<'a>> {
     let out = match json {
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/ndjson_core/ndjson.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/ndjson_core/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use chrono::{NaiveDate, NaiveDateTime};
+use chrono::{DateTime, FixedOffset, NaiveDate, NaiveDateTime};
 use polars_arrow::export::arrow::array::PrimitiveArray;
 use polars_core::prelude::*;
 use polars_core::utils::arrow::types::NativeType;
 
-use super::patterns;
+use super::patterns::{self, PatternWithOffset};
 #[cfg(feature = "dtype-date")]
 use crate::chunkedarray::date::naive_date_to_date;
 use crate::chunkedarray::utf8::patterns::Pattern;
 use crate::chunkedarray::utf8::strptime;
 use crate::prelude::utf8::strptime::StrpTimeState;
 
 pub trait StrpTimeParser<T> {
@@ -78,18 +78,19 @@
     }
 }
 
 #[derive(Clone)]
 pub struct DatetimeInfer<T> {
     patterns: &'static [&'static str],
     latest_fmt: &'static str,
-    transform: fn(&str, &str) -> Option<T>,
+    transform: fn(&str, &str, Option<FixedOffset>, bool) -> Option<T>,
     transform_bytes: StrpTimeState,
     fmt_len: u16,
     pub logical_type: DataType,
+    utc: bool,
 }
 
 #[cfg(feature = "dtype-datetime")]
 impl TryFrom<Pattern> for DatetimeInfer<i64> {
     type Error = PolarsError;
 
     fn try_from(value: Pattern) -> PolarsResult<Self> {
@@ -97,22 +98,33 @@
             Pattern::DatetimeDMY => Ok(DatetimeInfer {
                 patterns: patterns::DATETIME_D_M_Y,
                 latest_fmt: patterns::DATETIME_D_M_Y[0],
                 transform: transform_datetime_us,
                 transform_bytes: StrpTimeState::default(),
                 fmt_len: 0,
                 logical_type: DataType::Datetime(TimeUnit::Microseconds, None),
+                utc: false,
             }),
             Pattern::DatetimeYMD => Ok(DatetimeInfer {
                 patterns: patterns::DATETIME_Y_M_D,
                 latest_fmt: patterns::DATETIME_Y_M_D[0],
                 transform: transform_datetime_us,
                 transform_bytes: StrpTimeState::default(),
                 fmt_len: 0,
                 logical_type: DataType::Datetime(TimeUnit::Microseconds, None),
+                utc: false,
+            }),
+            Pattern::DatetimeYMDZ => Ok(DatetimeInfer {
+                patterns: patterns::DATETIME_Y_M_D_Z,
+                latest_fmt: patterns::DATETIME_Y_M_D_Z[0],
+                transform: transform_tzaware_datetime_us,
+                transform_bytes: StrpTimeState::default(),
+                fmt_len: 0,
+                logical_type: DataType::Datetime(TimeUnit::Microseconds, None),
+                utc: false,
             }),
             _ => polars_bail!(ComputeError: "could not convert pattern"),
         }
     }
 }
 
 #[cfg(feature = "dtype-date")]
@@ -124,53 +136,55 @@
             Pattern::DateDMY => Ok(DatetimeInfer {
                 patterns: patterns::DATE_D_M_Y,
                 latest_fmt: patterns::DATE_D_M_Y[0],
                 transform: transform_date,
                 transform_bytes: StrpTimeState::default(),
                 fmt_len: 0,
                 logical_type: DataType::Date,
+                utc: false,
             }),
             Pattern::DateYMD => Ok(DatetimeInfer {
                 patterns: patterns::DATE_Y_M_D,
                 latest_fmt: patterns::DATE_Y_M_D[0],
                 transform: transform_date,
                 transform_bytes: StrpTimeState::default(),
                 fmt_len: 0,
                 logical_type: DataType::Date,
+                utc: false,
             }),
             _ => polars_bail!(ComputeError: "could not convert pattern"),
         }
     }
 }
 
 impl<T: NativeType> DatetimeInfer<T> {
-    pub fn parse(&mut self, val: &str) -> Option<T> {
-        match (self.transform)(val, self.latest_fmt) {
+    pub fn parse(&mut self, val: &str, offset: Option<FixedOffset>) -> Option<T> {
+        match (self.transform)(val, self.latest_fmt, offset, self.utc) {
             Some(parsed) => Some(parsed),
             // try other patterns
             None => {
                 for fmt in self.patterns {
                     self.fmt_len = 0;
-                    if let Some(parsed) = (self.transform)(val, fmt) {
+                    if let Some(parsed) = (self.transform)(val, fmt, offset, self.utc) {
                         self.latest_fmt = fmt;
                         return Some(parsed);
                     }
                 }
                 None
             }
         }
     }
 
-    fn coerce_utf8(&mut self, ca: &Utf8Chunked) -> Series {
+    fn coerce_utf8(&mut self, ca: &Utf8Chunked, offset: Option<FixedOffset>) -> Series {
         let chunks = ca
             .downcast_iter()
             .map(|array| {
                 let iter = array
                     .into_iter()
-                    .map(|opt_val| opt_val.and_then(|val| self.parse(val)));
+                    .map(|opt_val| opt_val.and_then(|val| self.parse(val, offset)));
                 Box::new(PrimitiveArray::from_trusted_len_iter(iter)) as ArrayRef
             })
             .collect();
         let mut out = match self.logical_type {
             DataType::Date => unsafe { Int32Chunked::from_chunks(ca.name(), chunks) }
                 .into_series()
                 .cast(&self.logical_type)
@@ -183,133 +197,239 @@
         };
         out.rename(ca.name());
         out
     }
 }
 
 #[cfg(feature = "dtype-date")]
-fn transform_date(val: &str, fmt: &str) -> Option<i32> {
+fn transform_date(val: &str, fmt: &str, _offset: Option<FixedOffset>, _utc: bool) -> Option<i32> {
     NaiveDate::parse_from_str(val, fmt)
         .ok()
         .map(naive_date_to_date)
 }
 
 #[cfg(feature = "dtype-datetime")]
-pub(crate) fn transform_datetime_ns(val: &str, fmt: &str) -> Option<i64> {
+pub(crate) fn transform_datetime_ns(
+    val: &str,
+    fmt: &str,
+    _offset: Option<FixedOffset>,
+    _utc: bool,
+) -> Option<i64> {
     let out = NaiveDateTime::parse_from_str(val, fmt)
         .ok()
         .map(datetime_to_timestamp_ns);
     out.or_else(|| {
         NaiveDate::parse_from_str(val, fmt)
             .ok()
             .map(|nd| datetime_to_timestamp_ns(nd.and_hms_opt(0, 0, 0).unwrap()))
     })
 }
 
+fn transform_tzaware_datetime_ns(
+    val: &str,
+    fmt: &str,
+    offset: Option<FixedOffset>,
+    utc: bool,
+) -> Option<i64> {
+    let dt = DateTime::parse_from_str(val, fmt);
+    match utc {
+        true => dt.ok().map(|dt| datetime_to_timestamp_ns(dt.naive_utc())),
+        false => match Some(dt.ok()?.timezone()) == offset {
+            true => dt.ok().map(|dt| datetime_to_timestamp_ns(dt.naive_utc())),
+            false => None,
+        },
+    }
+}
+
 #[cfg(feature = "dtype-datetime")]
-pub(crate) fn transform_datetime_us(val: &str, fmt: &str) -> Option<i64> {
+pub(crate) fn transform_datetime_us(
+    val: &str,
+    fmt: &str,
+    _offset: Option<FixedOffset>,
+    _utc: bool,
+) -> Option<i64> {
     let out = NaiveDateTime::parse_from_str(val, fmt)
         .ok()
         .map(datetime_to_timestamp_us);
     out.or_else(|| {
         NaiveDate::parse_from_str(val, fmt)
             .ok()
             .map(|nd| datetime_to_timestamp_us(nd.and_hms_opt(0, 0, 0).unwrap()))
     })
 }
 
+fn transform_tzaware_datetime_us(
+    val: &str,
+    fmt: &str,
+    offset: Option<FixedOffset>,
+    utc: bool,
+) -> Option<i64> {
+    let dt = DateTime::parse_from_str(val, fmt);
+    match utc {
+        true => dt.ok().map(|dt| datetime_to_timestamp_us(dt.naive_utc())),
+        false => match Some(dt.ok()?.timezone()) == offset {
+            true => dt.ok().map(|dt| datetime_to_timestamp_us(dt.naive_utc())),
+            false => None,
+        },
+    }
+}
+
 #[cfg(feature = "dtype-datetime")]
-pub(crate) fn transform_datetime_ms(val: &str, fmt: &str) -> Option<i64> {
+pub(crate) fn transform_datetime_ms(
+    val: &str,
+    fmt: &str,
+    _offset: Option<FixedOffset>,
+    _utc: bool,
+) -> Option<i64> {
     let out = NaiveDateTime::parse_from_str(val, fmt)
         .ok()
         .map(datetime_to_timestamp_ms);
     out.or_else(|| {
         NaiveDate::parse_from_str(val, fmt)
             .ok()
             .map(|nd| datetime_to_timestamp_ms(nd.and_hms_opt(0, 0, 0).unwrap()))
     })
 }
 
-pub fn infer_pattern_single(val: &str) -> Option<Pattern> {
+fn transform_tzaware_datetime_ms(
+    val: &str,
+    fmt: &str,
+    offset: Option<FixedOffset>,
+    utc: bool,
+) -> Option<i64> {
+    let dt = DateTime::parse_from_str(val, fmt);
+    match utc {
+        true => dt.ok().map(|dt| datetime_to_timestamp_ms(dt.naive_utc())),
+        false => match Some(dt.ok()?.timezone()) == offset {
+            true => dt.ok().map(|dt| datetime_to_timestamp_ms(dt.naive_utc())),
+            false => None,
+        },
+    }
+}
+
+pub fn infer_pattern_single(val: &str) -> Option<PatternWithOffset> {
     // Dates come first, because we see datetimes as superset of dates
     infer_pattern_date_single(val).or_else(|| infer_pattern_datetime_single(val))
 }
 
-fn infer_pattern_datetime_single(val: &str) -> Option<Pattern> {
+fn infer_pattern_datetime_single(val: &str) -> Option<PatternWithOffset> {
     if patterns::DATETIME_D_M_Y.iter().any(|fmt| {
         NaiveDateTime::parse_from_str(val, fmt).is_ok()
             || NaiveDate::parse_from_str(val, fmt).is_ok()
     }) {
-        Some(Pattern::DatetimeDMY)
+        Some(PatternWithOffset {
+            pattern: Pattern::DatetimeDMY,
+            offset: None,
+        })
     } else if patterns::DATETIME_Y_M_D.iter().any(|fmt| {
         NaiveDateTime::parse_from_str(val, fmt).is_ok()
             || NaiveDate::parse_from_str(val, fmt).is_ok()
     }) {
-        Some(Pattern::DatetimeYMD)
+        Some(PatternWithOffset {
+            pattern: Pattern::DatetimeYMD,
+            offset: None,
+        })
     } else {
-        None
+        patterns::DATETIME_Y_M_D_Z
+            .iter()
+            .find_map(|fmt| DateTime::parse_from_str(val, fmt).ok())
+            .map(|dt| PatternWithOffset {
+                pattern: Pattern::DatetimeYMDZ,
+                offset: Some(dt.timezone()),
+            })
     }
 }
 
-fn infer_pattern_date_single(val: &str) -> Option<Pattern> {
+fn infer_pattern_date_single(val: &str) -> Option<PatternWithOffset> {
     if patterns::DATE_D_M_Y
         .iter()
         .any(|fmt| NaiveDate::parse_from_str(val, fmt).is_ok())
     {
-        Some(Pattern::DateDMY)
+        Some(PatternWithOffset {
+            pattern: Pattern::DateDMY,
+            offset: None,
+        })
     } else if patterns::DATE_Y_M_D
         .iter()
         .any(|fmt| NaiveDate::parse_from_str(val, fmt).is_ok())
     {
-        Some(Pattern::DateYMD)
+        Some(PatternWithOffset {
+            pattern: Pattern::DateYMD,
+            offset: None,
+        })
     } else {
         None
     }
 }
 
 #[cfg(feature = "dtype-datetime")]
 pub(crate) fn to_datetime(
     ca: &Utf8Chunked,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
+    utc: bool,
 ) -> PolarsResult<DatetimeChunked> {
     match ca.first_non_null() {
         None => Ok(Int64Chunked::full_null(ca.name(), ca.len()).into_datetime(tu, tz.cloned())),
         Some(idx) => {
             let subset = ca.slice(idx as i64, ca.len());
-            let pattern = subset
+            let pattern_with_offset = subset
                 .into_iter()
                 .find_map(|opt_val| opt_val.and_then(infer_pattern_datetime_single))
                 .ok_or_else(|| polars_err!(parse_fmt_idk = "date"))?;
-            let mut infer = DatetimeInfer::<i64>::try_from(pattern).unwrap();
-            match tu {
-                TimeUnit::Nanoseconds => infer.transform = transform_datetime_ns,
-                TimeUnit::Microseconds => infer.transform = transform_datetime_us,
-                TimeUnit::Milliseconds => infer.transform = transform_datetime_ms,
+            let mut infer = DatetimeInfer::<i64>::try_from(pattern_with_offset.pattern)?;
+            match (tu, pattern_with_offset.offset) {
+                (TimeUnit::Nanoseconds, None) => infer.transform = transform_datetime_ns,
+                (TimeUnit::Microseconds, None) => infer.transform = transform_datetime_us,
+                (TimeUnit::Milliseconds, None) => infer.transform = transform_datetime_ms,
+                (TimeUnit::Nanoseconds, _) => infer.transform = transform_tzaware_datetime_ns,
+                (TimeUnit::Microseconds, _) => infer.transform = transform_tzaware_datetime_us,
+                (TimeUnit::Milliseconds, _) => infer.transform = transform_tzaware_datetime_ms,
+            }
+            infer.utc = utc;
+            if tz.is_some() && pattern_with_offset.offset.is_some() {
+                polars_bail!(ComputeError: "cannot parse tz-aware values with tz-aware dtype - please drop the time zone from the dtype.")
+            }
+            match pattern_with_offset.offset {
+                #[cfg(feature = "timezones")]
+                Some(offset) => infer.coerce_utf8(ca, Some(offset)).datetime().map(|ca| {
+                    let mut ca = ca.clone();
+                    ca.set_time_unit(tu);
+                    match utc {
+                        true => Ok(ca.replace_time_zone(Some("UTC"))?),
+                        false => Ok(ca
+                            .replace_time_zone(Some("UTC"))?
+                            .convert_time_zone(offset.to_string())?),
+                    }
+                })?,
+                _ => infer.coerce_utf8(ca, None).datetime().map(|ca| {
+                    let mut ca = ca.clone();
+                    ca.set_time_unit(tu);
+                    match (tz, utc) {
+                        #[cfg(feature = "timezones")]
+                        (Some(tz), false) => Ok(ca.replace_time_zone(Some(tz))?),
+                        #[cfg(feature = "timezones")]
+                        (None, true) => Ok(ca.replace_time_zone(Some("UTC"))?),
+                        #[cfg(feature = "timezones")]
+                        (Some(_), true) => unreachable!(), // has already been validated in strptime
+                        _ => Ok(ca),
+                    }
+                })?,
             }
-            infer.coerce_utf8(ca).datetime().map(|ca| {
-                let mut ca = ca.clone();
-                ca.set_time_unit(tu);
-                match tz {
-                    #[cfg(feature = "timezones")]
-                    Some(tz) => Ok(ca.replace_time_zone(Some(tz))?),
-                    _ => Ok(ca),
-                }
-            })?
         }
     }
 }
 #[cfg(feature = "dtype-date")]
 pub(crate) fn to_date(ca: &Utf8Chunked) -> PolarsResult<DateChunked> {
     match ca.first_non_null() {
         None => Ok(Int32Chunked::full_null(ca.name(), ca.len()).into_date()),
         Some(idx) => {
             let subset = ca.slice(idx as i64, ca.len());
-            let pattern = subset
+            let pattern_with_offset = subset
                 .into_iter()
                 .find_map(|opt_val| opt_val.and_then(infer_pattern_date_single))
                 .ok_or_else(|| polars_err!(parse_fmt_idk = "date"))?;
-            let mut infer = DatetimeInfer::<i32>::try_from(pattern).unwrap();
-            infer.coerce_utf8(ca).date().cloned()
+            let mut infer = DatetimeInfer::<i32>::try_from(pattern_with_offset.pattern).unwrap();
+            infer.coerce_utf8(ca, None).date().cloned()
         }
     }
 }
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pub mod infer;
 mod patterns;
 mod strptime;
 
 use chrono::ParseError;
-pub use patterns::Pattern;
+pub use patterns::{Pattern, PatternWithOffset};
 
 use super::*;
 #[cfg(feature = "dtype-date")]
 use crate::chunkedarray::date::naive_date_to_date;
 #[cfg(feature = "dtype-time")]
 use crate::chunkedarray::time::time_to_time64ns;
 use crate::prelude::utf8::strptime::StrpTimeState;
@@ -382,21 +382,21 @@
     /// Parsing string values and return a [`DatetimeChunked`]
     fn as_datetime(
         &self,
         fmt: Option<&str>,
         tu: TimeUnit,
         cache: bool,
         tz_aware: bool,
-        _utc: bool,
+        utc: bool,
         tz: Option<&TimeZone>,
     ) -> PolarsResult<DatetimeChunked> {
         let utf8_ca = self.as_utf8();
         let fmt = match fmt {
             Some(fmt) => fmt,
-            None => return infer::to_datetime(utf8_ca, tu, tz),
+            None => return infer::to_datetime(utf8_ca, tu, tz, utc),
         };
         let fmt = strptime::compile_fmt(fmt);
         let cache = cache && utf8_ca.len() > 50;
 
         let func = match tu {
             TimeUnit::Nanoseconds => datetime_to_timestamp_ns,
             TimeUnit::Microseconds => datetime_to_timestamp_us,
@@ -411,15 +411,15 @@
                 let mut cache_map = PlHashMap::new();
                 let mut tz = None;
 
                 let mut convert = |s: &str| {
                     DateTime::parse_from_str(s, &fmt)
                         .ok()
                         .map(|dt| {
-                            if !_utc {
+                            if !utc {
                                 if let Some(tz_found) = tz {
                                     polars_ensure!(
                                         tz_found == dt.timezone(),
                                         ComputeError: "different timezones found during 'strptime' \
                                         operation (you might want to use `utc=True` and then set \
                                         the time zone after parsing"
                                 );
@@ -453,15 +453,15 @@
                             })
                             .transpose()
                             .map(|options| options.flatten())
                     })
                     .collect::<PolarsResult<_>>()?;
 
                 ca.rename(utf8_ca.name());
-                if !_utc {
+                if !utc {
                     let tz = tz.map(|of| format!("{of}"));
                     Ok(ca.into_datetime(tu, tz))
                 } else {
                     Ok(ca.into_datetime(tu, Some("UTC".to_string())))
                 }
             }
             #[cfg(not(feature = "timezones"))]
@@ -480,15 +480,15 @@
                 self::strptime::fmt_len(fmt.as_bytes())
             {
                 let mut strptime_cache = StrpTimeState::default();
                 let mut convert = |s: &str| {
                     // Safety:
                     // fmt_len is correct, it was computed with this `fmt` str.
                     match unsafe { strptime_cache.parse(s.as_bytes(), fmt.as_bytes(), fmt_len) } {
-                        None => transform(s, &fmt),
+                        None => transform(s, &fmt, None, utc),
                         Some(ndt) => Some(func(ndt)),
                     }
                 };
                 if utf8_ca.null_count() == 0 {
                     utf8_ca
                         .into_no_null_iter()
                         .map(|val| {
@@ -516,26 +516,32 @@
             } else {
                 let mut cache_map = PlHashMap::new();
                 utf8_ca
                     .into_iter()
                     .map(|opt_s| {
                         opt_s.and_then(|s| {
                             if cache {
-                                *cache_map.entry(s).or_insert_with(|| transform(s, &fmt))
+                                *cache_map
+                                    .entry(s)
+                                    .or_insert_with(|| transform(s, &fmt, None, false))
                             } else {
-                                transform(s, &fmt)
+                                transform(s, &fmt, None, false)
                             }
                         })
                     })
                     .collect_trusted()
             };
             ca.rename(utf8_ca.name());
-            match tz {
+            match (tz, utc) {
                 #[cfg(feature = "timezones")]
-                Some(tz) => ca.into_datetime(tu, None).replace_time_zone(Some(tz)),
+                (Some(tz), false) => ca.into_datetime(tu, None).replace_time_zone(Some(tz)),
+                #[cfg(feature = "timezones")]
+                (None, true) => ca.into_datetime(tu, None).replace_time_zone(Some("UTC")),
+                #[cfg(feature = "timezones")]
+                (Some(_), true) => unreachable!(), // has already been validated in strptime
                 _ => Ok(ca.into_datetime(tu, None)),
             }
         }
     }
 }
 
 pub trait AsUtf8 {
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/date_range.rs`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                     let stop = localize_timestamp(stop, tu, tz);
                     Int64Chunked::new_vec(
                         name,
                         date_range_vec(start?, stop?, every, closed, tu, Some(&tz))?,
                     )
                     .into_datetime(tu, _tz.cloned())
                 }
-                _ => polars_bail!(ComputeError: "unable to parse time zone: {}", tz),
+                _ => polars_bail!(ComputeError: "unable to parse time zone: '{}'", tz),
             },
         },
         _ => Int64Chunked::new_vec(
             name,
             date_range_vec(start, stop, every, closed, tu, NO_TIMEZONE)?,
         )
         .into_datetime(tu, None),
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 use std::cmp::Ordering;
 use std::ops::Mul;
 
 use chrono::{Datelike, NaiveDate, NaiveDateTime, NaiveTime, Timelike, Weekday};
+use polars_arrow::error::polars_err;
 use polars_arrow::export::arrow::temporal_conversions::{
     timestamp_ms_to_datetime, timestamp_ns_to_datetime, timestamp_us_to_datetime, MILLISECONDS,
 };
 use polars_arrow::time_zone::PolarsTimeZone;
 use polars_core::export::arrow::temporal_conversions::MICROSECONDS;
 use polars_core::prelude::{
     datetime_to_timestamp_ms, datetime_to_timestamp_ns, datetime_to_timestamp_us, polars_bail,
     PolarsResult,
 };
 use polars_core::utils::arrow::temporal_conversions::NANOSECONDS;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 
 use super::calendar::{
-    is_leap_year, last_day_of_month, NS_DAY, NS_HOUR, NS_MICROSECOND, NS_MILLISECOND, NS_MINUTE,
-    NS_SECOND, NS_WEEK,
+    NS_DAY, NS_HOUR, NS_MICROSECOND, NS_MILLISECOND, NS_MINUTE, NS_SECOND, NS_WEEK,
 };
 #[cfg(feature = "timezones")]
 use crate::utils::{localize_datetime, unlocalize_datetime};
 
 #[derive(Copy, Clone, Debug, Eq, PartialEq, Hash)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub struct Duration {
@@ -435,15 +435,17 @@
                 let mut total = (year * 12) + (month as i32 - 1);
                 let remainder = total % self.months as i32;
                 total -= remainder;
 
                 // recreate a new time from the year and month combination
                 let (year, month) = ((total / 12), ((total % 12) + 1) as u32);
 
-                let dt = new_datetime(year, month, 1, 0, 0, 0, 0);
+                let dt = new_datetime(year, month, 1, 0, 0, 0, 0).ok_or(polars_err!(
+                    ComputeError: format!("date '{}-{}-1' does not exist", year, month)
+                ))?;
                 match tz {
                     #[cfg(feature = "timezones")]
                     Some(tz) => Ok(datetime_to_timestamp(localize_datetime(dt, tz)?)),
                     _ => Ok(datetime_to_timestamp(dt)),
                 }
             }
             _ => {
@@ -515,46 +517,40 @@
             let ts = match tz {
                 #[cfg(feature = "timezones")]
                 Some(tz) => unlocalize_datetime(timestamp_to_datetime(t), tz),
                 _ => timestamp_to_datetime(t),
             };
             let mut year = ts.year();
             let mut month = ts.month() as i32;
-            let mut day = ts.day();
+            let day = ts.day();
             year += (months / 12) as i32;
             month += (months % 12) as i32;
 
             // if the month overflowed or underflowed, adjust the year
             // accordingly. Because we add the modulo for the months
             // the year will only adjust by one
             if month > 12 {
                 year += 1;
                 month -= 12;
             } else if month <= 0 {
                 year -= 1;
                 month += 12;
             }
 
-            // Normalize the day if we are past the end of the month.
-            let mut last_day_of_month = last_day_of_month(month);
-            if month == (chrono::Month::February.number_from_month() as i32) && is_leap_year(year) {
-                last_day_of_month += 1;
-            }
-
-            if day > last_day_of_month {
-                day = last_day_of_month
-            }
-
             // Retrieve the original time and construct a data
             // with the new year, month and day
             let hour = ts.hour();
             let minute = ts.minute();
             let sec = ts.second();
             let nsec = ts.nanosecond();
-            let dt = new_datetime(year, month as u32, day, hour, minute, sec, nsec);
+            let dt = new_datetime(year, month as u32, day, hour, minute, sec, nsec).ok_or(
+                polars_err!(
+                    ComputeError: format!("cannot advance '{}' by {} month(s)", ts, d.months)
+                ),
+            )?;
             new_t = match tz {
                 #[cfg(feature = "timezones")]
                 Some(tz) => datetime_to_timestamp(localize_datetime(dt, tz)?),
                 _ => datetime_to_timestamp(dt),
             };
         }
 
@@ -651,19 +647,18 @@
     year: i32,
     month: u32,
     days: u32,
     hour: u32,
     min: u32,
     sec: u32,
     nano: u32,
-) -> NaiveDateTime {
-    let date = NaiveDate::from_ymd_opt(year, month, days).unwrap();
-    let time = NaiveTime::from_hms_nano_opt(hour, min, sec, nano).unwrap();
-
-    NaiveDateTime::new(date, time)
+) -> Option<NaiveDateTime> {
+    let date = NaiveDate::from_ymd_opt(year, month, days)?;
+    let time = NaiveTime::from_hms_nano_opt(hour, min, sec, nano)?;
+    Some(NaiveDateTime::new(date, time))
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
 
     #[test]
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/take_agg.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/take_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files 2% similar despite different names*

```diff
@@ -78,30 +78,30 @@
     }
 }
 
 #[cfg(feature = "timezones")]
 pub fn replace_timezone(
     arr: &PrimitiveArray<i64>,
     tu: TimeUnit,
-    from: String,
-    to: String,
+    from: &str,
+    to: &str,
 ) -> PolarsResult<ArrayRef> {
     Ok(match from.parse::<chrono_tz::Tz>() {
         Ok(from_tz) => match to.parse::<chrono_tz::Tz>() {
             Ok(to_tz) => convert_to_timestamp(from_tz, to_tz, arr, tu)?,
-            Err(_) => match parse_offset(&to) {
+            Err(_) => match parse_offset(to) {
                 Ok(to_tz) => convert_to_timestamp(from_tz, to_tz, arr, tu)?,
-                Err(_) => polars_bail!(ComputeError: "unable to parse time zone: {}", to),
+                Err(_) => polars_bail!(ComputeError: "unable to parse time zone: '{}'", to),
             },
         },
-        Err(_) => match parse_offset(&from) {
+        Err(_) => match parse_offset(from) {
             Ok(from_tz) => match to.parse::<chrono_tz::Tz>() {
                 Ok(to_tz) => convert_to_timestamp(from_tz, to_tz, arr, tu)?,
-                Err(_) => match parse_offset(&to) {
+                Err(_) => match parse_offset(to) {
                     Ok(to_tz) => convert_to_timestamp(from_tz, to_tz, arr, tu)?,
-                    Err(_) => polars_bail!(ComputeError: "unable to parse time zone: {}", to),
+                    Err(_) => polars_bail!(ComputeError: "unable to parse time zone: '{}'", to),
                 },
             },
-            Err(_) => polars_bail!(ComputeError: "unable to parse time zone: {}", from),
+            Err(_) => polars_bail!(ComputeError: "unable to parse time zone: '{}'", from),
         },
     })
 }
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/time_zone.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/time_zone.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files 2% similar despite different names*

```diff
@@ -334,28 +334,26 @@
                 ca.as_date(options.fmt.as_deref(), options.cache)?
                     .into_series()
             } else {
                 ca.as_date_not_exact(options.fmt.as_deref())?.into_series()
             }
         }
         DataType::Datetime(tu, tz) => {
-            let tz = match (tz, tz_aware, options.utc) {
-                (Some(tz), false, false) => Some(tz.clone()),
+            match (tz, tz_aware, options.utc) {
                 (Some(_), true, _) => polars_bail!(
                     ComputeError:
                     "cannot use strptime with both a tz-aware format and a tz-aware dtype, \
                     please drop time zone from the dtype"
                 ),
                 (Some(_), _, true) => polars_bail!(
                     ComputeError:
-                    "cannot use strptime with both 'utc=True' and tz-aware datetime, \
+                    "cannot use strptime with both 'utc=True' and tz-aware dtype, \
                     please drop time zone from the dtype"
                 ),
-                (None, _, true) => Some("UTC".to_string()),
-                (None, _, false) => None,
+                _ => (),
             };
             if options.exact {
                 ca.as_datetime(
                     options.fmt.as_deref(),
                     *tu,
                     options.cache,
                     tz_aware,
@@ -376,15 +374,21 @@
                 .into_series()
         }
         dt => polars_bail!(ComputeError: "not implemented for dtype {}", dt),
     };
     if options.strict {
         polars_ensure!(
             out.null_count() == ca.null_count(),
-            ComputeError: "strict conversion to dates failed, try setting strict=False",
+            ComputeError:
+            "strict conversion to date(time)s failed.\n\
+            \n\
+            You might want to try:\n\
+            - setting `strict=False`,\n\
+            - explicitly specifying a `fmt`,\n\
+            - setting `utf=True` (if you are parsing datetimes with multiple offsets)."
         );
     }
     Ok(out.into_series())
 }
 
 #[cfg(feature = "concat_str")]
 pub(super) fn concat(s: &Series, delimiter: &str) -> PolarsResult<Series> {
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/functions.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files 3% similar despite different names*

```diff
@@ -91,16 +91,21 @@
                     | Last(expr) => {
                         // default context because `col()` would return a list in aggregation context
                         arena.get(*expr).to_field(schema, Context::Default, arena)
                     }
                     Sum(expr) => {
                         let mut field =
                             arena.get(*expr).to_field(schema, Context::Default, arena)?;
-                        if matches!(field.data_type(), UInt8 | Int8 | Int16 | UInt16) {
-                            field.coerce(DataType::Int64);
+                        let dt = match field.data_type() {
+                            Boolean => Some(IDX_DTYPE),
+                            UInt8 | Int8 | Int16 | UInt16 => Some(Int64),
+                            _ => None,
+                        };
+                        if let Some(dt) = dt {
+                            field.coerce(dt);
                         }
                         Ok(field)
                     }
                     Median(expr) => {
                         let mut field =
                             arena.get(*expr).to_field(schema, Context::Default, arena)?;
                         float_type(&mut field);
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -66,39 +66,62 @@
 
 #[derive(Debug)]
 pub enum ErrorState {
     NotYetEncountered { err: PolarsError },
     AlreadyEncountered { prev_err_msg: String },
 }
 
-#[derive(Debug, Clone)]
+impl std::fmt::Display for ErrorState {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        match self {
+            ErrorState::NotYetEncountered { err } => write!(f, "NotYetEncountered({err})")?,
+            ErrorState::AlreadyEncountered { prev_err_msg } => {
+                write!(f, "AlreadyEncountered({prev_err_msg})")?
+            }
+        };
+
+        Ok(())
+    }
+}
+
+#[derive(Clone)]
 pub struct ErrorStateSync(Arc<Mutex<ErrorState>>);
 
 impl std::ops::Deref for ErrorStateSync {
     type Target = Arc<Mutex<ErrorState>>;
 
     fn deref(&self) -> &Self::Target {
         &self.0
     }
 }
 
+impl std::fmt::Debug for ErrorStateSync {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        write!(f, "ErrorStateSync({})", &*self.0.lock().unwrap())
+    }
+}
+
 impl ErrorStateSync {
     fn take(&self) -> PolarsError {
-        let mut err = self.0.lock().unwrap();
-        match &*err {
+        let mut curr_err = self.0.lock().unwrap();
+
+        match &*curr_err {
             ErrorState::NotYetEncountered { err: polars_err } => {
-                let msg = format!("{polars_err:?}");
-                let err = std::mem::replace(
-                    &mut *err,
-                    ErrorState::AlreadyEncountered { prev_err_msg: msg },
+                // Need to finish using `polars_err` here so that NLL considers `err` dropped
+                let prev_err_msg = polars_err.to_string();
+                // Place AlreadyEncountered in `self` for future users of `self`
+                let prev_err = std::mem::replace(
+                    &mut *curr_err,
+                    ErrorState::AlreadyEncountered { prev_err_msg },
                 );
-                let ErrorState::NotYetEncountered { err } = err else {
-                    unreachable!("polars bug in LogicalPlan error handling")
-                };
-                err
+                // Since we're in this branch, we know err was a NotYetEncountered
+                match prev_err {
+                    ErrorState::NotYetEncountered { err } => err,
+                    ErrorState::AlreadyEncountered { .. } => unreachable!(),
+                }
             }
             ErrorState::AlreadyEncountered { prev_err_msg } => {
                 polars_err!(
                     ComputeError: "LogicalPlan already failed with error: '{}'", prev_err_msg,
                 )
             }
         }
```

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.17.1/local_dependencies/polars-error/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.17.1/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.17.1/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/Cargo.toml` & `polars_lts_cpu-0.17.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.17.0"
+version = "0.17.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_lts_cpu-0.17.0/LICENSE` & `polars_lts_cpu-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/Makefile` & `polars_lts_cpu-0.17.1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 .PHONY: fmt
 fmt: .venv  ## Run autoformatting and linting
 	$(VENV_BIN)/black .
 	$(VENV_BIN)/blackdoc .
 	$(VENV_BIN)/ruff .
 	$(VENV_BIN)/typos ..
-	$(VENV_BIN)/python scripts/check_decorators_stacklevels.py
+	$(VENV_BIN)/python scripts/check_stacklevels.py
 	cargo fmt --all
 	-dprint fmt
 	-$(VENV_BIN)/mypy
 
 .PHONY: clippy
 clippy:  ## Run clippy
 	cargo clippy -- -D warnings
```

### Comparing `polars_lts_cpu-0.17.0/README.md` & `polars_lts_cpu-0.17.1/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/build.rs` & `polars_lts_cpu-0.17.1/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/Makefile` & `polars_lts_cpu-0.17.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.17.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.17.1/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/conf.py` & `polars_lts_cpu-0.17.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/api.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/config.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/functions.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/io.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/docs/source/reference/testing.rst` & `polars_lts_cpu-0.17.1/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/__init__.py` & `polars_lts_cpu-0.17.1/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/api.py` & `polars_lts_cpu-0.17.1/polars/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from functools import reduce
 from operator import or_
 from typing import TYPE_CHECKING, Callable, TypeVar
 from warnings import warn
 
 from polars import internals as pli
+from polars.utils.various import find_stacklevel
 
 if TYPE_CHECKING:
     from polars.dataframe import DataFrame
     from polars.expr import Expr
     from polars.lazyframe import LazyFrame
     from polars.series import Series
 
@@ -57,15 +58,15 @@
     def namespace(ns_class: type[NS]) -> type[NS]:
         if name in _reserved_namespaces:
             raise AttributeError(f"Cannot override reserved namespace {name!r}")
         elif hasattr(cls, name):
             warn(
                 f"Overriding existing custom namespace {name!r} (on {cls.__name__})",
                 UserWarning,
-                stacklevel=2,
+                stacklevel=find_stacklevel(),
             )
 
         setattr(cls, name, NameSpace(name, ns_class))
         cls._accessors.add(name)
         return ns_class
 
     return namespace
```

### Comparing `polars_lts_cpu-0.17.0/polars/config.py` & `polars_lts_cpu-0.17.1/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/convert.py` & `polars_lts_cpu-0.17.1/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/dataframe/_html.py` & `polars_lts_cpu-0.17.1/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/dataframe/frame.py` & `polars_lts_cpu-0.17.1/polars/dataframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 from polars.utils._wrap import wrap_ldf, wrap_s
 from polars.utils.convert import _timedelta_to_pl_duration
 from polars.utils.decorators import deprecated_alias
 from polars.utils.meta import get_index_type
 from polars.utils.various import (
     _prepare_row_count_args,
     _process_null_values,
+    find_stacklevel,
     handle_projection_columns,
     is_bool_sequence,
     is_int_sequence,
     is_str_sequence,
     normalise_filepath,
     parse_version,
     range_to_slice,
@@ -6062,15 +6063,17 @@
         >>> df = pl.DataFrame(
         ...     {
         ...         "foo": ["one", "one", "one", "two", "two", "two"],
         ...         "bar": ["A", "B", "C", "A", "B", "C"],
         ...         "baz": [1, 2, 3, 4, 5, 6],
         ...     }
         ... )
-        >>> df.pivot(values="baz", index="foo", columns="bar")
+        >>> df.pivot(
+        ...     values="baz", index="foo", columns="bar", aggregate_function="first"
+        ... )
         shape: (2, 4)
         ┌─────┬─────┬─────┬─────┐
         │ foo ┆ A   ┆ B   ┆ C   │
         │ --- ┆ --- ┆ --- ┆ --- │
         │ str ┆ i64 ┆ i64 ┆ i64 │
         ╞═════╪═════╪═════╪═════╡
         │ one ┆ 1   ┆ 2   ┆ 3   │
@@ -6087,15 +6090,15 @@
 
         if aggregate_function is no_default:
             warnings.warn(
                 "In a future version of polars, the default `aggregate_function` "
                 "will change from `'first'` to `None`. Please pass `'first'` to keep the "
                 "current behaviour, or `None` to accept the new one.",
                 DeprecationWarning,
-                stacklevel=4,
+                stacklevel=find_stacklevel(),
             )
             aggregate_function = "first"
 
         if isinstance(aggregate_function, str):
             if aggregate_function == "first":
                 aggregate_expr = F.element().first()._pyexpr
             elif aggregate_function == "sum":
```

### Comparing `polars_lts_cpu-0.17.0/polars/dataframe/groupby.py` & `polars_lts_cpu-0.17.1/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/datatypes/__init__.py` & `polars_lts_cpu-0.17.1/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/datatypes/classes.py` & `polars_lts_cpu-0.17.1/polars/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/datatypes/constants.py` & `polars_lts_cpu-0.17.1/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/datatypes/constructor.py` & `polars_lts_cpu-0.17.1/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/datatypes/convert.py` & `polars_lts_cpu-0.17.1/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/dependencies.py` & `polars_lts_cpu-0.17.1/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/exceptions.py` & `polars_lts_cpu-0.17.1/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/expr/binary.py` & `polars_lts_cpu-0.17.1/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/expr/categorical.py` & `polars_lts_cpu-0.17.1/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/expr/datetime.py` & `polars_lts_cpu-0.17.1/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/expr/expr.py` & `polars_lts_cpu-0.17.1/polars/expr/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from polars.expr.meta import ExprMetaNameSpace
 from polars.expr.string import ExprStringNameSpace
 from polars.expr.struct import ExprStructNameSpace
 from polars.utils._parse_expr_input import expr_to_lit_or_expr, selection_to_pyexpr_list
 from polars.utils.convert import _timedelta_to_pl_duration
 from polars.utils.decorators import deprecated_alias
 from polars.utils.meta import threadpool_size
-from polars.utils.various import sphinx_accessor
+from polars.utils.various import find_stacklevel, sphinx_accessor
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import arg_where as py_arg_where
     from polars.polars import reduce as pyreduce
 if TYPE_CHECKING:
     import sys
 
@@ -3251,16 +3251,16 @@
 
         Parameters
         ----------
         function
             Lambda/ function to apply.
         return_dtype
             Dtype of the output Series.
-            If not set, polars will assume that
-            the dtype remains unchanged.
+            If not set, the dtype will be
+            ``polars.Unknown``.
         skip_nulls
             Don't apply the function over values
             that contain nulls. This is faster.
         pass_name
             Pass the Series name to the custom function
             This is more expensive.
         strategy : {'thread_local', 'threading'}
@@ -3435,15 +3435,15 @@
 
         """
         warnings.warn(
             "`Series/Expr.explode()` is deprecated in favor of the identical method"
             " under the list and string namespaces. Use `.arr.explode()` or"
             " `.str.explode()` instead.",
             DeprecationWarning,
-            stacklevel=2,
+            stacklevel=find_stacklevel(),
         )
         return self._from_pyexpr(self._pyexpr.explode())
 
     def take_every(self, n: int) -> Self:
         """
         Take every nth value in the Series and return as a new Series.
 
@@ -3461,15 +3461,15 @@
         │ 4   │
         │ 7   │
         └─────┘
 
         """
         return self._from_pyexpr(self._pyexpr.take_every(n))
 
-    def head(self, n: int = 10) -> Self:
+    def head(self, n: int | Expr = 10) -> Self:
         """
         Get the first `n` rows.
 
         Parameters
         ----------
         n
             Number of rows to return.
@@ -3486,17 +3486,17 @@
         ╞═════╡
         │ 1   │
         │ 2   │
         │ 3   │
         └─────┘
 
         """
-        return self._from_pyexpr(self._pyexpr.head(n))
+        return self.slice(0, n)
 
-    def tail(self, n: int = 10) -> Self:
+    def tail(self, n: int | Expr = 10) -> Self:
         """
         Get the last `n` rows.
 
         Parameters
         ----------
         n
             Number of rows to return.
@@ -3513,17 +3513,18 @@
         ╞═════╡
         │ 5   │
         │ 6   │
         │ 7   │
         └─────┘
 
         """
-        return self._from_pyexpr(self._pyexpr.tail(n))
+        offset = -expr_to_lit_or_expr(n, str_to_lit=False)
+        return self.slice(offset, n)
 
-    def limit(self, n: int = 10) -> Self:
+    def limit(self, n: int | Expr = 10) -> Self:
         """
         Get the first `n` rows (alias for :func:`Expr.head`).
 
         Parameters
         ----------
         n
             Number of rows to return.
@@ -6212,15 +6213,15 @@
         seed
             Seed for the random number generator. If set to None (default), a random
             seed is generated using the ``random`` module.
 
         Examples
         --------
         >>> df = pl.DataFrame({"a": [1, 2, 3]})
-        >>> df.select(pl.col("a").sample(frac=1.0, with_replacement=True, seed=1))
+        >>> df.select(pl.col("a").sample(fraction=1.0, with_replacement=True, seed=1))
         shape: (3, 1)
         ┌─────┐
         │ a   │
         │ --- │
         │ i64 │
         ╞═════╡
         │ 3   │
```

### Comparing `polars_lts_cpu-0.17.0/polars/expr/list.py` & `polars_lts_cpu-0.17.1/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/expr/meta.py` & `polars_lts_cpu-0.17.1/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/expr/string.py` & `polars_lts_cpu-0.17.1/polars/expr/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Time,
     is_polars_dtype,
     py_type_to_dtype,
 )
 from polars.utils import no_default
 from polars.utils._parse_expr_input import expr_to_lit_or_expr
 from polars.utils._wrap import wrap_expr
+from polars.utils.various import find_stacklevel
 
 if TYPE_CHECKING:
     from polars.expr.expr import Expr
     from polars.type_aliases import PolarsDataType, PolarsTemporalType, TransferEncoding
     from polars.utils import NoDefault
 
 
@@ -125,15 +126,15 @@
         if tz_aware is no_default:
             tz_aware = False
         else:
             warnings.warn(
                 "`tz_aware` is now auto-inferred from `fmt` and will be removed "
                 "in a future version. You can safely drop this argument.",
                 category=DeprecationWarning,
-                stacklevel=2,
+                stacklevel=find_stacklevel(),
             )
 
         if datatype == Date:
             return wrap_expr(self._pyexpr.str_parse_date(fmt, strict, exact, cache))
         elif datatype == Datetime:
             time_unit = datatype.time_unit  # type: ignore[union-attr]
             time_zone = datatype.time_zone  # type: ignore[union-attr]
```

### Comparing `polars_lts_cpu-0.17.0/polars/expr/struct.py` & `polars_lts_cpu-0.17.1/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/functions/__init__.py` & `polars_lts_cpu-0.17.1/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/functions/eager.py` & `polars_lts_cpu-0.17.1/polars/functions/eager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from polars.utils._wrap import wrap_df, wrap_expr, wrap_ldf, wrap_s
 from polars.utils.convert import (
     _datetime_to_pl_timestamp,
     _timedelta_to_pl_duration,
     _tzinfo_to_str,
 )
 from polars.utils.decorators import deprecated_alias
+from polars.utils.various import find_stacklevel
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import concat_df as _concat_df
     from polars.polars import concat_lf as _concat_lf
     from polars.polars import concat_series as _concat_series
     from polars.polars import py_date_range as _py_date_range
     from polars.polars import py_date_range_lazy as _py_date_range_lazy
@@ -75,30 +76,30 @@
     >>> df = pl.DataFrame(
     ...     {
     ...         "foo": [1, 2],
     ...         "bar": [3, 4],
     ...         "ham": ["a", "b"],
     ...     }
     ... )
-    >>> pl.get_dummies(df.to_dummies(), columns=["foo", "bar"])
+    >>> pl.get_dummies(df.to_dummies(), columns=["foo", "bar"])  # doctest: +SKIP
     shape: (2, 6)
     ┌───────┬───────┬───────┬───────┬───────┬───────┐
     │ foo_1 ┆ foo_2 ┆ bar_3 ┆ bar_4 ┆ ham_a ┆ ham_b │
     │ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---   │
     │ u8    ┆ u8    ┆ u8    ┆ u8    ┆ u8    ┆ u8    │
     ╞═══════╪═══════╪═══════╪═══════╪═══════╪═══════╡
     │ 1     ┆ 0     ┆ 1     ┆ 0     ┆ 1     ┆ 0     │
     │ 0     ┆ 1     ┆ 0     ┆ 1     ┆ 0     ┆ 1     │
     └───────┴───────┴───────┴───────┴───────┴───────┘
 
     """
     warnings.warn(
         "`pl.get_dummies(df)` has been deprecated; use `df.to_dummies()`",
         category=DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     return df.to_dummies(columns=columns, separator=separator)
 
 
 @overload
 def concat(
     items: Iterable[DataFrame],
@@ -461,14 +462,33 @@
     Series: '' [datetime[μs, America/New_York]]
     [
         2022-01-01 00:00:00 EST
         2022-02-01 00:00:00 EST
         2022-03-01 00:00:00 EST
     ]
 
+    Combine with ``offset_by`` to get the last day of the month:
+
+    >>> (
+    ...     pl.date_range(
+    ...         datetime(2022, 1, 1),
+    ...         datetime(2022, 3, 1),
+    ...         "1mo",
+    ...     )
+    ...     .dt.offset_by("1mo")
+    ...     .dt.offset_by("-1d")
+    ... )
+    shape: (3,)
+    Series: '' [datetime[μs]]
+    [
+        2022-01-31 00:00:00
+        2022-02-28 00:00:00
+        2022-03-31 00:00:00
+    ]
+
     """
     if name is None:
         name = ""
     if isinstance(interval, timedelta):
         interval = _timedelta_to_pl_duration(interval)
     elif " " in interval:
         interval = interval.replace(" ", "")
@@ -557,15 +577,15 @@
     --------
     This functionality is experimental and may change without it being considered a
     breaking change.
 
     Examples
     --------
     >>> a = pl.Series("a", [v / 10 for v in range(-30, 30, 5)])
-    >>> pl.cut(a, bins=[-1, 1])
+    >>> pl.cut(a, bins=[-1, 1])  # doctest: +SKIP
     shape: (12, 3)
     ┌──────┬─────────────┬──────────────┐
     │ a    ┆ break_point ┆ category     │
     │ ---  ┆ ---         ┆ ---          │
     │ f64  ┆ f64         ┆ cat          │
     ╞══════╪═════════════╪══════════════╡
     │ -3.0 ┆ -1.0        ┆ (-inf, -1.0] │
@@ -579,15 +599,15 @@
     │ 2.5  ┆ inf         ┆ (1.0, inf]   │
     └──────┴─────────────┴──────────────┘
 
     """
     warnings.warn(
         "`pl.cut(series)` has been deprecated; use `series.cut()`",
         category=DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     return s.cut(bins, labels, break_point_label, category_label)
 
 
 @overload
 def align_frames(
     *frames: DataFrame,
```

### Comparing `polars_lts_cpu-0.17.0/polars/functions/lazy.py` & `polars_lts_cpu-0.17.1/polars/functions/lazy.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from polars.utils._wrap import wrap_df, wrap_expr
 from polars.utils.convert import (
     _datetime_to_pl_timestamp,
     _time_to_pl_time,
     _timedelta_to_pl_timedelta,
 )
 from polars.utils.decorators import deprecated_alias
+from polars.utils.various import find_stacklevel
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import arange as pyarange
     from polars.polars import arg_sort_by as py_arg_sort_by
     from polars.polars import arg_where as py_arg_where
     from polars.polars import as_struct as _as_struct
     from polars.polars import coalesce_exprs as _coalesce_exprs
@@ -1388,28 +1389,28 @@
     See Also
     --------
     corr
 
     Examples
     --------
     >>> df = pl.DataFrame({"a": [1, 8, 3], "b": [4, 5, 2], "c": ["foo", "bar", "foo"]})
-    >>> df.select(pl.spearman_rank_corr("a", "b"))
+    >>> df.select(pl.spearman_rank_corr("a", "b"))  # doctest: +SKIP
     shape: (1, 1)
     ┌─────┐
     │ a   │
     │ --- │
     │ f64 │
     ╞═════╡
     │ 0.5 │
     └─────┘
     """
     warnings.warn(
         "`spearman_rank_corr()` is deprecated in favor of `corr()`",
         DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     if isinstance(a, str):
         a = col(a)
     if isinstance(b, str):
         b = col(b)
     return wrap_expr(pyspearman_rank_corr(a._pyexpr, b._pyexpr, ddof, propagate_nans))
 
@@ -1435,28 +1436,28 @@
     See Also
     --------
     corr
 
     Examples
     --------
     >>> df = pl.DataFrame({"a": [1, 8, 3], "b": [4, 5, 2], "c": ["foo", "bar", "foo"]})
-    >>> df.select(pl.pearson_corr("a", "b"))
+    >>> df.select(pl.pearson_corr("a", "b"))  # doctest: +SKIP
     shape: (1, 1)
     ┌──────────┐
     │ a        │
     │ ---      │
     │ f64      │
     ╞══════════╡
     │ 0.544705 │
     └──────────┘
     """
     warnings.warn(
         "`pearson_corr()` is deprecated in favor of `corr()`",
         DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     if isinstance(a, str):
         a = col(a)
     if isinstance(b, str):
         b = col(b)
     return wrap_expr(pypearson_corr(a._pyexpr, b._pyexpr, ddof))
```

### Comparing `polars_lts_cpu-0.17.0/polars/functions/whenthen.py` & `polars_lts_cpu-0.17.1/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/__init__.py` & `polars_lts_cpu-0.17.1/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/_utils.py` & `polars_lts_cpu-0.17.1/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/avro.py` & `polars_lts_cpu-0.17.1/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/csv/_utils.py` & `polars_lts_cpu-0.17.1/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.17.1/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/csv/functions.py` & `polars_lts_cpu-0.17.1/polars/io/csv/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         Try to keep reading lines if some lines yield errors.
         Before using this option, try to increase the number of lines used for schema
         inference with e.g ``infer_schema_length=10000`` or override automatic dtype
         inference for specific columns with the ``dtypes`` option or use
         ``infer_schema_length=0`` to read all columns as ``pl.Utf8`` to check which
         values might cause an issue.
     try_parse_dates
-        Try to automatically parse dates. Most ISO8601-like time zone naive formats can
+        Try to automatically parse dates. Most ISO8601-like formats can
         be inferred, as well as a handful of others. If this does not succeed,
         the column remains of data type ``pl.Utf8``.
         If ``use_pyarrow=True``, dates will always be parsed.
     n_threads
         Number of threads to use in csv parsing.
         Defaults to the number of physical cpu's of your system.
     infer_schema_length
@@ -463,15 +463,15 @@
         By default a missing value is considered to be null; if you would prefer missing
         utf8 values to be treated as the empty string you can set this param True.
     ignore_errors
         Try to keep reading lines if some lines yield errors.
         First try ``infer_schema_length=0`` to read all columns as
         ``pl.Utf8`` to check which values might cause an issue.
     try_parse_dates
-        Try to automatically parse dates. Most ISO8601-like time zone naive formats can
+        Try to automatically parse dates. Most ISO8601-like formats can
         be inferred, as well as a handful of others. If this does not succeed,
         the column remains of data type ``pl.Utf8``.
     n_threads
         Number of threads to use in csv parsing.
         Defaults to the number of physical cpu's of your system.
     infer_schema_length
         Maximum number of lines to read to infer schema.
@@ -771,15 +771,15 @@
         Skip this number of rows when the header is parsed.
     row_count_name
         If not None, this will insert a row count column with the given name into
         the DataFrame.
     row_count_offset
         Offset to start the row_count column (only used if the name is set).
     try_parse_dates
-        Try to automatically parse dates. Most ISO8601-like time zone naive formats
+        Try to automatically parse dates. Most ISO8601-like formats
         can be inferred, as well as a handful of others. If this does not succeed,
         the column remains of data type ``pl.Utf8``.
     eol_char
         Single byte end of line character
     new_columns
         Provide an explicit list of string column names to use (for example, when
         scanning a headerless CSV file). Note that unlike ``read_csv`` it is considered
```

### Comparing `polars_lts_cpu-0.17.0/polars/io/database.py` & `polars_lts_cpu-0.17.1/polars/io/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING, Any
 
 from polars.convert import from_arrow
+from polars.utils.various import find_stacklevel
 
 if TYPE_CHECKING:
     from polars.dataframe import DataFrame
     from polars.type_aliases import DbReadEngine
 
 
 def read_database(
@@ -186,15 +187,15 @@
     >>> pl.read_sql(queries, uri)  # doctest: +SKIP
 
     """
     warnings.warn(
         "`read_sql` has been renamed; this"
         " redirect is temporary, please use `read_database` instead",
         category=DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     return read_database(
         query=query,
         connection_uri=connection_uri,
         partition_on=partition_on,
         partition_range=partition_range,
         partition_num=partition_num,
```

### Comparing `polars_lts_cpu-0.17.0/polars/io/delta.py` & `polars_lts_cpu-0.17.1/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.17.1/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/excel/functions.py` & `polars_lts_cpu-0.17.1/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.17.1/polars/io/parquet/anonymous_scan.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING, Any
 
-import polars.io.ipc
+import polars.io.parquet
 from polars import internals as pli
 from polars.dependencies import pickle
 from polars.io._utils import _prepare_file_arg
 
 if TYPE_CHECKING:
     from polars.dataframe import DataFrame
     from polars.lazyframe import LazyFrame
 
 
-def _scan_ipc_fsspec(
+def _scan_parquet_fsspec(
     source: str,
     storage_options: dict[str, object] | None = None,
 ) -> LazyFrame:
-    func = partial(_scan_ipc_impl, source, storage_options=storage_options)
+    func = partial(_scan_parquet_impl, source, storage_options=storage_options)
     func_serialized = pickle.dumps(func)
 
     storage_options = storage_options or {}
     with _prepare_file_arg(source, **storage_options) as data:
-        schema = polars.io.ipc.read_ipc_schema(data)
+        schema = polars.io.parquet.read_parquet_schema(data)
 
     return pli.LazyFrame._scan_python_function(schema, func_serialized)
 
 
-def _scan_ipc_impl(  # noqa: D417
-    source: str, columns: list[str] | None, **kwargs: Any
+def _scan_parquet_impl(  # noqa: D417
+    source: str,
+    columns: list[str] | None,
+    predicate: str | None,
+    n_rows: int | None,
+    **kwargs: Any,
 ) -> DataFrame:
     """
     Take the projected columns and materialize an arrow table.
 
     Parameters
     ----------
-    uri
+    source
         Source URI
     columns
         Columns that are projected
 
     """
     import polars as pl
 
-    return pl.read_ipc(source, columns=columns, **kwargs)
+    return pl.read_parquet(source, columns=columns, n_rows=n_rows, **kwargs)
```

### Comparing `polars_lts_cpu-0.17.0/polars/io/ipc/functions.py` & `polars_lts_cpu-0.17.1/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/json.py` & `polars_lts_cpu-0.17.1/polars/io/json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/ndjson.py` & `polars_lts_cpu-0.17.1/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.17.1/polars/io/ipc/anonymous_scan.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING, Any
 
-import polars.io.parquet
+import polars.io.ipc
 from polars import internals as pli
 from polars.dependencies import pickle
 from polars.io._utils import _prepare_file_arg
 
 if TYPE_CHECKING:
     from polars.dataframe import DataFrame
     from polars.lazyframe import LazyFrame
 
 
-def _scan_parquet_fsspec(
+def _scan_ipc_fsspec(
     source: str,
     storage_options: dict[str, object] | None = None,
 ) -> LazyFrame:
-    func = partial(_scan_parquet_impl, source, storage_options=storage_options)
+    func = partial(_scan_ipc_impl, source, storage_options=storage_options)
     func_serialized = pickle.dumps(func)
 
     storage_options = storage_options or {}
     with _prepare_file_arg(source, **storage_options) as data:
-        schema = polars.io.parquet.read_parquet_schema(data)
+        schema = polars.io.ipc.read_ipc_schema(data)
 
     return pli.LazyFrame._scan_python_function(schema, func_serialized)
 
 
-def _scan_parquet_impl(  # noqa: D417
-    uri: str, columns: list[str] | None, **kwargs: Any
+def _scan_ipc_impl(  # noqa: D417
+    source: str,
+    columns: list[str] | None,
+    predicate: str | None,
+    n_rows: int | None,
+    **kwargs: Any,
 ) -> DataFrame:
     """
     Take the projected columns and materialize an arrow table.
 
     Parameters
     ----------
-    uri
+    source
         Source URI
     columns
         Columns that are projected
 
     """
     import polars as pl
 
-    return pl.read_parquet(uri, columns=columns, **kwargs)
+    return pl.read_ipc(source, columns=columns, n_rows=n_rows, **kwargs)
```

### Comparing `polars_lts_cpu-0.17.0/polars/io/parquet/functions.py` & `polars_lts_cpu-0.17.1/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.17.1/polars/io/pyarrow_dataset/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING
 
 from polars.io.pyarrow_dataset.anonymous_scan import _scan_pyarrow_dataset
+from polars.utils.various import find_stacklevel
 
 if TYPE_CHECKING:
     from polars.dependencies import pyarrow as pa
     from polars.lazyframe import LazyFrame
 
 
 def scan_pyarrow_dataset(
@@ -95,10 +96,10 @@
     └───────┴────────┴────────────┘
 
     """
     warnings.warn(
         "`scan_ds` has been renamed; this"
         " redirect is temporary, please use `scan_pyarrow_dataset` instead",
         category=DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     return scan_pyarrow_dataset(ds, allow_pyarrow_filter=allow_pyarrow_filter)
```

### Comparing `polars_lts_cpu-0.17.0/polars/lazyframe/frame.py` & `polars_lts_cpu-0.17.1/polars/lazyframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from polars.utils._parse_expr_input import expr_to_lit_or_expr, selection_to_pyexpr_list
 from polars.utils._wrap import wrap_df
 from polars.utils.convert import _timedelta_to_pl_duration
 from polars.utils.various import (
     _in_notebook,
     _prepare_row_count_args,
     _process_null_values,
+    find_stacklevel,
     normalise_filepath,
 )
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import PyLazyFrame
 
 
@@ -498,15 +499,15 @@
         schema: pa.schema | dict[str, PolarsDataType],
         scan_fn: bytes,
         pyarrow: bool = False,
     ) -> Self:
         self = cls.__new__(cls)
         if isinstance(schema, dict):
             self._ldf = PyLazyFrame.scan_from_python_function_pl_schema(
-                [(name, dt) for name, dt in schema.items()], scan_fn, pyarrow
+                list(schema.items()), scan_fn, pyarrow
             )
         else:
             self._ldf = PyLazyFrame.scan_from_python_function_arrow_schema(
                 list(schema), scan_fn, pyarrow
             )
         return self
 
@@ -929,15 +930,15 @@
         ...     "a"
         ... ).describe_plan()  # doctest: +SKIP
 
         """
         warnings.warn(
             "`LazyFrame.describe_plan` has been deprecated; Please use `LazyFrame.explain` instead",
             category=DeprecationWarning,
-            stacklevel=2,
+            stacklevel=find_stacklevel(),
         )
         if optimized:
             ldf = self._ldf.optimization_toggle(
                 type_coercion,
                 predicate_pushdown,
                 projection_pushdown,
                 simplify_expression,
@@ -959,15 +960,15 @@
         common_subplan_elimination: bool = True,
         streaming: bool = False,
     ) -> str:
         """Create a string representation of the optimized query plan."""
         warnings.warn(
             "`LazyFrame.describe_optimized_plan` has been deprecated; Please use `LazyFrame.explain` instead",
             category=DeprecationWarning,
-            stacklevel=2,
+            stacklevel=find_stacklevel(),
         )
         ldf = self._ldf.optimization_toggle(
             type_coercion,
             predicate_pushdown,
             projection_pushdown,
             simplify_expression,
             slice_pushdown,
```

### Comparing `polars_lts_cpu-0.17.0/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.17.1/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/_numpy.py` & `polars_lts_cpu-0.17.1/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/binary.py` & `polars_lts_cpu-0.17.1/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/categorical.py` & `polars_lts_cpu-0.17.1/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/datetime.py` & `polars_lts_cpu-0.17.1/polars/series/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/list.py` & `polars_lts_cpu-0.17.1/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/series.py` & `polars_lts_cpu-0.17.1/polars/series/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1153,76 +1153,79 @@
         -------
         Dictionary with summary statistics of a Series.
 
         Examples
         --------
         >>> series_num = pl.Series([1, 2, 3, 4, 5])
         >>> series_num.describe()
-        shape: (6, 2)
+        shape: (7, 2)
         ┌────────────┬──────────┐
         │ statistic  ┆ value    │
         │ ---        ┆ ---      │
         │ str        ┆ f64      │
         ╞════════════╪══════════╡
-        │ min        ┆ 1.0      │
-        │ max        ┆ 5.0      │
+        │ count      ┆ 5.0      │
         │ null_count ┆ 0.0      │
         │ mean       ┆ 3.0      │
         │ std        ┆ 1.581139 │
-        │ count      ┆ 5.0      │
+        │ min        ┆ 1.0      │
+        │ max        ┆ 5.0      │
+        │ median     ┆ 3.0      │
         └────────────┴──────────┘
 
         >>> series_str = pl.Series(["a", "a", None, "b", "c"])
         >>> series_str.describe()
         shape: (3, 2)
         ┌────────────┬───────┐
         │ statistic  ┆ value │
         │ ---        ┆ ---   │
         │ str        ┆ i64   │
         ╞════════════╪═══════╡
-        │ unique     ┆ 4     │
-        │ null_count ┆ 1     │
         │ count      ┆ 5     │
+        │ null_count ┆ 1     │
+        │ unique     ┆ 4     │
         └────────────┴───────┘
 
         """
         stats: dict[str, PythonLiteral | None]
 
         if self.len() == 0:
             raise ValueError("Series must contain at least one value")
         elif self.is_numeric():
             s = self.cast(Float64)
             stats = {
-                "min": s.min(),
-                "max": s.max(),
+                "count": s.len(),
                 "null_count": s.null_count(),
                 "mean": s.mean(),
                 "std": s.std(),
-                "count": s.len(),
+                "min": s.min(),
+                "max": s.max(),
+                "median": s.median(),
             }
         elif self.is_boolean():
             stats = {
-                "sum": self.sum(),
-                "null_count": self.null_count(),
                 "count": self.len(),
+                "null_count": self.null_count(),
+                "sum": self.sum(),
             }
         elif self.is_utf8():
             stats = {
-                "unique": len(self.unique()),
-                "null_count": self.null_count(),
                 "count": self.len(),
+                "null_count": self.null_count(),
+                "unique": len(self.unique()),
             }
         elif self.is_temporal():
             # we coerce all to string, because a polars column
             # only has a single dtype and dates: datetime and count: int don't match
             stats = {
+                "count": str(self.len()),
+                "null_count": str(self.null_count()),
                 "min": str(self.dt.min()),
                 "max": str(self.dt.max()),
-                "null_count": str(self.null_count()),
-                "count": str(self.len()),
+                "median": str(self.dt.median()),
             }
         else:
             raise TypeError("This type is not supported")
 
         return pli.DataFrame({"statistic": stats.keys(), "value": stats.values()})
 
     def sum(self) -> int | float:
```

### Comparing `polars_lts_cpu-0.17.0/polars/series/string.py` & `polars_lts_cpu-0.17.1/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/struct.py` & `polars_lts_cpu-0.17.1/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/series/utils.py` & `polars_lts_cpu-0.17.1/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/slice.py` & `polars_lts_cpu-0.17.1/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/sql/context.py` & `polars_lts_cpu-0.17.1/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/string_cache.py` & `polars_lts_cpu-0.17.1/polars/string_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import contextlib
 import warnings
 from typing import TYPE_CHECKING
 
+from polars.utils.various import find_stacklevel
+
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import enable_string_cache as _enable_string_cache
     from polars.polars import using_string_cache as _using_string_cache
 
 if TYPE_CHECKING:
     from types import TracebackType
 
@@ -127,15 +129,15 @@
     .. deprecated:: 0.17.0
 
     """
     warnings.warn(
         "`toggle_string_cache` has been renamed; this"
         " redirect is temporary, please use `enable_string_cache` instead",
         category=DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     enable_string_cache(toggle)
 
 
 def using_string_cache() -> bool:
     """Return the current state of the global string cache (enabled/disabled)."""
     return _using_string_cache()
```

### Comparing `polars_lts_cpu-0.17.0/polars/testing/_parametric.py` & `polars_lts_cpu-0.17.1/polars/testing/_parametric.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/testing/_private.py` & `polars_lts_cpu-0.17.1/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/testing/asserts.py` & `polars_lts_cpu-0.17.1/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/testing/parametric.py` & `polars_lts_cpu-0.17.1/polars/testing/parametric.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/type_aliases.py` & `polars_lts_cpu-0.17.1/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/__init__.py` & `polars_lts_cpu-0.17.1/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/_construction.py` & `polars_lts_cpu-0.17.1/polars/utils/_construction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1335,15 +1335,15 @@
     elif df.index.equals(RangeIndex(start=0, stop=len(df), step=1)):
         # is default: simple range index
         return True
     else:
         # finally, is the index _equivalent_ to a default unnamed
         # integer index with frame data that was previously sorted
         return (
-            df.index.dtype == "int"  # type: ignore[comparison-overlap]
+            str(df.index.dtype).startswith("int")
             and (df.index.sort_values() == np.arange(len(df))).all()
         )
 
 
 def pandas_to_pydf(
     data: pd.DataFrame,
     schema: SchemaDefinition | None = None,
```

### Comparing `polars_lts_cpu-0.17.0/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.17.1/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/_scan.py` & `polars_lts_cpu-0.17.1/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/_wrap.py` & `polars_lts_cpu-0.17.1/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/build_info.py` & `polars_lts_cpu-0.17.1/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/convert.py` & `polars_lts_cpu-0.17.1/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/decorators.py` & `polars_lts_cpu-0.17.1/polars/utils/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 from __future__ import annotations
 
 import functools
 import inspect
 import warnings
 from typing import TYPE_CHECKING, Any, Callable, TypeVar
 
+from polars.utils.various import find_stacklevel
+
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info >= (3, 10):
         from typing import ParamSpec
     else:
         from typing_extensions import ParamSpec
 
     P = ParamSpec("P")
     T = TypeVar("T")
 
 
-def deprecated_alias(
-    *, stacklevel: int = 3, **aliases: str
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
+def deprecated_alias(**aliases: str) -> Callable[[Callable[P, T]], Callable[P, T]]:
     """
     Deprecate a function or method argument.
 
     Decorator for deprecated function and method arguments. Use as follows:
 
     @deprecated_alias(old_arg='new_arg')
     def myfunc(new_arg):
         ...
     """
 
     def deco(function: Callable[P, T]) -> Callable[P, T]:
         @functools.wraps(function)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
-            _rename_kwargs(function.__name__, kwargs, aliases, stacklevel=stacklevel)
+            _rename_kwargs(function.__name__, kwargs, aliases)
             return function(*args, **kwargs)
 
         return wrapper
 
     return deco
 
 
 def _rename_kwargs(
     func_name: str,
     kwargs: dict[str, object],
     aliases: dict[str, str],
-    *,
-    stacklevel: int = 3,
 ) -> None:
     """
     Rename the keyword arguments of a function.
 
     Helper function for deprecating function and method arguments.
     """
     for alias, new in aliases.items():
@@ -62,39 +60,35 @@
                 )
             warnings.warn(
                 message=(
                     f"`{alias}` is deprecated as an argument to `{func_name}`; use"
                     f" `{new}` instead."
                 ),
                 category=DeprecationWarning,
-                stacklevel=stacklevel,
+                stacklevel=find_stacklevel(),
             )
             kwargs[new] = kwargs.pop(alias)
 
 
 def deprecate_nonkeyword_arguments(
     allowed_args: list[str] | None = None,
     message: str | None = None,
-    *,
-    stacklevel: int = 2,
 ) -> Callable[[Callable[P, T]], Callable[P, T]]:
     """
     Decorator to deprecate the use of non-keyword arguments of a function.
 
     Parameters
     ----------
     allowed_args
         The names of some first arguments of the decorated function that are allowed to
         be given as positional arguments. Should include "self" when decorating class
         methods. If set to None (default), equal to all arguments that do not have a
         default value.
     message
         Optionally overwrite the default warning message.
-    stacklevel
-        Stacklevel with which to raise warning.
     """
 
     def decorate(function: Callable[P, T]) -> Callable[P, T]:
         old_sig = inspect.signature(function)
 
         if allowed_args is not None:
             allow_args = allowed_args
@@ -128,15 +122,15 @@
             msg = msg_format.format(except_args=_format_argument_list(allow_args))
         else:
             msg = message
 
         @functools.wraps(function)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             if len(args) > num_allowed_args:
-                warnings.warn(msg, DeprecationWarning, stacklevel=stacklevel)
+                warnings.warn(msg, DeprecationWarning, stacklevel=find_stacklevel())
             return function(*args, **kwargs)
 
         wrapper.__signature__ = new_sig  # type: ignore[attr-defined]
         return wrapper
 
     return decorate
 
@@ -169,15 +163,15 @@
     def _redirecting_getattr_(obj: T, item: Any) -> Any:
         if isinstance(item, str) and item in from_to:
             new_item = from_to[item]
             warnings.warn(
                 f"`{type(obj).__name__}.{item}` has been renamed; this"
                 f" redirect is temporary, please use `.{new_item}` instead",
                 category=DeprecationWarning,
-                stacklevel=2,
+                stacklevel=find_stacklevel(),
             )
             item = new_item
         return obj.__getattribute__(item)
 
     def _cls_(cls: type[T]) -> type[T]:
         # note: __getattr__ is only invoked if item isn't found on the class
         cls.__getattr__ = _redirecting_getattr_  # type: ignore[attr-defined]
```

### Comparing `polars_lts_cpu-0.17.0/polars/utils/meta.py` & `polars_lts_cpu-0.17.1/polars/utils/meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Various public utility functions."""
 from __future__ import annotations
 
 import contextlib
 import warnings
 from typing import TYPE_CHECKING
 
+from polars.utils.various import find_stacklevel
+
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import get_index_type as _get_index_type
     from polars.polars import threadpool_size as _threadpool_size
 
 if TYPE_CHECKING:
     from polars.datatypes import DataTypeClass
 
@@ -27,15 +29,15 @@
 
 def get_idx_type() -> DataTypeClass:
     """Get the datatype used for Polars indexing."""
     warnings.warn(
         "`get_idx_type` has been renamed; this"
         " redirect is temporary, please use `get_index_type` instead",
         category=DeprecationWarning,
-        stacklevel=2,
+        stacklevel=find_stacklevel(),
     )
     return get_index_type()
 
 
 def threadpool_size() -> int:
     """
     Get the number of threads in the Polars thread pool.
```

### Comparing `polars_lts_cpu-0.17.0/polars/utils/polars_version.py` & `polars_lts_cpu-0.17.1/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/polars/utils/show_versions.py` & `polars_lts_cpu-0.17.1/polars/utils/show_versions.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 import importlib
 import sys
 
 from polars.utils.meta import get_index_type
 from polars.utils.polars_version import get_polars_version
 
+# metadata module must be imported explicitly
+if sys.version_info >= (3, 8):
+    import importlib.metadata
+
 
 def show_versions() -> None:
     """
     Print out version of Polars and dependencies to stdout.
 
     Examples
     --------
```

### Comparing `polars_lts_cpu-0.17.0/polars/utils/various.py` & `polars_lts_cpu-0.17.1/polars/utils/various.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
+import inspect
 import os
 import re
 import sys
 from collections.abc import MappingView, Sized
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Generator, Iterable, Sequence, TypeVar
 
+import polars as pl
+
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 from polars import functions as F
 from polars.datatypes import (
@@ -331,7 +334,30 @@
 
     def __repr__(self) -> str:
         return "<no_default>"
 
 
 no_default = _NoDefault.no_default  # Sentinel indicating the default value.
 NoDefault = Literal[_NoDefault.no_default]
+
+
+def find_stacklevel() -> int:
+    """
+    Find the first place in the stack that is not inside polars (tests notwithstanding).
+
+    Taken from:
+    https://github.com/pandas-dev/pandas/blob/ab89c53f48df67709a533b6a95ce3d911871a0a8/pandas/util/_exceptions.py#L30-L51
+    """
+    pkg_dir = os.path.dirname(pl.__file__)
+    test_dir = os.path.join(pkg_dir, "tests")
+
+    # https://stackoverflow.com/questions/17407119/python-inspect-stack-is-slow
+    frame = inspect.currentframe()
+    n = 0
+    while frame:
+        fname = inspect.getfile(frame)
+        if fname.startswith(pkg_dir) and not fname.startswith(test_dir):
+            frame = frame.f_back
+            n += 1
+        else:
+            break
+    return n
```

### Comparing `polars_lts_cpu-0.17.0/pyproject.toml` & `polars_lts_cpu-0.17.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 ]
 markers = [
   "write_disk: Tests that write to disk",
   "slow: Tests with a longer than average runtime.",
   "benchmark: Tests that should be run on a Polars release build.",
 ]
 filterwarnings = "error" # Fail on warnings
+xfail_strict = true
 
 [tool.coverage.run]
 source = ["polars"]
 branch = true
 
 [tool.coverage.report]
 fail_under = 85
```

### Comparing `polars_lts_cpu-0.17.0/requirements-dev.txt` & `polars_lts_cpu-0.17.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/apply/dataframe.rs` & `polars_lts_cpu-0.17.1/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/apply/mod.rs` & `polars_lts_cpu-0.17.1/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/apply/series.rs` & `polars_lts_cpu-0.17.1/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.17.1/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/arrow_interop/to_rust.rs` & `polars_lts_cpu-0.17.1/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/batched_csv.rs` & `polars_lts_cpu-0.17.1/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/conversion.rs` & `polars_lts_cpu-0.17.1/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/dataframe.rs` & `polars_lts_cpu-0.17.1/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/datatypes.rs` & `polars_lts_cpu-0.17.1/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/error.rs` & `polars_lts_cpu-0.17.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/file.rs` & `polars_lts_cpu-0.17.1/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/lazy/apply.rs` & `polars_lts_cpu-0.17.1/src/lazy/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/lazy/dataframe.rs` & `polars_lts_cpu-0.17.1/src/lazy/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/lazy/dsl.rs` & `polars_lts_cpu-0.17.1/src/lazy/dsl.rs`

 * *Files 0% similar despite different names*

```diff
@@ -763,15 +763,15 @@
     }
     #[cfg(feature = "binary_encoding")]
     pub fn str_hex_decode(&self, strict: bool) -> PyExpr {
         self.clone()
             .inner
             .map(
                 move |s| s.utf8()?.hex_decode(strict).map(|s| Some(s.into_series())),
-                GetOutput::same_type(),
+                GetOutput::from_type(DataType::Binary),
             )
             .with_fmt("str.hex_decode")
             .into()
     }
     pub fn str_base64_encode(&self) -> PyExpr {
         self.clone()
             .inner
@@ -789,15 +789,15 @@
             .inner
             .map(
                 move |s| {
                     s.utf8()?
                         .base64_decode(strict)
                         .map(|s| Some(s.into_series()))
                 },
-                GetOutput::same_type(),
+                GetOutput::from_type(DataType::Binary),
             )
             .with_fmt("str.base64_decode")
             .into()
     }
 
     pub fn str_parse_int(&self, radix: u32, strict: bool) -> PyExpr {
         self.inner
```

### Comparing `polars_lts_cpu-0.17.0/src/lazy/meta.rs` & `polars_lts_cpu-0.17.1/src/lazy/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/lazy/mod.rs` & `polars_lts_cpu-0.17.1/src/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/lib.rs` & `polars_lts_cpu-0.17.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/list_construction.rs` & `polars_lts_cpu-0.17.1/src/list_construction.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/npy.rs` & `polars_lts_cpu-0.17.1/src/npy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/object.rs` & `polars_lts_cpu-0.17.1/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/series.rs` & `polars_lts_cpu-0.17.1/src/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/set.rs` & `polars_lts_cpu-0.17.1/src/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/src/sql.rs` & `polars_lts_cpu-0.17.1/src/sql.rs`

 * *Files 23% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     clippy::wrong_self_convention,
     clippy::should_implement_trait,
     clippy::len_without_is_empty
 )]
 impl PySQLContext {
     #[staticmethod]
     #[allow(clippy::new_without_default)]
-    pub fn new() -> PyResult<PySQLContext> {
-        Ok(PySQLContext {
-            context: SQLContext::try_new().map_err(PyPolarsErr::from)?,
-        })
+    pub fn new() -> PySQLContext {
+        PySQLContext {
+            context: SQLContext::new(),
+        }
     }
 
     pub fn register(&mut self, name: &str, lf: PyLazyFrame) {
         self.context.register(name, lf.ldf)
     }
 
     pub fn execute(&mut self, query: &str) -> PyResult<PyLazyFrame> {
```

### Comparing `polars_lts_cpu-0.17.0/src/utils.rs` & `polars_lts_cpu-0.17.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/README.md` & `polars_lts_cpu-0.17.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.17.1/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.17.1/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/benchmark/test_release.py` & `polars_lts_cpu-0.17.1/tests/benchmark/test_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,10 +155,10 @@
     # for this query to make sense
     n = 150_000
 
     # int64 is important to hit the page size
     df = pl.arange(0, n, eager=True, dtype=pl.Int64).to_frame()
     f = "/tmp/tmp.parquet"
     df.write_parquet(f, statistics=True, use_pyarrow=False, row_group_size=n)
-    assert pl.scan_parquet(f).filter(pl.col("arange") > n - 3).collect().to_dict(
-        False
-    ) == {"arange": [149998, 149999]}
+    result = pl.scan_parquet(f).filter(pl.col("arange") > n - 3).collect()
+    expected = pl.DataFrame({"arange": [149998, 149999]})
+    assert_frame_equal(result, expected)
```

### Comparing `polars_lts_cpu-0.17.0/tests/docs/run_doctest.py` & `polars_lts_cpu-0.17.1/tests/docs/run_doctest.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 """
 from __future__ import annotations
 
 import doctest
 import importlib
 import sys
 import unittest
+import warnings
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Any, Iterator
 
 import polars
 
 if TYPE_CHECKING:
@@ -65,14 +66,17 @@
 
     # Below the implementation of the IGNORE_RESULT directive
     # You can ignore the result of a doctest by adding "doctest: +IGNORE_RESULT" into
     # the code block. The difference with SKIP is that if the code errors on running,
     # that will still be reported.
     IGNORE_RESULT = doctest.register_optionflag("IGNORE_RESULT")
 
+    # Set doctests to fail on warnings
+    warnings.simplefilter("error", DeprecationWarning)
+
     OutputChecker = doctest.OutputChecker
 
     class CustomOutputChecker(OutputChecker):
         def check_output(self, want: str, got: str, optionflags: Any) -> bool:
             if IGNORE_RESULT_ALL:
                 return True
             if IGNORE_RESULT & optionflags:
```

### Comparing `polars_lts_cpu-0.17.0/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.17.1/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.17.1/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/parametric/test_series.py` & `polars_lts_cpu-0.17.1/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/parametric/test_testing.py` & `polars_lts_cpu-0.17.1/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/conftest.py` & `polars_lts_cpu-0.17.1/tests/unit/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,37 @@
 
 
 @pytest.fixture(params=ISO8601_FORMATS_DATETIME)
 def iso8601_format_datetime(request: pytest.FixtureRequest) -> list[str]:
     return cast(List[str], request.param)
 
 
+ISO8601_TZ_AWARE_FORMATS_DATETIME = []
+
+for T in ["T", " "]:
+    for hms in (
+        [
+            f"{T}%H:%M:%S",
+            f"{T}%H%M%S",
+            f"{T}%H:%M",
+            f"{T}%H%M",
+        ]
+        + [f"{T}%H:%M:%S.{fraction}" for fraction in ["%9f", "%6f", "%3f"]]
+        + [f"{T}%H%M%S.{fraction}" for fraction in ["%9f", "%6f", "%3f"]]
+    ):
+        for date_sep in ("/", "-", ""):
+            fmt = f"%Y{date_sep}%m{date_sep}%d{hms}%#z"
+            ISO8601_TZ_AWARE_FORMATS_DATETIME.append(fmt)
+
+
+@pytest.fixture(params=ISO8601_TZ_AWARE_FORMATS_DATETIME)
+def iso8601_tz_aware_format_datetime(request: pytest.FixtureRequest) -> list[str]:
+    return cast(List[str], request.param)
+
+
 ISO8601_FORMATS_DATE = []
 
 for date_sep in ("/", "-", ""):
     fmt = f"%Y{date_sep}%m{date_sep}%d"
     ISO8601_FORMATS_DATE.append(fmt)
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.17.1/tests/unit/datatypes/test_temporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -643,15 +643,15 @@
             [datetime(2000, 1, 1, 0, 0), datetime(2000, 1, 2, 0, 0)],
             [datetime(2022, 6, 1, 0, 0), datetime(2022, 6, 2, 0, 0)],
         ],
     }
 
 
 def test_date_range_invalid_time_zone() -> None:
-    with pytest.raises(ComputeError, match="unable to parse time zone: foo"):
+    with pytest.raises(ComputeError, match="unable to parse time zone: 'foo'"):
         pl.date_range(
             datetime(2001, 1, 1), datetime(2001, 1, 3), interval="1d", time_zone="foo"
         )
 
 
 @pytest.mark.parametrize(
     ("one", "two"),
@@ -1945,26 +1945,26 @@
 )
 def test_strptime_empty(time_unit: TimeUnit, time_zone: str | None) -> None:
     ts = pl.Series([None]).cast(pl.Utf8).str.strptime(pl.Datetime(time_unit, time_zone))
     assert ts.dtype == pl.Datetime(time_unit, time_zone)
 
 
 def test_strptime_with_invalid_tz() -> None:
-    with pytest.raises(ComputeError, match="unable to parse time zone: foo"):
+    with pytest.raises(ComputeError, match="unable to parse time zone: 'foo'"):
         pl.Series(["2020-01-01 03:00:00"]).str.strptime(pl.Datetime("us", "foo"))
     with pytest.raises(
         ComputeError,
         match="cannot use strptime with both a tz-aware format and a tz-aware dtype",
     ):
         pl.Series(["2020-01-01 03:00:00+01:00"]).str.strptime(
             pl.Datetime("us", "foo"), "%Y-%m-%d %H:%M:%S%z"
         )
     with pytest.raises(
         ComputeError,
-        match="cannot use strptime with both 'utc=True' and tz-aware datetime",
+        match="cannot use strptime with both 'utc=True' and tz-aware dtype",
     ):
         pl.Series(["2020-01-01 03:00:00"]).str.strptime(
             pl.Datetime("us", "foo"), "%Y-%m-%d %H:%M:%S", utc=True
         )
 
 
 def test_strptime_unguessable_format() -> None:
@@ -1973,15 +1973,15 @@
         match="could not find an appropriate format to parse dates, please define a fmt",
     ):
         pl.Series(["foobar"]).str.strptime(pl.Datetime)
 
 
 def test_convert_time_zone_invalid() -> None:
     ts = pl.Series(["2020-01-01"]).str.strptime(pl.Datetime)
-    with pytest.raises(ComputeError, match="unable to parse timezone: 'foo'"):
+    with pytest.raises(ComputeError, match="unable to parse time zone: 'foo'"):
         ts.dt.replace_time_zone("UTC").dt.convert_time_zone("foo")
 
 
 def test_convert_time_zone_lazy_schema() -> None:
     ts_us = pl.Series(["2020-01-01"]).str.strptime(pl.Datetime("us", "UTC"))
     ts_ms = pl.Series(["2020-01-01"]).str.strptime(pl.Datetime("ms", "UTC"))
     ldf = pl.DataFrame({"ts_us": ts_us, "ts_ms": ts_ms}).lazy()
@@ -2157,14 +2157,23 @@
 def test_date_range_descending() -> None:
     with pytest.raises(ComputeError, match="'start' cannot be greater than 'stop'"):
         pl.date_range(datetime(2000, 3, 20), datetime(2000, 3, 5), interval="1h")
     with pytest.raises(ComputeError, match="'interval' cannot be negative"):
         pl.date_range(datetime(2000, 3, 20), datetime(2000, 3, 21), interval="-1h")
 
 
+def test_date_range_end_of_month_5441() -> None:
+    start = date(2020, 1, 31)
+    stop = date(2021, 1, 31)
+    with pytest.raises(
+        ComputeError, match=r"cannot advance '2020-01-31 00:00:00' by 1 month\(s\)"
+    ):
+        pl.date_range(start, stop, interval="1mo")
+
+
 def test_logical_nested_take() -> None:
     frame = pl.DataFrame(
         {
             "ix": [2, 1],
             "dt": [[datetime(2001, 1, 1)], [datetime(2001, 1, 2)]],
             "d": [[date(2001, 1, 1)], [date(2001, 1, 1)]],
             "t": [[time(10)], [time(10)]],
@@ -2669,14 +2678,47 @@
         assert parsed.dt.nanosecond().item() == 123456789
     if "%6f" in iso8601_format_datetime:
         assert parsed.dt.nanosecond().item() == 123456000
     if "%3f" in iso8601_format_datetime:
         assert parsed.dt.nanosecond().item() == 123000000
 
 
+def test_infer_iso8601_tz_aware_datetime(iso8601_tz_aware_format_datetime: str) -> None:
+    # construct an example time string
+    time_string = (
+        iso8601_tz_aware_format_datetime.replace("%Y", "2134")
+        .replace("%m", "12")
+        .replace("%d", "13")
+        .replace("%H", "01")
+        .replace("%M", "12")
+        .replace("%S", "34")
+        .replace("%3f", "123")
+        .replace("%6f", "123456")
+        .replace("%9f", "123456789")
+        .replace("%#z", "+01:00")
+    )
+    parsed = pl.Series([time_string]).str.strptime(pl.Datetime("ns"))
+    assert parsed.dt.year().item() == 2134
+    assert parsed.dt.month().item() == 12
+    assert parsed.dt.day().item() == 13
+    if "%H" in iso8601_tz_aware_format_datetime:
+        assert parsed.dt.hour().item() == 1
+    if "%M" in iso8601_tz_aware_format_datetime:
+        assert parsed.dt.minute().item() == 12
+    if "%S" in iso8601_tz_aware_format_datetime:
+        assert parsed.dt.second().item() == 34
+    if "%9f" in iso8601_tz_aware_format_datetime:
+        assert parsed.dt.nanosecond().item() == 123456789
+    if "%6f" in iso8601_tz_aware_format_datetime:
+        assert parsed.dt.nanosecond().item() == 123456000
+    if "%3f" in iso8601_tz_aware_format_datetime:
+        assert parsed.dt.nanosecond().item() == 123000000
+    assert parsed.dtype == pl.Datetime("ns", "+01:00")
+
+
 def test_infer_iso8601_date(iso8601_format_date: str) -> None:
     # construct an example date string
     time_string = (
         iso8601_format_date.replace("%Y", "2134")
         .replace("%m", "12")
         .replace("%d", "13")
     )
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.17.1/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.17.1/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.17.1/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.17.1/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.17.1/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import gzip
 import io
-import sys
 import tempfile
 import textwrap
 import typing
 import zlib
 from datetime import date, datetime, time, timedelta, timezone
 from pathlib import Path
 from typing import TYPE_CHECKING
@@ -744,14 +743,39 @@
     2021-10-10,2021-10-10
     """
     )
     df = pl.read_csv(data.encode(), try_parse_dates=True)
     assert df.null_count().row(0) == (0, 0)
 
 
+def test_tz_aware_try_parse_dates() -> None:
+    data = (
+        "a,b,c,d\n"
+        "2020-01-01T01:00:00+01:00,2021-04-28T00:00:00+02:00,2021-03-28T00:00:00+01:00,2\n"
+        "2020-01-01T02:00:00+01:00,2021-04-29T00:00:00+02:00,2021-03-29T00:00:00+02:00,3\n"
+    )
+    result = pl.read_csv(io.StringIO(data), try_parse_dates=True)
+    expected = pl.DataFrame(
+        {
+            "a": [
+                datetime(2020, 1, 1, 1, tzinfo=timezone(timedelta(hours=1))),
+                datetime(2020, 1, 1, 2, tzinfo=timezone(timedelta(hours=1))),
+            ],
+            "b": [
+                datetime(2021, 4, 28, tzinfo=timezone(timedelta(hours=2))),
+                datetime(2021, 4, 29, tzinfo=timezone(timedelta(hours=2))),
+            ],
+            # column 'c' has mixed offsets, so `try_parse_dates`  can't parse it
+            "c": ["2021-03-28T00:00:00+01:00", "2021-03-29T00:00:00+02:00"],
+            "d": [2, 3],
+        }
+    )
+    assert_frame_equal(result, expected)
+
+
 def test_csv_string_escaping() -> None:
     df = pl.DataFrame({"a": ["Free trip to A,B", '''Special rate "1.79"''']})
     f = io.BytesIO()
     df.write_csv(f)
     f.seek(0)
     df_read = pl.read_csv(f)
     assert_frame_equal(df_read, df)
@@ -1195,15 +1219,14 @@
     # the lines at the end have larger rows as the numbers increase
     N = 5_000
     csv = "\n".join(str(x) for x in range(N))
     assert pl.read_csv(io.StringIO(csv), n_rows=N).height == 4999
 
 
 @pytest.mark.write_disk()
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 def test_csv_scan_categorical() -> None:
     N = 5_000
     df = pl.DataFrame({"x": ["A"] * N})
     with tempfile.TemporaryDirectory() as temp_dir:
         file_path = Path(temp_dir) / "test_csv_scan_categorical.csv"
         df.write_csv(file_path)
         result = pl.scan_csv(file_path, dtypes={"x": pl.Categorical}).collect()
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_database.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_ipc.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,16 +28,27 @@
     buf2 = io.BytesIO()
     df.write_ipc(buf2, compression=compression)
     buf2.seek(0)
     read_df = pl.read_ipc(buf2, use_pyarrow=False)
     assert_frame_equal_local_categoricals(df, read_df)
 
 
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
-@pytest.mark.parametrize("compression", COMPRESSIONS)
+@pytest.mark.parametrize(
+    "compression",
+    [
+        pytest.param(
+            "uncompressed",
+            marks=pytest.mark.xfail(
+                sys.platform == "win32", reason="Does not work on Windows"
+            ),
+        ),
+        "lz4",
+        "zstd",
+    ],
+)
 @pytest.mark.parametrize("path_type", [str, Path])
 @pytest.mark.write_disk()
 def test_from_to_file(
     df: pl.DataFrame, compression: IpcCompression, path_type: type[str] | type[Path]
 ) -> None:
     with tempfile.TemporaryDirectory() as temp_dir:
         file_path = Path(temp_dir) / "small.ipc"
@@ -104,15 +115,14 @@
     f.seek(0)
 
     expected = {"a": pl.Int64, "b": pl.Utf8, "c": pl.Boolean}
     assert pl.read_ipc_schema(f) == expected
 
 
 @pytest.mark.write_disk()
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 @pytest.mark.parametrize("compression", COMPRESSIONS)
 @pytest.mark.parametrize("path_type", [str, Path])
 def test_ipc_schema_from_file(
     df_no_lists: pl.DataFrame,
     compression: IpcCompression,
     path_type: type[str] | type[Path],
 ) -> None:
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_json.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_lazy_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import sys
 import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import pandas as pd
 import pytest
 
@@ -307,15 +306,14 @@
     )
     assert (
         "parquet file can be skipped, the statistics were sufficient"
         " to apply the predicate." in captured
     )
 
 
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 @pytest.mark.write_disk()
 def test_streaming_categorical() -> None:
     df = pl.DataFrame(
         [
             pl.Series("name", ["Bob", "Alice", "Bob"], pl.Categorical),
             pl.Series("amount", [100, 200, 300]),
         ]
@@ -336,15 +334,14 @@
             expected = pl.DataFrame(
                 {"name": ["Bob", "Alice"], "amount": [400, 200]},
                 schema_overrides={"name": pl.Categorical},
             )
             assert_frame_equal(result, expected)
 
 
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 @pytest.mark.write_disk()
 def test_parquet_struct_categorical() -> None:
     df = pl.DataFrame(
         [
             pl.Series("a", ["bob"], pl.Categorical),
             pl.Series("b", ["foo"], pl.Categorical),
         ]
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_other.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import io
-import sys
 import tempfile
 import typing
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
@@ -353,15 +352,14 @@
         pq.write_table(table, f, compression="snappy")
         f.seek(0)
         read = pl.read_parquet(f)
         assert_frame_equal(read, df)
 
 
 @pytest.mark.write_disk()
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 def test_sink_parquet(io_files_path: Path) -> None:
     file = io_files_path / "small.parquet"
 
     with tempfile.TemporaryDirectory() as temp_dir:
         file_path = Path(temp_dir) / "sink.parquet"
 
         df_scanned = pl.scan_parquet(file)
@@ -370,15 +368,14 @@
         with pl.StringCache():
             result = pl.read_parquet(file_path)
             df_read = pl.read_parquet(file)
             assert_frame_equal(result, df_read)
 
 
 @pytest.mark.write_disk()
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 def test_sink_ipc(io_files_path: Path) -> None:
     file = io_files_path / "small.parquet"
 
     with tempfile.TemporaryDirectory() as temp_dir:
         file_path = Path(temp_dir) / "sink.ipc"
 
         df_scanned = pl.scan_parquet(file)
@@ -387,15 +384,14 @@
         with pl.StringCache():
             result = pl.read_ipc(file_path)
             df_read = pl.read_parquet(file)
             assert_frame_equal(result, df_read)
 
 
 @pytest.mark.write_disk()
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 def test_fetch_union() -> None:
     df1 = pl.DataFrame({"a": [0, 1, 2], "b": [1, 2, 3]})
     df2 = pl.DataFrame({"a": [3, 4, 5], "b": [4, 5, 6]})
 
     with tempfile.TemporaryDirectory() as temp_dir:
         file_path_1 = Path(temp_dir) / "df_fetch_1.parquet"
         file_path_2 = Path(temp_dir) / "df_fetch_2.parquet"
@@ -412,15 +408,14 @@
 
     expected = pl.DataFrame({"a": [0, 3], "b": [1, 4]})
     assert_frame_equal(result_glob, expected)
 
 
 @pytest.mark.slow()
 @typing.no_type_check
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 def test_struct_pyarrow_dataset_5796() -> None:
     num_rows = 2**17 + 1
 
     df = pl.from_records(
         [dict(id=i, nested=dict(a=i)) for i in range(num_rows)]  # noqa: C408
     )
     with tempfile.TemporaryDirectory() as temp_dir:
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.17.1/tests/unit/io/test_pyarrow_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import sys
 import tempfile
 import typing
 from datetime import date, datetime, time
 from pathlib import Path
 
 import pyarrow.dataset as ds
 import pytest
@@ -19,15 +18,14 @@
 
     expected = query(pl.scan_ipc(file_path))
     out = query(pl.scan_pyarrow_dataset(dset))
     assert_frame_equal(out, expected)
 
 
 @pytest.mark.write_disk()
-@pytest.mark.xfail(sys.platform == "win32", reason="Does not work on Windows")
 def test_dataset(df: pl.DataFrame) -> None:
     with tempfile.TemporaryDirectory() as temp_dir:
         file_path = Path(temp_dir) / "small.ipc"
         df.write_ipc(file_path)
 
         helper_dataset_test(
             file_path,
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_string.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,36 @@
         s.str.decode(encoding="hex")
     with pytest.raises(Exception):
         s.str.decode(encoding="base64")
     with pytest.raises(ValueError):
         s.str.decode("utf8")  # type: ignore[arg-type]
 
 
+def test_hex_decode_return_dtype() -> None:
+    data = {"a": ["68656c6c6f", "776f726c64"]}
+    expr = pl.col("a").str.decode("hex")
+
+    df = pl.DataFrame(data).select(expr)
+    assert df.schema == {"a": pl.Binary}
+
+    ldf = pl.LazyFrame(data).select(expr)
+    assert ldf.schema == {"a": pl.Binary}
+
+
+def test_base64_decode_return_dtype() -> None:
+    data = {"a": ["Zm9v", "YmFy"]}
+    expr = pl.col("a").str.decode("base64")
+
+    df = pl.DataFrame(data).select(expr)
+    assert df.schema == {"a": pl.Binary}
+
+    ldf = pl.LazyFrame(data).select(expr)
+    assert ldf.schema == {"a": pl.Binary}
+
+
 def test_str_replace_str_replace_all() -> None:
     s = pl.Series(["hello", "world", "test", "rooted"])
     expected = pl.Series(["hell0", "w0rld", "test", "r0oted"])
     assert_series_equal(s.str.replace("o", "0"), expected)
 
     expected = pl.Series(["hell0", "w0rld", "test", "r00ted"])
     assert_series_equal(s.str.replace_all("o", "0"), expected)
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_strptime.py`

 * *Files 14% similar despite different names*

```diff
@@ -160,21 +160,84 @@
         ("2018-09-05", datetime(2018, 9, 5)),
         ("2018-09-05T04:05:01", datetime(2018, 9, 5, 4, 5, 1)),
         ("2018-09-05T04:24:01.9", datetime(2018, 9, 5, 4, 24, 1, 900000)),
         ("2018-09-05T04:24:02.11", datetime(2018, 9, 5, 4, 24, 2, 110000)),
         ("2018-09-05T14:24:02.123", datetime(2018, 9, 5, 14, 24, 2, 123000)),
         ("2019-04-18T02:45:55.555000000", datetime(2019, 4, 18, 2, 45, 55, 555000)),
         ("2019-04-18T22:45:55.555123", datetime(2019, 4, 18, 22, 45, 55, 555123)),
+        (
+            "2018-09-05T04:05:01+01:00",
+            datetime(2018, 9, 5, 4, 5, 1, tzinfo=timezone(timedelta(hours=1))),
+        ),
+        (
+            "2018-09-05T04:24:01.9+01:00",
+            datetime(2018, 9, 5, 4, 24, 1, 900000, tzinfo=timezone(timedelta(hours=1))),
+        ),
+        (
+            "2018-09-05T04:24:02.11+01:00",
+            datetime(2018, 9, 5, 4, 24, 2, 110000, tzinfo=timezone(timedelta(hours=1))),
+        ),
+        (
+            "2018-09-05T14:24:02.123+01:00",
+            datetime(
+                2018, 9, 5, 14, 24, 2, 123000, tzinfo=timezone(timedelta(hours=1))
+            ),
+        ),
+        (
+            "2019-04-18T02:45:55.555000000+01:00",
+            datetime(
+                2019, 4, 18, 2, 45, 55, 555000, tzinfo=timezone(timedelta(hours=1))
+            ),
+        ),
+        (
+            "2019-04-18T22:45:55.555123+01:00",
+            datetime(
+                2019, 4, 18, 22, 45, 55, 555123, tzinfo=timezone(timedelta(hours=1))
+            ),
+        ),
     ],
 )
 def test_datetime_strptime_patterns_single(time_string: str, expected: str) -> None:
     result = pl.Series([time_string]).str.strptime(pl.Datetime).item()
     assert result == expected
 
 
+@pytest.mark.parametrize("time_unit", ["ms", "us", "ns"])
+def test_infer_tz_aware_time_unit(time_unit: TimeUnit) -> None:
+    result = pl.Series(["2020-01-02T04:00:00+02:00"]).str.strptime(
+        pl.Datetime(time_unit)
+    )
+    assert result.dtype == pl.Datetime(time_unit, "+02:00")
+    assert result.item() == datetime(
+        2020, 1, 2, 4, 0, tzinfo=timezone(timedelta(hours=2))
+    )
+
+
+@pytest.mark.parametrize("time_unit", ["ms", "us", "ns"])
+def test_infer_tz_aware_with_utc(time_unit: TimeUnit) -> None:
+    result = pl.Series(["2020-01-02T04:00:00+02:00"]).str.strptime(
+        pl.Datetime(time_unit), utc=True
+    )
+    assert result.dtype == pl.Datetime(time_unit, "UTC")
+    assert result.item() == datetime(2020, 1, 2, 2, 0, tzinfo=timezone.utc)
+
+
+def test_infer_tz_aware_raises() -> None:
+    msg = "cannot parse tz-aware values with tz-aware dtype - please drop the time zone from the dtype"
+    with pytest.raises(ComputeError, match=msg):
+        pl.Series(["2020-01-02T04:00:00+02:00"]).str.strptime(
+            pl.Datetime("us", "Europe/Vienna")
+        )
+    msg = "cannot use strptime with both 'utc=True' and tz-aware dtype, please drop time zone from the dtype"
+    with pytest.raises(ComputeError, match=msg):
+        pl.Series(["2020-01-02T04:00:00+02:00"]).str.strptime(
+            pl.Datetime("us", "Europe/Vienna"), utc=True
+        )
+
+
 def test_datetime_strptime_patterns_consistent() -> None:
     # note that all should be year first
     df = pl.Series(
         "date",
         [
             "2018-09-05",
             "2018-09-05T04:05:01",
@@ -316,15 +379,15 @@
     ).to_list() == [date(2022, 9, 18), None]
 
 
 def test_replace_timezone_invalid_timezone() -> None:
     ts = pl.Series(["2020-01-01 00:00:00+01:00"]).str.strptime(
         pl.Datetime, "%Y-%m-%d %H:%M:%S%z"
     )
-    with pytest.raises(ComputeError, match=r"unable to parse time zone: foo"):
+    with pytest.raises(ComputeError, match=r"unable to parse time zone: 'foo'"):
         ts.dt.replace_time_zone("foo")
 
 
 def test_replace_time_zone_ambiguous_or_non_existent() -> None:
     with pytest.raises(
         ArrowError,
         match="datetime '2021-11-07 01:00:00' is ambiguous in time zone 'US/Central'",
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.17.1/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_statistics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import numpy as np
 
 import polars as pl
+from polars.testing import assert_frame_equal
 
 
 def test_corr() -> None:
     df = pl.DataFrame(
         {
             "a": [1, 2, 4],
             "b": [-1, 23, 8],
         }
     )
-    assert df.corr().to_dict(False) == {
-        "a": [1.0, 0.18898223650461357],
-        "b": [0.1889822365046136, 1.0],
-    }
+    result = df.corr()
+    expected = pl.DataFrame(
+        {
+            "a": [1.0, 0.18898223650461357],
+            "b": [0.1889822365046136, 1.0],
+        }
+    )
+    assert_frame_equal(result, expected)
 
 
 def test_cut() -> None:
     a = pl.Series("a", [v / 10 for v in range(-30, 30, 5)])
     out = a.cut(bins=[-1, 1])
 
     assert out.shape == (12, 3)
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_transpose.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,56 +2,65 @@
 from typing import Iterator
 
 import polars as pl
 from polars.testing import assert_frame_equal
 
 
 def test_transpose_supertype() -> None:
-    assert pl.DataFrame(
-        {"a": [1, 2, 3], "b": ["foo", "bar", "ham"]}
-    ).transpose().to_dict(False) == {
-        "column_0": ["1", "foo"],
-        "column_1": ["2", "bar"],
-        "column_2": ["3", "ham"],
-    }
+    df = pl.DataFrame({"a": [1, 2, 3], "b": ["foo", "bar", "ham"]})
+    result = df.transpose()
+    expected = pl.DataFrame(
+        {
+            "column_0": ["1", "foo"],
+            "column_1": ["2", "bar"],
+            "column_2": ["3", "ham"],
+        }
+    )
+    assert_frame_equal(result, expected)
 
 
 def test_transpose_struct() -> None:
-    assert pl.DataFrame(
+    df = pl.DataFrame(
         {
             "a": ["foo", "bar", "ham"],
             "b": [
                 {"a": date(2022, 1, 1), "b": True},
                 {"a": date(2022, 1, 2), "b": False},
                 {"a": date(2022, 1, 3), "b": False},
             ],
         }
-    ).transpose().to_dict(False) == {
-        "column_0": ["foo", "{2022-01-01,true}"],
-        "column_1": ["bar", "{2022-01-02,false}"],
-        "column_2": ["ham", "{2022-01-03,false}"],
-    }
-
-    assert (
-        pl.DataFrame(
-            {
-                "b": [
-                    {"a": date(2022, 1, 1), "b": True},
-                    {"a": date(2022, 1, 2), "b": False},
-                    {"a": date(2022, 1, 3), "b": False},
-                ]
-            }
-        )
-        .transpose()
-        .to_dict(False)
-    ) == {
-        "column_0": [{"a": date(2022, 1, 1), "b": True}],
-        "column_1": [{"a": date(2022, 1, 2), "b": False}],
-        "column_2": [{"a": date(2022, 1, 3), "b": False}],
-    }
+    )
+    result = df.transpose()
+    expected = pl.DataFrame(
+        {
+            "column_0": ["foo", "{2022-01-01,true}"],
+            "column_1": ["bar", "{2022-01-02,false}"],
+            "column_2": ["ham", "{2022-01-03,false}"],
+        }
+    )
+    assert_frame_equal(result, expected)
+
+    df = pl.DataFrame(
+        {
+            "b": [
+                {"a": date(2022, 1, 1), "b": True},
+                {"a": date(2022, 1, 2), "b": False},
+                {"a": date(2022, 1, 3), "b": False},
+            ]
+        }
+    )
+    result = df.transpose()
+    expected = pl.DataFrame(
+        {
+            "column_0": [{"a": date(2022, 1, 1), "b": True}],
+            "column_1": [{"a": date(2022, 1, 2), "b": False}],
+            "column_2": [{"a": date(2022, 1, 3), "b": False}],
+        }
+    )
+    assert_frame_equal(result, expected)
 
 
 def test_transpose_arguments() -> None:
     df = pl.DataFrame({"a": [1, 2, 3], "b": [1, 2, 3]})
     expected = pl.DataFrame(
         {
             "column": ["a", "b"],
@@ -101,17 +110,22 @@
             "my_column_2": [3, 3],
         }
     )
     assert_frame_equal(expected, out)
 
 
 def test_transpose_logical_data() -> None:
-    assert pl.DataFrame(
+    df = pl.DataFrame(
         {
             "a": [date(2022, 2, 1), date(2022, 2, 2), date(2022, 1, 3)],
             "b": [datetime(2022, 1, 1), datetime(2022, 1, 2), datetime(2022, 1, 3)],
         }
-    ).transpose().to_dict(False) == {
-        "column_0": [datetime(2022, 2, 1, 0, 0), datetime(2022, 1, 1, 0, 0)],
-        "column_1": [datetime(2022, 2, 2, 0, 0), datetime(2022, 1, 2, 0, 0)],
-        "column_2": [datetime(2022, 1, 3, 0, 0), datetime(2022, 1, 3, 0, 0)],
-    }
+    )
+    result = df.transpose()
+    expected = pl.DataFrame(
+        {
+            "column_0": [datetime(2022, 2, 1, 0, 0), datetime(2022, 1, 1, 0, 0)],
+            "column_1": [datetime(2022, 2, 2, 0, 0), datetime(2022, 1, 2, 0, 0)],
+            "column_2": [datetime(2022, 1, 3, 0, 0), datetime(2022, 1, 3, 0, 0)],
+        }
+    )
+    assert_frame_equal(result, expected)
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.17.1/tests/unit/operations/test_window.py`

 * *Files 15% similar despite different names*

```diff
@@ -171,32 +171,36 @@
     df = pl.DataFrame(
         {
             "group": [0, 0, 0, 1, 1, 1],
             "val": [20, 40, 30, 2, 4, 3],
         }
     )
 
-    assert (
-        df.with_columns(
-            pl.col("val")
-            .cumulative_eval(pl.element().max())
-            .over("group")
-            .alias("cumulative_eval_max")
-        ).to_dict(False)
-    ) == {
-        "group": [0, 0, 0, 1, 1, 1],
-        "val": [20, 40, 30, 2, 4, 3],
-        "cumulative_eval_max": [20, 40, 40, 2, 4, 4],
-    }
+    result = df.with_columns(
+        pl.col("val")
+        .cumulative_eval(pl.element().max())
+        .over("group")
+        .alias("cumulative_eval_max")
+    )
+    expected = pl.DataFrame(
+        {
+            "group": [0, 0, 0, 1, 1, 1],
+            "val": [20, 40, 30, 2, 4, 3],
+            "cumulative_eval_max": [20, 40, 40, 2, 4, 4],
+        }
+    )
+    assert_frame_equal(result, expected)
 
     # 6394
     df = pl.DataFrame({"group": [1, 1, 2, 3], "value": [1, None, 3, None]})
-    assert df.select(
+    result = df.select(
         pl.col("value").cumulative_eval(pl.element().mean()).over("group")
-    ).to_dict(False) == {"value": [1.0, 1.0, 3.0, None]}
+    )
+    expected = pl.DataFrame({"value": [1.0, 1.0, 3.0, None]})
+    assert_frame_equal(result, expected)
 
 
 def test_count_window() -> None:
     assert (
         pl.DataFrame(
             {
                 "a": [1, 1, 2],
@@ -206,31 +210,32 @@
         .to_list()
     ) == [2, 2, 1]
 
 
 def test_window_cached_keys_sorted_update_4183() -> None:
     df = pl.DataFrame(
         {
-            "customer_ID": [
-                "0",
-                "0",
-                "1",
-            ],
+            "customer_ID": ["0", "0", "1"],
             "date": [1, 2, 3],
         }
     )
-    assert df.sort(by=["customer_ID", "date"]).select(
+    result = df.sort(by=["customer_ID", "date"]).select(
         [
             pl.count("date").over(pl.col("customer_ID")).alias("count"),
             pl.col("date")
             .rank(method="ordinal")
             .over(pl.col("customer_ID"))
             .alias("rank"),
         ]
-    ).to_dict(False) == {"count": [2, 2, 1], "rank": [1, 2, 1]}
+    )
+    expected = pl.DataFrame(
+        {"count": [2, 2, 1], "rank": [1, 2, 1]},
+        schema={"count": pl.UInt32, "rank": pl.UInt32},
+    )
+    assert_frame_equal(result, expected)
 
 
 def test_window_functions_list_types() -> None:
     df = pl.DataFrame(
         {
             "col_int": [1, 1, 2, 2],
             "col_list": [[1], [1], [2], [2]],
@@ -278,58 +283,57 @@
     df = pl.DataFrame(
         {
             "x": [1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 2, 13, 4, 15, 6, None, None, 19],
             "y": [0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1],
         }
     )
 
-    assert df.with_columns(
-        [
-            pl.when(pl.col("x") >= pl.col("x").quantile(0.1))
-            .then(1)
-            .otherwise(None)
-            .over("y")
-            .alias("foo")
-        ]
-    ).to_dict(False) == {
-        "x": [1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 2, 13, 4, 15, 6, None, None, 19],
-        "y": [0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1],
-        "foo": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, None, None, 1],
-    }
+    result = df.with_columns(
+        pl.when(pl.col("x") >= pl.col("x").quantile(0.1))
+        .then(1)
+        .otherwise(None)
+        .over("y")
+        .alias("foo")
+    )
+    expected = pl.DataFrame(
+        {
+            "x": [1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 2, 13, 4, 15, 6, None, None, 19],
+            "y": [0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+            "foo": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, None, None, 1],
+        },
+        # Resulting column is Int32, see https://github.com/pola-rs/polars/issues/8041
+        schema_overrides={"foo": pl.Int32},
+    )
+    assert_frame_equal(result, expected)
 
 
 def test_window_5868() -> None:
     df = pl.DataFrame({"value": [None, 2], "id": [None, 1]})
 
-    assert df.with_columns(pl.col("value").max().over("id")).to_dict(False) == {
-        "value": [None, 2],
-        "id": [None, 1],
-    }
+    result_df = df.with_columns(pl.col("value").max().over("id"))
+    expected_df = pl.DataFrame({"value": [None, 2], "id": [None, 1]})
+    assert_frame_equal(result_df, expected_df)
 
     df = pl.DataFrame({"a": [None, 1, 2, 3, 3, 3, 4, 4]})
 
-    assert df.select(pl.col("a").sum().over("a"))["a"].to_list() == [
-        None,
-        1,
-        2,
-        9,
-        9,
-        9,
-        8,
-        8,
-    ]
-    assert df.with_columns(pl.col("a").set_sorted()).select(
-        pl.col("a").sum().over("a")
-    )["a"].to_list() == [None, 1, 2, 9, 9, 9, 8, 8]
-
-    assert df.drop_nulls().select(pl.col("a").sum().over("a"))["a"].to_list() == [
-        1,
-        2,
-        9,
-        9,
-        9,
-        8,
-        8,
-    ]
-    assert df.drop_nulls().with_columns(pl.col("a").set_sorted()).select(
-        pl.col("a").sum().over("a")
-    )["a"].to_list() == [1, 2, 9, 9, 9, 8, 8]
+    result = df.select(pl.col("a").sum().over("a")).get_column("a")
+    expected = pl.Series("a", [None, 1, 2, 9, 9, 9, 8, 8])
+    assert_series_equal(result, expected)
+
+    result = (
+        df.with_columns(pl.col("a").set_sorted())
+        .select(pl.col("a").sum().over("a"))
+        .get_column("a")
+    )
+    assert_series_equal(result, expected)
+
+    result = df.drop_nulls().select(pl.col("a").sum().over("a")).get_column("a")
+    expected = pl.Series("a", [1, 2, 9, 9, 9, 8, 8])
+    assert_series_equal(result, expected)
+
+    result = (
+        df.drop_nulls()
+        .with_columns(pl.col("a").set_sorted())
+        .select(pl.col("a").sum().over("a"))
+        .get_column("a")
+    )
+    assert_series_equal(result, expected)
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_api.py` & `polars_lts_cpu-0.17.1/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_arity.py` & `polars_lts_cpu-0.17.1/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_cfg.py` & `polars_lts_cpu-0.17.1/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_constructors.py` & `polars_lts_cpu-0.17.1/tests/unit/test_constructors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_cse.py` & `polars_lts_cpu-0.17.1/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.17.1/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_df.py` & `polars_lts_cpu-0.17.1/tests/unit/test_df.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_empty.py` & `polars_lts_cpu-0.17.1/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_errors.py` & `polars_lts_cpu-0.17.1/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.17.1/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_exprs.py` & `polars_lts_cpu-0.17.1/tests/unit/test_exprs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1030,7 +1030,23 @@
         df.select(
             any=(pl.col("x") == pl.col("y"))
             | (pl.col("x") == pl.col("y"))
             | (pl.col("y") == pl.col("z"))
             | (pl.col("y").cast(int) == pl.col("z"))
         ),
     )
+
+
+def test_head() -> None:
+    df = pl.DataFrame({"a": [1, 2, 3, 4, 5]})
+    assert df.select(pl.col("a").head(0)).to_dict(False) == {"a": []}
+    assert df.select(pl.col("a").head(3)).to_dict(False) == {"a": [1, 2, 3]}
+    assert df.select(pl.col("a").head(10)).to_dict(False) == {"a": [1, 2, 3, 4, 5]}
+    assert df.select(pl.col("a").head(pl.count() / 2)).to_dict(False) == {"a": [1, 2]}
+
+
+def test_tail() -> None:
+    df = pl.DataFrame({"a": [1, 2, 3, 4, 5]})
+    assert df.select(pl.col("a").tail(0)).to_dict(False) == {"a": []}
+    assert df.select(pl.col("a").tail(3)).to_dict(False) == {"a": [3, 4, 5]}
+    assert df.select(pl.col("a").tail(10)).to_dict(False) == {"a": [1, 2, 3, 4, 5]}
+    assert df.select(pl.col("a").tail(pl.count() / 2)).to_dict(False) == {"a": [4, 5]}
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_fmt.py` & `polars_lts_cpu-0.17.1/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_functions.py` & `polars_lts_cpu-0.17.1/tests/unit/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_interchange.py` & `polars_lts_cpu-0.17.1/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_interop.py` & `polars_lts_cpu-0.17.1/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_lazy.py` & `polars_lts_cpu-0.17.1/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.17.1/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_predicates.py` & `polars_lts_cpu-0.17.1/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_projections.py` & `polars_lts_cpu-0.17.1/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_queries.py` & `polars_lts_cpu-0.17.1/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_rows.py` & `polars_lts_cpu-0.17.1/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_schema.py` & `polars_lts_cpu-0.17.1/tests/unit/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,7 +369,13 @@
 
 def test_deep_subexpression_f32_schema_7129() -> None:
     df = pl.DataFrame({"a": [1.1, 2.3, 3.4, 4.5]}, schema={"a": pl.Float32()})
     assert df.with_columns(pl.col("a") - pl.col("a").median()).dtypes == [pl.Float32]
     assert df.with_columns(
         (pl.col("a") - pl.col("a").mean()) / (pl.col("a").std() + 0.001)
     ).dtypes == [pl.Float32]
+
+
+def test_bool_sum_schema() -> None:
+    assert pl.LazyFrame({"a": [True, False]}).select(pl.col("a").sum()).schema == {
+        "a": pl.UInt32
+    }
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_serde.py` & `polars_lts_cpu-0.17.1/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_series.py` & `polars_lts_cpu-0.17.1/tests/unit/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1126,22 +1126,24 @@
     assert dict(num_s.describe().rows()) == {  # type: ignore[arg-type]
         "count": 3.0,
         "max": 3.0,
         "mean": 2.0,
         "min": 1.0,
         "null_count": 0.0,
         "std": 1.0,
+        "median": 2.0,
     }
     assert dict(float_s.describe().rows()) == {  # type: ignore[arg-type]
         "count": 3.0,
         "max": 8.9,
         "mean": 4.933333333333334,
         "min": 1.3,
         "null_count": 0.0,
         "std": 3.8109491381194442,
+        "median": 4.6,
     }
     assert dict(str_s.describe().rows()) == {  # type: ignore[arg-type]
         "count": 3,
         "null_count": 0,
         "unique": 3,
     }
     assert dict(bool_s.describe().rows()) == {  # type: ignore[arg-type]
@@ -1149,14 +1151,15 @@
         "null_count": 1,
         "sum": 3,
     }
     assert dict(date_s.describe().rows()) == {  # type: ignore[arg-type]
         "count": "3",
         "max": "2021-01-03",
         "min": "2021-01-01",
+        "median": "2021-01-02",
         "null_count": "0",
     }
 
     with pytest.raises(ValueError):
         assert empty_s.describe()
```

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_sql.py` & `polars_lts_cpu-0.17.1/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_streaming.py` & `polars_lts_cpu-0.17.1/tests/unit/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/test_testing.py` & `polars_lts_cpu-0.17.1/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.17.1/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.0/Cargo.lock` & `polars_lts_cpu-0.17.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1708,15 +1708,15 @@
 checksum = "1d0dd4be24fcdcfeaa12a432d588dc59bbad6cad3510c67e74a2b6b2fc950564"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.17.0"
+version = "0.17.1"
 dependencies = [
  "ahash",
  "bincode",
  "built",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_lts_cpu-0.17.0/PKG-INFO` & `polars_lts_cpu-0.17.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.17.0
+Version: 0.17.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,51 +13,51 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: typing_extensions >= 4.0.1; python_version < '3.11'
-Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
-Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
-Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
-Requires-Dist: pandas; extra == 'pandas'
-Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
-Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
-Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
-Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
+Requires-Dist: matplotlib; extra == 'matplotlib'
 Requires-Dist: fsspec; extra == 'fsspec'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
+Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
 Requires-Dist: connectorx; extra == 'connectorx'
+Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Requires-Dist: pandas; extra == 'sqlalchemy'
-Requires-Dist: matplotlib; extra == 'matplotlib'
-Provides-Extra: xlsxwriter
-Provides-Extra: xlsx2csv
-Provides-Extra: deltalake
-Provides-Extra: pandas
-Provides-Extra: all
-Provides-Extra: numpy
-Provides-Extra: timezone
+Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
+Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
+Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
+Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
+Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
+Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
+Requires-Dist: pandas; extra == 'pandas'
+Provides-Extra: matplotlib
 Provides-Extra: fsspec
-Provides-Extra: pyarrow
+Provides-Extra: deltalake
 Provides-Extra: connectorx
+Provides-Extra: xlsx2csv
 Provides-Extra: sqlalchemy
-Provides-Extra: matplotlib
+Provides-Extra: timezone
+Provides-Extra: numpy
+Provides-Extra: xlsxwriter
+Provides-Extra: all
+Provides-Extra: pyarrow
+Provides-Extra: pandas
 License-File: LICENSE
 Summary: Blazingly fast DataFrame library
 Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 Project-URL: Homepage, https://www.pola.rs/
 Project-URL: Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/index.html
-Project-URL: Repository, https://github.com/pola-rs/polars
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/polars_github_logo_rect_dark_name.svg">
   <br>
 </h1>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.0 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.1 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Rust Classifier: Topic ::
 Scientific/Engineering Requires-Dist: typing_extensions >= 4.0.1;
-python_version < '3.11' Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
-Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Requires-Dist: deltalake
->= 0.8.0; extra == 'deltalake' Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
-Requires-Dist: pandas; extra == 'pandas' Requires-Dist: polars
-[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
-extra == 'all' Requires-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist:
+python_version < '3.11' Requires-Dist: matplotlib; extra == 'matplotlib'
+Requires-Dist: fsspec; extra == 'fsspec' Requires-Dist: deltalake >= 0.8.0;
+extra == 'deltalake' Requires-Dist: connectorx; extra == 'connectorx' Requires-
+Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Requires-Dist: sqlalchemy; extra
+== 'sqlalchemy' Requires-Dist: pandas; extra == 'sqlalchemy' Requires-Dist:
 backports.zoneinfo; (python_version < '3.9') and extra == 'timezone' Requires-
 Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone' Requires-
-Dist: fsspec; extra == 'fsspec' Requires-Dist: pyarrow>=7.0.0; extra ==
-'pyarrow' Requires-Dist: connectorx; extra == 'connectorx' Requires-Dist:
-sqlalchemy; extra == 'sqlalchemy' Requires-Dist: pandas; extra == 'sqlalchemy'
-Requires-Dist: matplotlib; extra == 'matplotlib' Provides-Extra: xlsxwriter
-Provides-Extra: xlsx2csv Provides-Extra: deltalake Provides-Extra: pandas
-Provides-Extra: all Provides-Extra: numpy Provides-Extra: timezone Provides-
-Extra: fsspec Provides-Extra: pyarrow Provides-Extra: connectorx Provides-
-Extra: sqlalchemy Provides-Extra: matplotlib License-File: LICENSE Summary:
-Blazingly fast DataFrame library Keywords: dataframe,arrow,out-of-core Author-
-email: Ritchie Vink
+Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist: xlsxwriter; extra ==
+'xlsxwriter' Requires-Dist: polars
+[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
+extra == 'all' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist:
+pyarrow>=7.0.0; extra == 'pandas' Requires-Dist: pandas; extra == 'pandas'
+Provides-Extra: matplotlib Provides-Extra: fsspec Provides-Extra: deltalake
+Provides-Extra: connectorx Provides-Extra: xlsx2csv Provides-Extra: sqlalchemy
+Provides-Extra: timezone Provides-Extra: numpy Provides-Extra: xlsxwriter
+Provides-Extra: all Provides-Extra: pyarrow Provides-Extra: pandas License-
+File: LICENSE Summary: Blazingly fast DataFrame library Keywords:
+dataframe,arrow,out-of-core Author-email: Ritchie Vink
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Changelog, https://github.com/pola-rs/
-polars/releases Project-URL: Homepage, https://www.pola.rs/ Project-URL:
-Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/
-index.html Project-URL: Repository, https://github.com/pola-rs/polars
+charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/pola-rs/
+polars Project-URL: Changelog, https://github.com/pola-rs/polars/releases
+Project-URL: Homepage, https://www.pola.rs/ Project-URL: Documentation, https:/
+/pola-rs.github.io/polars/py-polars/html/reference/index.html
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
            Latest_Release] [NPM_Latest_Release] [DOI_Latest_Release]
 Documentation: Python - Rust - Node.js | StackOverflow: Python - Rust - Node.js
                             | User_Guide | Discord
```

