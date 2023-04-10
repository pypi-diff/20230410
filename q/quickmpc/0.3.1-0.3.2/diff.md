# Comparing `tmp/quickmpc-0.3.1.tar.gz` & `tmp/quickmpc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-32hd68ss/quickmpc-0.3.1.tar", last modified: Thu Mar 16 03:48:38 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-omv8n967/quickmpc-0.3.2.tar", last modified: Mon Apr 10 10:12:30 2023, max compression
```

## Comparing `quickmpc-0.3.1.tar` & `quickmpc-0.3.2.tar`

### file list

```diff
@@ -1,100 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-16 03:48:22.000000 quickmpc-0.3.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-16 03:48:22.000000 quickmpc-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-16 03:48:22.000000 quickmpc-0.3.1/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-16 03:48:22.000000 quickmpc-0.3.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 03:48:22.000000 quickmpc-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-16 03:48:22.000000 quickmpc-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-16 03:48:38.000000 quickmpc-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-16 03:48:22.000000 quickmpc-0.3.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-03-16 03:48:22.000000 quickmpc-0.3.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-16 03:48:22.000000 quickmpc-0.3.1/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-16 03:48:22.000000 quickmpc-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/demo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/data/data-meshcode.csv
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/data/data1-1.csv
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/data/data1-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/data/data1-3.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/demo/integration_demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/integration_demo/execute_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/integration_demo/progress_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/integration_demo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/demo/unit_demo/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/delete_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/demo_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/execute_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/get_computation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/get_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/get_elapsed_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/get_join_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-16 03:48:22.000000 quickmpc-0.3.1/demo/unit_demo/send_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-16 03:48:22.000000 quickmpc-0.3.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-16 03:48:22.000000 quickmpc-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-16 03:48:37.000000 quickmpc-0.3.1/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/generate_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16959 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/utils/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-16 03:48:22.000000 quickmpc-0.3.1/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-16 03:48:38.000000 quickmpc-0.3.1/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-16 03:48:38.000000 quickmpc-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-16 03:48:22.000000 quickmpc-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 03:48:38.000000 quickmpc-0.3.1/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_files/data1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_files/data2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_files/data3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-16 03:48:22.000000 quickmpc-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 10:12:15.000000 quickmpc-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 10:12:15.000000 quickmpc-0.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 10:12:30.000000 quickmpc-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 10:12:15.000000 quickmpc-0.3.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-10 10:12:15.000000 quickmpc-0.3.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-10 10:12:15.000000 quickmpc-0.3.2/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-10 10:12:15.000000 quickmpc-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data-meshcode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data1-1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data1-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data1-3.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/integration_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/integration_demo/execute_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/integration_demo/progress_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/integration_demo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/unit_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/delete_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/demo_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/execute_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_computation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_elapsed_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_join_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/send_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-10 10:12:15.000000 quickmpc-0.3.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-10 10:12:15.000000 quickmpc-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/qmpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-10 10:12:30.000000 quickmpc-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 10:12:15.000000 quickmpc-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/unit_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server1.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server2.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server2.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server3.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server3.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/unit_tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tox.ini
```

### Comparing `quickmpc-0.3.1/.vscode/settings.json` & `quickmpc-0.3.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/LICENSE` & `quickmpc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/Pipfile.lock` & `quickmpc-0.3.2/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9522739651416122%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'58f7099bf99712610ba131af2c8131d6f5ff77bcb6cf34a64532a368df00f6d8'}}",*

 * * "'default'": "{'googleapis-common-protos': {'hashes': "*

 * *              "['sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44', "*

 * *              "'sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f'], "*

 * *              "'version': '==1.59.0'}, 'grpcio': {'hashes': "*

 * *              "['sha256:040eb421613b57c696063abde405916dd830203c184c9000fc8c3b3b3c950325 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "7dd2f073613bb63b539b0b62c232edf1525f0e5672b326cf0b76c11ac1b7baff"
+            "sha256": "58f7099bf99712610ba131af2c8131d6f5ff77bcb6cf34a64532a368df00f6d8"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.7"
         },
         "sources": [
             {
@@ -83,70 +83,70 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "googleapis-common-protos": {
             "hashes": [
-                "sha256:c727251ec025947d545184ba17e3578840fc3a24a0516a020479edab660457df",
-                "sha256:ca3befcd4580dab6ad49356b46bf165bb68ff4b32389f028f1abd7c10ab9519a"
+                "sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44",
+                "sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.58.0"
+            "version": "==1.59.0"
         },
         "grpcio": {
             "hashes": [
-                "sha256:094e64236253590d9d4075665c77b329d707b6fca864dd62b144255e199b4f87",
-                "sha256:0dc5354e38e5adf2498312f7241b14c7ce3484eefa0082db4297189dcbe272e6",
-                "sha256:0e1a9e1b4a23808f1132aa35f968cd8e659f60af3ffd6fb00bcf9a65e7db279f",
-                "sha256:0fb93051331acbb75b49a2a0fd9239c6ba9528f6bdc1dd400ad1cb66cf864292",
-                "sha256:16c71740640ba3a882f50b01bf58154681d44b51f09a5728180a8fdc66c67bd5",
-                "sha256:172405ca6bdfedd6054c74c62085946e45ad4d9cec9f3c42b4c9a02546c4c7e9",
-                "sha256:17ec9b13cec4a286b9e606b48191e560ca2f3bbdf3986f91e480a95d1582e1a7",
-                "sha256:22b011674090594f1f3245960ced7386f6af35485a38901f8afee8ad01541dbd",
-                "sha256:24ac1154c4b2ab4a0c5326a76161547e70664cd2c39ba75f00fc8a2170964ea2",
-                "sha256:257478300735ce3c98d65a930bbda3db172bd4e00968ba743e6a1154ea6edf10",
-                "sha256:29cb97d41a4ead83b7bcad23bdb25bdd170b1e2cba16db6d3acbb090bc2de43c",
-                "sha256:2b170eaf51518275c9b6b22ccb59450537c5a8555326fd96ff7391b5dd75303c",
-                "sha256:31bb6bc7ff145e2771c9baf612f4b9ebbc9605ccdc5f3ff3d5553de7fc0e0d79",
-                "sha256:3c2b3842dcf870912da31a503454a33a697392f60c5e2697c91d133130c2c85d",
-                "sha256:3f9b0023c2c92bebd1be72cdfca23004ea748be1813a66d684d49d67d836adde",
-                "sha256:471d39d3370ca923a316d49c8aac66356cea708a11e647e3bdc3d0b5de4f0a40",
-                "sha256:49d680356a975d9c66a678eb2dde192d5dc427a7994fb977363634e781614f7c",
-                "sha256:4c4423ea38a7825b8fed8934d6d9aeebdf646c97e3c608c3b0bcf23616f33877",
-                "sha256:506b9b7a4cede87d7219bfb31014d7b471cfc77157da9e820a737ec1ea4b0663",
-                "sha256:538d981818e49b6ed1e9c8d5e5adf29f71c4e334e7d459bf47e9b7abb3c30e09",
-                "sha256:59dffade859f157bcc55243714d57b286da6ae16469bf1ac0614d281b5f49b67",
-                "sha256:5a6ebcdef0ef12005d56d38be30f5156d1cb3373b52e96f147f4a24b0ddb3a9d",
-                "sha256:5dca372268c6ab6372d37d6b9f9343e7e5b4bc09779f819f9470cd88b2ece3c3",
-                "sha256:6df3b63538c362312bc5fa95fb965069c65c3ea91d7ce78ad9c47cab57226f54",
-                "sha256:6f0b89967ee11f2b654c23b27086d88ad7bf08c0b3c2a280362f28c3698b2896",
-                "sha256:75e29a90dc319f0ad4d87ba6d20083615a00d8276b51512e04ad7452b5c23b04",
-                "sha256:7942b32a291421460d6a07883033e392167d30724aa84987e6956cd15f1a21b9",
-                "sha256:9235dcd5144a83f9ca6f431bd0eccc46b90e2c22fe27b7f7d77cabb2fb515595",
-                "sha256:97d67983189e2e45550eac194d6234fc38b8c3b5396c153821f2d906ed46e0ce",
-                "sha256:9ff42c5620b4e4530609e11afefa4a62ca91fa0abb045a8957e509ef84e54d30",
-                "sha256:a8a0b77e992c64880e6efbe0086fe54dfc0bbd56f72a92d9e48264dcd2a3db98",
-                "sha256:aacb54f7789ede5cbf1d007637f792d3e87f1c9841f57dd51abf89337d1b8472",
-                "sha256:bc59f7ba87972ab236f8669d8ca7400f02a0eadf273ca00e02af64d588046f02",
-                "sha256:cc2bece1737b44d878cc1510ea04469a8073dbbcdd762175168937ae4742dfb3",
-                "sha256:cd3baccea2bc5c38aeb14e5b00167bd4e2373a373a5e4d8d850bd193edad150c",
-                "sha256:dad6533411d033b77f5369eafe87af8583178efd4039c41d7515d3336c53b4f1",
-                "sha256:e223a9793522680beae44671b9ed8f6d25bbe5ddf8887e66aebad5e0686049ef",
-                "sha256:e473525c28251558337b5c1ad3fa969511e42304524a4e404065e165b084c9e4",
-                "sha256:e4ef09f8997c4be5f3504cefa6b5c6cc3cf648274ce3cede84d4342a35d76db6",
-                "sha256:e6dfc2b6567b1c261739b43d9c59d201c1b89e017afd9e684d85aa7a186c9f7a",
-                "sha256:eacad297ea60c72dd280d3353d93fb1dcca952ec11de6bb3c49d12a572ba31dd",
-                "sha256:f1158bccbb919da42544a4d3af5d9296a3358539ffa01018307337365a9a0c64",
-                "sha256:f1fec3abaf274cdb85bf3878167cfde5ad4a4d97c68421afda95174de85ba813",
-                "sha256:f96ace1540223f26fbe7c4ebbf8a98e3929a6aa0290c8033d12526847b291c0f",
-                "sha256:fbdbe9a849854fe484c00823f45b7baab159bdd4a46075302281998cb8719df5"
+                "sha256:040eb421613b57c696063abde405916dd830203c184c9000fc8c3b3b3c950325",
+                "sha256:165b05af77e6aecb4210ae7663e25acf234ba78a7c1c157fa5f2efeb0d6ec53c",
+                "sha256:200d69857f9910f7458b39b9bcf83ee4a180591b40146ba9e49314e3a7419313",
+                "sha256:22bdfac4f7f27acdd4da359b5e7e1973dc74bf1ed406729b07d0759fde2f064b",
+                "sha256:2a8e17286c4240137d933b8ca506465472248b4ce0fe46f3404459e708b65b68",
+                "sha256:2cd2e4cefb724cab1ba2df4b7535a9980531b9ec51b4dbb5f137a1f3a3754ef0",
+                "sha256:2f8ff75e61e1227ba7a3f16b2eadbcc11d0a54096d52ab75a6b88cfbe56f55d1",
+                "sha256:2fdd6333ce96435408565a9dbbd446212cd5d62e4d26f6a3c0feb1e3c35f1cc8",
+                "sha256:30e09b5e0531685e176f49679b6a3b190762cc225f4565e55a899f5e14b3aa62",
+                "sha256:3667c06e37d6cd461afdd51cefe6537702f3d1dc5ff4cac07e88d8b4795dc16f",
+                "sha256:36c8abbc5f837111e7bd619612eedc223c290b0903b952ce0c7b00840ea70f14",
+                "sha256:3709048fe0aa23dda09b3e69849a12055790171dab9e399a72ea8f9dfbf9ac80",
+                "sha256:3c1b9f8afa62ff265d86a4747a2990ec5a96e4efce5d5888f245a682d66eca47",
+                "sha256:3ea4341efe603b049e8c9a5f13c696ca37fcdf8a23ca35f650428ad3606381d9",
+                "sha256:3f9a7d88082b2a17ae7bd3c2354d13bab0453899e0851733f6afa6918373f476",
+                "sha256:49ede0528e9dac7e8a9fe30b16c73b630ddd9a576bf4b675eb6b0c53ee5ca00f",
+                "sha256:54b0c29bdd9a3b1e1b61443ab152f060fc719f1c083127ab08d03fac5efd51be",
+                "sha256:54e36c2ee304ff15f2bfbdc43d2b56c63331c52d818c364e5b5214e5bc2ad9f6",
+                "sha256:5694448256e3cdfe5bd358f1574a3f2f51afa20cc834713c4b9788d60b7cc646",
+                "sha256:5e77ee138100f0bb55cbd147840f87ee6241dbd25f09ea7cd8afe7efff323449",
+                "sha256:5eed34994c095e2bf7194ffac7381c6068b057ef1e69f8f08db77771350a7566",
+                "sha256:6604f614016127ae10969176bbf12eb0e03d2fb3d643f050b3b69e160d144fb4",
+                "sha256:68a7514b754e38e8de9075f7bb4dee919919515ec68628c43a894027e40ddec4",
+                "sha256:6972b009638b40a448d10e1bc18e2223143b8a7aa20d7def0d78dd4af4126d12",
+                "sha256:6c677581ce129f5fa228b8f418cee10bd28dd449f3a544ea73c8ba590ee49d0b",
+                "sha256:6c99a73a6260bdf844b2e5ddad02dcd530310f80e1fa72c300fa19c1c7496962",
+                "sha256:82b0ad8ac825d4bb31bff9f638557c045f4a6d824d84b21e893968286f88246b",
+                "sha256:881ecb34feabf31c6b3b9bbbddd1a5b57e69f805041e5a2c6c562a28574f71c4",
+                "sha256:8de30f0b417744288cec65ec8cf84b8a57995cf7f1e84ccad2704d93f05d0aae",
+                "sha256:b69c7adc7ed60da1cb1b502853db61f453fc745f940cbcc25eb97c99965d8f41",
+                "sha256:be1bf35ce82cdbcac14e39d5102d8de4079a1c1a6a06b68e41fcd9ef64f9dd28",
+                "sha256:be7b2265b7527bb12109a7727581e274170766d5b3c9258d4e466f4872522d7a",
+                "sha256:c02abd55409bfb293371554adf6a4401197ec2133dd97727c01180889014ba4d",
+                "sha256:c831f31336e81243f85b6daff3e5e8a123302ce0ea1f2726ad752fd7a59f3aee",
+                "sha256:cd0daac21d9ef5e033a5100c1d3aa055bbed28bfcf070b12d8058045c4e821b1",
+                "sha256:cd9a5e68e79c5f031500e67793048a90209711e0854a9ddee8a3ce51728de4e5",
+                "sha256:d5cd1389669a847555df54177b911d9ff6f17345b2a6f19388707b7a9f724c88",
+                "sha256:d81528ffe0e973dc840ec73a4132fd18b8203ad129d7410155d951a0a7e4f5d0",
+                "sha256:e860a3222139b41d430939bbec2ec9c3f6c740938bf7a04471a9a8caaa965a2e",
+                "sha256:e95c7ccd4c5807adef1602005513bf7c7d14e5a41daebcf9d8d30d8bf51b8f81",
+                "sha256:eafbe7501a3268d05f2e450e1ddaffb950d842a8620c13ec328b501d25d2e2c3",
+                "sha256:eef0450a4b5ed11feab639bf3eb1b6e23d0efa9b911bf7b06fb60e14f5f8a585",
+                "sha256:f601aaeae18dab81930fb8d4f916b0da21e89bb4b5f7367ef793f46b4a76b7b0",
+                "sha256:f7a0d0bf44438869d307f85a54f25a896ad6b4b0ca12370f76892ad732928d87",
+                "sha256:ffaaf7e93fcb437356b5a4b23bf36e8a3d0221399ff77fd057e4bc77776a24be"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.51.1"
+            "version": "==1.51.3"
         },
         "grpcio-status": {
             "hashes": [
                 "sha256:5357dcd69e51ba3f7b86d57698bd44d2ef295528eb7219b237eb596183334d39",
                 "sha256:78442ac7d2813c56f9cc04f713efd7088596b10f88a4ddd09279211cc48402d5"
             ],
             "index": "pypi",
@@ -210,19 +210,19 @@
                 "sha256:fa404d7c9cd621836220f3b9cb593eb2c475182d5c768b449407506b61f91159"
             ],
             "index": "pypi",
             "version": "==1.46.3"
         },
         "natsort": {
             "hashes": [
-                "sha256:04fe18fdd2b9e5957f19f687eb117f102ef8dde6b574764e536e91194bed4f5f",
-                "sha256:57f85b72c688b09e053cdac302dd5b5b53df5f73ae20b4874fcbffd8bf783d11"
+                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
+                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
             ],
             "index": "pypi",
-            "version": "==8.2.0"
+            "version": "==8.3.1"
         },
         "numpy": {
             "hashes": [
                 "sha256:1dbe1c91269f880e364526649a52eff93ac30035507ae980d2fed33aaee633ac",
                 "sha256:357768c2e4451ac241465157a3e929b265dfac85d9214074985b1786244f2ef3",
                 "sha256:3820724272f9913b597ccd13a467cc492a0da6b05df26ea09e78b171a0bb9da6",
                 "sha256:4391bd07606be175aafd267ef9bea87cf1b8210c787666ce82073b05f202add1",
@@ -307,53 +307,53 @@
                 "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
             ],
             "index": "pypi",
             "version": "==1.5.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:a78d01d1e2c175c474884671dde039962c9d74c7223db7369771fcf6e29ceeab",
-                "sha256:bd6eb2d6722568de6d14b87c44a96fac54b2a45ff5e940e639979a3d1792adb6"
+                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
+                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==66.0.0"
+            "version": "==67.6.0"
         },
         "tqdm": {
             "hashes": [
-                "sha256:5f4f682a004951c1b450bc753c710e9280c5746ce6ffedee253ddbcbf54cf1e4",
-                "sha256:6fee160d6ffcd1b1c68c65f14c829c22832bc401726335ce92c52d395944a6a1"
+                "sha256:1871fb68a86b8fb3b59ca4cdd3dcccbc7e6d613eeed31f4c332531977b89beb5",
+                "sha256:c4f53a17fe37e132815abceec022631be8ffe1b9381c2e6e30aa70edc99e9671"
             ],
             "index": "pypi",
-            "version": "==4.64.1"
+            "version": "==4.65.0"
         }
     },
     "develop": {
         "attrs": {
             "hashes": [
                 "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
                 "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==22.2.0"
         },
         "autopep8": {
             "hashes": [
-                "sha256:be5bc98c33515b67475420b7b1feafc8d32c1a69862498eda4983b45bffd2687",
-                "sha256:d27a8929d8dcd21c0f4b3859d2d07c6c25273727b98afc984c039df0f0d86566"
+                "sha256:86e9303b5e5c8160872b2f5ef611161b2893e9bfe8ccc7e2f76385947d57a2f1",
+                "sha256:f9849cdd62108cb739dbcdbfb7fdcc9a30d1b63c4cc3e1c1f893b5360941b61c"
             ],
             "index": "pypi",
-            "version": "==2.0.1"
+            "version": "==2.0.2"
         },
         "cachetools": {
             "hashes": [
-                "sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe",
-                "sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da"
+                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
+                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
-            "version": "==5.2.1"
+            "version": "==5.3.0"
         },
         "chardet": {
             "hashes": [
                 "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
                 "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
             "markers": "python_version >= '3.7'",
@@ -372,118 +372,107 @@
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:75997740323c5f12e18f10b494bc11c03e42843129f980f17c04352cc7b09d40",
+                "sha256:eb8f0f2d37ed68223ea63e3bddf2fac99667e4362c88b3f762e434d160190d18"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.10.2"
         },
         "flake8": {
             "hashes": [
                 "sha256:326a54ace7878a5ad1538110f2145bc6a134df43fff290475fd4e7ba38a6deea",
                 "sha256:80a66cd9bd66b0679da030fc930c0a4d09237dd72f354d899427b5c6718223b9"
             ],
             "index": "pypi",
             "version": "==2.5.5"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
+                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
             ],
             "markers": "python_version < '3.8'",
-            "version": "==6.0.0"
+            "version": "==6.1.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "isort": {
             "hashes": [
-                "sha256:6db30c5ded9815d813932c04c2f85a360bcdd35fed496f4d8f35495ef0a261b6",
-                "sha256:c033fd0edb91000a7f09527fe5c75321878f98322a77ddcc81adbd83724afb7b"
+                "sha256:6be1f76a507cb2ecf16c7cf14a37e41609ca082330be4e3436a18ef74add55db",
+                "sha256:ba1d72fb2595a01c7895a5128f9585a5cc4b6d395f1c8d514989b9a7eb2a8746"
             ],
             "index": "pypi",
-            "version": "==5.11.4"
+            "version": "==5.11.5"
         },
         "mccabe": {
             "hashes": [
                 "sha256:9a2b12ebd876e77c72e41ebf401cc2e7c5b566649d50105ca49822688642207b",
                 "sha256:cbc2938f6c01061bc6d21d0c838c2489664755cb18676f0734d7617f4577d09e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.4.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:0714258640194d75677e86c786e80ccf294972cc76885d3ebbb560f11db0003d",
-                "sha256:0c8f3be99e8a8bd403caa8c03be619544bc2c77a7093685dcf308c6b109426c6",
-                "sha256:0cca5adf694af539aeaa6ac633a7afe9bbd760df9d31be55ab780b77ab5ae8bf",
-                "sha256:1c8cd4fb70e8584ca1ed5805cbc7c017a3d1a29fb450621089ffed3e99d1857f",
-                "sha256:1f7d1a520373e2272b10796c3ff721ea1a0712288cafaa95931e66aa15798813",
-                "sha256:209ee89fbb0deed518605edddd234af80506aec932ad28d73c08f1400ef80a33",
-                "sha256:26efb2fcc6b67e4d5a55561f39176821d2adf88f2745ddc72751b7890f3194ad",
-                "sha256:37bd02ebf9d10e05b00d71302d2c2e6ca333e6c2a8584a98c00e038db8121f05",
-                "sha256:3a700330b567114b673cf8ee7388e949f843b356a73b5ab22dd7cff4742a5297",
-                "sha256:3c0165ba8f354a6d9881809ef29f1a9318a236a6d81c690094c5df32107bde06",
-                "sha256:3d80e36b7d7a9259b740be6d8d906221789b0d836201af4234093cae89ced0cd",
-                "sha256:4175593dc25d9da12f7de8de873a33f9b2b8bdb4e827a7cae952e5b1a342e243",
-                "sha256:4307270436fd7694b41f913eb09210faff27ea4979ecbcd849e57d2da2f65305",
-                "sha256:5e80e758243b97b618cdf22004beb09e8a2de1af481382e4d84bc52152d1c476",
-                "sha256:641411733b127c3e0dab94c45af15fea99e4468f99ac88b39efb1ad677da5711",
-                "sha256:652b651d42f155033a1967739788c436491b577b6a44e4c39fb340d0ee7f0d70",
-                "sha256:6d7464bac72a85cb3491c7e92b5b62f3dcccb8af26826257760a552a5e244aa5",
-                "sha256:74e259b5c19f70d35fcc1ad3d56499065c601dfe94ff67ae48b85596b9ec1461",
-                "sha256:7d17e0a9707d0772f4a7b878f04b4fd11f6f5bcb9b3813975a9b13c9332153ab",
-                "sha256:901c2c269c616e6cb0998b33d4adbb4a6af0ac4ce5cd078afd7bc95830e62c1c",
-                "sha256:98e781cd35c0acf33eb0295e8b9c55cdbef64fcb35f6d3aa2186f289bed6e80d",
-                "sha256:a12c56bf73cdab116df96e4ff39610b92a348cc99a1307e1da3c3768bbb5b135",
-                "sha256:ac6e503823143464538efda0e8e356d871557ef60ccd38f8824a4257acc18d93",
-                "sha256:b8472f736a5bfb159a5e36740847808f6f5b659960115ff29c7cecec1741c648",
-                "sha256:b86ce2c1866a748c0f6faca5232059f881cda6dda2a893b9a8373353cfe3715a",
-                "sha256:bc9ec663ed6c8f15f4ae9d3c04c989b744436c16d26580eaa760ae9dd5d662eb",
-                "sha256:c9166b3f81a10cdf9b49f2d594b21b31adadb3d5e9db9b834866c3258b695be3",
-                "sha256:d13674f3fb73805ba0c45eb6c0c3053d218aa1f7abead6e446d474529aafc372",
-                "sha256:de32edc9b0a7e67c2775e574cb061a537660e51210fbf6006b0b36ea695ae9bb",
-                "sha256:e62ebaad93be3ad1a828a11e90f0e76f15449371ffeecca4a0a0b9adc99abcef"
+                "sha256:0a28a76785bf57655a8ea5eb0540a15b0e781c807b5aa798bd463779988fa1d5",
+                "sha256:19ba15f9627a5723e522d007fe708007bae52b93faab00f95d72f03e1afa9598",
+                "sha256:21b437be1c02712a605591e1ed1d858aba681757a1e55fe678a15c2244cd68a5",
+                "sha256:26cdd6a22b9b40b2fd71881a8a4f34b4d7914c679f154f43385ca878a8297389",
+                "sha256:2888ce4fe5aae5a673386fa232473014056967f3904f5abfcf6367b5af1f612a",
+                "sha256:2b0c373d071593deefbcdd87ec8db91ea13bd8f1328d44947e88beae21e8d5e9",
+                "sha256:315ac73cc1cce4771c27d426b7ea558fb4e2836f89cb0296cbe056894e3a1f78",
+                "sha256:39c7119335be05630611ee798cc982623b9e8f0cff04a0b48dfc26100e0b97af",
+                "sha256:4b398d8b1f4fba0e3c6463e02f8ad3346f71956b92287af22c9b12c3ec965a9f",
+                "sha256:4e4e8b362cdf99ba00c2b218036002bdcdf1e0de085cdb296a49df03fb31dfc4",
+                "sha256:59bbd71e5c58eed2e992ce6523180e03c221dcd92b52f0e792f291d67b15a71c",
+                "sha256:5b5f81b40d94c785f288948c16e1f2da37203c6006546c5d947aab6f90aefef2",
+                "sha256:5cb14ff9919b7df3538590fc4d4c49a0f84392237cbf5f7a816b4161c061829e",
+                "sha256:61bf08362e93b6b12fad3eab68c4ea903a077b87c90ac06c11e3d7a09b56b9c1",
+                "sha256:64cc3afb3e9e71a79d06e3ed24bb508a6d66f782aff7e56f628bf35ba2e0ba51",
+                "sha256:69b35d1dcb5707382810765ed34da9db47e7f95b3528334a3c999b0c90fe523f",
+                "sha256:9401e33814cec6aec8c03a9548e9385e0e228fc1b8b0a37b9ea21038e64cdd8a",
+                "sha256:a380c041db500e1410bb5b16b3c1c35e61e773a5c3517926b81dfdab7582be54",
+                "sha256:ae9ceae0f5b9059f33dbc62dea087e942c0ccab4b7a003719cb70f9b8abfa32f",
+                "sha256:b7c7b708fe9a871a96626d61912e3f4ddd365bf7f39128362bc50cbd74a634d5",
+                "sha256:c1c10fa12df1232c936830839e2e935d090fc9ee315744ac33b8a32216b93707",
+                "sha256:ce61663faf7a8e5ec6f456857bfbcec2901fbdb3ad958b778403f63b9e606a1b",
+                "sha256:d64c28e03ce40d5303450f547e07418c64c241669ab20610f273c9e6290b4b0b",
+                "sha256:d809f88734f44a0d44959d795b1e6f64b2bbe0ea4d9cc4776aa588bb4229fc1c",
+                "sha256:dbb19c9f662e41e474e0cff502b7064a7edc6764f5262b6cd91d698163196799",
+                "sha256:ef6a01e563ec6a4940784c574d33f6ac1943864634517984471642908b30b6f7"
             ],
             "index": "pypi",
-            "version": "==0.991"
+            "version": "==1.1.1"
         },
         "mypy-extensions": {
             "hashes": [
-                "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d",
-                "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
-            "version": "==0.4.3"
-        },
-        "mypy-protobuf": {
-            "hashes": [
-                "sha256:7d75a079651b105076776a35a5405e3fa773b8a167118f1b712e443e9a6c18a2",
-                "sha256:da33dfde7547ff57e5ba5564126cbfa114f14413b2fa50759b1fa5de1e4ab511"
-            ],
-            "index": "pypi",
-            "version": "==3.4.0"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
                 "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
             ],
             "markers": "python_version >= '3.7'",
@@ -494,57 +483,28 @@
                 "sha256:b22cfae5db09833bb9bd7c8463b53e1a9c9b39f12e304a8d0bba729c501827ee",
                 "sha256:fe249b52e20498e59e0b5c5256aa52ee99fc295b26ec9eaa85776ffdb9fe6374"
             ],
             "version": "==1.7.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490",
-                "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"
+                "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa",
+                "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.2"
+            "version": "==3.1.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
-        "protobuf": {
-            "hashes": [
-                "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7",
-                "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c",
-                "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2",
-                "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b",
-                "sha256:44246bab5dd4b7fbd3c0c80b6f16686808fab0e4aca819ade6e8d294a29c7050",
-                "sha256:447d43819997825d4e71bf5769d869b968ce96848b6479397e29fc24c4a5dfe9",
-                "sha256:67a3598f0a2dcbc58d02dd1928544e7d88f764b47d4a286202913f0b2801c2e7",
-                "sha256:74480f79a023f90dc6e18febbf7b8bac7508420f2006fabd512013c0c238f454",
-                "sha256:819559cafa1a373b7096a482b504ae8a857c89593cf3a25af743ac9ecbd23480",
-                "sha256:899dc660cd599d7352d6f10d83c95df430a38b410c1b66b407a6b29265d66469",
-                "sha256:8c0c984a1b8fef4086329ff8dd19ac77576b384079247c770f29cc8ce3afa06c",
-                "sha256:9aae4406ea63d825636cc11ffb34ad3379335803216ee3a856787bcf5ccc751e",
-                "sha256:a7ca6d488aa8ff7f329d4c545b2dbad8ac31464f1d8b1c87ad1346717731e4db",
-                "sha256:b6cc7ba72a8850621bfec987cb72623e703b7fe2b9127a161ce61e61558ad905",
-                "sha256:bf01b5720be110540be4286e791db73f84a2b721072a3711efff6c324cdf074b",
-                "sha256:c02ce36ec760252242a33967d51c289fd0e1c0e6e5cc9397e2279177716add86",
-                "sha256:d9e4432ff660d67d775c66ac42a67cf2453c27cb4d738fc22cb53b5d84c135d4",
-                "sha256:daa564862dd0d39c00f8086f88700fdbe8bc717e993a21e90711acfed02f2402",
-                "sha256:de78575669dddf6099a8a0f46a27e82a1783c557ccc38ee620ed8cc96d3be7d7",
-                "sha256:e64857f395505ebf3d2569935506ae0dfc4a15cb80dc25261176c784662cdcc4",
-                "sha256:e67f9af1b607eb3a89aafc9bc68a9d1172aae788b2445cb9fd781bd97531f1f1",
-                "sha256:f4bd856d702e5b0d96a00ec6b307b0f51c1982c2bf9c0052cf9019e9a544ba99",
-                "sha256:f4c42102bc82a51108e449cbb32b19b180022941c727bac0cfd50170341f16ee"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.20.3"
-        },
         "pycodestyle": {
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.10.0"
@@ -555,43 +515,43 @@
                 "sha256:f39e33a4c03beead8774f005bd3ecf0c3f2f264fa0201de965fce0aff1d34263"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pyproject-api": {
             "hashes": [
-                "sha256:0962df21f3e633b8ddb9567c011e6c1b3dcdfc31b7860c0ede7e24c5a1200fbe",
-                "sha256:4c111277dfb96bcd562c6245428f27250b794bfe3e210b8714c4f893952f2c17"
+                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
+                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.0"
+            "version": "==1.5.1"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
+                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.2.2"
         },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:307993257d792a12a63ff86a0b67a71a5ab2d4a2cc12bbae947115224d4ac3fb",
-                "sha256:6dddc4c69718b65aacbef0921ffa8af065b0f63ff0b24ffc403477975853c918"
+                "sha256:52c92a96e2c3fd47c5301e9c26f5a871466133d5376958c1ed95ef4ff4629cbe",
+                "sha256:da10ca1d809b99fae80b706b9dc9656b1daf505a395ac427d130a8a85502d08f"
             ],
             "index": "pypi",
-            "version": "==4.3.5"
+            "version": "==4.4.7"
         },
         "typed-ast": {
             "hashes": [
                 "sha256:0261195c2062caf107831e92a76764c81227dae162c4f75192c0d489faf751a2",
                 "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1",
                 "sha256:183afdf0ec5b1b211724dfef3d2cad2d767cbefac291f24d69b00546c1837fb6",
                 "sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62",
@@ -617,55 +577,55 @@
                 "sha256:ed855bbe3eb3715fca349c80174cfcfd699c2f9de574d40527b8429acae23a66"
             ],
             "markers": "python_version < '3.8'",
             "version": "==1.5.4"
         },
         "types-protobuf": {
             "hashes": [
-                "sha256:6c87c7f8df61d57a53de8221777e4fcc3c7ed24419fbf43b8e9f50887f3773fa",
-                "sha256:824109e0fe87525a9d2da4cc4eec36ca004f1a0f3d1c0838cfd2873a484cffdd"
+                "sha256:1e59294618c9518f35f17ae1a3d866cdf7e998eb4b9907d41e9ebe5b84fde636",
+                "sha256:bf2b414d815dc387c0a041d9207db054c7cdb94591bb233d9b71a85243e05efc"
             ],
             "index": "pypi",
-            "version": "==4.21.0.3"
+            "version": "==4.22.0.0"
         },
         "types-tabulate": {
             "hashes": [
-                "sha256:4a79474714cea156bcd2185bb9bddd8fb9d3d5227c8d0a7f21bf21caf5f60e67",
-                "sha256:a1cc2aa52d2a9abfe0acbb361ccd49e3400794086a41626ce8784ed2e1ec0b0d"
+                "sha256:be2ea0de05f615ccfcbadf6206aa720e265955eb1de23e343aec9d8bf3fa9aaa",
+                "sha256:e486292c279f19247865bdabe802419740a0e74b53444e7f7a8009e08129da5d"
             ],
             "index": "pypi",
-            "version": "==0.9.0.0"
+            "version": "==0.9.0.1"
         },
         "types-tqdm": {
             "hashes": [
-                "sha256:b7fb2daec65722cd92a4fb377b0c9575ce19d6012a1875b48bc14a44c72db546",
-                "sha256:ba8deb1ba9370403ef2bacc4d61267af23b5b1f135dd14d516769b04cbf49615"
+                "sha256:3377b5e34396b4e1661f8df7390051490918b8be36ae0f7b6864c1d806e95ef5",
+                "sha256:8707a0dd16a1f2061e316ddc5ef07908d7465193f0d2ed24be75b55e6b9e6cbe"
             ],
             "index": "pypi",
-            "version": "==4.64.7.11"
+            "version": "==4.65.0.0"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
+                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.4.0"
+            "version": "==4.5.0"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4",
-                "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==20.17.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.21.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa",
-                "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `quickmpc-0.3.1/README-ja.md` & `quickmpc-0.3.2/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/README.md` & `quickmpc-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/README-ja.md` & `quickmpc-0.3.2/demo/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/README.md` & `quickmpc-0.3.2/demo/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/integration_demo/execute_demo.py` & `quickmpc-0.3.2/demo/integration_demo/execute_demo.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/integration_demo/progress_demo.py` & `quickmpc-0.3.2/demo/integration_demo/progress_demo.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/unit_demo/delete_share.py` & `quickmpc-0.3.2/demo/unit_demo/delete_share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/unit_demo/demo_sharize.py` & `quickmpc-0.3.2/demo/unit_demo/demo_sharize.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/unit_demo/execute_computation.py` & `quickmpc-0.3.2/demo/unit_demo/execute_computation.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/unit_demo/get_computation_result.py` & `quickmpc-0.3.2/demo/unit_demo/get_computation_result.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/unit_demo/get_elapsed_time.py` & `quickmpc-0.3.2/demo/unit_demo/get_elapsed_time.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/unit_demo/get_join_table.py` & `quickmpc-0.3.2/demo/unit_demo/get_join_table.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/demo/unit_demo/send_share.py` & `quickmpc-0.3.2/demo/unit_demo/send_share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/mypy.ini` & `quickmpc-0.3.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/quickmpc/README.md` & `quickmpc-0.3.2/quickmpc/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # QuickMPC-libClient-pyが提供する機能
 
 ## QMPC.parse_csv_file
 csvファイルからテーブルデータを読み込んでパースする．
 ### Parameters
 - file: `str`
 	- 読み込むファイル名
@@ -146,50 +145,14 @@
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
 	- res["job_id"]: `str`
 		- 計算スレッドのID
 
-## QMPC.linear_regression
-線形回帰の学習を行う
-### Parameters
-- join_order: `Tuple[List[str], List[int], List[int]]`
-	- join_order[0]: data_idのリスト
-	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
-	- join_order[2]: 結合に用いるIDの列リスト
-	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
-- inp: `Tuple[List[int], List[int]]`
-	- inp[0]: 設計変数行列のリスト
-	- inp[1]: 目的値の列リスト
-### Returns
-- res: `Dict`
-	- res["is_ok"]: `bool`
-		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
-
-## QMPC.logistic_regression
-ロジスティック回帰の学習を行う
-### Parameters
-- join_order: `Tuple[List[str], List[int], List[int]]`
-	- join_order[0]: data_idのリスト
-	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
-	- join_order[2]: 結合に用いるIDの列リスト
-	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
-- inp: `Tuple[List[int], List[int]]`
-	- inp[0]: 設計変数行列のリスト
-	- inp[1]: 目的値の列リスト
-### Returns
-- res: `Dict`
-	- res["is_ok"]: `bool`
-		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
-
 ## QMPC.meshcode
 メッシュコードを計算する
 ### Parameters
 - join_order: `Tuple[List[str], List[int], List[int]]`
 	- join_order[0]: data_idのリスト
 	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
 	- join_order[2]: 結合に用いるIDの列リスト
@@ -199,32 +162,14 @@
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
 	- res["job_id"]: `str`
 		- 計算スレッドのID
 
-## QMPC.decision_tree
-決定木の学習を行う
-### Parameters
-- join_order: `Tuple[List[str], List[int], List[int]]`
-	- join_order[0]: data_idのリスト
-	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
-	- join_order[2]: 結合に用いるIDの列リスト
-	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
-- inp: `Tuple[List[int], List[int]]`
-	- inp[0]: 設計変数行列のリスト
-	- inp[1]: 目的値の列リスト
-### Returns
-- res: `Dict`
-	- res["is_ok"]: `bool`
-		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
-
 ## QMPC.get_join_table
 テーブルを結合する
 ### Parameters
 - join_order: `Tuple[List[str], List[int], List[int]]`
 	- join_order[0]: data_idのリスト
 	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
 	- join_order[2]: 結合に用いるIDの列リスト
```

### Comparing `quickmpc-0.3.1/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x63ommon_types/common_types.proto\x12\x0fpb_common_types\"{\n\x11ProcedureProgress\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x10\n\x08progress\x18\x03 \x01(\x02\x12\x11\n\tcompleted\x18\x04 \x01(\x08\x12\x14\n\x07\x64\x65tails\x18\x05 \x01(\tH\x00\x88\x01\x01\x42\n\n\x08_details\"\x83\x01\n\x0bJobProgress\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12*\n\x06status\x18\x02 \x01(\x0e\x32\x1a.pb_common_types.JobStatus\x12\x36\n\nprogresses\x18\x03 \x03(\x0b\x32\".pb_common_types.ProcedureProgress\"\x8d\x01\n\nStacktrace\x12\x31\n\x06\x66rames\x18\x01 \x03(\x0b\x32!.pb_common_types.Stacktrace.Frame\x1aL\n\x05\x46rame\x12\x17\n\x0fsource_location\x18\x01 \x01(\t\x12\x13\n\x0bsource_line\x18\x02 \x01(\x04\x12\x15\n\rfunction_name\x18\x03 \x01(\t\"\x93\x01\n\x0cJobErrorInfo\x12\x0c\n\x04what\x18\x01 \x01(\t\x12\x1c\n\x0f\x61\x64\x64itional_info\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x34\n\nstacktrace\x18\x03 \x01(\x0b\x32\x1b.pb_common_types.StacktraceH\x01\x88\x01\x01\x42\x12\n\x10_additional_infoB\r\n\x0b_stacktrace\"I\n\x06Schema\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.pb_common_types.ShareValueTypeEnum*Y\n\tJobStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x0b\n\x07PRE_JOB\x10\x02\x12\x0b\n\x07READ_DB\x10\x03\x12\x0b\n\x07\x43OMPUTE\x10\x04\x12\r\n\tCOMPLETED\x10\x05*\xf5\x01\n\x11\x43omputationMethod\x12\"\n\x1e\x43OMPUTATION_METHOD_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x43OMPUTATION_METHOD_MEAN\x10\x01\x12\x1f\n\x1b\x43OMPUTATION_METHOD_VARIANCE\x10\x02\x12\x1a\n\x16\x43OMPUTATION_METHOD_SUM\x10\x03\x12\x1d\n\x19\x43OMPUTATION_METHOD_CORREL\x10\x04\x12 \n\x1c\x43OMPUTATION_METHOD_MESH_CODE\x10\x05\x12!\n\x1d\x43OMPUTATION_METHOD_JOIN_TABLE\x10\x06*\x8b\x01\n\x12ShareValueTypeEnum\x12 \n\x1cSHARE_VALUE_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1cSHARE_VALUE_TYPE_FIXED_POINT\x10\x01\x12\x31\n-SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION\x10\x02\x42\x39Z7github.com/acompany-develop/QuickMPC/proto/common_typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x63ommon_types/common_types.proto\x12\x0fpb_common_types\"{\n\x11ProcedureProgress\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x10\n\x08progress\x18\x03 \x01(\x02\x12\x11\n\tcompleted\x18\x04 \x01(\x08\x12\x14\n\x07\x64\x65tails\x18\x05 \x01(\tH\x00\x88\x01\x01\x42\n\n\x08_details\"\x83\x01\n\x0bJobProgress\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12*\n\x06status\x18\x02 \x01(\x0e\x32\x1a.pb_common_types.JobStatus\x12\x36\n\nprogresses\x18\x03 \x03(\x0b\x32\".pb_common_types.ProcedureProgress\"\x8d\x01\n\nStacktrace\x12\x31\n\x06\x66rames\x18\x01 \x03(\x0b\x32!.pb_common_types.Stacktrace.Frame\x1aL\n\x05\x46rame\x12\x17\n\x0fsource_location\x18\x01 \x01(\t\x12\x13\n\x0bsource_line\x18\x02 \x01(\x04\x12\x15\n\rfunction_name\x18\x03 \x01(\t\"\x93\x01\n\x0cJobErrorInfo\x12\x0c\n\x04what\x18\x01 \x01(\t\x12\x1c\n\x0f\x61\x64\x64itional_info\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x34\n\nstacktrace\x18\x03 \x01(\x0b\x32\x1b.pb_common_types.StacktraceH\x01\x88\x01\x01\x42\x12\n\x10_additional_infoB\r\n\x0b_stacktrace\"I\n\x06Schema\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.pb_common_types.ShareValueTypeEnum*g\n\tJobStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x0c\n\x08RECEIVED\x10\x02\x12\x0b\n\x07PRE_JOB\x10\x03\x12\x0b\n\x07READ_DB\x10\x04\x12\x0b\n\x07\x43OMPUTE\x10\x05\x12\r\n\tCOMPLETED\x10\x06*\xf5\x01\n\x11\x43omputationMethod\x12\"\n\x1e\x43OMPUTATION_METHOD_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x43OMPUTATION_METHOD_MEAN\x10\x01\x12\x1f\n\x1b\x43OMPUTATION_METHOD_VARIANCE\x10\x02\x12\x1a\n\x16\x43OMPUTATION_METHOD_SUM\x10\x03\x12\x1d\n\x19\x43OMPUTATION_METHOD_CORREL\x10\x04\x12 \n\x1c\x43OMPUTATION_METHOD_MESH_CODE\x10\x05\x12!\n\x1d\x43OMPUTATION_METHOD_JOIN_TABLE\x10\x06*\x8b\x01\n\x12ShareValueTypeEnum\x12 \n\x1cSHARE_VALUE_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1cSHARE_VALUE_TYPE_FIXED_POINT\x10\x01\x12\x31\n-SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION\x10\x02\x42\x39Z7github.com/acompany-develop/QuickMPC/proto/common_typesb\x06proto3')
 
 _JOBSTATUS = DESCRIPTOR.enum_types_by_name['JobStatus']
 JobStatus = enum_type_wrapper.EnumTypeWrapper(_JOBSTATUS)
 _COMPUTATIONMETHOD = DESCRIPTOR.enum_types_by_name['ComputationMethod']
 ComputationMethod = enum_type_wrapper.EnumTypeWrapper(_COMPUTATIONMETHOD)
 _SHAREVALUETYPEENUM = DESCRIPTOR.enum_types_by_name['ShareValueTypeEnum']
 ShareValueTypeEnum = enum_type_wrapper.EnumTypeWrapper(_SHAREVALUETYPEENUM)
 UNKNOWN = 0
 ERROR = 1
-PRE_JOB = 2
-READ_DB = 3
-COMPUTE = 4
-COMPLETED = 5
+RECEIVED = 2
+PRE_JOB = 3
+READ_DB = 4
+COMPUTE = 5
+COMPLETED = 6
 COMPUTATION_METHOD_UNSPECIFIED = 0
 COMPUTATION_METHOD_MEAN = 1
 COMPUTATION_METHOD_VARIANCE = 2
 COMPUTATION_METHOD_SUM = 3
 COMPUTATION_METHOD_CORREL = 4
 COMPUTATION_METHOD_MESH_CODE = 5
 COMPUTATION_METHOD_JOIN_TABLE = 6
@@ -88,19 +89,19 @@
 _sym_db.RegisterMessage(Schema)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'Z7github.com/acompany-develop/QuickMPC/proto/common_types'
     _JOBSTATUS._serialized_start = 680
-    _JOBSTATUS._serialized_end = 769
-    _COMPUTATIONMETHOD._serialized_start = 772
-    _COMPUTATIONMETHOD._serialized_end = 1017
-    _SHAREVALUETYPEENUM._serialized_start = 1020
-    _SHAREVALUETYPEENUM._serialized_end = 1159
+    _JOBSTATUS._serialized_end = 783
+    _COMPUTATIONMETHOD._serialized_start = 786
+    _COMPUTATIONMETHOD._serialized_end = 1031
+    _SHAREVALUETYPEENUM._serialized_start = 1034
+    _SHAREVALUETYPEENUM._serialized_end = 1173
     _PROCEDUREPROGRESS._serialized_start = 52
     _PROCEDUREPROGRESS._serialized_end = 175
     _JOBPROGRESS._serialized_start = 178
     _JOBPROGRESS._serialized_end = 309
     _STACKTRACE._serialized_start = 312
     _STACKTRACE._serialized_end = 453
     _STACKTRACE_FRAME._serialized_start = 377
```

### Comparing `quickmpc-0.3.1/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -18,38 +18,40 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _JobStatus:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _JobStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_JobStatus.ValueType], builtins.type):
+class _JobStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_JobStatus.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN: _JobStatus.ValueType  # 0
     ERROR: _JobStatus.ValueType  # 1
-    PRE_JOB: _JobStatus.ValueType  # 2
-    READ_DB: _JobStatus.ValueType  # 3
-    COMPUTE: _JobStatus.ValueType  # 4
-    COMPLETED: _JobStatus.ValueType  # 5
+    RECEIVED: _JobStatus.ValueType  # 2
+    PRE_JOB: _JobStatus.ValueType  # 3
+    READ_DB: _JobStatus.ValueType  # 4
+    COMPUTE: _JobStatus.ValueType  # 5
+    COMPLETED: _JobStatus.ValueType  # 6
 
 class JobStatus(_JobStatus, metaclass=_JobStatusEnumTypeWrapper): ...
 
 UNKNOWN: JobStatus.ValueType  # 0
 ERROR: JobStatus.ValueType  # 1
-PRE_JOB: JobStatus.ValueType  # 2
-READ_DB: JobStatus.ValueType  # 3
-COMPUTE: JobStatus.ValueType  # 4
-COMPLETED: JobStatus.ValueType  # 5
+RECEIVED: JobStatus.ValueType  # 2
+PRE_JOB: JobStatus.ValueType  # 3
+READ_DB: JobStatus.ValueType  # 4
+COMPUTE: JobStatus.ValueType  # 5
+COMPLETED: JobStatus.ValueType  # 6
 global___JobStatus = JobStatus
 
 class _ComputationMethod:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ComputationMethodEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ComputationMethod.ValueType], builtins.type):
+class _ComputationMethodEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ComputationMethod.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     COMPUTATION_METHOD_UNSPECIFIED: _ComputationMethod.ValueType  # 0
     COMPUTATION_METHOD_MEAN: _ComputationMethod.ValueType  # 1
     COMPUTATION_METHOD_VARIANCE: _ComputationMethod.ValueType  # 2
     COMPUTATION_METHOD_SUM: _ComputationMethod.ValueType  # 3
     COMPUTATION_METHOD_CORREL: _ComputationMethod.ValueType  # 4
     COMPUTATION_METHOD_MESH_CODE: _ComputationMethod.ValueType  # 5
@@ -66,28 +68,27 @@
 COMPUTATION_METHOD_JOIN_TABLE: ComputationMethod.ValueType  # 6
 global___ComputationMethod = ComputationMethod
 
 class _ShareValueTypeEnum:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ShareValueTypeEnumEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ShareValueTypeEnum.ValueType], builtins.type):
+class _ShareValueTypeEnumEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ShareValueTypeEnum.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SHARE_VALUE_TYPE_UNSPECIFIED: _ShareValueTypeEnum.ValueType  # 0
     SHARE_VALUE_TYPE_FIXED_POINT: _ShareValueTypeEnum.ValueType  # 1
     SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION: _ShareValueTypeEnum.ValueType  # 2
 
 class ShareValueTypeEnum(_ShareValueTypeEnum, metaclass=_ShareValueTypeEnumEnumTypeWrapper): ...
 
 SHARE_VALUE_TYPE_UNSPECIFIED: ShareValueTypeEnum.ValueType  # 0
 SHARE_VALUE_TYPE_FIXED_POINT: ShareValueTypeEnum.ValueType  # 1
 SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION: ShareValueTypeEnum.ValueType  # 2
 global___ShareValueTypeEnum = ShareValueTypeEnum
 
-@typing_extensions.final
 class ProcedureProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     PROGRESS_FIELD_NUMBER: builtins.int
     COMPLETED_FIELD_NUMBER: builtins.int
@@ -113,15 +114,14 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_details", b"_details", "details", b"details"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_details", b"_details", "completed", b"completed", "description", b"description", "details", b"details", "id", b"id", "progress", b"progress"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_details", b"_details"]) -> typing_extensions.Literal["details"] | None: ...
 
 global___ProcedureProgress = ProcedureProgress
 
-@typing_extensions.final
 class JobProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     PROGRESSES_FIELD_NUMBER: builtins.int
     job_uuid: builtins.str
@@ -135,19 +135,17 @@
         status: global___JobStatus.ValueType = ...,
         progresses: collections.abc.Iterable[global___ProcedureProgress] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "progresses", b"progresses", "status", b"status"]) -> None: ...
 
 global___JobProgress = JobProgress
 
-@typing_extensions.final
 class Stacktrace(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
     class Frame(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         SOURCE_LOCATION_FIELD_NUMBER: builtins.int
         SOURCE_LINE_FIELD_NUMBER: builtins.int
         FUNCTION_NAME_FIELD_NUMBER: builtins.int
         source_location: builtins.str
@@ -170,15 +168,14 @@
         *,
         frames: collections.abc.Iterable[global___Stacktrace.Frame] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["frames", b"frames"]) -> None: ...
 
 global___Stacktrace = Stacktrace
 
-@typing_extensions.final
 class JobErrorInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WHAT_FIELD_NUMBER: builtins.int
     ADDITIONAL_INFO_FIELD_NUMBER: builtins.int
     STACKTRACE_FIELD_NUMBER: builtins.int
     what: builtins.str
@@ -197,15 +194,14 @@
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_additional_info", b"_additional_info"]) -> typing_extensions.Literal["additional_info"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_stacktrace", b"_stacktrace"]) -> typing_extensions.Literal["stacktrace"] | None: ...
 
 global___JobErrorInfo = JobErrorInfo
 
-@typing_extensions.final
 class Schema(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
     type: global___ShareValueTypeEnum.ValueType
```

### Comparing `quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
 class SendSharesRequest(google.protobuf.message.Message):
     """*
     the message of SendSharesRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -52,15 +51,14 @@
         matching_column: builtins.int = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id", "matching_column", b"matching_column", "piece_id", b"piece_id", "schema", b"schema", "sent_at", b"sent_at", "shares", b"shares", "token", b"token"]) -> None: ...
 
 global___SendSharesRequest = SendSharesRequest
 
-@typing_extensions.final
 class SendSharesResponse(google.protobuf.message.Message):
     """*
     the message of SendSharesResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -74,15 +72,14 @@
         message: builtins.str = ...,
         is_ok: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "message", b"message"]) -> None: ...
 
 global___SendSharesResponse = SendSharesResponse
 
-@typing_extensions.final
 class DeleteSharesRequest(google.protobuf.message.Message):
     """*
     the message of DeleteSharesRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -97,15 +94,14 @@
         dataIds: collections.abc.Iterable[builtins.str] | None = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["dataIds", b"dataIds", "token", b"token"]) -> None: ...
 
 global___DeleteSharesRequest = DeleteSharesRequest
 
-@typing_extensions.final
 class DeleteSharesResponse(google.protobuf.message.Message):
     """*
     the message of DeleteSharesResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -119,15 +115,14 @@
         message: builtins.str = ...,
         is_ok: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "message", b"message"]) -> None: ...
 
 global___DeleteSharesResponse = DeleteSharesResponse
 
-@typing_extensions.final
 class GetSchemaRequest(google.protobuf.message.Message):
     """*
     the message of GetSchemaRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -141,15 +136,14 @@
         data_id: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id", "token", b"token"]) -> None: ...
 
 global___GetSchemaRequest = GetSchemaRequest
 
-@typing_extensions.final
 class GetSchemaResponse(google.protobuf.message.Message):
     """*
     the message of GetSchemaResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -167,15 +161,14 @@
         is_ok: builtins.bool = ...,
         schema: collections.abc.Iterable[common_types.common_types_pb2.Schema] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "message", b"message", "schema", b"schema"]) -> None: ...
 
 global___GetSchemaResponse = GetSchemaResponse
 
-@typing_extensions.final
 class JoinOrder(google.protobuf.message.Message):
     """*
     the message of ExecuteComputationRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -195,15 +188,14 @@
         join: collections.abc.Iterable[builtins.int] | None = ...,
         index: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["dataIds", b"dataIds", "index", b"index", "join", b"join"]) -> None: ...
 
 global___JoinOrder = JoinOrder
 
-@typing_extensions.final
 class Input(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SRC_FIELD_NUMBER: builtins.int
     TARGET_FIELD_NUMBER: builtins.int
     @property
     def src(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
@@ -215,15 +207,14 @@
         src: collections.abc.Iterable[builtins.int] | None = ...,
         target: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["src", b"src", "target", b"target"]) -> None: ...
 
 global___Input = Input
 
-@typing_extensions.final
 class ExecuteComputationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     METHOD_ID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     TABLE_FIELD_NUMBER: builtins.int
     ARG_FIELD_NUMBER: builtins.int
@@ -242,15 +233,14 @@
         arg: global___Input | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["arg", b"arg", "table", b"table"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["arg", b"arg", "method_id", b"method_id", "table", b"table", "token", b"token"]) -> None: ...
 
 global___ExecuteComputationRequest = ExecuteComputationRequest
 
-@typing_extensions.final
 class ExecuteComputationResponse(google.protobuf.message.Message):
     """
     the message of ExecuteComputationResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -267,15 +257,14 @@
         is_ok: builtins.bool = ...,
         job_uuid: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "job_uuid", b"job_uuid", "message", b"message"]) -> None: ...
 
 global___ExecuteComputationResponse = ExecuteComputationResponse
 
-@typing_extensions.final
 class GetComputationResultRequest(google.protobuf.message.Message):
     """*
     the message of GetComputationResultRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -289,15 +278,14 @@
         job_uuid: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
 global___GetComputationResultRequest = GetComputationResultRequest
 
-@typing_extensions.final
 class GetComputationResultResponse(google.protobuf.message.Message):
     """*
     the message of GetComputationResultResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -342,30 +330,28 @@
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_progress", b"_progress"]) -> typing_extensions.Literal["progress"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["result_type", b"result_type"]) -> typing_extensions.Literal["is_dim1", "is_dim2", "is_schema"] | None: ...
 
 global___GetComputationResultResponse = GetComputationResultResponse
 
-@typing_extensions.final
 class GetDataListRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_FIELD_NUMBER: builtins.int
     token: builtins.str
     def __init__(
         self,
         *,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token", b"token"]) -> None: ...
 
 global___GetDataListRequest = GetDataListRequest
 
-@typing_extensions.final
 class GetDataListResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     IS_OK_FIELD_NUMBER: builtins.int
     result: builtins.str
     is_ok: builtins.bool
@@ -375,15 +361,14 @@
         result: builtins.str = ...,
         is_ok: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "result", b"result"]) -> None: ...
 
 global___GetDataListResponse = GetDataListResponse
 
-@typing_extensions.final
 class GetElapsedTimeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     job_uuid: builtins.str
     token: builtins.str
@@ -393,15 +378,14 @@
         job_uuid: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
 global___GetElapsedTimeRequest = GetElapsedTimeRequest
 
-@typing_extensions.final
 class GetElapsedTimeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_OK_FIELD_NUMBER: builtins.int
     ELAPSED_TIME_FIELD_NUMBER: builtins.int
     is_ok: builtins.bool
     elapsed_time: builtins.float
@@ -411,15 +395,14 @@
         is_ok: builtins.bool = ...,
         elapsed_time: builtins.float = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["elapsed_time", b"elapsed_time", "is_ok", b"is_ok"]) -> None: ...
 
 global___GetElapsedTimeResponse = GetElapsedTimeResponse
 
-@typing_extensions.final
 class GetJobErrorInfoRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     job_uuid: builtins.str
     token: builtins.str
@@ -429,15 +412,14 @@
         job_uuid: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
 global___GetJobErrorInfoRequest = GetJobErrorInfoRequest
 
-@typing_extensions.final
 class GetJobErrorInfoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_ERROR_INFO_FIELD_NUMBER: builtins.int
     IS_OK_FIELD_NUMBER: builtins.int
     @property
     def job_error_info(self) -> common_types.common_types_pb2.JobErrorInfo: ...
```

### Comparing `quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/quickmpc/qmpc.py` & `quickmpc-0.3.2/quickmpc/qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/quickmpc/qmpc_server.py` & `quickmpc-0.3.2/quickmpc/qmpc_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,33 @@
 import json
 import logging
 import os
 import struct
 import time
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass, field, InitVar
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
+import google.protobuf.json_format
 import grpc
 import numpy as np
 import tqdm  # type: ignore
 from grpc_status import rpc_status  # type: ignore
-import google.protobuf.json_format
 
-from .exception import ArgmentError, QMPCJobError, QMPCServerError
-from .proto.common_types.common_types_pb2 import (JobErrorInfo,
-                                                  JobStatus,
-                                                  Schema,
-                                                  ShareValueTypeEnum)
+from .exception import ArgumentError, QMPCJobError, QMPCServerError
+from .proto.common_types.common_types_pb2 import (JobErrorInfo, JobStatus,
+                                                  Schema, ShareValueTypeEnum)
 from .proto.libc_to_manage_pb2 import (DeleteSharesRequest,
                                        ExecuteComputationRequest,
                                        GetComputationResultRequest,
                                        GetComputationResultResponse,
                                        GetDataListRequest,
                                        GetElapsedTimeRequest,
-                                       GetJobErrorInfoRequest,
-                                       Input,
+                                       GetJobErrorInfoRequest, Input,
                                        JoinOrder, SendSharesRequest)
 from .proto.libc_to_manage_pb2_grpc import LibcToManageStub
 from .share import Share
 from .utils.if_present import if_present
 from .utils.make_pieces import MakePiece
 from .utils.overload_tools import Dim1, Dim2, Dim3, methoddispatch
 from .utils.parse_csv import format_check
@@ -46,14 +43,16 @@
 
 @dataclass(frozen=True)
 class QMPCServer:
     endpoints: InitVar[List[str]]
     __client_stubs: Tuple[LibcToManageStub] = field(init=False)
     __party_size: int = field(init=False)
     token: str
+    retry_num: int = 10
+    retry_wait_time: int = 5
 
     def __post_init__(self, endpoints: List[str]) -> None:
         stubs = [LibcToManageStub(QMPCServer.__create_grpc_channel(ep))
                  for ep in endpoints]
         object.__setattr__(self, "_QMPCServer__client_stubs", stubs)
         object.__setattr__(self, "_QMPCServer__party_size", len(endpoints))
 
@@ -67,15 +66,15 @@
         elif o.scheme == 'https':
             # secureなchannelを作成
             credential: grpc.ChannelCredentials \
                 = grpc.ssl_channel_credentials()
             channel = grpc.secure_channel(o.netloc, credential)
         else:
             logger.error(f'仕様を満たさない形式のendpointが渡された: {endpoint}')
-            raise ArgmentError(
+            raise ArgumentError(
                 "endpointsにサポートされてないプロトコルが指定されています．http/httpsのいずれかを指定してください．")
 
         return channel
 
     @staticmethod
     def _argument_check(join_order: Tuple[List, List, List]):
         if len(join_order[0]) - 1 != len(join_order[1]):
@@ -87,47 +86,57 @@
             return False
         # TODO joinをenumにする
         if not all([0 <= join <= 2 for join in join_order[1]]):
             logger.error('join value must be in the range of 0 to 2')
             return False
         return True
 
+    def __retry(self, f: Callable, *request: Any) -> Any:
+        for _ in range(self.retry_num):
+            try:
+                return f(*request)
+            except grpc.RpcError as e:
+                logger.error(f'{e.details()} ({e.code()})')
+
+                # エラーが詳細な情報を持っているか確認
+                status = rpc_status.from_call(e)
+                if status is not None:
+                    for detail in status.details:
+                        if detail.Is(
+                            JobErrorInfo.DESCRIPTOR
+                        ):
+                            # CC で Job 実行時にエラーが発生していた場合
+                            # 例外を rethrow する
+                            err_info = JobErrorInfo()
+                            detail.Unpack(err_info)
+                            logger.error(f"job error information: {err_info}")
+
+                            raise QMPCJobError(err_info) from e
+
+                # MC で Internal Server Error が発生している場合
+                # 例外を rethrow する
+                if e.code() == grpc.StatusCode.UNKNOWN:
+                    raise QMPCServerError("backend server return error") from e
+            except Exception as e:
+                logger.error(e)
+            time.sleep(self.retry_wait_time)
+        raise RuntimeError(f"All {self.retry_num} times it was an error")
+
     @staticmethod
     def __futures_result(
             futures: Iterable, enable_progress_bar=True) -> Tuple[bool, List]:
         """ エラーチェックしてfutureのresultを得る """
         is_ok: bool = True
         response: List = []
         try:
             if enable_progress_bar:
                 futures = tqdm.tqdm(futures, desc='receive')
             response = [f.result() for f in futures]
-        except grpc.RpcError as e:
-            is_ok = False
-            logger.error(f'{e.details()} ({e.code()})')
-
-            # エラーが詳細な情報を持っているか確認
-            status = rpc_status.from_call(e)
-            if status is not None:
-                for detail in status.details:
-                    if detail.Is(
-                        JobErrorInfo.DESCRIPTOR   # type: ignore[attr-defined]
-                    ):
-                        # CC で Job 実行時にエラーが発生していた場合
-                        # 例外を rethrow する
-                        err_info = JobErrorInfo()
-                        detail.Unpack(err_info)
-                        logger.error(f"job error information: {err_info}")
-
-                        raise QMPCJobError(err_info) from e
-
-            # MC で Internal Server Error が発生している場合
-            # 例外を rethrow する
-            if e.code() == grpc.StatusCode.UNKNOWN:
-                raise QMPCServerError("backend server return error") from e
+        except (QMPCJobError, QMPCServerError):
+            raise
         except Exception as e:
             is_ok = False
             logger.error(e)
 
         for b in response:
             if hasattr(b, "is_ok"):
                 is_ok &= b.is_ok
@@ -169,20 +178,20 @@
             res_list.append(res)
         res_dict: Dict = {"is_ok": is_ok, "responses": res_list}
         return res_dict
 
     @methoddispatch(is_static_method=True)
     @staticmethod
     def __convert_schema(_):
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @__convert_schema.register(Dim1)
     @staticmethod
     def __convert_schema_dummy(schema: List):
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @__convert_schema.register((Dim1, str))
     @staticmethod
     def __convert_schema_str(schema: List[str]) -> List[Schema]:
         return [
             Schema(name=name,
                    type=ShareValueTypeEnum.SHARE_VALUE_TYPE_FIXED_POINT)
@@ -192,15 +201,15 @@
     @staticmethod
     def __convert_schema_typed(
             schema: List[Schema]) -> List[Schema]:
         return schema
 
     @methoddispatch()
     def send_share(self, _):
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @send_share.register(Dim2)
     @send_share.register(Dim3)
     def __send_share_impl(self, secrets: List,
                           schema: List[Union[str, Schema]],
                           matching_column: int,
                           piece_size: int) -> Dict:
@@ -229,45 +238,46 @@
             str(sorted_secrets).encode() + struct.pack('d', time.time())
         ).hexdigest()
         shares = [Share.sharize(s, self.__party_size)
                   for s in tqdm.tqdm(pieces, desc='sharize')]
         sent_at = str(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
 
         # リクエストパラメータを設定して非同期にリクエスト送信
-        executor = ThreadPoolExecutor()
-        futures = [executor.submit(stub.SendShares,
-                                   SendSharesRequest(
-                                       data_id=data_id,
-                                       shares=json.dumps(s),
-                                       schema=typed_schema,
-                                       piece_id=piece_id,
-                                       sent_at=sent_at,
-                                       matching_column=matching_column,
-                                       token=self.token))
-                   for piece_id, share_piece in enumerate(shares)
-                   for stub, s in zip(self.__client_stubs, share_piece)
-                   ]
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry,
+                                       stub.SendShares,
+                                       SendSharesRequest(
+                                           data_id=data_id,
+                                           shares=json.dumps(s),
+                                           schema=typed_schema,
+                                           piece_id=piece_id,
+                                           sent_at=sent_at,
+                                           matching_column=matching_column,
+                                           token=self.token))
+                       for piece_id, share_piece in enumerate(shares)
+                       for stub, s in zip(self.__client_stubs, share_piece)
+                       ]
         is_ok, _ = QMPCServer.__futures_result(futures)
         return {"is_ok": is_ok, "data_id": data_id}
 
     def delete_share(self, data_ids: List[str]) -> Dict:
         """ Shareを削除 """
         req = DeleteSharesRequest(dataIds=data_ids, token=self.token)
         # 非同期にリクエスト送信
-        executor = ThreadPoolExecutor()
-        futures = [executor.submit(stub.DeleteShares, req)
-                   for stub in self.__client_stubs]
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry, stub.DeleteShares, req)
+                       for stub in self.__client_stubs]
         is_ok, _ = QMPCServer.__futures_result(futures)
         return {"is_ok": is_ok}
 
     def execute_computation(self, method_id: int,
                             join_order: Tuple[List, List, List],
                             inp: Tuple[List, List]) -> Dict:
         if not self._argument_check(join_order):
-            raise ArgmentError("引数が正しくありません．")
+            raise ArgumentError("引数が正しくありません．")
 
         """ 計算リクエストを送信 """
         join_order_req = JoinOrder(
             dataIds=join_order[0],
             join=join_order[1],
             index=join_order[2])
         input_req = Input(
@@ -277,65 +287,70 @@
             method_id=method_id,
             token=self.token,
             table=join_order_req,
             arg=input_req,
         )
 
         # 非同期にリクエスト送信
-        executor = ThreadPoolExecutor()
-        # JobidをMCから貰う関係で単一MC（現在はSP（ID=0）のみ対応）にリクエストを送る
-        futures = [executor.submit(
-            self.__client_stubs[0].ExecuteComputation, req)]
+        with ThreadPoolExecutor() as executor:
+            # JobidをMCから貰う関係で単一MC（現在はSP（ID=0）のみ対応）にリクエストを送る
+            futures = [
+                executor.submit(self.__retry,
+                                self.__client_stubs[0].ExecuteComputation,
+                                req)]
 
         is_ok, response = QMPCServer.__futures_result(futures)
         job_uuid = response[0].job_uuid if is_ok else None
 
         return {"is_ok": is_ok, "job_uuid": job_uuid}
 
     def get_data_list(self) -> Dict:
         # 非同期にリクエスト送信
-        executor = ThreadPoolExecutor()
-        futures = [executor.submit(stub.GetDataList,
-                                   GetDataListRequest(token=self.token))
-                   for stub in self.__client_stubs]
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry,
+                                       stub.GetDataList,
+                                       GetDataListRequest(token=self.token))
+                       for stub in self.__client_stubs]
         is_ok, response = QMPCServer.__futures_result(futures)
         results = [eval(r.result) for r in response] if is_ok else None
 
         return {"is_ok": is_ok, "results": results}
 
     def get_elapsed_time(self, job_uuid: str) -> Dict:
         # リクエストパラメータを設定
         req = GetElapsedTimeRequest(
             job_uuid=job_uuid,
             token=self.token
         )
         # 非同期にリクエスト送信
-        executor = ThreadPoolExecutor()
-        futures = [executor.submit(stub.GetElapsedTime,
-                                   req)
-                   for stub in self.__client_stubs]
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry,
+                                       stub.GetElapsedTime,
+                                       req)
+                       for stub in self.__client_stubs]
         is_ok, response = QMPCServer.__futures_result(futures)
         elapsed_time = max([res.elapsed_time
                             for res in response]) if is_ok else None
         return {"is_ok": is_ok, "elapsed_time": elapsed_time}
 
     def get_computation_result(self, job_uuid: str,
                                path: Optional[str]) -> Dict:
         """ コンテナから結果を取得 """
         # リクエストパラメータを設定
         req = GetComputationResultRequest(
             job_uuid=job_uuid,
             token=self.token
         )
         # 非同期にリクエスト送信
-        executor = ThreadPoolExecutor()
-        futures = [executor.submit(QMPCServer.__stream_result,
-                                   stub.GetComputationResult(req),
-                                   job_uuid, party, path)
-                   for party, stub in enumerate(self.__client_stubs)]
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry,
+                                       QMPCServer.__stream_result,
+                                       stub.GetComputationResult(req),
+                                       job_uuid, party, path)
+                       for party, stub in enumerate(self.__client_stubs)]
         is_ok, response = QMPCServer.__futures_result(
             futures, enable_progress_bar=False)
         results_sorted = [sorted(res["responses"], key=lambda r: r.piece_id)
                           for res in response]
         # NOTE: statusは0番目(piece_id=1)の要素にのみ含まれている
         statuses = [res[0].status for res in results_sorted] \
             if results_sorted else None
@@ -396,17 +411,17 @@
     def get_job_error_info(self, job_uuid: str) -> Dict:
         # リクエストパラメータを設定
         req = GetJobErrorInfoRequest(
             job_uuid=job_uuid,
             token=self.token
         )
         # 非同期にリクエスト送信
-        executor = ThreadPoolExecutor()
-        futures = [executor.submit(stub.GetJobErrorInfo, req)
-                   for stub in self.__client_stubs]
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry, stub.GetJobErrorInfo, req)
+                       for stub in self.__client_stubs]
         is_ok, response = QMPCServer.__futures_result(
             futures, enable_progress_bar=False)
 
         job_error_info = [
             res.job_error_info if res.HasField("job_error_info") else None
             for res in response
         ]
```

### Comparing `quickmpc-0.3.1/quickmpc/share.py` & `quickmpc-0.3.2/quickmpc/share.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import logging
 from dataclasses import dataclass
 from decimal import Decimal
-from typing import (ClassVar, List, Tuple,
-                    Callable, Any, Union,
-                    Optional, Sequence)
+from typing import (Any, Callable, ClassVar, List,
+                    Optional, Sequence, Tuple, Union)
 
 import numpy as np
 
-from .utils.overload_tools import (DictList, DictList2,
-                                   Dim1, Dim2, Dim3, methoddispatch)
-from .proto.common_types.common_types_pb2 import (ShareValueTypeEnum,
-                                                  Schema)
+from .exception import ArgumentError
+from .proto.common_types.common_types_pb2 import Schema, ShareValueTypeEnum
+from .utils.overload_tools import (DictList, DictList2, Dim1,
+                                   Dim2, Dim3, methoddispatch)
 from .utils.random import ChaCha20, RandomInterface
-from .exception import ArgmentError
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class Share:
     __share_random_range: ClassVar[Tuple[Decimal, Decimal]] =\
         (Decimal(-(1 << 64)), Decimal(1 << 64))
 
     @methoddispatch(is_static_method=True)
     @staticmethod
     def __to_str(_):
         logger.error("Invalid argument on stringfy.")
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @__to_str.register(Decimal)
     @staticmethod
     def __decimal_to_str(val: Decimal) -> str:
         # InfinityをCCで読み込めるinfに変換
         return 'inf' if Decimal.is_infinite(val) else str(val)
 
@@ -39,27 +37,27 @@
     def __int_to_str(val: int) -> str:
         return str(val)
 
     @methoddispatch(is_static_method=True)
     @staticmethod
     def sharize(_, __):
         logger.error("Invalid argument on sharize.")
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @methoddispatch(is_static_method=True)
     @staticmethod
     def recons(_):
         logger.error("Invalid argument on recons.")
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @methoddispatch(is_static_method=True)
     @staticmethod
     def convert_type(_, __):
         logger.error("Invalid argument on convert_type.")
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @sharize.register(int)
     @sharize.register(float)
     @staticmethod
     def __sharize_scalar(secrets: float, party_size: int = 3) -> List[str]:
         """ スカラ値のシェア化 """
         rnd: RandomInterface = ChaCha20()
@@ -96,15 +94,15 @@
     @sharize.register((Dim1, int))
     @staticmethod
     def __sharize_1dimension_int(secrets: List[int], party_size: int = 3) \
             -> List[List[str]]:
         """ 1次元リストのシェア化 """
         rnd: RandomInterface = ChaCha20()
         secrets_size: int = len(secrets)
-        max_val = max(secrets) * 2
+        max_val = (max(secrets)+1) * 2
         shares: np.ndarray = np.array([
             rnd.get_list(-max_val, max_val, secrets_size)
             for __ in range(party_size - 1)])
         s1: np.ndarray = np.subtract(np.frompyfunc(int, 1, 1)(secrets),
                                      np.sum(shares, axis=0))
         shares_str: List[List[str]] = np.vectorize(
             Share.__to_str)([s1, *shares]).tolist()
@@ -144,59 +142,51 @@
             share_dict: List[dict] = Share.sharize(secret_dict, party_size)
             for ss, sd in zip(shares_str, share_dict):
                 ss.append(sd)
         return shares_str
 
     @recons.register(Dim1)
     @staticmethod
-    def __recons_list1(shares: List, f: Callable[[Any], Any] = float):
+    def __recons_list1(shares: List[Union[int, Decimal]]):
         """ 1次元リストのシェアを復元 """
-        try:
-            # 文字列がfloatかどうかcheck
-            [float(x) for x in shares]
-        except ValueError:
-            return shares[0]
         return sum(shares)
 
     @recons.register(Dim2)
     @recons.register(Dim3)
     @staticmethod
-    def __recons_list(shares: List[List],
-                      f: Callable[[Any], Any] = float) -> List:
+    def __recons_list(shares: List[List[Union[int, Decimal]]]) -> List:
         """ リストのシェアを復元 """
         secrets: List = [
-            Share.recons([shares_pi[i] for shares_pi in shares], f)
+            Share.recons([shares_pi[i] for shares_pi in shares])
             for i in range(len(shares[0]))
         ]
         return secrets
 
     @recons.register(DictList)
     @staticmethod
-    def __recons_dictlist(shares: List[dict],
-                          f: Callable[[Any], Any] = float) -> dict:
+    def __recons_dictlist(shares: List[dict]) -> dict:
         """ 辞書型を復元 """
         secrets: dict = dict()
         for key in shares[0].keys():
             val = []
             for s in shares:
                 val.append(s[key])
-            secrets[key] = Share.recons(val, f)
+            secrets[key] = Share.recons(val)
         return secrets
 
     @recons.register(DictList2)
     @staticmethod
-    def __recons_dictlist2(shares: List[List[dict]],
-                           f: Callable[[Any], Any] = float) -> list:
+    def __recons_dictlist2(shares: List[List[dict]]) -> list:
         """ 辞書型配列を復元 """
         secrets: list = list()
         for i in range(len(shares[0])):
             val = []
             for s in shares:
                 val.append(s[i])
-            secrets.append(Share.recons(val, f))
+            secrets.append(Share.recons(val))
         return secrets
 
     @staticmethod
     def get_pre_convert_func(
             schema: Optional[Schema]) -> Callable[[str], Any]:
         """ スキーマに合った変換関数を返す  """
         if schema is None:
```

### Comparing `quickmpc-0.3.1/quickmpc/utils/make_pieces.py` & `quickmpc-0.3.2/quickmpc/utils/make_pieces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import operator
 from dataclasses import dataclass
 from typing import List
 
-from ..exception import ArgmentError
+from ..exception import ArgumentError
 from .overload_tools import Dim1, Dim2, methoddispatch
 
 
 @dataclass(frozen=True)
 class MakePiece:
 
     @methoddispatch(is_static_method=True)
@@ -25,15 +25,15 @@
     @staticmethod
     def __get_byte_str(s: str):
         return len(s)
 
     @methoddispatch(is_static_method=True)
     @staticmethod
     def make_pieces(_, __):
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @staticmethod
     def check_max_size(max_size: int):
         # NOTE: Couchbaseのアイテムサイズ上限:1MB
         # NOTE: grpcの送受信データサイズ上限:4MB
         lower_limit_size: int = 1
         upper_limit_size: int = 1_000_000
```

### Comparing `quickmpc-0.3.1/quickmpc/utils/overload_tools.py` & `quickmpc-0.3.2/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/quickmpc/utils/parse_csv.py` & `quickmpc-0.3.2/quickmpc/utils/parse_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import csv
 import logging
-from hashlib import sha512
 from dataclasses import dataclass
-from typing import List, Tuple, Dict, Union, Sequence, Optional
-
-from .overload_tools import (Dim1, methoddispatch)
-from ..exception import ArgmentError
-
-from ..proto.common_types.common_types_pb2 import (ShareValueTypeEnum,
-                                                   Schema)
+from hashlib import sha512
+from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
+from ..exception import ArgumentError
+from ..proto.common_types.common_types_pb2 import Schema, ShareValueTypeEnum
+from .overload_tools import Dim1, methoddispatch
+
 logger = logging.getLogger(__name__)
 
 SUPPORT_TAGS: Dict[str, ShareValueTypeEnum.ValueType] = {
     'id': ShareValueTypeEnum.Value('SHARE_VALUE_TYPE_FIXED_POINT'),
 }
 
 ShareValueType = Union[float, int]
 
 
 @dataclass(frozen=True)
 class FormatChecker:
     @methoddispatch(is_static_method=True)
     @staticmethod
     def check_duplicate(_):
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @check_duplicate.register(Dim1)
     @staticmethod
     def check_duplicate_dummy(schema: List[str]):
-        raise ArgmentError("不正な引数が与えられています．")
+        raise ArgumentError("不正な引数が与えられています．")
 
     @check_duplicate.register((Dim1, str))
     @staticmethod
     def check_duplicate_strs(schema: List[str]) -> bool:
         return len(schema) == len(set(schema))
 
     @check_duplicate.register((Dim1, Schema))
```

### Comparing `quickmpc-0.3.1/quickmpc/utils/random.py` & `quickmpc-0.3.2/quickmpc/utils/random.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import ClassVar, List
+import math
 
 from nacl.utils import random, randombytes_deterministic
 
+from ..exception import ArgumentError
 from .overload_tools import methoddispatch
-from ..exception import ArgmentError
 
 
 # 乱数生成のインタフェース
 class RandomInterface(ABC):
     @abstractmethod
     def get(self, a, b) -> int:
         ...
@@ -25,43 +26,44 @@
 
     # 128bit符号付き整数最大，最小値
     mx: ClassVar[int] = (1 << 128)-1
     mn: ClassVar[int] = -(1 << 128)
 
     @methoddispatch()
     def get(self, a, b):
-        raise ArgmentError(
+        raise ArgumentError(
             "乱数の閾値はどちらもintもしくはdecimalでなければなりません．"
             f"a is {type(a)}, b is {type(b)}")
 
     @get.register(int)
     def __get_int(self, a: int, b: int) -> int:
-        # TRNGで32byte(256bit)生成
+        # TRNGで [a,b) の乱数生成
         self.__exception_check(a, b)
-        byte_val: bytes = self.__get_32byte()
-        int32byte = int.from_bytes(byte_val, "big")
-        return int32byte % (b-a)+a
+        interval_byte = self.__get_byte_size(b-a)
+        byte_val: bytes = random(interval_byte)
+        int_val = int.from_bytes(byte_val, "big")
+        return int_val % (b - a) + a
 
     @get.register(Decimal)
     def __get_decimal(self, a: Decimal, b: Decimal) -> Decimal:
         # 256bit整数を取り出して[a,b]に正規化する
         self.__exception_check(a, b)
         val: int = self.get(self.mn, self.mx)
         return Decimal(val-self.mn)/(self.mx-self.mn)*(b-a)+a
 
     @methoddispatch()
     def get_list(self, a, b, size: int):
-        raise ArgmentError(
+        raise ArgumentError(
             "乱数の閾値はどちらもintもしくはdecimalでなければなりません．"
             f"a is {type(a)}, b is {type(b)}")
 
     @get_list.register(int)
     def __get_list_int(self, a: int, b: int, size: int) -> List[int]:
         # TRNGの32byteをseedとしてCSPRNGでsize分生成
-        byte_size: int = 16
+        byte_size: int = self.__get_byte_size(b-a)
         self.__exception_check(a, b)
         seed: bytes = self.__get_32byte()
         bytes_list: bytes = randombytes_deterministic(size*byte_size, seed)
         int_list = [int.from_bytes(bytes_list[i:i+byte_size], "big")
                     for i in range(0, len(bytes_list), byte_size)]
         return [x % (b-a)+a for x in int_list]
 
@@ -70,19 +72,23 @@
             -> List[Decimal]:
         # 128bit整数を取り出して[a,b]に正規化する
         self.__exception_check(a, b)
         valList: List[int] = self.get_list(self.mn, self.mx, size)
         return [Decimal(val-self.mn)/(self.mx-self.mn)*(b-a)+a
                 for val in valList]
 
+    def __get_byte_size(self, x: int) -> int:
+        # 整数の byte サイズを取得
+        return max(math.ceil(math.log2(x))//8 + 1, 32)
+
     def __get_32byte(self) -> bytes:
         return random()
 
     def __exception_check(self, a, b) -> None:
         if a >= b:
-            raise ArgmentError(
+            raise ArgumentError(
                 "乱数の下限は上限より小さい必要があります．"
                 f"{a} < {b}")
         if type(a) != type(b):
-            raise ArgmentError(
+            raise ArgumentError(
                 "乱数の下限と上限の型は一致させる必要があります．"
                 f"{type(a)} != {type(b)}")
```

### Comparing `quickmpc-0.3.1/quickmpc/utils/restore.py` & `quickmpc-0.3.2/quickmpc/utils/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/quickmpc.egg-info/SOURCES.txt` & `quickmpc-0.3.2/quickmpc.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 quickmpc.egg-info/PKG-INFO
 quickmpc.egg-info/SOURCES.txt
 quickmpc.egg-info/dependency_links.txt
 quickmpc.egg-info/requires.txt
 quickmpc.egg-info/top_level.txt
 quickmpc/proto/README.md
 quickmpc/proto/__init__.py
-quickmpc/proto/generate_grpc.py
 quickmpc/proto/libc_to_manage_pb2.py
 quickmpc/proto/libc_to_manage_pb2.pyi
 quickmpc/proto/libc_to_manage_pb2_grpc.py
 quickmpc/proto/libc_to_manage_pb2_grpc.pyi
 quickmpc/proto/common_types/__init__.py
 quickmpc/proto/common_types/common_types_pb2.py
 quickmpc/proto/common_types/common_types_pb2.pyi
@@ -75,10 +74,16 @@
 tests/unit_tests/test_share_sharize.py
 tests/unit_tests/certificates/server1.key
 tests/unit_tests/certificates/server1.pem
 tests/unit_tests/certificates/server2.key
 tests/unit_tests/certificates/server2.pem
 tests/unit_tests/certificates/server3.key
 tests/unit_tests/certificates/server3.pem
-tests/unit_tests/test_files/data1.csv
-tests/unit_tests/test_files/data2.csv
-tests/unit_tests/test_files/data3.csv
+tests/unit_tests/test_files/bitvector.csv
+tests/unit_tests/test_files/diff_col.csv
+tests/unit_tests/test_files/edge_data.csv
+tests/unit_tests/test_files/empty.csv
+tests/unit_tests/test_files/none.csv
+tests/unit_tests/test_files/normal.csv
+tests/unit_tests/test_files/not_csv.csv
+tests/unit_tests/test_files/over_number.csv
+tests/unit_tests/test_files/string_data.csv
```

### Comparing `quickmpc-0.3.1/tests/unit_tests/certificates/server1.key` & `quickmpc-0.3.2/tests/unit_tests/certificates/server1.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/certificates/server1.pem` & `quickmpc-0.3.2/tests/unit_tests/certificates/server1.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/certificates/server2.key` & `quickmpc-0.3.2/tests/unit_tests/certificates/server2.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/certificates/server2.pem` & `quickmpc-0.3.2/tests/unit_tests/certificates/server2.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/certificates/server3.key` & `quickmpc-0.3.2/tests/unit_tests/certificates/server3.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/certificates/server3.pem` & `quickmpc-0.3.2/tests/unit_tests/certificates/server3.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/conftest.py` & `quickmpc-0.3.2/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/local_server.py` & `quickmpc-0.3.2/tests/unit_tests/local_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.3.2/tests/unit_tests/test_make_pieces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 import pytest
 
-from quickmpc.exception import ArgmentError
+from quickmpc.exception import ArgumentError
 from quickmpc.utils.make_pieces import MakePiece
 
 
 class TestQMPC:
 
     MATRIX: List[List[str]] = [[str(i) * i for i in range(1, 6)]] * 5
 
@@ -59,16 +59,16 @@
         assert (actual == expected)
 
     @pytest.mark.parametrize(
         ("args, error"),
         [
             ([MATRIX, 0], RuntimeError),          # サイズが小さい場合
             ([MATRIX, 1_000_001], RuntimeError),  # サイズが大きい場合
-            ([0, 0], ArgmentError),               # 引数タイプが無効な場合: 0 次元
-            ([[MATRIX], 0], ArgmentError),        # 引数タイプが無効な場合: 3 次元
+            ([0, 0], ArgumentError),               # 引数タイプが無効な場合: 0 次元
+            ([[MATRIX], 0], ArgumentError),        # 引数タイプが無効な場合: 3 次元
         ]
     )
     def test_make_pieces_errorhandring(self, args, error):
         """ 異常値を与えてエラーが出るかTest """
         with pytest.raises(error):
             MakePiece.make_pieces(*args)
```

### Comparing `quickmpc-0.3.1/tests/unit_tests/test_over_load.py` & `quickmpc-0.3.2/tests/unit_tests/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/test_random.py` & `quickmpc-0.3.2/tests/unit_tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/test_restore.py` & `quickmpc-0.3.2/tests/unit_tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.1/tests/unit_tests/test_share_recons.py` & `quickmpc-0.3.2/tests/unit_tests/test_share_recons.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,78 @@
 import math
 from decimal import Decimal
 
 import numpy as np
 import pytest
 
+from quickmpc.exception import ArgumentError
 from quickmpc.share import Share
 
 
 class TestQMPC:
 
+    @staticmethod
+    def isclose(val, true_val):
+        ok: bool = True
+        if isinstance(val, list):
+            for v, t in zip(val, true_val):
+                ok &= TestQMPC.isclose(v, t)
+        elif isinstance(val, dict):
+            for v, t in zip(val.values(), true_val.values()):
+                ok &= TestQMPC.isclose(v, t)
+        else:
+            ok &= math.isclose(val, true_val)
+        return ok
+
     @pytest.mark.parametrize(
-        ("shares"),
+        ("shares", "expected"),
         [
             # 1次元配列のシェア
-            (["1", "2", "3"]),
-            (["2.4", "4.2", "4.1"]),
+            # int
+            ([1, 2, 3], 6),
+            # float
+            ([2.4, 4.2, 4.1], 10.7),
+            # Decimal
+            ([Decimal(2.4), Decimal(4.2), Decimal(4.1)], Decimal(10.7)),
+
             # 2次元配列のシェア
-            ([["1"], ["2"], ["3"]]),
-            ([["3000", "500"], ["2500", "1100"], ["100", "200"]]),
-            ([["2.4", "9.1"], ["4.2", "6.7"], ["4.1", "1.5"]]),
+            # int
+            ([[1, 4], [2, 5], [3, 6]], [6, 15]),
+            # float
+            ([[1.1, 4.2], [2.3, 5.4], [3.5, 6.6]], [6.9, 16.2]),
+            # Decimal
+            ([[Decimal(1.1), Decimal(4.2)], [Decimal(2.3), Decimal(5.4)],
+              [Decimal(3.5), Decimal(6.6)]], [Decimal(6.9), Decimal(16.2)]),
+
             # 3次元配列のシェア
-            ([[["1"]], [["2"]], [["3"]]]),
-            ([[["30.0", "5.22"], ["4.89", "1.001"]], [["25.1", "11.901"],
-             ["1200", "400"]], [["100", "200"], ["300", "800"]]])
+            # int
+            ([[[1, 4], [7, 8]],
+              [[2, 5], [9, 10]],
+              [[3, 6], [11, 12]]],
+                [[6, 15], [27, 30]]),
+            # float
+            ([[[1.1, 4.2], [7.1, 8.2]],
+              [[2.3, 5.4], [9.1, 10.2]],
+              [[3.5, 6.6], [11.1, 12.2]]],
+             [[6.9, 16.2], [27.3, 30.6]]),
+            # Decimal
+            ([[[Decimal(1.1), Decimal(4.2)], [Decimal(7.1), (8.2)]],
+              [[Decimal(2.3), Decimal(5.4)], [Decimal(9.1), (10.2)]],
+              [[Decimal(3.5), Decimal(6.6)], [Decimal(11.1), (12.2)]]],
+             [[Decimal(6.9), Decimal(16.2)], [Decimal(27.3), (30.6)]]),
+
         ]
     )
-    def test_recons_list(self, shares: list):
+    def test_recons_list(self, shares: list, expected):
         """ 3パーティの復元が正しくできるかTest """
-        conved: list = [Share.convert_type(s) for s in shares]
-        secrets: list = Share.recons(conved)
-        secrets = Share.convert_type(secrets)
-        shares_float: np.ndarray = \
-            np.vectorize(Decimal)(Share.sharize(secrets))
-        assert (np.allclose(secrets,
-                            np.vectorize(float)(np.sum(shares_float, axis=0))))
+        secrets: list = Share.recons(shares)
+        assert TestQMPC.isclose(secrets, expected)
 
     @pytest.mark.parametrize(
-        ("shares", "secrets_true"),
+        ("shares", "expected"),
         [
             # 辞書型配列のシェア
             ([{"a": 1}, {"a": 2}, {"a": 3}],
              {"a": 6}),
             ([{"a": 1.1, "b": 2}, {"a": 4.1, "b": 9.1}, {"a": 3.1, "b": -2.1}],
              {"a": 8.3, "b": 9}),
             ([{"a": 1.1, "child": {"b": 2, "c": [1, 3]}},
@@ -56,64 +88,73 @@
                 [{"a": 8.3}, {"b": 9}]),
             ([[{"a": 1.1}, {"child": {"b": 2, "c": [1, 3]}}],
                 [{"a": 4.1}, {"child": {"b": 9.1, "c": [2, 1]}}],
                 [{"a": 3.1}, {"child": {"b": -2.1, "c": [1, 8]}}]],
                 [{"a": 8.3}, {"child": {"b": 9, "c": [4, 12]}}]),
         ]
     )
-    def test_recons_dict(self, shares: list, secrets_true: list):
+    def test_recons_dict(self, shares: dict, expected: dict):
         """ 3パーティの辞書型の復元が正しくできるかTest """
         secrets: list = Share.recons(shares)
-
-        def isclose(val, true_val):
-            ok: bool = True
-            if isinstance(val, list):
-                for v, t in zip(val, true_val):
-                    ok &= isclose(v, t)
-            elif isinstance(val, dict):
-                for v, t in zip(val.values(), true_val.values()):
-                    ok &= isclose(v, t)
-            else:
-                ok &= math.isclose(val, true_val)
-            return ok
-
-        assert (isclose(secrets, secrets_true))
+        assert TestQMPC.isclose(secrets, expected)
 
     @pytest.mark.parametrize(
-        ("shares"),
+        ("shares", "expected"),
         [
             # 2パーティのシェア
-            ([["1", "5"], ["2", "9"]]),
-            ([[["1", "2"], ["3", "4"]], [["5", "6"], ["7", "8"]]]),
-            ([["2.4", "9.1"], ["4.2", "6.7"], ["4.1", "1.5"]]),
-            # 3次元配列のシェア
+            ([[1, 5], [2, 9]], [3, 14]),
+            ([[[1, 2], [3, 4]], [[5, 6], [7, 8]]], [[6, 8], [10, 12]]),
+            ([[2.4, 9.1], [4.2, 6.7], [4.1, 1.5]], [10.7, 17.3]),
             # 4パーティのシェア
-            ([["3000"], ["2500"], ["200"], ["400"]]),
-            ([[["3000"]], [["2500"]], [["200"]], [["400"]]]),
+            ([[3000], [2500], [200], [400]], [6100]),
+            ([[[3000]], [[2500]], [[200]], [[400]]], [[6100]]),
             # 5パーティのシェア
-            ([["3000"], ["2500"], ["200"], ["400"], ["11235"]]),
-            ([[["3000"]], [["2500"]], [["200"]], [["400"]], [["11235"]]]),
+            ([[3000], [2500], [200], [400], [11235]], [17335]),
+            ([[[3000]], [[2500]], [[200]], [[400]], [[11235]]], [[17335]]),
         ]
     )
-    def test_recons_multi(self, shares: list):
+    def test_recons_multi(self, shares: list, expected: list):
         """ nパーティのシェアの復元が正しくできるかTest """
-        conved: list = [Share.convert_type(s) for s in shares]
-        secrets: list = Share.recons(conved)
-        secrets = Share.convert_type(secrets)
-        shares_float: np.ndarray = \
-            np.vectorize(Decimal)(Share.sharize(secrets))
-        assert (np.allclose(secrets,
-                            np.vectorize(float)(np.sum(shares_float, axis=0))))
+        secrets: list = Share.recons(shares)
+        assert TestQMPC.isclose(secrets, expected)
+
+    @pytest.mark.parametrize(
+        ("shares", "expected"),
+        [
+            ([1e1200 for _ in range(3)], 3e1200),
+            ([Decimal(1e1200) for _ in range(3)], Decimal(3e1200)),
+            ([-1e1200 for _ in range(3)], -3e1200),
+            ([Decimal(-1e1200) for _ in range(3)], Decimal(-3e1200)),
+            ([1e-50 for _ in range(3)], 3e-50),
+            ([Decimal(1e-50) for _ in range(3)], Decimal(3e-50)),
+            ([-1e-50 for _ in range(3)], -3e-50),
+            ([Decimal(-1e-50) for _ in range(3)], Decimal(-3e-50)),
+        ]
+    )
+    def test_recons_edge(self, shares: list, expected):
+        """ 3パーティの復元が正しくできるかTest """
+        secrets = Share.recons(shares)
+        assert TestQMPC.isclose(secrets, expected)
 
-    def test_recons_errorhandring(self):
+    @pytest.mark.parametrize(
+        ("shares", "expected"),
+        [
+            # scalar value is not allowed
+            (1, ArgumentError),
+
+            # string value is not allowed
+            ("hey", ArgumentError),
+            (["hey"], TypeError),  # TODO: quickmpcのArgumentErrorが出るようにしたい
+            ([["hey"]], TypeError),
+        ]
+    )
+    def test_recons_errorhandring(self, shares, expected):
         """ 異常値を与えてエラーが出るかTest """
-        with pytest.raises(Exception):
-            Share.recons(1)
-        with pytest.raises(Exception):
-            Share.recons("hey")
+        with pytest.raises(expected):
+            Share.recons(shares)
 
     @pytest.mark.parametrize(
         ("secrets"),
         [
             # 1次元配列の秘密情報
             ([1]), ([3.0, 5.12, 21.05]), ([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]),
             # 2次元配列の秘密情報
@@ -129,20 +170,7 @@
         """ nパーティのシェア化，復元が正しくできてるかTest"""
         for party_size in range(2, 10):
             shares: list = Share.sharize(secrets, party_size=party_size)
             conved: list = [Share.convert_type(s) for s in shares]
             secrets_2: list = Share.recons(conved)
             secrets_2 = Share.convert_type(secrets_2)
             assert (np.allclose(secrets, secrets_2))
-
-    @pytest.mark.parametrize(
-        ("shares"),
-        [
-            # str
-            ([["a", "b"], ["a", "b"]]),
-            ([["a", "b", "c"], ["a", "b", "c"], ["a", "b", "c"]])
-        ]
-    )
-    def test_sharize_recons_not_share(self, shares: list):
-        """ 数値でない(Shareでない)値を復元せず返却できるかTest """
-        secrets: list = Share.recons(shares)
-        assert (shares[0] == secrets)
```

