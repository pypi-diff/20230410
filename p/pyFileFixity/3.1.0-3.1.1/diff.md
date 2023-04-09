# Comparing `tmp/pyFileFixity-3.1.0.tar.gz` & `tmp/pyFileFixity-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFileFixity-3.1.0.tar", last modified: Sun Apr  9 09:37:49 2023, max compression
+gzip compressed data, was "pyFileFixity-3.1.1.tar", last modified: Sun Apr  9 23:53:37 2023, max compression
```

## Comparing `pyFileFixity-3.1.0.tar` & `pyFileFixity-3.1.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.096807 pyFileFixity-3.1.0/
--rw-rw-rw-   0        0        0      626 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/.coveragerc
--rw-rw-rw-   0        0        0     1106 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/LICENSE
--rw-rw-rw-   0        0        0     1155 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    67892 2023-04-09 09:37:49.096807 pyFileFixity-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    65577 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.081183 pyFileFixity-3.1.0/pyFileFixity/
--rw-rw-rw-   0        0        0      177 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/__init__.py
--rw-rw-rw-   0        0        0     8205 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/easy_profiler.py
--rw-rw-rw-   0        0        0     1032 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/ecc_specification.txt
--rw-rw-rw-   0        0        0    13147 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/ecc_speedtest.py
--rw-rw-rw-   0        0        0    18667 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/filetamper.py
--rw-rw-rw-   0        0        0    60875 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/header_ecc.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.081183 pyFileFixity-3.1.0/pyFileFixity/lib/
--rw-rw-rw-   0        0        0        3 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/_compat.py
--rw-rw-rw-   0        0        0    22551 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/aux_funcs.py
--rw-rw-rw-   0        0        0    17370 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/eccman.py
--rw-rw-rw-   0        0        0     3459 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/hasher.py
--rw-rw-rw-   0        0        0    14183 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/md5py.py
--rw-rw-rw-   0        0        0    30966 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/six.py
--rw-rw-rw-   0        0        0     3144 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/lib/tee.py
--rw-rw-rw-   0        0        0     7566 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/pff.py
--rw-rw-rw-   0        0        0    27920 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/repair_ecc.py
--rw-rw-rw-   0        0        0    38261 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/replication_repair.py
--rw-rw-rw-   0        0        0    27706 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/resiliency_tester.py
--rw-rw-rw-   0        0        0     1983 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/resiliency_tester_config.txt
--rw-rw-rw-   0        0        0    37567 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/rfigc.py
--rw-rw-rw-   0        0        0    69990 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/structural_adaptive_ecc.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.096807 pyFileFixity-3.1.0/pyFileFixity/tests/
--rw-rw-rw-   0        0        0        1 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/__init__.py
--rw-rw-rw-   0        0        0     6753 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/aux_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.096807 pyFileFixity-3.1.0/pyFileFixity/tests/files/
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.096807 pyFileFixity-3.1.0/pyFileFixity/tests/files/Sub2/
--rw-rw-rw-   0        0        0        6 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/files/Sub2/testsub2.txt
--rw-rw-rw-   0        0        0    67254 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/files/alice.pdf
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.096807 pyFileFixity-3.1.0/pyFileFixity/tests/files/sub/
--rw-rw-rw-   0        0        0     2048 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/files/sub/Snark.zip
--rw-rw-rw-   0        0        0      255 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/files/sub/testsub.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/files/testaa.txt
--rw-rw-rw-   0        0        0    19719 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/files/tux.jpg
--rw-rw-rw-   0        0        0     3667 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/files/tuxsmall.jpg
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.096807 pyFileFixity-3.1.0/pyFileFixity/tests/results/
--rw-rw-rw-   0        0        0     2087 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg
--rw-rw-rw-   0        0        0     1661 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg
--rw-rw-rw-   0        0        0     1614 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_algo.db
--rw-rw-rw-   0        0        0     6473 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_dir.db
--rw-rw-rw-   0        0        0     1614 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_one_file.db
--rw-rw-rw-   0        0        0     1614 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db
--rw-rw-rw-   0        0        0     6473 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_repair_ecc_check.db
--rw-rw-rw-   0        0        0    47542 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_repair_ecc_sa_check.db
--rw-rw-rw-   0        0        0      697 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_rfigc_test_dir.csv
--rw-rw-rw-   0        0        0      132 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_rfigc_test_error_file.log
--rw-rw-rw-   0        0        0      162 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_rfigc_test_one_file.csv
--rw-rw-rw-   0        0        0      694 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_rfigc_test_update_append.csv
--rw-rw-rw-   0        0        0      166 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_rfigc_test_update_remove.csv
--rw-rw-rw-   0        0        0     2883 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db
--rw-rw-rw-   0        0        0    47542 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db
--rw-rw-rw-   0        0        0     2883 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db
--rw-rw-rw-   0        0        0     2883 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db
--rw-rw-rw-   0        0        0     6753 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_aux_funcs.py
--rw-rw-rw-   0        0        0     7042 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_eccman.py
--rw-rw-rw-   0        0        0     1755 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_hasher.py
--rw-rw-rw-   0        0        0     8255 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_header_ecc.py
--rw-rw-rw-   0        0        0     8394 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_repair_ecc.py
--rw-rw-rw-   0        0        0    13155 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_replication_repair.py
--rw-rw-rw-   0        0        0     8708 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_resiliency_tester.py
--rw-rw-rw-   0        0        0     6577 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_rfigc.py
--rw-rw-rw-   0        0        0    10655 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_structural_adaptive_ecc.py
--rw-rw-rw-   0        0        0     2303 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyFileFixity/tests/test_tee.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:37:49.081183 pyFileFixity-3.1.0/pyFileFixity.egg-info/
--rw-rw-rw-   0        0        0    67892 2023-04-09 09:37:49.000000 pyFileFixity-3.1.0/pyFileFixity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-04-09 09:37:49.000000 pyFileFixity-3.1.0/pyFileFixity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:37:49.000000 pyFileFixity-3.1.0/pyFileFixity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-09 09:37:49.000000 pyFileFixity-3.1.0/pyFileFixity.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      168 2023-04-09 09:37:49.000000 pyFileFixity-3.1.0/pyFileFixity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-09 09:37:49.000000 pyFileFixity-3.1.0/pyFileFixity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10708 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 09:37:49.112432 pyFileFixity-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1762 2023-04-09 09:36:39.000000 pyFileFixity-3.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:37.361517 pyFileFixity-3.1.1/
+-rw-rw-rw-   0        0        0      626 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/.coveragerc
+-rw-rw-rw-   0        0        0     1106 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1155 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    64472 2023-04-09 23:53:37.361517 pyFileFixity-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    62157 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:36.798953 pyFileFixity-3.1.1/pyFileFixity/
+-rw-rw-rw-   0        0        0      177 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/__init__.py
+-rw-rw-rw-   0        0        0     8205 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/easy_profiler.py
+-rw-rw-rw-   0        0        0     1032 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/ecc_specification.txt
+-rw-rw-rw-   0        0        0    13147 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/ecc_speedtest.py
+-rw-rw-rw-   0        0        0    18667 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/filetamper.py
+-rw-rw-rw-   0        0        0    60875 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/header_ecc.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:36.798953 pyFileFixity-3.1.1/pyFileFixity/lib/
+-rw-rw-rw-   0        0        0        3 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/_compat.py
+-rw-rw-rw-   0        0        0    22551 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/aux_funcs.py
+-rw-rw-rw-   0        0        0    17370 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/eccman.py
+-rw-rw-rw-   0        0        0     3459 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/hasher.py
+-rw-rw-rw-   0        0        0    14183 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/md5py.py
+-rw-rw-rw-   0        0        0    30966 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/six.py
+-rw-rw-rw-   0        0        0     3144 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/lib/tee.py
+-rw-rw-rw-   0        0        0     7566 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/pff.py
+-rw-rw-rw-   0        0        0    27920 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/repair_ecc.py
+-rw-rw-rw-   0        0        0    38261 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/replication_repair.py
+-rw-rw-rw-   0        0        0    27706 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/resiliency_tester.py
+-rw-rw-rw-   0        0        0     1983 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/resiliency_tester_config.txt
+-rw-rw-rw-   0        0        0    37567 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/rfigc.py
+-rw-rw-rw-   0        0        0    69990 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/structural_adaptive_ecc.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:36.814578 pyFileFixity-3.1.1/pyFileFixity/tests/
+-rw-rw-rw-   0        0        0        1 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/__init__.py
+-rw-rw-rw-   0        0        0     6753 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/aux_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:37.361517 pyFileFixity-3.1.1/pyFileFixity/tests/files/
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:37.361517 pyFileFixity-3.1.1/pyFileFixity/tests/files/Sub2/
+-rw-rw-rw-   0        0        0        6 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/files/Sub2/testsub2.txt
+-rw-rw-rw-   0        0        0    67254 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/files/alice.pdf
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:37.361517 pyFileFixity-3.1.1/pyFileFixity/tests/files/sub/
+-rw-rw-rw-   0        0        0     2048 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/files/sub/Snark.zip
+-rw-rw-rw-   0        0        0      255 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/files/sub/testsub.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/files/testaa.txt
+-rw-rw-rw-   0        0        0    19719 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/files/tux.jpg
+-rw-rw-rw-   0        0        0     3667 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/files/tuxsmall.jpg
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:37.361517 pyFileFixity-3.1.1/pyFileFixity/tests/results/
+-rw-rw-rw-   0        0        0     2087 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg
+-rw-rw-rw-   0        0        0     1661 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg
+-rw-rw-rw-   0        0        0     1614 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_algo.db
+-rw-rw-rw-   0        0        0     6473 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_dir.db
+-rw-rw-rw-   0        0        0     1614 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_one_file.db
+-rw-rw-rw-   0        0        0     1614 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db
+-rw-rw-rw-   0        0        0     6473 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_repair_ecc_check.db
+-rw-rw-rw-   0        0        0    47542 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_repair_ecc_sa_check.db
+-rw-rw-rw-   0        0        0      697 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_rfigc_test_dir.csv
+-rw-rw-rw-   0        0        0      132 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_rfigc_test_error_file.log
+-rw-rw-rw-   0        0        0      162 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_rfigc_test_one_file.csv
+-rw-rw-rw-   0        0        0      694 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_rfigc_test_update_append.csv
+-rw-rw-rw-   0        0        0      166 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_rfigc_test_update_remove.csv
+-rw-rw-rw-   0        0        0     2883 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db
+-rw-rw-rw-   0        0        0    47542 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db
+-rw-rw-rw-   0        0        0     2883 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db
+-rw-rw-rw-   0        0        0     2883 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db
+-rw-rw-rw-   0        0        0     6753 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_aux_funcs.py
+-rw-rw-rw-   0        0        0     7042 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_eccman.py
+-rw-rw-rw-   0        0        0     1755 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_hasher.py
+-rw-rw-rw-   0        0        0     8255 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_header_ecc.py
+-rw-rw-rw-   0        0        0     8394 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_repair_ecc.py
+-rw-rw-rw-   0        0        0    13155 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_replication_repair.py
+-rw-rw-rw-   0        0        0     8708 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_resiliency_tester.py
+-rw-rw-rw-   0        0        0     6577 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_rfigc.py
+-rw-rw-rw-   0        0        0    10655 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_structural_adaptive_ecc.py
+-rw-rw-rw-   0        0        0     2303 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyFileFixity/tests/test_tee.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:53:36.798953 pyFileFixity-3.1.1/pyFileFixity.egg-info/
+-rw-rw-rw-   0        0        0    64472 2023-04-09 23:53:36.000000 pyFileFixity-3.1.1/pyFileFixity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2651 2023-04-09 23:53:36.000000 pyFileFixity-3.1.1/pyFileFixity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 23:53:36.000000 pyFileFixity-3.1.1/pyFileFixity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-09 23:53:36.000000 pyFileFixity-3.1.1/pyFileFixity.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      168 2023-04-09 23:53:36.000000 pyFileFixity-3.1.1/pyFileFixity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-09 23:53:36.000000 pyFileFixity-3.1.1/pyFileFixity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10708 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 23:53:37.361517 pyFileFixity-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1762 2023-04-09 23:51:22.000000 pyFileFixity-3.1.1/tox.ini
```

### Comparing `pyFileFixity-3.1.0/.coveragerc` & `pyFileFixity-3.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/LICENSE` & `pyFileFixity-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/MANIFEST.in` & `pyFileFixity-3.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/PKG-INFO` & `pyFileFixity-3.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFileFixity
-Version: 3.1.0
+Version: 3.1.1
 Summary: Helping file fixity (long term storage of data) via redundant error correcting codes and hash auditing.
 Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/pyFileFixity
 Project-URL: Documentation, https://github.com/lrq3000/pyFileFixity/blob/master/README.rst
 Project-URL: Source, https://github.com/lrq3000/pyFileFixity
@@ -89,15 +89,15 @@
 
 .. contents:: Table of contents
    :backlinks: top
 
 Quickstart
 ----------
 
-Runs on Python 3 up to Python 3.11. Both PyPy 3 and PyPy 2 are supported. Older versions such as Python 2.7.10 are still being automatically unit tested with continuous integration but support can be dropped at any moment.
+Runs on Python 3 up to Python 3.12-dev. PyPy 3 is also supported.
 
 - To install or update on Python 3:
 
 ``pip install --upgrade pyfilefixity``
 
 - For Python 2.7, the latest working version was v3.0.2:
 
@@ -198,18 +198,14 @@
 
 - To run speedtests of encoding/decoding error correction codes on your machine:
 
 ``pff speedtest``
 
 - In case the ``pff`` command does not work, it can be replaced with ``python -m pyFileFixity.pff`` .
 
-- DEPRECATED (because Gooey is not maintained anymore it seems): To use the GUI with any tool, use ``--gui`` and do not supply any other argument, eg: ``python rfigc.py --gui``.
-
-- You can also use `PyPy <http://pypy.org/>`_ or Cython to hugely speedup the processing time of any tool here.
-
 The problem of long term storage
 --------------------------------
 
 Why are data corrupted with time? One sole reason: entropy.
 Entropy refers to the universal tendency for systems to become
 less ordered over time. Data corruption is exactly that: a disorder
 in bits order. In other words: *the Universe hates your data*.
@@ -668,18 +664,21 @@
 file header), then, without counting the hash per block and other
 meta-data, the final ECC file will be about 2 \* resiliency\_rate \*
 number\_of\_files \* header\_size = 24.5 MB. This size can be lower if
 there are many files smaller than 1KB. This is a pretty low storage
 overhead to backup the headers of such a big number of files.
 
 The script is pure-python as are its dependencies: it is thus completely
-cross-platform and open source. However, this imply that it is quite
-slow, but PyPy v2.5.0 was successfully tested against the script without
-any modification, and a speed increase of more 100x could be observed,
-so that you can expect a rate of more than 1MB/s, which is quite fast.
+cross-platform and open source. The default ecc algo
+(ecc_algo=3 uses `reedsolo <https://github.com/tomerfiliba-org/reedsolomon>`_)
+also provides a speed-optimized C-compiled implementation (``creedsolo``) that will be used
+if available for the user's platform, so pyFileFixity should be fast by default.
+Alternatively, it's possible to use a JIT compiler such as PyPy,
+although this means that ``creedsolo`` will not be useable, so PyPy
+may accelerate other functions but slower ecc encoding/decoding.
 
 Structural Adaptive Error Correction Encoder
 --------------------------------------------
 
 This script implements a variable error correction rate encoder: each
 file is ecc encoded using a variable resiliency rate -- using a high
 constant resiliency rate for the header part (resiliency rate stage 1,
@@ -764,78 +763,14 @@
 -  ``--ecc_algo 3``: use the second codec, which is the fastest.
    The generated ECC will be compatible with algo 1 and 2.
 -  ``--ecc_algo 4``: also use the second, fastest RS codec, but
    with different parameters (US FAA ADSB UAT RS FEC norm),
    thus the generated ECC won't be compatible with algo 1 to 3.
    But do not be scared, the ECC will work just the same.
 
-Cython implementation
----------------------
-
-This section describes how to use the Cython implementation. However,
-you should first try PyPy, as it may give great performances too.
-
-Simply follow the instruction to install the `reedsolo <https://github.com/tomerfiliba-org/reedsolomon>`_ module with
-the cythonized module.
-
-Then make sure to use ``ecc_algo=3`` in all your ``eccman`` calls, and you
-are then good to go, the cythonized module ``creedsolo`` will always be used
-for both encoding and decoding transparently.
-
-THE REST OF THIS SECTION IS OLD AND DEPRECATED, because the Cython compilation is now
-done directly in the Reed-Solomon submodules, instead of here, so you
-should not need to worry about it, just pip install with the requirements.txt
-and you should be set. The information below is left for historical purposes:
-
-A speedy Cython implementation of the Reed-Solomon library is included.
-It should provide C-speed for all scripts (as long as you use
---ecc\_algo 1 or 2, not 3 nor 4). It is not needed, since a pure-python
-implementation is used by default, but it can be useful if you want to
-encode big datasets of several hundred of GB.
-
-If you want to build the C/Cython implementation, do the following:
-
-1- Install a C compiler for your platform. On Linux, gcc should already
-be installed. On Windows, you need to use the Visual Studio C compiler
-(not MinGW nor Cygwin gcc, they won't work). You can use the "Microsoft
-Visual C++ Compiler for Python 2.7", and follow these instructions to
-make it work if you have Python < 2.7.10:
-
-https://github.com/cython/cython/wiki/CythonExtensionsOnWindows
-
-2- cd to this folder (where pyFileFixity resides), and execute the
-following command:
-
-``python setup.py build_ext --inplace --compiler=msvc``
-
-If everything goes alright, the C compiler will compile the .c files
-(that were pre-generated by Cython) and you can then use PyFileFixity
-scripts just as usual and you should see a huge speedup. Else, if it
-doesn't work, you might need to generate .c files using Cython for your
-platform (because the pre-generated .c files may be incompatible with
-your platform). To do that, you just need to install Cython, which is an
-easy task with nowadays Python distributions such as Anaconda: download
-32-bit Anaconda installer (on Windows you should avoid the 64-bit, it
-may produce weird issues with Cython), then after install, open the
-Anaconda Command Prompt and execute: ``conda install cython``. This will
-install all the necessary stuff along the cython library. Then you can
-simply execute again the command
-``python setup.py build_ext --inplace --compiler=msvc`` and it will this
-time rebuild from scratch, by autodetecting that you have Cython
-installed, the setup.py script will automatically generate .c files from
-.pyx files and then .pyd files (binaries) from .c files.
-
-If you get issues, you can see the following post on how to install
-Cython:
-
-https://github.com/cython/cython/wiki/InstallingOnWindows
-
-3- You can now launch pyFileFixity like usual, it should automatically
-detect the C/Cython compiled files and use that to speedup processing.
-
 Note about speed: Also, use a smaller --max\_block\_size to greatly
 speedup the operations! That's the trick used to compute very quickly RS
 ECC on optical discs. You give up a bit of resiliency of course (because
 blocks are smaller, thus you protect a smaller number of characters per
 ECC. In the end, this should not change much about real resiliency, but
 in case you get a big bit error burst on a contiguous block, you may
 lose a whole block at once. That's why using RS255 is better, but it's
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyFileFixity-3.1.0/README.rst` & `pyFileFixity-3.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 .. contents:: Table of contents
    :backlinks: top
 
 Quickstart
 ----------
 
-Runs on Python 3 up to Python 3.11. Both PyPy 3 and PyPy 2 are supported. Older versions such as Python 2.7.10 are still being automatically unit tested with continuous integration but support can be dropped at any moment.
+Runs on Python 3 up to Python 3.12-dev. PyPy 3 is also supported.
 
 - To install or update on Python 3:
 
 ``pip install --upgrade pyfilefixity``
 
 - For Python 2.7, the latest working version was v3.0.2:
 
@@ -153,18 +153,14 @@
 
 - To run speedtests of encoding/decoding error correction codes on your machine:
 
 ``pff speedtest``
 
 - In case the ``pff`` command does not work, it can be replaced with ``python -m pyFileFixity.pff`` .
 
-- DEPRECATED (because Gooey is not maintained anymore it seems): To use the GUI with any tool, use ``--gui`` and do not supply any other argument, eg: ``python rfigc.py --gui``.
-
-- You can also use `PyPy <http://pypy.org/>`_ or Cython to hugely speedup the processing time of any tool here.
-
 The problem of long term storage
 --------------------------------
 
 Why are data corrupted with time? One sole reason: entropy.
 Entropy refers to the universal tendency for systems to become
 less ordered over time. Data corruption is exactly that: a disorder
 in bits order. In other words: *the Universe hates your data*.
@@ -623,18 +619,21 @@
 file header), then, without counting the hash per block and other
 meta-data, the final ECC file will be about 2 \* resiliency\_rate \*
 number\_of\_files \* header\_size = 24.5 MB. This size can be lower if
 there are many files smaller than 1KB. This is a pretty low storage
 overhead to backup the headers of such a big number of files.
 
 The script is pure-python as are its dependencies: it is thus completely
-cross-platform and open source. However, this imply that it is quite
-slow, but PyPy v2.5.0 was successfully tested against the script without
-any modification, and a speed increase of more 100x could be observed,
-so that you can expect a rate of more than 1MB/s, which is quite fast.
+cross-platform and open source. The default ecc algo
+(ecc_algo=3 uses `reedsolo <https://github.com/tomerfiliba-org/reedsolomon>`_)
+also provides a speed-optimized C-compiled implementation (``creedsolo``) that will be used
+if available for the user's platform, so pyFileFixity should be fast by default.
+Alternatively, it's possible to use a JIT compiler such as PyPy,
+although this means that ``creedsolo`` will not be useable, so PyPy
+may accelerate other functions but slower ecc encoding/decoding.
 
 Structural Adaptive Error Correction Encoder
 --------------------------------------------
 
 This script implements a variable error correction rate encoder: each
 file is ecc encoded using a variable resiliency rate -- using a high
 constant resiliency rate for the header part (resiliency rate stage 1,
@@ -719,78 +718,14 @@
 -  ``--ecc_algo 3``: use the second codec, which is the fastest.
    The generated ECC will be compatible with algo 1 and 2.
 -  ``--ecc_algo 4``: also use the second, fastest RS codec, but
    with different parameters (US FAA ADSB UAT RS FEC norm),
    thus the generated ECC won't be compatible with algo 1 to 3.
    But do not be scared, the ECC will work just the same.
 
-Cython implementation
----------------------
-
-This section describes how to use the Cython implementation. However,
-you should first try PyPy, as it may give great performances too.
-
-Simply follow the instruction to install the `reedsolo <https://github.com/tomerfiliba-org/reedsolomon>`_ module with
-the cythonized module.
-
-Then make sure to use ``ecc_algo=3`` in all your ``eccman`` calls, and you
-are then good to go, the cythonized module ``creedsolo`` will always be used
-for both encoding and decoding transparently.
-
-THE REST OF THIS SECTION IS OLD AND DEPRECATED, because the Cython compilation is now
-done directly in the Reed-Solomon submodules, instead of here, so you
-should not need to worry about it, just pip install with the requirements.txt
-and you should be set. The information below is left for historical purposes:
-
-A speedy Cython implementation of the Reed-Solomon library is included.
-It should provide C-speed for all scripts (as long as you use
---ecc\_algo 1 or 2, not 3 nor 4). It is not needed, since a pure-python
-implementation is used by default, but it can be useful if you want to
-encode big datasets of several hundred of GB.
-
-If you want to build the C/Cython implementation, do the following:
-
-1- Install a C compiler for your platform. On Linux, gcc should already
-be installed. On Windows, you need to use the Visual Studio C compiler
-(not MinGW nor Cygwin gcc, they won't work). You can use the "Microsoft
-Visual C++ Compiler for Python 2.7", and follow these instructions to
-make it work if you have Python < 2.7.10:
-
-https://github.com/cython/cython/wiki/CythonExtensionsOnWindows
-
-2- cd to this folder (where pyFileFixity resides), and execute the
-following command:
-
-``python setup.py build_ext --inplace --compiler=msvc``
-
-If everything goes alright, the C compiler will compile the .c files
-(that were pre-generated by Cython) and you can then use PyFileFixity
-scripts just as usual and you should see a huge speedup. Else, if it
-doesn't work, you might need to generate .c files using Cython for your
-platform (because the pre-generated .c files may be incompatible with
-your platform). To do that, you just need to install Cython, which is an
-easy task with nowadays Python distributions such as Anaconda: download
-32-bit Anaconda installer (on Windows you should avoid the 64-bit, it
-may produce weird issues with Cython), then after install, open the
-Anaconda Command Prompt and execute: ``conda install cython``. This will
-install all the necessary stuff along the cython library. Then you can
-simply execute again the command
-``python setup.py build_ext --inplace --compiler=msvc`` and it will this
-time rebuild from scratch, by autodetecting that you have Cython
-installed, the setup.py script will automatically generate .c files from
-.pyx files and then .pyd files (binaries) from .c files.
-
-If you get issues, you can see the following post on how to install
-Cython:
-
-https://github.com/cython/cython/wiki/InstallingOnWindows
-
-3- You can now launch pyFileFixity like usual, it should automatically
-detect the C/Cython compiled files and use that to speedup processing.
-
 Note about speed: Also, use a smaller --max\_block\_size to greatly
 speedup the operations! That's the trick used to compute very quickly RS
 ECC on optical discs. You give up a bit of resiliency of course (because
 blocks are smaller, thus you protect a smaller number of characters per
 ECC. In the end, this should not change much about real resiliency, but
 in case you get a big bit error burst on a contiguous block, you may
 lose a whole block at once. That's why using RS255 is better, but it's
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyFileFixity-3.1.0/pyFileFixity/easy_profiler.py` & `pyFileFixity-3.1.1/pyFileFixity/easy_profiler.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/ecc_specification.txt` & `pyFileFixity-3.1.1/pyFileFixity/ecc_specification.txt`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/ecc_speedtest.py` & `pyFileFixity-3.1.1/pyFileFixity/ecc_speedtest.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/filetamper.py` & `pyFileFixity-3.1.1/pyFileFixity/filetamper.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/header_ecc.py` & `pyFileFixity-3.1.1/pyFileFixity/header_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/lib/_compat.py` & `pyFileFixity-3.1.1/pyFileFixity/lib/_compat.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/lib/aux_funcs.py` & `pyFileFixity-3.1.1/pyFileFixity/lib/aux_funcs.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/lib/eccman.py` & `pyFileFixity-3.1.1/pyFileFixity/lib/eccman.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/lib/hasher.py` & `pyFileFixity-3.1.1/pyFileFixity/lib/hasher.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/lib/md5py.py` & `pyFileFixity-3.1.1/pyFileFixity/lib/md5py.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/lib/six.py` & `pyFileFixity-3.1.1/pyFileFixity/lib/six.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/lib/tee.py` & `pyFileFixity-3.1.1/pyFileFixity/lib/tee.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/pff.py` & `pyFileFixity-3.1.1/pyFileFixity/pff.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/repair_ecc.py` & `pyFileFixity-3.1.1/pyFileFixity/repair_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/replication_repair.py` & `pyFileFixity-3.1.1/pyFileFixity/replication_repair.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/resiliency_tester.py` & `pyFileFixity-3.1.1/pyFileFixity/resiliency_tester.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/resiliency_tester_config.txt` & `pyFileFixity-3.1.1/pyFileFixity/resiliency_tester_config.txt`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/rfigc.py` & `pyFileFixity-3.1.1/pyFileFixity/rfigc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/structural_adaptive_ecc.py` & `pyFileFixity-3.1.1/pyFileFixity/structural_adaptive_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/aux_tests.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/aux_tests.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/files/alice.pdf` & `pyFileFixity-3.1.1/pyFileFixity/tests/files/alice.pdf`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/files/sub/Snark.zip` & `pyFileFixity-3.1.1/pyFileFixity/tests/files/sub/Snark.zip`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/files/tux.jpg` & `pyFileFixity-3.1.1/pyFileFixity/tests/files/tux.jpg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/files/tuxsmall.jpg` & `pyFileFixity-3.1.1/pyFileFixity/tests/files/tuxsmall.jpg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_algo.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_algo.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_dir.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_dir.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_one_file.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_one_file.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_repair_ecc_check.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_repair_ecc_check.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_repair_ecc_sa_check.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_repair_ecc_sa_check.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_rfigc_test_dir.csv` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_rfigc_test_dir.csv`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_rfigc_test_update_append.csv` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_rfigc_test_update_append.csv`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db` & `pyFileFixity-3.1.1/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_aux_funcs.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_aux_funcs.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_eccman.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_eccman.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_hasher.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_hasher.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_header_ecc.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_header_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_repair_ecc.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_repair_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_replication_repair.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_replication_repair.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_resiliency_tester.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_resiliency_tester.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_rfigc.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_rfigc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_structural_adaptive_ecc.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_structural_adaptive_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity/tests/test_tee.py` & `pyFileFixity-3.1.1/pyFileFixity/tests/test_tee.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyFileFixity.egg-info/PKG-INFO` & `pyFileFixity-3.1.1/pyFileFixity.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFileFixity
-Version: 3.1.0
+Version: 3.1.1
 Summary: Helping file fixity (long term storage of data) via redundant error correcting codes and hash auditing.
 Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/pyFileFixity
 Project-URL: Documentation, https://github.com/lrq3000/pyFileFixity/blob/master/README.rst
 Project-URL: Source, https://github.com/lrq3000/pyFileFixity
@@ -89,15 +89,15 @@
 
 .. contents:: Table of contents
    :backlinks: top
 
 Quickstart
 ----------
 
-Runs on Python 3 up to Python 3.11. Both PyPy 3 and PyPy 2 are supported. Older versions such as Python 2.7.10 are still being automatically unit tested with continuous integration but support can be dropped at any moment.
+Runs on Python 3 up to Python 3.12-dev. PyPy 3 is also supported.
 
 - To install or update on Python 3:
 
 ``pip install --upgrade pyfilefixity``
 
 - For Python 2.7, the latest working version was v3.0.2:
 
@@ -198,18 +198,14 @@
 
 - To run speedtests of encoding/decoding error correction codes on your machine:
 
 ``pff speedtest``
 
 - In case the ``pff`` command does not work, it can be replaced with ``python -m pyFileFixity.pff`` .
 
-- DEPRECATED (because Gooey is not maintained anymore it seems): To use the GUI with any tool, use ``--gui`` and do not supply any other argument, eg: ``python rfigc.py --gui``.
-
-- You can also use `PyPy <http://pypy.org/>`_ or Cython to hugely speedup the processing time of any tool here.
-
 The problem of long term storage
 --------------------------------
 
 Why are data corrupted with time? One sole reason: entropy.
 Entropy refers to the universal tendency for systems to become
 less ordered over time. Data corruption is exactly that: a disorder
 in bits order. In other words: *the Universe hates your data*.
@@ -668,18 +664,21 @@
 file header), then, without counting the hash per block and other
 meta-data, the final ECC file will be about 2 \* resiliency\_rate \*
 number\_of\_files \* header\_size = 24.5 MB. This size can be lower if
 there are many files smaller than 1KB. This is a pretty low storage
 overhead to backup the headers of such a big number of files.
 
 The script is pure-python as are its dependencies: it is thus completely
-cross-platform and open source. However, this imply that it is quite
-slow, but PyPy v2.5.0 was successfully tested against the script without
-any modification, and a speed increase of more 100x could be observed,
-so that you can expect a rate of more than 1MB/s, which is quite fast.
+cross-platform and open source. The default ecc algo
+(ecc_algo=3 uses `reedsolo <https://github.com/tomerfiliba-org/reedsolomon>`_)
+also provides a speed-optimized C-compiled implementation (``creedsolo``) that will be used
+if available for the user's platform, so pyFileFixity should be fast by default.
+Alternatively, it's possible to use a JIT compiler such as PyPy,
+although this means that ``creedsolo`` will not be useable, so PyPy
+may accelerate other functions but slower ecc encoding/decoding.
 
 Structural Adaptive Error Correction Encoder
 --------------------------------------------
 
 This script implements a variable error correction rate encoder: each
 file is ecc encoded using a variable resiliency rate -- using a high
 constant resiliency rate for the header part (resiliency rate stage 1,
@@ -764,78 +763,14 @@
 -  ``--ecc_algo 3``: use the second codec, which is the fastest.
    The generated ECC will be compatible with algo 1 and 2.
 -  ``--ecc_algo 4``: also use the second, fastest RS codec, but
    with different parameters (US FAA ADSB UAT RS FEC norm),
    thus the generated ECC won't be compatible with algo 1 to 3.
    But do not be scared, the ECC will work just the same.
 
-Cython implementation
----------------------
-
-This section describes how to use the Cython implementation. However,
-you should first try PyPy, as it may give great performances too.
-
-Simply follow the instruction to install the `reedsolo <https://github.com/tomerfiliba-org/reedsolomon>`_ module with
-the cythonized module.
-
-Then make sure to use ``ecc_algo=3`` in all your ``eccman`` calls, and you
-are then good to go, the cythonized module ``creedsolo`` will always be used
-for both encoding and decoding transparently.
-
-THE REST OF THIS SECTION IS OLD AND DEPRECATED, because the Cython compilation is now
-done directly in the Reed-Solomon submodules, instead of here, so you
-should not need to worry about it, just pip install with the requirements.txt
-and you should be set. The information below is left for historical purposes:
-
-A speedy Cython implementation of the Reed-Solomon library is included.
-It should provide C-speed for all scripts (as long as you use
---ecc\_algo 1 or 2, not 3 nor 4). It is not needed, since a pure-python
-implementation is used by default, but it can be useful if you want to
-encode big datasets of several hundred of GB.
-
-If you want to build the C/Cython implementation, do the following:
-
-1- Install a C compiler for your platform. On Linux, gcc should already
-be installed. On Windows, you need to use the Visual Studio C compiler
-(not MinGW nor Cygwin gcc, they won't work). You can use the "Microsoft
-Visual C++ Compiler for Python 2.7", and follow these instructions to
-make it work if you have Python < 2.7.10:
-
-https://github.com/cython/cython/wiki/CythonExtensionsOnWindows
-
-2- cd to this folder (where pyFileFixity resides), and execute the
-following command:
-
-``python setup.py build_ext --inplace --compiler=msvc``
-
-If everything goes alright, the C compiler will compile the .c files
-(that were pre-generated by Cython) and you can then use PyFileFixity
-scripts just as usual and you should see a huge speedup. Else, if it
-doesn't work, you might need to generate .c files using Cython for your
-platform (because the pre-generated .c files may be incompatible with
-your platform). To do that, you just need to install Cython, which is an
-easy task with nowadays Python distributions such as Anaconda: download
-32-bit Anaconda installer (on Windows you should avoid the 64-bit, it
-may produce weird issues with Cython), then after install, open the
-Anaconda Command Prompt and execute: ``conda install cython``. This will
-install all the necessary stuff along the cython library. Then you can
-simply execute again the command
-``python setup.py build_ext --inplace --compiler=msvc`` and it will this
-time rebuild from scratch, by autodetecting that you have Cython
-installed, the setup.py script will automatically generate .c files from
-.pyx files and then .pyd files (binaries) from .c files.
-
-If you get issues, you can see the following post on how to install
-Cython:
-
-https://github.com/cython/cython/wiki/InstallingOnWindows
-
-3- You can now launch pyFileFixity like usual, it should automatically
-detect the C/Cython compiled files and use that to speedup processing.
-
 Note about speed: Also, use a smaller --max\_block\_size to greatly
 speedup the operations! That's the trick used to compute very quickly RS
 ECC on optical discs. You give up a bit of resiliency of course (because
 blocks are smaller, thus you protect a smaller number of characters per
 ECC. In the end, this should not change much about real resiliency, but
 in case you get a big bit error burst on a contiguous block, you may
 lose a whole block at once. That's why using RS255 is better, but it's
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyFileFixity-3.1.0/pyFileFixity.egg-info/SOURCES.txt` & `pyFileFixity-3.1.1/pyFileFixity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/pyproject.toml` & `pyFileFixity-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.1.0/tox.ini` & `pyFileFixity-3.1.1/tox.ini`

 * *Files identical despite different names*

