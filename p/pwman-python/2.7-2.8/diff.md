# Comparing `tmp/pwman-python-2.7.tar.gz` & `tmp/pwman-python-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwman-python-2.7.tar", last modified: Sat Mar 11 21:28:50 2023, max compression
+gzip compressed data, was "pwman-python-2.8.tar", last modified: Mon Apr 10 19:37:51 2023, max compression
```

## Comparing `pwman-python-2.7.tar` & `pwman-python-2.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.637682 pwman-python-2.7/
--rw-r--r--   0 root         (0) root         (0)    18092 2023-03-11 21:28:48.000000 pwman-python-2.7/COPYING
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-11 21:28:48.000000 pwman-python-2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4374 2023-03-11 21:28:50.637682 pwman-python-2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4831 2023-03-11 21:28:49.000000 pwman-python-2.7/README.html
--rw-r--r--   0 root         (0) root         (0)     3589 2023-03-11 21:28:48.000000 pwman-python-2.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.629682 pwman-python-2.7/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.629682 pwman-python-2.7/doc/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.633682 pwman-python-2.7/doc/api/libpwman/
--rw-r--r--   0 root         (0) root         (0)     4007 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/aes.html
--rw-r--r--   0 root         (0) root         (0)    12765 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/cryptsql.html
--rw-r--r--   0 root         (0) root         (0)    39356 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/database.html
--rw-r--r--   0 root         (0) root         (0)     3868 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/dbdiff.html
--rw-r--r--   0 root         (0) root         (0)     5888 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/exception.html
--rw-r--r--   0 root         (0) root         (0)    10554 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/fileobj.html
--rw-r--r--   0 root         (0) root         (0)     4218 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/mlock.html
--rw-r--r--   0 root         (0) root         (0)     8077 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/otp.html
--rw-r--r--   0 root         (0) root         (0)    37557 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/ui.html
--rw-r--r--   0 root         (0) root         (0)     3295 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/undo.html
--rw-r--r--   0 root         (0) root         (0)     2673 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/util.html
--rw-r--r--   0 root         (0) root         (0)     1345 2023-03-11 21:28:49.000000 pwman-python-2.7/doc/api/libpwman/version.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.633682 pwman-python-2.7/doc/foreign-licenses/
--rw-r--r--   0 root         (0) root         (0)    12769 2023-03-11 21:28:48.000000 pwman-python-2.7/doc/foreign-licenses/PYTHON-LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      269 2023-03-11 21:28:48.000000 pwman-python-2.7/doc/foreign-licenses/README
--rw-r--r--   0 root         (0) root         (0)      863 2023-03-11 21:28:48.000000 pwman-python-2.7/examplescript.py
--rwxr-xr-x   0 root         (0) root         (0)      404 2023-03-11 21:28:48.000000 pwman-python-2.7/gitconfig.sh
--rwxr-xr-x   0 root         (0) root         (0)      853 2023-03-11 21:28:48.000000 pwman-python-2.7/install_to_venv.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.633682 pwman-python-2.7/libpwman/
--rw-r--r--   0 root         (0) root         (0)      326 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7508 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3219 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/aes.py
--rw-r--r--   0 root         (0) root         (0)    12782 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/cryptsql.py
--rw-r--r--   0 root         (0) root         (0)    24637 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/database.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/dbdiff.py
--rw-r--r--   0 root         (0) root         (0)      251 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/exception.py
--rw-r--r--   0 root         (0) root         (0)     3548 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/fileobj.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/mlock.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/otp.py
--rw-r--r--   0 root         (0) root         (0)    44456 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/ui.py
--rw-r--r--   0 root         (0) root         (0)     1371 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/undo.py
--rw-r--r--   0 root         (0) root         (0)     1776 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/util.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-03-11 21:28:48.000000 pwman-python-2.7/libpwman/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.633682 pwman-python-2.7/maintenance/
--rwxr-xr-x   0 root         (0) root         (0)      453 2023-03-11 21:28:48.000000 pwman-python-2.7/maintenance/cleantree.sh
--rwxr-xr-x   0 root         (0) root         (0)      103 2023-03-11 21:28:48.000000 pwman-python-2.7/maintenance/deb-dependencies-install.sh
--rwxr-xr-x   0 root         (0) root         (0)     1519 2023-03-11 21:28:48.000000 pwman-python-2.7/maintenance/gen-doc.sh
--rw-r--r--   0 root         (0) root         (0)      900 2023-03-11 21:28:48.000000 pwman-python-2.7/maintenance/win-install-dependencies.cmd
--rw-r--r--   0 root         (0) root         (0)     3674 2023-03-11 21:28:48.000000 pwman-python-2.7/maintenance/win-standalone-build.cmd
--rwxr-xr-x   0 root         (0) root         (0)      276 2023-03-11 21:28:48.000000 pwman-python-2.7/pwman
--rw-r--r--   0 root         (0) root         (0)      849 2023-03-11 21:28:48.000000 pwman-python-2.7/pwman.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.633682 pwman-python-2.7/pwman_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4374 2023-03-11 21:28:50.000000 pwman-python-2.7/pwman_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1365 2023-03-11 21:28:50.000000 pwman-python-2.7/pwman_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-11 21:28:50.000000 pwman-python-2.7/pwman_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-11 21:28:50.000000 pwman-python-2.7/pwman_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-11 21:28:50.000000 pwman-python-2.7/pwman_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-11 21:28:48.000000 pwman-python-2.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-11 21:28:50.637682 pwman-python-2.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2022 2023-03-11 21:28:48.000000 pwman-python-2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 21:28:50.633682 pwman-python-2.7/tests/
--rw-r--r--   0 root         (0) root         (0)      133 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/pwman_tstlib.py
--rwxr-xr-x   0 root         (0) root         (0)     1315 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/run.sh
--rw-r--r--   0 root         (0) root         (0)      520 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/test_database_v0.db
--rw-r--r--   0 root         (0) root         (0)     1680 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/test_database_v0.py
--rw-r--r--   0 root         (0) root         (0)     2621 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/test_database_v1.db
--rw-r--r--   0 root         (0) root         (0)     3441 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/test_database_v1.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/test_escape.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/test_otp.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-03-11 21:28:48.000000 pwman-python-2.7/tests/test_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.594332 pwman-python-2.8/
+-rw-r--r--   0 root         (0) root         (0)    18092 2023-04-10 19:37:49.000000 pwman-python-2.8/COPYING
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-10 19:37:49.000000 pwman-python-2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4374 2023-04-10 19:37:51.594332 pwman-python-2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-04-10 19:37:50.000000 pwman-python-2.8/README.html
+-rw-r--r--   0 root         (0) root         (0)     3589 2023-04-10 19:37:49.000000 pwman-python-2.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.590332 pwman-python-2.8/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.590332 pwman-python-2.8/doc/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.594332 pwman-python-2.8/doc/api/libpwman/
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/aes.html
+-rw-r--r--   0 root         (0) root         (0)    12876 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/cryptsql.html
+-rw-r--r--   0 root         (0) root         (0)    39835 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/database.html
+-rw-r--r--   0 root         (0) root         (0)     3868 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/dbdiff.html
+-rw-r--r--   0 root         (0) root         (0)     5888 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/exception.html
+-rw-r--r--   0 root         (0) root         (0)    10554 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/fileobj.html
+-rw-r--r--   0 root         (0) root         (0)     4218 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/mlock.html
+-rw-r--r--   0 root         (0) root         (0)     8077 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/otp.html
+-rw-r--r--   0 root         (0) root         (0)    43114 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/ui.html
+-rw-r--r--   0 root         (0) root         (0)     6301 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/ui_escape.html
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/util.html
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-04-10 19:37:50.000000 pwman-python-2.8/doc/api/libpwman/version.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.594332 pwman-python-2.8/doc/foreign-licenses/
+-rw-r--r--   0 root         (0) root         (0)    12769 2023-04-10 19:37:49.000000 pwman-python-2.8/doc/foreign-licenses/PYTHON-LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-10 19:37:49.000000 pwman-python-2.8/doc/foreign-licenses/README
+-rw-r--r--   0 root         (0) root         (0)      863 2023-04-10 19:37:49.000000 pwman-python-2.8/examplescript.py
+-rwxr-xr-x   0 root         (0) root         (0)      404 2023-04-10 19:37:49.000000 pwman-python-2.8/gitconfig.sh
+-rwxr-xr-x   0 root         (0) root         (0)      853 2023-04-10 19:37:49.000000 pwman-python-2.8/install_to_venv.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.594332 pwman-python-2.8/libpwman/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/aes.py
+-rw-r--r--   0 root         (0) root         (0)    12852 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/cryptsql.py
+-rw-r--r--   0 root         (0) root         (0)    24849 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/database.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/dbdiff.py
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/exception.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/fileobj.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/mlock.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/otp.py
+-rw-r--r--   0 root         (0) root         (0)    52799 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/ui_escape.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/util.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-10 19:37:49.000000 pwman-python-2.8/libpwman/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.594332 pwman-python-2.8/maintenance/
+-rwxr-xr-x   0 root         (0) root         (0)      453 2023-04-10 19:37:49.000000 pwman-python-2.8/maintenance/cleantree.sh
+-rwxr-xr-x   0 root         (0) root         (0)      103 2023-04-10 19:37:49.000000 pwman-python-2.8/maintenance/deb-dependencies-install.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1519 2023-04-10 19:37:49.000000 pwman-python-2.8/maintenance/gen-doc.sh
+-rw-r--r--   0 root         (0) root         (0)      900 2023-04-10 19:37:49.000000 pwman-python-2.8/maintenance/win-install-dependencies.cmd
+-rw-r--r--   0 root         (0) root         (0)     3674 2023-04-10 19:37:49.000000 pwman-python-2.8/maintenance/win-standalone-build.cmd
+-rwxr-xr-x   0 root         (0) root         (0)      276 2023-04-10 19:37:49.000000 pwman-python-2.8/pwman
+-rw-r--r--   0 root         (0) root         (0)      849 2023-04-10 19:37:49.000000 pwman-python-2.8/pwman.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.594332 pwman-python-2.8/pwman_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4374 2023-04-10 19:37:51.000000 pwman-python-2.8/pwman_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-04-10 19:37:51.000000 pwman-python-2.8/pwman_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:37:51.000000 pwman-python-2.8/pwman_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-10 19:37:51.000000 pwman-python-2.8/pwman_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-10 19:37:51.000000 pwman-python-2.8/pwman_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-10 19:37:49.000000 pwman-python-2.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 19:37:51.594332 pwman-python-2.8/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1728 2023-04-10 19:37:49.000000 pwman-python-2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:37:51.594332 pwman-python-2.8/tests/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/pwman_tstlib.py
+-rwxr-xr-x   0 root         (0) root         (0)     1325 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/run.sh
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/test_database_v0.db
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/test_database_v0.py
+-rw-r--r--   0 root         (0) root         (0)     2621 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/test_database_v1.db
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/test_database_v1.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/test_escape.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/test_otp.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-04-10 19:37:49.000000 pwman-python-2.8/tests/test_ui.py
```

### Comparing `pwman-python-2.7/COPYING` & `pwman-python-2.8/COPYING`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/PKG-INFO` & `pwman-python-2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwman-python
-Version: 2.7
+Version: 2.8
 Summary: Commandline password manager
 Home-page: https://bues.ch/h/pwman
 Author: Michael Büsch
 Author-email: m@bues.ch
 Keywords: password manager command line TOTP 2FA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pwman-python-2.7/README.html` & `pwman-python-2.8/README.html`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/README.rst` & `pwman-python-2.8/README.rst`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/doc/api/libpwman/aes.html` & `pwman-python-2.8/doc/api/libpwman/aes.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module aes</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">aes</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/aes.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/aes.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/aes.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/aes.py</a></td></tr></table>
     <p><span class="code">#&nbsp;<a href="#AES">AES</a>&nbsp;wrapper<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor pkg-content-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
    index
-aes /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/aes.py
+aes /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/aes.py
 # AES wrapper
 # Copyright (c) 2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Modules
    � os�
```

### Comparing `pwman-python-2.7/doc/api/libpwman/cryptsql.html` & `pwman-python-2.8/doc/api/libpwman/cryptsql.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module cryptsql</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">cryptsql</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/cryptsql.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/cryptsql.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/cryptsql.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/cryptsql.py</a></td></tr></table>
     <p><span class="code">#&nbsp;Crypto&nbsp;SQL<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor pkg-content-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
@@ -156,15 +156,16 @@
 <dl><dt><a name="CryptSQL-setRegexpFlags"><strong>setRegexpFlags</strong></a>(self, search=True, ignoreCase=True, multiLine=True, dotAll=True)</dt><dd><span class="code">Change&nbsp;the&nbsp;behavior&nbsp;of&nbsp;the&nbsp;REGEXP&nbsp;operator.</span></dd></dl>
 
 <dl><dt><a name="CryptSQL-sqlCreateFunction"><strong>sqlCreateFunction</strong></a>(self, name, nrParams, func)</dt><dd><span class="code">Create&nbsp;an&nbsp;SQL&nbsp;function.<br>
 See&nbsp;sqlite3.Connection.create_function&nbsp;for&nbsp;more&nbsp;details.</span></dd></dl>
 
 <dl><dt><a name="CryptSQL-sqlExec"><strong>sqlExec</strong></a>(self, code, params=[])</dt><dd><span class="code">Execute&nbsp;one&nbsp;SQL&nbsp;statement.</span></dd></dl>
 
-<dl><dt><a name="CryptSQL-sqlExecScript"><strong>sqlExecScript</strong></a>(self, code)</dt><dd><span class="code">Execute&nbsp;multiple&nbsp;SQL&nbsp;statements.</span></dd></dl>
+<dl><dt><a name="CryptSQL-sqlExecScript"><strong>sqlExecScript</strong></a>(self, code)</dt><dd><span class="code">Execute&nbsp;multiple&nbsp;SQL&nbsp;statements.<br>
+Warning:&nbsp;This&nbsp;implicitly&nbsp;commits&nbsp;pending&nbsp;transactions&nbsp;before&nbsp;executing.</span></dd></dl>
 
 <dl><dt><a name="CryptSQL-sqlIsEmpty"><strong>sqlIsEmpty</strong></a>(self)</dt><dd><span class="code">Returns&nbsp;True,&nbsp;if&nbsp;the&nbsp;database&nbsp;does&nbsp;not&nbsp;contain&nbsp;any&nbsp;tables.</span></dd></dl>
 
 <dl><dt><a name="CryptSQL-sqlPlainDump"><strong>sqlPlainDump</strong></a>(self)</dt><dd><span class="code">Get&nbsp;a&nbsp;plain&nbsp;text&nbsp;dump&nbsp;of&nbsp;the&nbsp;database.<br>
 Returns&nbsp;a&nbsp;string.</span></dd></dl>
 
 <dl><dt><a name="CryptSQL-sqlVacuum"><strong>sqlVacuum</strong></a>(self)</dt><dd><span class="code">Run&nbsp;the&nbsp;SQL&nbsp;VACUUM&nbsp;statement.<br>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
         index
-cryptsql /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/
+cryptsql /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/
          cryptsql.py
 # Crypto SQL
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Modules
    � functools re      sqlite3
@@ -65,16 +65,16 @@
                  __dict__
                  __suppress_context__
                  __traceback__
                  args
           
          class CryptSQL(builtins.object)
              CryptSQL(readOnly=True)
-   �      
-             Encrypted SQL database.
+              
+   �     Encrypted SQL database.
               
                Methods defined here:
                  __init__(self, readOnly=True)
                      readOnly: If True, no commit is possible.
                  close(self)
                      Close the currently opened database.
                      This does not commit. All uncommitted changes are lost.
@@ -94,41 +94,42 @@
                      Get the current passphrase string for encryption and decryption.
                  importSqlScript(self, script, clear=True)
                      Imports a plain text dump into the database.
                      script: The script string to import.
                      clear: If True, drop all tables from the database before importing.
                  isOpen(self)
                      Returns True, if a database file is opened.
-              open(self, filename)
-                     Open a database file and decrypt its contents into memory.
-                    filename: The database file path.
-                 setKey(self, key)
+                 open(self, filename)
+                  Open a database file and decrypt its contents into memory.
+                     filename: The database file path.
+                setKey(self, key)
                      Set the raw key.
                      Do not use this. setPassphrase probably is what you want.
                  setPassphrase(self, passphrase)
                      Set a new passphrase string for encryption and decryption.
                  setRegexpFlags(self, search=True, ignoreCase=True, multiLine=True, dotAll=True)
                      Change the behavior of the REGEXP operator.
                  sqlCreateFunction(self, name, nrParams, func)
                      Create an SQL function.
                      See sqlite3.Connection.create_function for more details.
                  sqlExec(self, code, params=[])
                      Execute one SQL statement.
                  sqlExecScript(self, code)
                      Execute multiple SQL statements.
+                     Warning: This implicitly commits pending transactions before executing.
                  sqlIsEmpty(self)
                      Returns True, if the database does not contain any tables.
                  sqlPlainDump(self)
                      Get a plain text dump of the database.
                      Returns a string.
                  sqlVacuum(self)
                      Run the SQL VACUUM statement.
                      This also commits all changes to the SQL database,
                      but not to the database file.
-               ===================================================================================
+               ====================================================================================
                Data descriptors defined here:
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
  
 Data
```

### Comparing `pwman-python-2.7/doc/api/libpwman/database.html` & `pwman-python-2.8/doc/api/libpwman/database.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module database</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">database</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/database.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/database.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/database.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/database.py</a></td></tr></table>
     <p><span class="code">#<br>
 #&nbsp;Simple&nbsp;password&nbsp;manager<br>
 #&nbsp;Encrypted&nbsp;database<br>
 #<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.<br>
 #</span></p>
@@ -144,14 +144,17 @@
 key:&nbsp;An&nbsp;optional&nbsp;key&nbsp;to&nbsp;use&nbsp;instead&nbsp;of&nbsp;the&nbsp;passphrase.&nbsp;Don't&nbsp;use&nbsp;it.<br>
 readOnly:&nbsp;Open&nbsp;the&nbsp;filename&nbsp;read-only.&nbsp;Commits&nbsp;will&nbsp;raise&nbsp;an&nbsp;exception.<br>
 silent:&nbsp;Do&nbsp;not&nbsp;print&nbsp;information&nbsp;messages&nbsp;to&nbsp;the&nbsp;console.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-addEntry"><strong>addEntry</strong></a>(self, entry)</dt><dd><span class="code">Create&nbsp;a&nbsp;new&nbsp;entry&nbsp;in&nbsp;the&nbsp;database.<br>
 entry:&nbsp;A&nbsp;<a href="#PWManEntry">PWManEntry</a>()&nbsp;instance.</span></dd></dl>
 
+<dl><dt><a name="PWManDatabase-categoryExists"><strong>categoryExists</strong></a>(self, category)</dt><dd><span class="code">Returns&nbsp;True,&nbsp;if&nbsp;a&nbsp;category&nbsp;exists&nbsp;in&nbsp;the&nbsp;database.<br>
+category:&nbsp;The&nbsp;name&nbsp;string&nbsp;of&nbsp;the&nbsp;category.</span></dd></dl>
+
 <dl><dt><a name="PWManDatabase-commit"><strong>commit</strong></a>(self)</dt><dd><span class="code">Write&nbsp;all&nbsp;changes&nbsp;to&nbsp;the&nbsp;encrypted&nbsp;database&nbsp;file.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-delEntry"><strong>delEntry</strong></a>(self, entry)</dt><dd><span class="code">Delete&nbsp;an&nbsp;existing&nbsp;entry&nbsp;from&nbsp;the&nbsp;database.<br>
 entry:&nbsp;The&nbsp;<a href="#PWManEntry">PWManEntry</a>()&nbsp;instance&nbsp;to&nbsp;delete&nbsp;from&nbsp;the&nbsp;database.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-dropUncommitted"><strong>dropUncommitted</strong></a>(self)</dt><dd><span class="code">Drop&nbsp;all&nbsp;changes&nbsp;that&nbsp;are&nbsp;not&nbsp;committed,&nbsp;yet.</span></dd></dl>
 
@@ -228,23 +231,23 @@
 
 <dl><dt><a name="PWManDatabase-importSqlScript"><strong>importSqlScript</strong></a>(self, *args, **kwargs)</dt><dd><span class="code">Imports&nbsp;a&nbsp;plain&nbsp;text&nbsp;dump&nbsp;into&nbsp;the&nbsp;database.<br>
 script:&nbsp;The&nbsp;script&nbsp;string&nbsp;to&nbsp;import.<br>
 clear:&nbsp;If&nbsp;True,&nbsp;drop&nbsp;all&nbsp;tables&nbsp;from&nbsp;the&nbsp;database&nbsp;before&nbsp;importing.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-isDirty"><strong>isDirty</strong></a>(self)</dt><dd><span class="code">Returns&nbsp;True,&nbsp;if&nbsp;the&nbsp;database&nbsp;contains&nbsp;uncommitted&nbsp;data.</span></dd></dl>
 
+<dl><dt><a name="PWManDatabase-moveEntries"><strong>moveEntries</strong></a>(self, fromCategory, toCategory)</dt><dd><span class="code">Move&nbsp;all&nbsp;entries&nbsp;from&nbsp;one&nbsp;category&nbsp;to&nbsp;another&nbsp;category.<br>
+fromCategory:&nbsp;The&nbsp;category&nbsp;to&nbsp;move&nbsp;all&nbsp;entries&nbsp;from.<br>
+toCategory:&nbsp;The&nbsp;(new)&nbsp;category&nbsp;to&nbsp;move&nbsp;all&nbsp;entries&nbsp;to.</span></dd></dl>
+
 <dl><dt><a name="PWManDatabase-moveEntry"><strong>moveEntry</strong></a>(self, entry, newCategory, newTitle)</dt><dd><span class="code">Move&nbsp;an&nbsp;existing&nbsp;entry&nbsp;to&nbsp;a&nbsp;new&nbsp;category&nbsp;and/or&nbsp;set&nbsp;a&nbsp;new&nbsp;entry&nbsp;title.<br>
 entry:&nbsp;The&nbsp;<a href="#PWManEntry">PWManEntry</a>()&nbsp;instance&nbsp;to&nbsp;move.<br>
 newCategory:&nbsp;The&nbsp;new&nbsp;category&nbsp;name&nbsp;string.<br>
 newTitle:&nbsp;The&nbsp;new&nbsp;title&nbsp;string.</span></dd></dl>
 
-<dl><dt><a name="PWManDatabase-renameCategory"><strong>renameCategory</strong></a>(self, category, toCategory)</dt><dd><span class="code">Change&nbsp;the&nbsp;name&nbsp;of&nbsp;a&nbsp;category.<br>
-category:&nbsp;The&nbsp;old&nbsp;name&nbsp;string&nbsp;of&nbsp;the&nbsp;category.<br>
-toCategory:&nbsp;The&nbsp;new&nbsp;name&nbsp;string&nbsp;of&nbsp;the&nbsp;category.</span></dd></dl>
-
 <dl><dt><a name="PWManDatabase-setEntryAttr"><strong>setEntryAttr</strong></a>(self, entryAttr)</dt><dd><span class="code">Set&nbsp;an&nbsp;attribute&nbsp;associated&nbsp;with&nbsp;an&nbsp;entry.<br>
 entryAttr:&nbsp;The&nbsp;new&nbsp;<a href="#PWManEntryAttr">PWManEntryAttr</a>()&nbsp;instance&nbsp;to&nbsp;write&nbsp;to&nbsp;the&nbsp;database.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;entryAttr.data&nbsp;is&nbsp;None,&nbsp;then&nbsp;the&nbsp;attribute&nbsp;is&nbsp;deleted.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-setEntryBulk"><strong>setEntryBulk</strong></a>(self, entryBulk)</dt><dd><span class="code">Set&nbsp;the&nbsp;bulk&nbsp;data&nbsp;associated&nbsp;with&nbsp;an&nbsp;entry.<br>
 entryBulk:&nbsp;The&nbsp;new&nbsp;<a href="#PWManEntryBulk">PWManEntryBulk</a>()&nbsp;instance&nbsp;to&nbsp;write&nbsp;to&nbsp;the&nbsp;database.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;entryBulk.data&nbsp;is&nbsp;None,&nbsp;then&nbsp;the&nbsp;bulk&nbsp;data&nbsp;is&nbsp;deleted.</span></dd></dl>
@@ -291,15 +294,16 @@
 <dl><dt><a name="PWManDatabase-setRegexpFlags"><strong>setRegexpFlags</strong></a>(self, search=True, ignoreCase=True, multiLine=True, dotAll=True)</dt><dd><span class="code">Change&nbsp;the&nbsp;behavior&nbsp;of&nbsp;the&nbsp;REGEXP&nbsp;operator.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-sqlCreateFunction"><strong>sqlCreateFunction</strong></a>(self, name, nrParams, func)</dt><dd><span class="code">Create&nbsp;an&nbsp;SQL&nbsp;function.<br>
 See&nbsp;sqlite3.Connection.create_function&nbsp;for&nbsp;more&nbsp;details.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-sqlExec"><strong>sqlExec</strong></a>(self, code, params=[])</dt><dd><span class="code">Execute&nbsp;one&nbsp;SQL&nbsp;statement.</span></dd></dl>
 
-<dl><dt><a name="PWManDatabase-sqlExecScript"><strong>sqlExecScript</strong></a>(self, code)</dt><dd><span class="code">Execute&nbsp;multiple&nbsp;SQL&nbsp;statements.</span></dd></dl>
+<dl><dt><a name="PWManDatabase-sqlExecScript"><strong>sqlExecScript</strong></a>(self, code)</dt><dd><span class="code">Execute&nbsp;multiple&nbsp;SQL&nbsp;statements.<br>
+Warning:&nbsp;This&nbsp;implicitly&nbsp;commits&nbsp;pending&nbsp;transactions&nbsp;before&nbsp;executing.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-sqlIsEmpty"><strong>sqlIsEmpty</strong></a>(self)</dt><dd><span class="code">Returns&nbsp;True,&nbsp;if&nbsp;the&nbsp;database&nbsp;does&nbsp;not&nbsp;contain&nbsp;any&nbsp;tables.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-sqlPlainDump"><strong>sqlPlainDump</strong></a>(self)</dt><dd><span class="code">Get&nbsp;a&nbsp;plain&nbsp;text&nbsp;dump&nbsp;of&nbsp;the&nbsp;database.<br>
 Returns&nbsp;a&nbsp;string.</span></dd></dl>
 
 <dl><dt><a name="PWManDatabase-sqlVacuum"><strong>sqlVacuum</strong></a>(self)</dt><dd><span class="code">Run&nbsp;the&nbsp;SQL&nbsp;VACUUM&nbsp;statement.<br>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
         index
-database /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/
+database /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/
          database.py
 #
 # Simple password manager
 # Encrypted database
 #
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
@@ -93,14 +93,17 @@
                      passphrase: The passphrase string for the database file.
                      key: An optional key to use instead of the passphrase. Don't use it.
                      readOnly: Open the filename read-only. Commits will raise an exception.
                      silent: Do not print information messages to the console.
                  addEntry(self, entry)
                      Create a new entry in the database.
                      entry: A PWManEntry() instance.
+                 categoryExists(self, category)
+                     Returns True, if a category exists in the database.
+                     category: The name string of the category.
                  commit(self)
                      Write all changes to the encrypted database file.
                  delEntry(self, entry)
                      Delete an existing entry from the database.
                      entry: The PWManEntry() instance to delete from the database.
                  dropUncommitted(self)
                      Drop all changes that are not committed, yet.
@@ -163,39 +166,39 @@
                      Returns a PWManEntryBulk() instance or None, if there is no bulk data.
                  getEntryTitles(self, category)
                      Get all titles from one category in the database.
                      category: The category name string.
                      Returns a sorted list of strings.
                  getEntryTotp(self, entry)
                      Get the TOTP parameters associated with an entry.
-                     entry: The PWManEntry() to get the TOTP parameters for.
-                  Returns a PWManEntryTOTP() instance, or None if there is no TOTP data.
-                 getGlobalAttr(self, name)
-                    Get a global attribute.
+                  entry: The PWManEntry() to get the TOTP parameters for.
+                     Returns a PWManEntryTOTP() instance, or None if there is no TOTP data.
+                getGlobalAttr(self, name)
+                     Get a global attribute.
                      A global attribute is not associated with an entry.
                      Returns None, if the attribute does not exist.
                  getOnDiskDb(self)
                      Get a read-only instance of PWManDatabase that contains
                      the current on-disk data. The on-disk data is the data
                      at the last commit.
                  importSqlScript(self, *args, **kwargs)
                      Imports a plain text dump into the database.
                      script: The script string to import.
                      clear: If True, drop all tables from the database before importing.
                  isDirty(self)
                      Returns True, if the database contains uncommitted data.
+                 moveEntries(self, fromCategory, toCategory)
+                     Move all entries from one category to another category.
+                     fromCategory: The category to move all entries from.
+                     toCategory: The (new) category to move all entries to.
                  moveEntry(self, entry, newCategory, newTitle)
                      Move an existing entry to a new category and/or set a new entry title.
                      entry: The PWManEntry() instance to move.
                      newCategory: The new category name string.
                      newTitle: The new title string.
-                 renameCategory(self, category, toCategory)
-                     Change the name of a category.
-                     category: The old name string of the category.
-                     toCategory: The new name string of the category.
                  setEntryAttr(self, entryAttr)
                      Set an attribute associated with an entry.
                      entryAttr: The new PWManEntryAttr() instance to write to the database.
                                 If entryAttr.data is None, then the attribute is deleted.
                  setEntryBulk(self, entryBulk)
                      Set the bulk data associated with an entry.
                      entryBulk: The new PWManEntryBulk() instance to write to the database.
@@ -206,16 +209,16 @@
                                 If entryTotp.key is None, then the TOTP data is deleted.
                  setGlobalAttr(self, name, data, setDirty=True)
                      Set a global attribute.
                      A global attribute is not associated with an entry.
                      If data is None or empty, the attribute is deleted from the database.
                  setPassphrase(self, passphrase)
                      Set a new passphrase string for encryption and decryption.
-               ==============================================================================================
-   �       Data and other attributes defined here:
+   �       ==============================================================================================
+               Data and other attributes defined here:
                  DB_TYPE = 'PWMan database'
                  DB_VER = ('0', '1')
                ==============================================================================================
                Methods inherited from libpwman.cryptsql.CryptSQL:
                  close(self)
                      Close the currently opened database.
                      This does not commit. All uncommitted changes are lost.
@@ -242,14 +245,15 @@
                  sqlCreateFunction(self, name, nrParams, func)
                      Create an SQL function.
                      See sqlite3.Connection.create_function for more details.
                  sqlExec(self, code, params=[])
                      Execute one SQL statement.
                  sqlExecScript(self, code)
                      Execute multiple SQL statements.
+                     Warning: This implicitly commits pending transactions before executing.
                  sqlIsEmpty(self)
                      Returns True, if the database does not contain any tables.
                  sqlPlainDump(self)
                      Get a plain text dump of the database.
                      Returns a string.
                  sqlVacuum(self)
                      Run the SQL VACUUM statement.
```

### Comparing `pwman-python-2.7/doc/api/libpwman/dbdiff.html` & `pwman-python-2.8/doc/api/libpwman/dbdiff.html`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module dbdiff</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">dbdiff</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/dbdiff.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/dbdiff.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/dbdiff.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/dbdiff.py</a></td></tr></table>
     <p><span class="code">#&nbsp;Simple&nbsp;password&nbsp;manager<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor pkg-content-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
       index
-dbdiff /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/
+dbdiff /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/
        dbdiff.py
 # Simple password manager
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Modules
    � difflib
```

### Comparing `pwman-python-2.7/doc/api/libpwman/exception.html` & `pwman-python-2.8/doc/api/libpwman/exception.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module exception</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">exception</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/exception.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/exception.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/exception.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/exception.py</a></td></tr></table>
     <p><span class="code">#&nbsp;Simple&nbsp;password&nbsp;manager<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor index-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Classes</strong></td></tr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
          index
-exception /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/
+exception /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/
           exception.py
 # Simple password manager
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Classes
            builtins.Exception(builtins.BaseException)
```

### Comparing `pwman-python-2.7/doc/api/libpwman/fileobj.html` & `pwman-python-2.8/doc/api/libpwman/fileobj.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module fileobj</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">fileobj</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/fileobj.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/fileobj.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/fileobj.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/fileobj.py</a></td></tr></table>
     <p><span class="code">#&nbsp;Simple&nbsp;<a href="builtins.html#object">object</a>&nbsp;file&nbsp;format.<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor pkg-content-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
        index
-fileobj /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/
+fileobj /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/
         fileobj.py
 # Simple object file format.
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Modules
    � errno
```

### Comparing `pwman-python-2.7/doc/api/libpwman/mlock.html` & `pwman-python-2.8/doc/api/libpwman/mlock.html`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module mlock</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">mlock</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/mlock.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/mlock.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/mlock.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/mlock.py</a></td></tr></table>
     <p><span class="code">#&nbsp;mlock&nbsp;support<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2019-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor pkg-content-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
      index
-mlock /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/mlock.py
+mlock /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/mlock.py
 # mlock support
 # Copyright (c) 2019-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Modules
    � os platform sys
```

### Comparing `pwman-python-2.7/doc/api/libpwman/otp.html` & `pwman-python-2.8/doc/api/libpwman/otp.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module otp</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">otp</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/otp.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/otp.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/otp.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/otp.py</a></td></tr></table>
     <p><span class="code">#&nbsp;HOTP/TOTP&nbsp;support<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2019-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor pkg-content-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
    index
-otp /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/otp.py
+otp /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/otp.py
 # HOTP/TOTP support
 # Copyright (c) 2019-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Modules
    � binascii hashlib hmac time
```

### Comparing `pwman-python-2.7/doc/api/libpwman/ui.html` & `pwman-python-2.8/doc/api/libpwman/ui.html`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <meta charset="utf-8">
 <title>Python: module ui</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">ui</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/ui.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/ui.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/ui.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/ui.py</a></td></tr></table>
     <p><span class="code">#&nbsp;Simple&nbsp;password&nbsp;manager<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor pkg-content-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
@@ -49,38 +49,52 @@
 </dl>
  <p>
 <table class="section">
 <tr class="decor title-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong>PWMan</strong> = <a name="PWMan">class __classcell__</a>(<a href="cmd.html#Cmd">cmd.Cmd</a>)</td></tr>
     
 <tr><td class="decor title-decor" rowspan=2><span class="code">&nbsp;&nbsp;&nbsp;</span></td>
-<td class="decor title-decor" colspan=2><span class="code"><a href="#PWMan">PWMan</a>(filename,&nbsp;passphrase,&nbsp;commitClearsUndo=False,&nbsp;timeout=None)<br>
+<td class="decor title-decor" colspan=2><span class="code"><a href="#PWMan">PWMan</a>(filename,&nbsp;passphrase,&nbsp;timeout=None)<br>
 &nbsp;<br>
 <br>&nbsp;</span></td></tr>
 <tr><td>&nbsp;</td>
 <td class="singlecolumn"><dl><dt>Method resolution order:</dt>
 <dd>__classcell__</dd>
 <dd><a href="cmd.html#Cmd">cmd.Cmd</a></dd>
 <dd><a href="builtins.html#object">builtins.object</a></dd>
 </dl>
 <hr>
 Methods defined here:<br>
-<dl><dt><a name="__classcell__-__init__"><strong>__init__</strong></a>(self, filename, passphrase, commitClearsUndo=False, timeout=None)</dt><dd><span class="code">Instantiate&nbsp;a&nbsp;line-oriented&nbsp;interpreter&nbsp;framework.<br>
+<dl><dt><a name="__classcell__-__init__"><strong>__init__</strong></a>(self, filename, passphrase, timeout=None)</dt><dd><span class="code">Instantiate&nbsp;a&nbsp;line-oriented&nbsp;interpreter&nbsp;framework.<br>
 &nbsp;<br>
 The&nbsp;optional&nbsp;argument&nbsp;'completekey'&nbsp;is&nbsp;the&nbsp;readline&nbsp;name&nbsp;of&nbsp;a<br>
 completion&nbsp;key;&nbsp;it&nbsp;defaults&nbsp;to&nbsp;the&nbsp;Tab&nbsp;key.&nbsp;If&nbsp;completekey&nbsp;is<br>
 not&nbsp;None&nbsp;and&nbsp;the&nbsp;readline&nbsp;module&nbsp;is&nbsp;available,&nbsp;command&nbsp;completion<br>
 is&nbsp;done&nbsp;automatically.&nbsp;The&nbsp;optional&nbsp;arguments&nbsp;stdin&nbsp;and&nbsp;stdout<br>
 specify&nbsp;alternate&nbsp;input&nbsp;and&nbsp;output&nbsp;file&nbsp;objects;&nbsp;if&nbsp;not&nbsp;specified,<br>
 sys.stdin&nbsp;and&nbsp;sys.stdout&nbsp;are&nbsp;used.</span></dd></dl>
 
 <dl><dt><a name="__classcell__-complete_add"><strong>complete_add</strong></a> = __complete_category_title(self, text, line, begidx, endidx)</dt></dl>
 
+<dl><dt><a name="__classcell__-complete_c"><strong>complete_c</strong></a> = <a href="#__classcell__-complete_commit">complete_commit</a>(self, text, line, begidx, endidx)</dt></dl>
+
 <dl><dt><a name="__classcell__-complete_cat"><strong>complete_cat</strong></a> = __complete_category_title_item(self, text, line, begidx, endidx)</dt></dl>
 
+<dl><dt><a name="__classcell__-complete_close"><strong>complete_close</strong></a>(self, text, line, begidx, endidx)</dt></dl>
+
+<dl><dt><a name="__classcell__-complete_commit"><strong>complete_commit</strong></a>(self, text, line, begidx, endidx)</dt></dl>
+
+<dl><dt><a name="__classcell__-complete_copy"><strong>complete_copy</strong></a> = <a href="#__classcell__-complete_move">complete_move</a>(self, text, line, begidx, endidx)</dt></dl>
+
+<dl><dt><a name="__classcell__-complete_cp"><strong>complete_cp</strong></a> = <a href="#__classcell__-complete_move">complete_move</a>(self, text, line, begidx, endidx)</dt></dl>
+
+<dl><dt><a name="__classcell__-complete_database"><strong>complete_database</strong></a>(self, text, line, begidx, endidx)</dt></dl>
+
+<dl><dt><a name="__classcell__-complete_db"><strong>complete_db</strong></a> = <a href="#__classcell__-complete_database">complete_database</a>(self, text, line, begidx, endidx)</dt></dl>
+
 <dl><dt><a name="__classcell__-complete_dbdump"><strong>complete_dbdump</strong></a>(self, text, line, begidx, endidx)</dt></dl>
 
 <dl><dt><a name="__classcell__-complete_dbimport"><strong>complete_dbimport</strong></a>(self, text, line, begidx, endidx)</dt></dl>
 
 <dl><dt><a name="__classcell__-complete_del"><strong>complete_del</strong></a> = __complete_category_title(self, text, line, begidx, endidx)</dt></dl>
 
 <dl><dt><a name="__classcell__-complete_diff"><strong>complete_diff</strong></a>(self, text, line, begidx, endidx)</dt></dl>
@@ -127,42 +141,108 @@
 
 <dl><dt><a name="__classcell__-complete_rm"><strong>complete_rm</strong></a> = __complete_category_title(self, text, line, begidx, endidx)</dt></dl>
 
 <dl><dt><a name="__classcell__-complete_t"><strong>complete_t</strong></a> = __complete_category_title(self, text, line, begidx, endidx)</dt></dl>
 
 <dl><dt><a name="__classcell__-complete_totp"><strong>complete_totp</strong></a> = __complete_category_title(self, text, line, begidx, endidx)</dt></dl>
 
+<dl><dt><a name="__classcell__-complete_w"><strong>complete_w</strong></a> = <a href="#__classcell__-complete_commit">complete_commit</a>(self, text, line, begidx, endidx)</dt></dl>
+
 <dl><dt><a name="__classcell__-default"><strong>default</strong></a>(self, line)</dt><dd><span class="code">Called&nbsp;on&nbsp;an&nbsp;input&nbsp;line&nbsp;when&nbsp;the&nbsp;command&nbsp;prefix&nbsp;is&nbsp;not&nbsp;recognized.<br>
 &nbsp;<br>
 If&nbsp;this&nbsp;method&nbsp;is&nbsp;not&nbsp;overridden,&nbsp;it&nbsp;prints&nbsp;an&nbsp;error&nbsp;message&nbsp;and<br>
 returns.</span></dd></dl>
 
 <dl><dt><a name="__classcell__-do_EOF"><strong>do_EOF</strong></a> = <a href="#__classcell__-do_quit">do_quit</a>(self, params)</dt></dl>
 
 <dl><dt><a name="__classcell__-do_add"><strong>do_add</strong></a> = <a href="#__classcell__-do_new">do_new</a>(self, params)</dt></dl>
 
 <dl><dt><a name="__classcell__-do_c"><strong>do_c</strong></a> = <a href="#__classcell__-do_commit">do_commit</a>(self, params)</dt></dl>
 
 <dl><dt><a name="__classcell__-do_cat"><strong>do_cat</strong></a> = <a href="#__classcell__-do_list">do_list</a>(self, params)</dt></dl>
 
-<dl><dt><a name="__classcell__-do_cls"><strong>do_cls</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Clear&nbsp;console&nbsp;screen&nbsp;and&nbsp;undo/redo&nbsp;buffer&nbsp;---<br>
+<dl><dt><a name="__classcell__-do_close"><strong>do_close</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Close&nbsp;a&nbsp;database&nbsp;---<br>
+Command:&nbsp;close&nbsp;[!]&nbsp;[NAME]<br>
+&nbsp;<br>
+If&nbsp;NAME&nbsp;is&nbsp;not&nbsp;given,&nbsp;then&nbsp;this&nbsp;closes&nbsp;the&nbsp;currently&nbsp;selected&nbsp;database.<br>
+If&nbsp;NAME&nbsp;is&nbsp;given,&nbsp;then&nbsp;this&nbsp;closes&nbsp;the&nbsp;named&nbsp;database.<br>
+&nbsp;<br>
+If&nbsp;!&nbsp;is&nbsp;specified,&nbsp;then&nbsp;the&nbsp;uncommitted&nbsp;changes&nbsp;will&nbsp;be&nbsp;dropped.<br>
+&nbsp;<br>
+If&nbsp;the&nbsp;currently&nbsp;used&nbsp;database&nbsp;is&nbsp;closed,&nbsp;the&nbsp;selected&nbsp;database<br>
+will&nbsp;be&nbsp;switched&nbsp;to&nbsp;'main'.<br>
+&nbsp;<br>
+The&nbsp;'main'&nbsp;database&nbsp;can&nbsp;only&nbsp;be&nbsp;closed&nbsp;last,<br>
+which&nbsp;in&nbsp;turn&nbsp;closes&nbsp;the&nbsp;application.<br>
+&nbsp;<br>
+Aliases:&nbsp;None</span></dd></dl>
+
+<dl><dt><a name="__classcell__-do_cls"><strong>do_cls</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Clear&nbsp;console&nbsp;screen&nbsp;---<br>
 Command:&nbsp;cls<br>
 &nbsp;<br>
-Clear&nbsp;the&nbsp;console&nbsp;screen&nbsp;and&nbsp;all&nbsp;undo/redo&nbsp;buffers.<br>
+Clear&nbsp;the&nbsp;console&nbsp;screen.<br>
 Note&nbsp;that&nbsp;this&nbsp;does&nbsp;not&nbsp;clear&nbsp;a&nbsp;possibly&nbsp;existing<br>
 'screen'&nbsp;session&nbsp;buffer&nbsp;or&nbsp;other&nbsp;advanced&nbsp;console&nbsp;buffers.<br>
 &nbsp;<br>
 Aliases:&nbsp;None</span></dd></dl>
 
-<dl><dt><a name="__classcell__-do_commit"><strong>do_commit</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Write&nbsp;changes&nbsp;to&nbsp;the&nbsp;database&nbsp;file&nbsp;---<br>
-&nbsp;<br>
+<dl><dt><a name="__classcell__-do_commit"><strong>do_commit</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Write&nbsp;changes&nbsp;to&nbsp;the&nbsp;database&nbsp;file(s)&nbsp;---<br>
 Command:&nbsp;commit<br>
 &nbsp;<br>
+Options:<br>
+&nbsp;&nbsp;-a&nbsp;&nbsp;&nbsp;Commit&nbsp;all&nbsp;open&nbsp;databases.<br>
+&nbsp;<br>
 Aliases:&nbsp;c&nbsp;w</span></dd></dl>
 
+<dl><dt><a name="__classcell__-do_copy"><strong>do_copy</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Copy&nbsp;an&nbsp;entry&nbsp;or&nbsp;a&nbsp;category&nbsp;---<br>
+&nbsp;<br>
+Copy&nbsp;an&nbsp;existing&nbsp;entry:<br>
+Command:&nbsp;copy&nbsp;CATEGORY&nbsp;TITLE&nbsp;TO_CATEGORY&nbsp;[NEW_TITLE]<br>
+(NEW_TITLE&nbsp;defaults&nbsp;to&nbsp;TITLE)<br>
+&nbsp;<br>
+Copy&nbsp;all&nbsp;entries&nbsp;from&nbsp;a&nbsp;category&nbsp;into&nbsp;another&nbsp;category:<br>
+Command:&nbsp;copy&nbsp;FROM_CATEGORY&nbsp;TO_CATEGORY<br>
+&nbsp;<br>
+Copy&nbsp;an&nbsp;entry&nbsp;from&nbsp;one&nbsp;database&nbsp;to&nbsp;another:<br>
+Command:&nbsp;copy&nbsp;-s&nbsp;main&nbsp;-d&nbsp;other&nbsp;CATEGORY&nbsp;TITLE&nbsp;TO_CATEGORY&nbsp;[NEW_TITLE]<br>
+(NEW_TITLE&nbsp;defaults&nbsp;to&nbsp;TITLE)<br>
+&nbsp;<br>
+Copy&nbsp;all&nbsp;entries&nbsp;from&nbsp;a&nbsp;category&nbsp;from&nbsp;one&nbsp;database&nbsp;into&nbsp;another&nbsp;database:<br>
+Command:&nbsp;copy&nbsp;-s&nbsp;main&nbsp;-d&nbsp;other&nbsp;FROM_CATEGORY&nbsp;[TO_CATEGORY]<br>
+(TO_CATEGORY&nbsp;defaults&nbsp;to&nbsp;FROM_CATEGORY)<br>
+&nbsp;<br>
+Options:<br>
+&nbsp;&nbsp;-s&nbsp;SOURCE_DATABASE_NAME<br>
+&nbsp;&nbsp;-d&nbsp;DESTINATION_DATABASE_NAME<br>
+&nbsp;&nbsp;Databases&nbsp;default&nbsp;to&nbsp;the&nbsp;currently&nbsp;selected&nbsp;database.<br>
+&nbsp;&nbsp;The&nbsp;named&nbsp;databases&nbsp;must&nbsp;be&nbsp;open.&nbsp;See&nbsp;'database'&nbsp;command.<br>
+&nbsp;<br>
+Aliases:&nbsp;cp</span></dd></dl>
+
+<dl><dt><a name="__classcell__-do_cp"><strong>do_cp</strong></a> = <a href="#__classcell__-do_copy">do_copy</a>(self, params)</dt></dl>
+
+<dl><dt><a name="__classcell__-do_database"><strong>do_database</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Open&nbsp;a&nbsp;database&nbsp;or&nbsp;switch&nbsp;to&nbsp;an&nbsp;already&nbsp;opened&nbsp;database&nbsp;---<br>
+Command:&nbsp;database&nbsp;[-f&nbsp;FILEPATH]&nbsp;[NAME]<br>
+&nbsp;<br>
+If&nbsp;neither&nbsp;FILEPATH&nbsp;nor&nbsp;NAME&nbsp;are&nbsp;given,&nbsp;then<br>
+a&nbsp;list&nbsp;of&nbsp;all&nbsp;currently&nbsp;opened&nbsp;databases&nbsp;will&nbsp;be&nbsp;printed.<br>
+The&nbsp;currently&nbsp;selected&nbsp;database&nbsp;will&nbsp;be&nbsp;marked&nbsp;with&nbsp;[@].<br>
+All&nbsp;databases&nbsp;with&nbsp;uncommitted&nbsp;changes&nbsp;will&nbsp;be&nbsp;marked&nbsp;with&nbsp;[*].<br>
+&nbsp;<br>
+If&nbsp;only&nbsp;NAME&nbsp;is&nbsp;given,&nbsp;then&nbsp;the&nbsp;selected&nbsp;database&nbsp;will<br>
+be&nbsp;switched&nbsp;to&nbsp;the&nbsp;named&nbsp;one.&nbsp;NAME&nbsp;must&nbsp;already&nbsp;be&nbsp;open.<br>
+&nbsp;<br>
+A&nbsp;new&nbsp;database&nbsp;can&nbsp;be&nbsp;opened&nbsp;with&nbsp;-f&nbsp;FILEPATH.<br>
+NAME&nbsp;is&nbsp;optional&nbsp;in&nbsp;this&nbsp;case.<br>
+The&nbsp;selected&nbsp;database&nbsp;will&nbsp;be&nbsp;switched&nbsp;to&nbsp;the&nbsp;newly&nbsp;opened&nbsp;one.<br>
+&nbsp;<br>
+Aliases:&nbsp;db</span></dd></dl>
+
+<dl><dt><a name="__classcell__-do_db"><strong>do_db</strong></a> = <a href="#__classcell__-do_database">do_database</a>(self, params)</dt></dl>
+
 <dl><dt><a name="__classcell__-do_dbdump"><strong>do_dbdump</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Dump&nbsp;the&nbsp;pwman&nbsp;SQL&nbsp;database&nbsp;---<br>
 Command:&nbsp;dbdump&nbsp;[OPTS]&nbsp;[FILEPATH]<br>
 &nbsp;<br>
 If&nbsp;FILEPATH&nbsp;is&nbsp;given,&nbsp;the&nbsp;database&nbsp;is&nbsp;dumped<br>
 unencrypted&nbsp;to&nbsp;the&nbsp;file.<br>
 If&nbsp;FILEPATH&nbsp;is&nbsp;omitted,&nbsp;the&nbsp;database&nbsp;is&nbsp;dumped<br>
 unencrypted&nbsp;to&nbsp;stdout.<br>
@@ -291,16 +371,18 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;none&nbsp;of&nbsp;them&nbsp;are&nbsp;specified&nbsp;by&nbsp;the&nbsp;user.<br>
 &nbsp;<br>
 Aliases:&nbsp;f</span></dd></dl>
 
 <dl><dt><a name="__classcell__-do_h"><strong>do_h</strong></a> = <a href="#__classcell__-do_help">do_help</a>(self, params)</dt></dl>
 
 <dl><dt><a name="__classcell__-do_help"><strong>do_help</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Shows&nbsp;help&nbsp;text&nbsp;about&nbsp;a&nbsp;command&nbsp;---<br>
+Command:&nbsp;help&nbsp;[COMMAND]<br>
 &nbsp;<br>
-Command:&nbsp;help<br>
+If&nbsp;COMMAND&nbsp;is&nbsp;not&nbsp;given:&nbsp;Show&nbsp;a&nbsp;command&nbsp;summary.<br>
+If&nbsp;COMMAND&nbsp;is&nbsp;given:&nbsp;Show&nbsp;detailed&nbsp;help&nbsp;about&nbsp;that&nbsp;command.<br>
 &nbsp;<br>
 Aliases:&nbsp;h</span></dd></dl>
 
 <dl><dt><a name="__classcell__-do_list"><strong>do_list</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Print&nbsp;a&nbsp;listing&nbsp;---<br>
 Command:&nbsp;list&nbsp;[category]&nbsp;[title]&nbsp;[item]<br>
 &nbsp;<br>
 If&nbsp;a&nbsp;category&nbsp;is&nbsp;given&nbsp;as&nbsp;parameter,&nbsp;list&nbsp;the&nbsp;<br>
@@ -310,26 +392,40 @@
 Item&nbsp;may&nbsp;be&nbsp;one&nbsp;of:&nbsp;user,&nbsp;password,&nbsp;bulk,&nbsp;totpkey&nbsp;or&nbsp;any&nbsp;attribute&nbsp;name.<br>
 &nbsp;<br>
 Aliases:&nbsp;ls&nbsp;cat</span></dd></dl>
 
 <dl><dt><a name="__classcell__-do_ls"><strong>do_ls</strong></a> = <a href="#__classcell__-do_list">do_list</a>(self, params)</dt></dl>
 
 <dl><dt><a name="__classcell__-do_masterp"><strong>do_masterp</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Change&nbsp;the&nbsp;master&nbsp;passphrase&nbsp;---<br>
-&nbsp;<br>
 Command:&nbsp;masterp<br>
 &nbsp;<br>
 Aliases:&nbsp;None</span></dd></dl>
 
 <dl><dt><a name="__classcell__-do_move"><strong>do_move</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Move/rename&nbsp;an&nbsp;existing&nbsp;entry&nbsp;or&nbsp;a&nbsp;category&nbsp;---<br>
 &nbsp;<br>
 Move/rename&nbsp;an&nbsp;existing&nbsp;entry:<br>
-Command:&nbsp;move&nbsp;category&nbsp;title&nbsp;newCategory&nbsp;[newTitle]<br>
+Command:&nbsp;move&nbsp;CATEGORY&nbsp;TITLE&nbsp;TO_CATEGORY&nbsp;[NEW_TITLE]<br>
+(NEW_TITLE&nbsp;defaults&nbsp;to&nbsp;TITLE)<br>
 &nbsp;<br>
-Rename&nbsp;an&nbsp;existing&nbsp;category:<br>
-Command:&nbsp;move&nbsp;category&nbsp;newCategory<br>
+Move&nbsp;all&nbsp;entries&nbsp;from&nbsp;one&nbsp;category&nbsp;into&nbsp;another&nbsp;category.<br>
+Command:&nbsp;move&nbsp;FROM_CATEGORY&nbsp;TO_CATEGORY<br>
+&nbsp;<br>
+Move&nbsp;an&nbsp;entry&nbsp;from&nbsp;one&nbsp;database&nbsp;to&nbsp;another:<br>
+Command:&nbsp;move&nbsp;-s&nbsp;main&nbsp;-d&nbsp;other&nbsp;CATEGORY&nbsp;TITLE&nbsp;TO_CATEGORY&nbsp;[NEW_TITLE]<br>
+(NEW_TITLE&nbsp;defaults&nbsp;to&nbsp;TITLE)<br>
+&nbsp;<br>
+Move&nbsp;all&nbsp;entries&nbsp;from&nbsp;a&nbsp;category&nbsp;from&nbsp;one&nbsp;database&nbsp;into&nbsp;another&nbsp;database:<br>
+Command:&nbsp;move&nbsp;-s&nbsp;main&nbsp;-d&nbsp;other&nbsp;FROM_CATEGORY&nbsp;[TO_CATEGORY]<br>
+(TO_CATEGORY&nbsp;defaults&nbsp;to&nbsp;FROM_CATEGORY)<br>
+&nbsp;<br>
+Options:<br>
+&nbsp;&nbsp;-s&nbsp;SOURCE_DATABASE_NAME<br>
+&nbsp;&nbsp;-d&nbsp;DESTINATION_DATABASE_NAME<br>
+&nbsp;&nbsp;Databases&nbsp;default&nbsp;to&nbsp;the&nbsp;currently&nbsp;selected&nbsp;database.<br>
+&nbsp;&nbsp;The&nbsp;named&nbsp;databases&nbsp;must&nbsp;be&nbsp;open.&nbsp;See&nbsp;'database'&nbsp;command.<br>
 &nbsp;<br>
 Aliases:&nbsp;mv&nbsp;rename</span></dd></dl>
 
 <dl><dt><a name="__classcell__-do_mv"><strong>do_mv</strong></a> = <a href="#__classcell__-do_move">do_move</a>(self, params)</dt></dl>
 
 <dl><dt><a name="__classcell__-do_n"><strong>do_n</strong></a> = <a href="#__classcell__-do_new">do_new</a>(self, params)</dt></dl>
 
@@ -346,22 +442,14 @@
 <dl><dt><a name="__classcell__-do_quit"><strong>do_quit</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Exit&nbsp;pwman&nbsp;---<br>
 Command:&nbsp;quit&nbsp;[!]<br>
 &nbsp;<br>
 Use&nbsp;the&nbsp;exclamation&nbsp;mark&nbsp;to&nbsp;force&nbsp;quit&nbsp;and&nbsp;discard&nbsp;changes.<br>
 &nbsp;<br>
 Aliases:&nbsp;q&nbsp;exit&nbsp;^D</span></dd></dl>
 
-<dl><dt><a name="__classcell__-do_redo"><strong>do_redo</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Redo&nbsp;the&nbsp;last&nbsp;undone&nbsp;command&nbsp;---<br>
-Command:&nbsp;redo<br>
-&nbsp;<br>
-Redoes&nbsp;the&nbsp;last&nbsp;undone&nbsp;command.<br>
-Also&nbsp;see&nbsp;'undo'&nbsp;help.<br>
-&nbsp;<br>
-Aliases:&nbsp;None</span></dd></dl>
-
 <dl><dt><a name="__classcell__-do_remove"><strong>do_remove</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Remove&nbsp;an&nbsp;existing&nbsp;entry&nbsp;---<br>
 Command:&nbsp;remove&nbsp;category&nbsp;[title]<br>
 &nbsp;<br>
 Remove&nbsp;an&nbsp;existing&nbsp;database&nbsp;entry.<br>
 &nbsp;<br>
 Aliases:&nbsp;rm&nbsp;del</span></dd></dl>
 
@@ -374,21 +462,14 @@
 <dl><dt><a name="__classcell__-do_totp"><strong>do_totp</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Generate&nbsp;a&nbsp;TOTP&nbsp;token&nbsp;---<br>
 Command:&nbsp;totp&nbsp;[CATEGORY&nbsp;TITLE]&nbsp;OR&nbsp;[TITLE]<br>
 &nbsp;<br>
 Generates&nbsp;a&nbsp;token&nbsp;using&nbsp;the&nbsp;Time-Based&nbsp;One-Time&nbsp;Password&nbsp;Algorithm.<br>
 &nbsp;<br>
 Aliases:&nbsp;t</span></dd></dl>
 
-<dl><dt><a name="__classcell__-do_undo"><strong>do_undo</strong></a>(self, params)</dt><dd><span class="code">---&nbsp;Undo&nbsp;the&nbsp;last&nbsp;command&nbsp;---<br>
-Command:&nbsp;undo<br>
-&nbsp;<br>
-Rewinds&nbsp;the&nbsp;last&nbsp;command&nbsp;that&nbsp;changed&nbsp;the&nbsp;database.<br>
-&nbsp;<br>
-Aliases:&nbsp;None</span></dd></dl>
-
 <dl><dt><a name="__classcell__-do_w"><strong>do_w</strong></a> = <a href="#__classcell__-do_commit">do_commit</a>(self, params)</dt></dl>
 
 <dl><dt><a name="__classcell__-emptyline"><strong>emptyline</strong></a>(self)</dt><dd><span class="code">Called&nbsp;when&nbsp;an&nbsp;empty&nbsp;line&nbsp;is&nbsp;entered&nbsp;in&nbsp;response&nbsp;to&nbsp;the&nbsp;prompt.<br>
 &nbsp;<br>
 If&nbsp;this&nbsp;method&nbsp;is&nbsp;not&nbsp;overridden,&nbsp;it&nbsp;repeats&nbsp;the&nbsp;last&nbsp;nonempty<br>
 command&nbsp;entered.</span></dd></dl>
 
@@ -403,23 +484,21 @@
 
 <dl><dt><a name="__classcell__-runOneCommand"><strong>runOneCommand</strong></a>(self, command)</dt></dl>
 
 <hr>
 Data and other attributes defined here:<br>
 <dl><dt><strong>CommandError</strong> = &lt;class 'ui.PWMan.CommandError'&gt;</dl>
 
-<dl><dt><strong>Opts</strong> = &lt;class 'ui.PWMan.Opts'&gt;<dd><span class="code"><a href="#PWMan-Opts">Opts</a>(_Opts__opts:&nbsp;list&nbsp;=&nbsp;&lt;factory&gt;,&nbsp;_Opts__params:&nbsp;list&nbsp;=&nbsp;&lt;factory&gt;,&nbsp;_Opts__atCmdIndex:&nbsp;dict&nbsp;=&nbsp;&lt;factory&gt;)</span></dl>
-
 <dl><dt><strong>Quit</strong> = &lt;class 'ui.PWMan.Quit'&gt;</dl>
 
-<dl><dt><strong>cmdHelpDatabase</strong> = (('commit', ('c', 'w'), 'Commit/write database file'), ('masterp', (), 'Change the master passphrase'), ('dbdump', (), 'Dump the database'), ('dbimport', (), 'Import a database dump file'), ('drop', (), 'Drop all uncommitted changes'))</dl>
+<dl><dt><strong>cmdHelpDatabase</strong> = (('database', ('db',), 'Open or select another database'), ('commit', ('c', 'w'), 'Commit/write selected db to disk'), ('drop', (), 'Drop uncommitted changes in selected db'), ('close', (), 'Close a database'), ('dbdump', (), 'Dump the selected database'), ('dbimport', (), 'Import a database dump file'), ('masterp', (), 'Change the master passphrase'))</dl>
 
-<dl><dt><strong>cmdHelpEdit</strong> = (('new', ('n', 'add'), 'Create new entry'), ('edit_user', ('eu',), "Edit the 'user' field of an entry"), ('edit_pw', ('ep',), "Edit the 'password' field of an entry"), ('edit_bulk', ('eb',), "Edit the 'bulk' field of an entry"), ('edit_totp', ('et',), 'Edit the TOTP key and parameters'), ('edit_attr', ('ea',), 'Edit an entry attribute'), ('move', ('mv', 'rename'), 'Move/rename an existing entry'), ('remove', ('rm', 'del'), 'Remove an existing entry'), ('undo', (), 'Undo the last command'), ('redo', (), 'Redo the last undone command'))</dl>
+<dl><dt><strong>cmdHelpEdit</strong> = (('new', ('n', 'add'), 'Create new entry'), ('edit_user', ('eu',), "Edit the 'user' field of an entry"), ('edit_pw', ('ep',), "Edit the 'password' field of an entry"), ('edit_bulk', ('eb',), "Edit the 'bulk' field of an entry"), ('edit_totp', ('et',), 'Edit the TOTP key and parameters'), ('edit_attr', ('ea',), 'Edit an entry attribute'), ('move', ('mv', 'rename'), 'Move/rename an existing entry'), ('copy', ('cp',), 'Copy an existing entry or category'), ('remove', ('rm', 'del'), 'Remove an existing entry'))</dl>
 
-<dl><dt><strong>cmdHelpMisc</strong> = (('help', ('h',), 'Show help about commands'), ('quit', ('q', 'exit', '^D'), 'Quit pwman'), ('cls', (), 'Clear screen and undo buffers'))</dl>
+<dl><dt><strong>cmdHelpMisc</strong> = (('help', ('h',), 'Show help about commands'), ('quit', ('q', 'exit', '^D'), 'Quit pwman'), ('cls', (), 'Clear screen'))</dl>
 
 <dl><dt><strong>cmdHelpShow</strong> = (('list', ('ls', 'cat'), 'List/print entry contents'), ('find', ('f',), 'Search the database for patterns'), ('totp', ('t',), 'Generate TOTP token'), ('diff', (), 'Show the database differences'))</dl>
 
 <hr>
 Methods inherited from <a href="cmd.html#Cmd">cmd.Cmd</a>:<br>
 <dl><dt><a name="__classcell__-cmdloop"><strong>cmdloop</strong></a>(self, intro=None)</dt><dd><span class="code">Repeatedly&nbsp;issue&nbsp;a&nbsp;prompt,&nbsp;accept&nbsp;input,&nbsp;parse&nbsp;an&nbsp;initial&nbsp;prefix<br>
 off&nbsp;the&nbsp;received&nbsp;input,&nbsp;and&nbsp;dispatch&nbsp;to&nbsp;action&nbsp;methods,&nbsp;passing&nbsp;them<br>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
   index
-ui /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/ui.py
+ui /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/ui.py
 # Simple password manager
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Modules
          functools re       sys
    � os        readline time
@@ -12,35 +12,42 @@
 Classes
            builtins.Exception(builtins.BaseException)
                  PWManTimeout
            cmd.Cmd(builtins.object)
                  __classcell__
           
          PWMan = class __classcell__(cmd.Cmd)
-             PWMan(filename, passphrase, commitClearsUndo=False, timeout=None)
+             PWMan(filename, passphrase, timeout=None)
               
 
               
                  Method resolution order:
                      __classcell__
                      cmd.Cmd
                      builtins.object
-               =====================================================================================================
+               ==========================================================================================
                Methods defined here:
-                 __init__(self, filename, passphrase, commitClearsUndo=False, timeout=None)
+                 __init__(self, filename, passphrase, timeout=None)
                      Instantiate a line-oriented interpreter framework.
                       
                      The optional argument 'completekey' is the readline name of a
                      completion key; it defaults to the Tab key. If completekey is
                      not None and the readline module is available, command completion
                      is done automatically. The optional arguments stdin and stdout
                      specify alternate input and output file objects; if not specified,
                      sys.stdin and sys.stdout are used.
                  complete_add = __complete_category_title(self, text, line, begidx, endidx)
+                 complete_c = complete_commit(self, text, line, begidx, endidx)
                  complete_cat = __complete_category_title_item(self, text, line, begidx, endidx)
+                 complete_close(self, text, line, begidx, endidx)
+                 complete_commit(self, text, line, begidx, endidx)
+                 complete_copy = complete_move(self, text, line, begidx, endidx)
+                 complete_cp = complete_move(self, text, line, begidx, endidx)
+                 complete_database(self, text, line, begidx, endidx)
+                 complete_db = complete_database(self, text, line, begidx, endidx)
                  complete_dbdump(self, text, line, begidx, endidx)
                  complete_dbimport(self, text, line, begidx, endidx)
                  complete_del = __complete_category_title(self, text, line, begidx, endidx)
                  complete_diff(self, text, line, begidx, endidx)
                  complete_ea = complete_edit_attr(self, text, line, begidx, endidx)
                  complete_eb = complete_edit_bulk(self, text, line, begidx, endidx)
                  complete_edit_attr(self, text, line, begidx, endidx)
@@ -60,38 +67,101 @@
                  complete_n = __complete_category_title(self, text, line, begidx, endidx)
                  complete_new = __complete_category_title(self, text, line, begidx, endidx)
                  complete_remove = __complete_category_title(self, text, line, begidx, endidx)
                  complete_rename = complete_move(self, text, line, begidx, endidx)
                  complete_rm = __complete_category_title(self, text, line, begidx, endidx)
                  complete_t = __complete_category_title(self, text, line, begidx, endidx)
                  complete_totp = __complete_category_title(self, text, line, begidx, endidx)
+                 complete_w = complete_commit(self, text, line, begidx, endidx)
                  default(self, line)
                      Called on an input line when the command prefix is not recognized.
                       
                      If this method is not overridden, it prints an error message and
                      returns.
                  do_EOF = do_quit(self, params)
                  do_add = do_new(self, params)
                  do_c = do_commit(self, params)
                  do_cat = do_list(self, params)
+                 do_close(self, params)
+                     --- Close a database ---
+                     Command: close [!] [NAME]
+                      
+                     If NAME is not given, then this closes the currently selected database.
+                     If NAME is given, then this closes the named database.
+                      
+                     If ! is specified, then the uncommitted changes will be dropped.
+                      
+                     If the currently used database is closed, the selected database
+                     will be switched to 'main'.
+                      
+                     The 'main' database can only be closed last,
+                     which in turn closes the application.
+                      
+                     Aliases: None
                  do_cls(self, params)
-                     --- Clear console screen and undo/redo buffer ---
+                     --- Clear console screen ---
                      Command: cls
                       
-                     Clear the console screen and all undo/redo buffers.
+                     Clear the console screen.
                      Note that this does not clear a possibly existing
                      'screen' session buffer or other advanced console buffers.
                       
                      Aliases: None
                  do_commit(self, params)
-                     --- Write changes to the database file ---
-                      
+                     --- Write changes to the database file(s) ---
                      Command: commit
                       
+                     Options:
+                       -a   Commit all open databases.
+                      
                      Aliases: c w
+                 do_copy(self, params)
+                     --- Copy an entry or a category ---
+                      
+                     Copy an existing entry:
+                     Command: copy CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+                     (NEW_TITLE defaults to TITLE)
+                      
+                     Copy all entries from a category into another category:
+                     Command: copy FROM_CATEGORY TO_CATEGORY
+                      
+                     Copy an entry from one database to another:
+                     Command: copy -s main -d other CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+                     (NEW_TITLE defaults to TITLE)
+                      
+                     Copy all entries from a category from one database into another database:
+                     Command: copy -s main -d other FROM_CATEGORY [TO_CATEGORY]
+                     (TO_CATEGORY defaults to FROM_CATEGORY)
+                      
+                     Options:
+                       -s SOURCE_DATABASE_NAME
+                       -d DESTINATION_DATABASE_NAME
+                       Databases default to the currently selected database.
+                       The named databases must be open. See 'database' command.
+                      
+                     Aliases: cp
+                 do_cp = do_copy(self, params)
+                 do_database(self, params)
+                     --- Open a database or switch to an already opened database ---
+                     Command: database [-f FILEPATH] [NAME]
+                      
+                     If neither FILEPATH nor NAME are given, then
+                     a list of all currently opened databases will be printed.
+                     The currently selected database will be marked with [@].
+                     All databases with uncommitted changes will be marked with [*].
+                      
+                     If only NAME is given, then the selected database will
+                     be switched to the named one. NAME must already be open.
+                      
+                     A new database can be opened with -f FILEPATH.
+                     NAME is optional in this case.
+                     The selected database will be switched to the newly opened one.
+                      
+                     Aliases: db
+                 do_db = do_database(self, params)
                  do_dbdump(self, params)
                      --- Dump the pwman SQL database ---
                      Command: dbdump [OPTS] [FILEPATH]
                       
                      If FILEPATH is given, the database is dumped
                      unencrypted to the file.
                      If FILEPATH is omitted, the database is dumped
@@ -166,17 +236,17 @@
                       
                      Aliases: ep
                  do_edit_totp(self, params)
                      --- Edit TOTP key and parameters ---
                      Command: edit_totp category title [KEY] [DIGITS] [HASH]
                       
                      Set Time-Based One-Time Password Algorithm key and parameters.
-                     If KEY is not provided, the TOTP parameters for this entry are deleted.
+                  If KEY is not provided, the TOTP parameters for this entry are deleted.
                      DIGITS default to 6, if not provided.
-                     HASH defaults to SHA1, if not provided.
+                    HASH defaults to SHA1, if not provided.
                       
                      Aliases: et
                  do_edit_user(self, params)
                      --- Edit the 'user' field of an existing entry ---
                      Command: edit_user category title NEWDATA...
                       
                      Change the 'user' field of an existing database entry.
@@ -190,66 +260,82 @@
                  do_eu = do_edit_user(self, params)
                  do_exit = do_quit(self, params)
                  do_f = do_find(self, params)
                  do_find(self, params)
                      --- Search the database ---
                      Command: find [OPTS] [IN_CATEGORY] PATTERN
                       
-                     Searches the database for patterns. If 'IN_CATEGORY' is given, only search
+   �             Searches the database for patterns. If 'IN_CATEGORY' is given, only search
                      in the specified category.
                      PATTERN may either use SQL LIKE wildcards (without -r)
                      or Python Regular Expression special characters (with -r).
                       
                      OPTS may be one or multiple of:
                        -c   Match 'category'       (only if no IN_CATEGORY parameter)
                        -t   Match 'title'          (*)
                        -u   Match 'user'           (*)
                        -p   Match 'password'       (*)
-                    -b   Match 'bulk'           (*)
+                       -b   Match 'bulk'           (*)
                        -a   Match 'attribute data' (*)
-                      -A   Match 'attribute name'
+                       -A   Match 'attribute name'
                        -r   Use Python Regular Expression matching
                       
                      (*) = These OPTS are enabled by default, if and only if
                            none of them are specified by the user.
                       
                      Aliases: f
                  do_h = do_help(self, params)
                  do_help(self, params)
                      --- Shows help text about a command ---
+                     Command: help [COMMAND]
                       
-                     Command: help
+                     If COMMAND is not given: Show a command summary.
+                     If COMMAND is given: Show detailed help about that command.
                       
                      Aliases: h
                  do_list(self, params)
                      --- Print a listing ---
                      Command: list [category] [title] [item]
                       
                      If a category is given as parameter, list the 
                      contents of the category. If category and entry
                      are given, list the contents of the entry.
                      If item is given, then only list one specific content item.
                      Item may be one of: user, password, bulk, totpkey or any attribute name.
-   �              
+                      
                      Aliases: ls cat
                  do_ls = do_list(self, params)
                  do_masterp(self, params)
                      --- Change the master passphrase ---
-                      
                      Command: masterp
                       
                      Aliases: None
                  do_move(self, params)
                      --- Move/rename an existing entry or a category ---
                       
                      Move/rename an existing entry:
-                     Command: move category title newCategory [newTitle]
+                     Command: move CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+                     (NEW_TITLE defaults to TITLE)
+                      
+                     Move all entries from one category into another category.
+                     Command: move FROM_CATEGORY TO_CATEGORY
                       
-                     Rename an existing category:
-                     Command: move category newCategory
+                     Move an entry from one database to another:
+                     Command: move -s main -d other CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+                     (NEW_TITLE defaults to TITLE)
+                      
+                     Move all entries from a category from one database into another database:
+                     Command: move -s main -d other FROM_CATEGORY [TO_CATEGORY]
+                     (TO_CATEGORY defaults to FROM_CATEGORY)
+                      
+                     Options:
+                       -s SOURCE_DATABASE_NAME
+                       -d DESTINATION_DATABASE_NAME
+                       Databases default to the currently selected database.
+                       The named databases must be open. See 'database' command.
                       
                      Aliases: mv rename
                  do_mv = do_move(self, params)
                  do_n = do_new(self, params)
                  do_new(self, params)
                      --- Create a new entry ---
                      Command: new [category] [title] [user] [password]
@@ -262,22 +348,14 @@
                  do_quit(self, params)
                      --- Exit pwman ---
                      Command: quit [!]
                       
                      Use the exclamation mark to force quit and discard changes.
                       
                      Aliases: q exit ^D
-                 do_redo(self, params)
-                     --- Redo the last undone command ---
-                     Command: redo
-                      
-                     Redoes the last undone command.
-                     Also see 'undo' help.
-                      
-                     Aliases: None
                  do_remove(self, params)
                      --- Remove an existing entry ---
                      Command: remove category [title]
                       
                      Remove an existing database entry.
                       
                      Aliases: rm del
@@ -287,57 +365,50 @@
                  do_totp(self, params)
                      --- Generate a TOTP token ---
                      Command: totp [CATEGORY TITLE] OR [TITLE]
                       
                      Generates a token using the Time-Based One-Time Password Algorithm.
                       
                      Aliases: t
-                 do_undo(self, params)
-                     --- Undo the last command ---
-                     Command: undo
-                      
-                     Rewinds the last command that changed the database.
-                      
-                     Aliases: None
                  do_w = do_commit(self, params)
                  emptyline(self)
                      Called when an empty line is entered in response to the prompt.
                       
                      If this method is not overridden, it repeats the last nonempty
                      command entered.
                  flunkDirty(self)
                  interactive(self)
                  postcmd(self, stop, line)
                      Hook method executed just after a command dispatch is finished.
                  precmd(self, line)
                      Hook method executed just before the command line is
                      interpreted, but after the input prompt is generated and issued.
                  runOneCommand(self, command)
-               =====================================================================================================
+               ==========================================================================================
                Data and other attributes defined here:
                  CommandError = <class 'ui.PWMan.CommandError'>
-                 Opts = <class 'ui.PWMan.Opts'>
-                     Opts(_Opts__opts: list = <factory>, _Opts__params: list = <factory>, _Opts__atCmdIndex:
-                      dict = <factory>)
                  Quit = <class 'ui.PWMan.Quit'>
-                 cmdHelpDatabase = (('commit', ('c', 'w'), 'Commit/write database file'), ('masterp', (), 'Change
-                 the master passphrase'), ('dbdump', (), 'Dump the database'), ('dbimport', (), 'Import a database
-                 dump file'), ('drop', (), 'Drop all uncommitted changes'))
-                 cmdHelpEdit = (('new', ('n', 'add'), 'Create new entry'), ('edit_user', ('eu',), "Edit the 'user'
-                 field of an entry"), ('edit_pw', ('ep',), "Edit the 'password' field of an entry"), ('edit_bulk',
-                 ('eb',), "Edit the 'bulk' field of an entry"), ('edit_totp', ('et',), 'Edit the TOTP key and
-                 parameters'), ('edit_attr', ('ea',), 'Edit an entry attribute'), ('move', ('mv', 'rename'), 'Move/
-                 rename an existing entry'), ('remove', ('rm', 'del'), 'Remove an existing entry'), ('undo', (),
-                 'Undo the last command'), ('redo', (), 'Redo the last undone command'))
-                 cmdHelpMisc = (('help', ('h',), 'Show help about commands'), ('quit', ('q', 'exit', '^D'), 'Quit
-                 pwman'), ('cls', (), 'Clear screen and undo buffers'))
-                 cmdHelpShow = (('list', ('ls', 'cat'), 'List/print entry contents'), ('find', ('f',), 'Search the
-                 database for patterns'), ('totp', ('t',), 'Generate TOTP token'), ('diff', (), 'Show the database
-                 differences'))
-               =====================================================================================================
+                 cmdHelpDatabase = (('database', ('db',), 'Open or select another database'), ('commit',
+                 ('c', 'w'), 'Commit/write selected db to disk'), ('drop', (), 'Drop uncommitted changes
+                 in selected db'), ('close', (), 'Close a database'), ('dbdump', (), 'Dump the selected
+                 database'), ('dbimport', (), 'Import a database dump file'), ('masterp', (), 'Change the
+                 master passphrase'))
+                 cmdHelpEdit = (('new', ('n', 'add'), 'Create new entry'), ('edit_user', ('eu',), "Edit
+                 the 'user' field of an entry"), ('edit_pw', ('ep',), "Edit the 'password' field of an
+                 entry"), ('edit_bulk', ('eb',), "Edit the 'bulk' field of an entry"), ('edit_totp',
+                 ('et',), 'Edit the TOTP key and parameters'), ('edit_attr', ('ea',), 'Edit an entry
+                 attribute'), ('move', ('mv', 'rename'), 'Move/rename an existing entry'), ('copy',
+                 ('cp',), 'Copy an existing entry or category'), ('remove', ('rm', 'del'), 'Remove an
+                 existing entry'))
+                 cmdHelpMisc = (('help', ('h',), 'Show help about commands'), ('quit', ('q', 'exit',
+                 '^D'), 'Quit pwman'), ('cls', (), 'Clear screen'))
+                 cmdHelpShow = (('list', ('ls', 'cat'), 'List/print entry contents'), ('find', ('f',),
+                 'Search the database for patterns'), ('totp', ('t',), 'Generate TOTP token'), ('diff',
+                 (), 'Show the database differences'))
+               ==========================================================================================
                Methods inherited from cmd.Cmd:
                  cmdloop(self, intro=None)
                      Repeatedly issue a prompt, accept input, parse an initial prefix
                      off the received input, and dispatch to action methods, passing them
                      the remainder of the line as argument.
                  columnize(self, list, displaywidth=80)
                      Display a list of strings as a compact set of columns.
@@ -371,21 +442,21 @@
                      'command' and 'args' may be None if the line couldn't be parsed.
                  postloop(self)
                      Hook method executed once when the cmdloop() method is about to
                      return.
                  preloop(self)
                      Hook method executed once when the cmdloop() method is called.
                  print_topics(self, header, cmds, cmdlen, maxcol)
-               =====================================================================================================
+               ==========================================================================================
                Data descriptors inherited from cmd.Cmd:
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
-               =====================================================================================================
+               ==========================================================================================
                Data and other attributes inherited from cmd.Cmd:
                  doc_header = 'Documented commands (type help <topic>):'
                  doc_leader = ''
                  identchars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_'
                  intro = None
                  lastcmd = ''
                  misc_header = 'Miscellaneous help topics:'
```

### Comparing `pwman-python-2.7/doc/api/libpwman/undo.html` & `pwman-python-2.8/doc/api/libpwman/util.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,45 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
-<title>Python: module undo</title>
+<title>Python: module util</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
-<td class="title">&nbsp;<br><strong class="title">undo</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/undo.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/undo.py</a></td></tr></table>
+<td class="title">&nbsp;<br><strong class="title">util</strong></td>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/util.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/util.py</a></td></tr></table>
     <p><span class="code">#&nbsp;Simple&nbsp;password&nbsp;manager<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
-<tr class="decor index-decor heading-text">
-<td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Classes</strong></td></tr>
+<tr class="decor pkg-content-decor heading-text">
+<td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Modules</strong></td></tr>
     
-<tr><td class="decor index-decor"><span class="code">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></td><td>&nbsp;</td>
-<td class="singlecolumn"><dl>
-<dt class="heading-text"><a href="builtins.html#object">builtins.object</a>
-</dt><dd>
-<dl>
-<dt class="heading-text"><a href="undo.html#UndoStack">UndoStack</a>
-</dt></dl>
-</dd>
-</dl>
- <p>
+<tr><td class="decor pkg-content-decor"><span class="code">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></td><td>&nbsp;</td>
+<td class="singlecolumn"><table><tr><td class="multicolumn"><a href="curses.html">curses</a><br>
+</td><td class="multicolumn"><a href="getpass.html">getpass</a><br>
+</td><td class="multicolumn"><a href="os.html">os</a><br>
+</td><td class="multicolumn"><a href="sys.html">sys</a><br>
+</td></tr></table></td></tr></table><p>
 <table class="section">
-<tr class="decor title-decor heading-text">
-<td class="section-title" colspan=3>&nbsp;<br><a name="UndoStack">class <strong>UndoStack</strong></a>(<a href="builtins.html#object">builtins.object</a>)</td></tr>
+<tr class="decor functions-decor heading-text">
+<td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Functions</strong></td></tr>
     
-<tr><td class="decor title-decor" rowspan=2><span class="code">&nbsp;&nbsp;&nbsp;</span></td>
-<td class="decor title-decor" colspan=2><span class="code"><a href="#UndoStack">UndoStack</a>(limit=32768)<br>
-&nbsp;<br>
-<br>&nbsp;</span></td></tr>
-<tr><td>&nbsp;</td>
-<td class="singlecolumn">Methods defined here:<br>
-<dl><dt><a name="UndoStack-__init__"><strong>__init__</strong></a>(self, limit=32768)</dt><dd><span class="code">Initialize&nbsp;self.&nbsp;&nbsp;See&nbsp;help(type(self))&nbsp;for&nbsp;accurate&nbsp;signature.</span></dd></dl>
-
-<dl><dt><a name="UndoStack-clear"><strong>clear</strong></a>(self)</dt></dl>
-
-<dl><dt><a name="UndoStack-do"><strong>do</strong></a>(self, doCommands, undoCommands)</dt></dl>
-
-<dl><dt><a name="UndoStack-freeze"><strong>freeze</strong></a>(self)</dt></dl>
-
-<dl><dt><a name="UndoStack-redo"><strong>redo</strong></a>(self)</dt></dl>
-
-<dl><dt><a name="UndoStack-thaw"><strong>thaw</strong></a>(self)</dt></dl>
-
-<dl><dt><a name="UndoStack-undo"><strong>undo</strong></a>(self)</dt></dl>
-
-<hr>
-Data descriptors defined here:<br>
-<dl><dt><strong>__dict__</strong></dt>
-<dd><span class="code">dictionary&nbsp;for&nbsp;instance&nbsp;variables&nbsp;(if&nbsp;defined)</span></dd>
-</dl>
-<dl><dt><strong>__weakref__</strong></dt>
-<dd><span class="code">list&nbsp;of&nbsp;weak&nbsp;references&nbsp;to&nbsp;the&nbsp;object&nbsp;(if&nbsp;defined)</span></dd>
-</dl>
-</td></tr></table></td></tr></table><p>
+<tr><td class="decor functions-decor"><span class="code">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></td><td>&nbsp;</td>
+<td class="singlecolumn"><dl><dt><a name="-clearScreen"><strong>clearScreen</strong></a>()</dt></dl>
+ <dl><dt><a name="-readPassphrase"><strong>readPassphrase</strong></a>(prompt, verify=False)</dt></dl>
+ <dl><dt><a name="-stdout"><strong>stdout</strong></a>(text, flush=True)</dt></dl>
+ <dl><dt><a name="-str2bool"><strong>str2bool</strong></a>(string, default=False)</dt></dl>
+ <dl><dt><a name="-uniq"><strong>uniq</strong></a>(l, sort=True)</dt></dl>
+</td></tr></table><p>
 <table class="section">
 <tr class="decor data-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Data</strong></td></tr>
     
 <tr><td class="decor data-decor"><span class="code">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></td><td>&nbsp;</td>
-<td class="singlecolumn"><strong>__all__</strong> = ['UndoStack']</td></tr></table>
+<td class="singlecolumn"><strong>__all__</strong> = ['str2bool', 'osIsWindows', 'osIsPosix', 'uniq', 'stdout', 'clearScreen', 'readPassphrase']<br>
+<strong>osIsPosix</strong> = True<br>
+<strong>osIsWindows</strong> = False</td></tr></table>
 </body></html>
```

#### html2text {}

```diff
@@ -1,33 +1,21 @@
     index
-undo /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/undo.py
+util /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/util.py
 # Simple password manager
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
-Classes
-           builtins.object
-                 UndoStack
-          
-         class UndoStack(builtins.object)
-             UndoStack(limit=32768)
-              
-
-              
-               Methods defined here:
-                 __init__(self, limit=32768)
-                     Initialize self.  See help(type(self)) for accurate signature.
-   �         clear(self)
-                 do(self, doCommands, undoCommands)
-              freeze(self)
-                 redo(self)
-                thaw(self)
-                 undo(self)
-               ===========================================================================
-               Data descriptors defined here:
-                 __dict__
-                     dictionary for instance variables (if defined)
-                 __weakref__
-                     list of weak references to the object (if defined)
+Modules
+   � curses getpass os sys
+ 
+Functions
+           clearScreen()
+           readPassphrase(prompt, verify=False)
+   �   stdout(text, flush=True)
+           str2bool(string, default=False)
+           uniq(l, sort=True)
  
 Data
-   � __all__ = ['UndoStack']
+         __all__ = ['str2bool', 'osIsWindows', 'osIsPosix', 'uniq', 'stdout',
+   � 'clearScreen', 'readPassphrase']
+         osIsPosix = True
+         osIsWindows = False
```

### Comparing `pwman-python-2.7/doc/api/libpwman/version.html` & `pwman-python-2.8/doc/api/libpwman/version.html`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 <meta charset="utf-8">
 <title>Python: module version</title>
 </head><body>
 
 <table class="heading">
 <tr class="heading-text decor">
 <td class="title">&nbsp;<br><strong class="title">version</strong></td>
-<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/version.py">/tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/version.py</a></td></tr></table>
+<td class="extra"><a href=".">index</a><br><a href="file:/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/version.py">/tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/version.py</a></td></tr></table>
     <p><span class="code">#&nbsp;Simple&nbsp;password&nbsp;manager<br>
 #&nbsp;Copyright&nbsp;(c)&nbsp;2011-2023&nbsp;Michael&nbsp;Büsch&nbsp;&lt;m@bues.ch&gt;<br>
 #&nbsp;Licensed&nbsp;under&nbsp;the&nbsp;GNU/GPL&nbsp;version&nbsp;2&nbsp;or&nbsp;later.</span></p>
 <p>
 <table class="section">
 <tr class="decor data-decor heading-text">
 <td class="section-title" colspan=3>&nbsp;<br><strong class="bigsection">Data</strong></td></tr>
     
 <tr><td class="decor data-decor"><span class="code">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></td><td>&nbsp;</td>
 <td class="singlecolumn"><strong>VERSION_EXTRA</strong> = ''<br>
 <strong>VERSION_MAJOR</strong> = 2<br>
-<strong>VERSION_MINOR</strong> = 7<br>
-<strong>VERSION_STRING</strong> = '2.7'<br>
+<strong>VERSION_MINOR</strong> = 8<br>
+<strong>VERSION_STRING</strong> = '2.8'<br>
 <strong>__all__</strong> = ['VERSION_MAJOR', 'VERSION_MINOR', 'VERSION_EXTRA', 'VERSION_STRING']</td></tr></table>
 </body></html>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
        index
-version /tmp/makerelease-pwman-python.rYoC18LZ/pwman-python-2.7/libpwman/
+version /tmp/makerelease-pwman-python.NVQhFLFA/pwman-python-2.8/libpwman/
         version.py
 # Simple password manager
 # Copyright (c) 2011-2023 Michael BÃ¼sch <m@bues.ch>
 # Licensed under the GNU/GPL version 2 or later.
  
 Data
          VERSION_EXTRA = ''
          VERSION_MAJOR = 2
-   � VERSION_MINOR = 7
-         VERSION_STRING = '2.7'
+   � VERSION_MINOR = 8
+         VERSION_STRING = '2.8'
          __all__ = ['VERSION_MAJOR', 'VERSION_MINOR', 'VERSION_EXTRA',
          'VERSION_STRING']
```

### Comparing `pwman-python-2.7/doc/foreign-licenses/PYTHON-LICENSE.txt` & `pwman-python-2.8/doc/foreign-licenses/PYTHON-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/examplescript.py` & `pwman-python-2.8/examplescript.py`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/install_to_venv.sh` & `pwman-python-2.8/install_to_venv.sh`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/libpwman/__main__.py` & `pwman-python-2.8/libpwman/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,22 +108,21 @@
 		print("%s.run(database) raised an exception:\n\n%s" % (
 		      pyModName, traceback.format_exc()),
 		      file=sys.stderr)
 		return 1
 	db.flunkDirty()
 	return 0
 
-def run_ui(dbPath, commitClearsUndo, timeout, commands):
+def run_ui(dbPath, timeout, commands):
 	passphrase = getPassphrase(dbPath, verbose=not commands)
 	if passphrase is None:
 		return 1
 	try:
 		p = libpwman.PWMan(filename=dbPath,
 				   passphrase=passphrase,
-				   commitClearsUndo=commitClearsUndo,
 				   timeout=timeout)
 		if commands:
 			for command in commands:
 				p.runOneCommand(command)
 		else:
 			p.interactive()
 		p.flunkDirty()
@@ -157,16 +156,14 @@
 		       default="unified",
 		       choices=("unified", "context", "ndiff", "html"),
 		       help="Select the diff format for the -D|--diff argument.")
 	p.add_argument("database", nargs="?", metavar="DB_PATH",
 		       type=pathlib.Path, default=libpwman.database.getDefaultDatabase(),
 		       help="Use DB_PATH as database file. If not given, %s is used." % (
 			    libpwman.database.getDefaultDatabase()))
-	p.add_argument("-U", "--commit-clear-undo", action="store_true",
-		       help="The commit command clears undo queue.")
 	p.add_argument("--no-mlock", action="store_true",
 		       help="Do not lock memory and allow swapping to disk.")
 	if libpwman.util.osIsPosix:
 		p.add_argument("-t", "--timeout", type=int, default=600, metavar="SECONDS",
 			       help="Sets the session timeout in seconds. Default is 10 minutes.")
 	args = p.parse_args()
 
@@ -217,15 +214,14 @@
 		elif args.call_pymod:
 			assert not interactiveMode
 			exitcode = run_script(dbPath=args.database,
 					      pyModName=args.call_pymod)
 		else:
 			assert interactiveMode != bool(args.command)
 			exitcode = run_ui(dbPath=args.database,
-					  commitClearsUndo=args.commit_clear_undo,
 					  timeout=args.timeout if libpwman.util.osIsPosix else None,
 					  commands=args.command)
 	except libpwman.database.CSQLError as e:
 		print("SQL error: " + str(e), file=sys.stderr)
 		return 1
 	except libpwman.PWManError as e:
 		print("Error: " + str(e), file=sys.stderr)
```

### Comparing `pwman-python-2.7/libpwman/aes.py` & `pwman-python-2.8/libpwman/aes.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,16 @@
 				iv=iv)
 			decData = cipher.decrypt(data)
 			if legacyPadding:
 				unpadData = self.__unpadLegacy(decData)
 			else:
 				unpadData = self.__cryptodome.Util.Padding.unpad(
 					padded_data=decData,
-					block_size=self.BLOCK_SIZE)
+					block_size=self.BLOCK_SIZE,
+					style="pkcs7")
 			return unpadData
 
 		if self.__pyaes is not None:
 			mode = self.__pyaes.AESModeOfOperationCBC(key=key, iv=iv)
 			if legacyPadding:
 				padding = self.__pyaes.PADDING_NONE
 			else:
```

### Comparing `pwman-python-2.7/libpwman/cryptsql.py` & `pwman-python-2.8/libpwman/cryptsql.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 			self.__c.execute(code, params)
 			return self
 		except (sql.Error, sql.DatabaseError) as e:
 			raise CSQLError("Database error: " + str(e))
 
 	def sqlExecScript(self, code):
 		"""Execute multiple SQL statements.
+		Warning: This implicitly commits pending transactions before executing.
 		"""
 		try:
 			self.__c.executescript(code)
 			return self
 		except (sql.Error, sql.DatabaseError) as e:
 			raise CSQLError("Database error: " + str(e))
 
@@ -142,15 +143,15 @@
 
 			# Get the file fields.
 			head = fc.getOne(b"HEAD", "Invalid file header object")
 			if head != CSQL_HEADER:
 				raise CSQLError("Invalid file header")
 			cipher = fc.getOne(b"CIPHER", "Invalid CYPHER object")
 			cipherMode = fc.getOne(b"CIPHER_MODE", "Invalid CYPHER_MODE object")
-			cipherIV = fc.getOne(b"CIPHER_IV")
+			cipherIV = fc.getOne(b"CIPHER_IV", "Invalid CIPHER_IV object")
 			keyLen = fc.getOne(b"KEY_LEN", "Invalid KEY_LEN object")
 			kdfMethod = fc.getOne(b"KDF_METHOD", "Invalid KDF_METHOD object")
 			kdfSalt = fc.getOne(b"KDF_SALT", "Invalid KDF_SALT object")
 			kdfIter = fc.getOne(b"KDF_ITER", "Invalid KDF_ITER object")
 			kdfHash = fc.getOne(b"KDF_HASH", "Invalid KDF_HASH object")
 			kdfMac = fc.getOne(b"KDF_MAC", "Invalid KDF_MAC object")
 			compress = fc.getOne(b"COMPRESS", default=b"NONE")
@@ -167,16 +168,14 @@
 				cipherBlockSize = AES.BLOCK_SIZE
 			else:
 				raise CSQLError("Unknown cipher/mode: %s/%s" % (
 					cipher.decode("UTF-8", "ignore"),
 					cipherMode.decode("UTF-8", "ignore")))
 
 			# Check the cipher IV.
-			if not cipherIV: # legacy
-				cipherIV = b'\x00' * cipherBlockSize
 			if len(cipherIV) != cipherBlockSize:
 				raise CSQLError("Invalid IV len: %d" % len(cipherIV))
 
 			# Check the cipher key length.
 			if keyLen == b"256":
 				keyLen = 256 // 8
 			else:
@@ -233,45 +232,44 @@
 					data=payload,
 					legacyPadding=(paddingMethod == b"PWMAN"))
 
 				# Decompress payload (legacy).
 				payload = compress.decompress(payload)
 
 				# Import the SQL database.
-				self.__db.cursor().executescript(payload.decode("UTF-8"))
+				self.importSqlScript(payload.decode("UTF-8"))
 
 				# Store the raw key.
 				self.__key = key
 
 			except (CSQLError, zlib.error, sql.Error, sql.DatabaseError, UnicodeError, ValueError) as e:
 				raise CSQLError("Failed to decrypt database. "
 						"Wrong passphrase?")
 		except FileObjError as e:
 			raise CSQLError("File error: %s" % str(e))
 
 	def isOpen(self):
 		"""Returns True, if a database file is opened.
 		"""
-		return bool(self.__db)
+		return self.__db is not None
 
 	def open(self, filename):
 		"""Open a database file and decrypt its contents into memory.
 		filename: The database file path.
 		"""
 		if self.isOpen():
 			raise CSQLError("A database is already open")
 		self.__db = sql.connect(":memory:")
 		self.__db.text_factory = str
 		self.setRegexpFlags()
 		self.sqlCreateFunction("regexp", 2, self._sqlRegexpMatch)
 		try:
 			self.__parseFile(filename)
 		except CSQLError as e:
-			self.__db = None
-			self.__filename = None
+			self.close()
 			raise e
 		self.__filename = filename
 
 	def close(self):
 		"""Close the currently opened database.
 		This does not commit. All uncommitted changes are lost.
 		"""
@@ -402,14 +400,15 @@
 	def sqlExec(self, code, params=[]):
 		"""Execute one SQL statement.
 		"""
 		return CryptSQLCursor(self.__db).sqlExec(code, params)
 
 	def sqlExecScript(self, code):
 		"""Execute multiple SQL statements.
+		Warning: This implicitly commits pending transactions before executing.
 		"""
 		return CryptSQLCursor(self.__db).sqlExecScript(code)
 
 	def sqlCreateFunction(self, name, nrParams, func):
 		"""Create an SQL function.
 		See sqlite3.Connection.create_function for more details.
 		"""
```

### Comparing `pwman-python-2.7/libpwman/database.py` & `pwman-python-2.8/libpwman/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,24 +201,29 @@
 			totp(id INTEGER PRIMARY KEY AUTOINCREMENT,
 			     entry INTEGER, key TEXT, digits INTEGER, hash TEXT);
 		""")
 
 	def __garbageCollect(self):
 		"""Remove rows from the SQL database that are not needed anymore.
 		"""
-		c = self.sqlExecScript("""
-			DELETE FROM bulk WHERE entry NOT IN (SELECT id FROM entries);
-			DELETE FROM entryattr WHERE entry NOT IN (SELECT id FROM entries);
-			DELETE FROM totp WHERE entry NOT IN (SELECT id FROM entries);
-		""")
+		# Do not use sqlExecScript here, as that would commit transactions.
+		c = self.sqlExec("DELETE FROM bulk WHERE entry NOT IN (SELECT id FROM entries);")
+		c = self.sqlExec("DELETE FROM entryattr WHERE entry NOT IN (SELECT id FROM entries);")
+		c = self.sqlExec("DELETE FROM totp WHERE entry NOT IN (SELECT id FROM entries);")
 
 	def setPassphrase(self, passphrase):
 		super().setPassphrase(passphrase)
 		self.__setDirty()
 
+	def categoryExists(self, category):
+		"""Returns True, if a category exists in the database.
+		category: The name string of the category.
+		"""
+		return category in self.getCategoryNames()
+
 	def getCategoryNames(self):
 		"""Get all category names in the database.
 		Returns a sorted list of strings.
 		"""
 		c = self.sqlExec("SELECT category FROM entries;")
 		categories = c.fetchAll()
 		if not categories:
@@ -234,30 +239,14 @@
 				 (category,))
 		titles = c.fetchAll()
 		if not titles:
 			return []
 		titles = sorted(t[0] for t in titles)
 		return titles
 
-	def renameCategory(self, category, toCategory):
-		"""Change the name of a category.
-		category: The old name string of the category.
-		toCategory: The new name string of the category.
-		"""
-		categories = self.getCategoryNames()
-		if category not in categories:
-			raise PWManError("Source category does not exist.")
-		if toCategory in categories:
-			raise PWManError("Target category does already exist.")
-		c = self.sqlExec("UPDATE entries SET category=? "
-				 "WHERE category=?;",
-				 (toCategory,
-				  category))
-		self.__setDirty()
-
 	def getEntry(self, category, title):
 		"""Get an entry from the database.
 		category: The name string of the category to get an entry from.
 		title: The title string of the entry to get.
 		Returns a PWManEntry() instance.
 		"""
 		c = self.sqlExec("SELECT id, category, title, user, pw FROM entries "
@@ -397,15 +386,15 @@
 			 for data in dataSet ]
 
 	def entryExists(self, category, title):
 		"""Returns True, if an entry exists in the database.
 		category: The name string of the category.
 		title: The title string of the entry.
 		"""
-		return bool(self.getEntry(category, title))
+		return self.getEntry(category, title) is not None
 
 	def addEntry(self, entry):
 		"""Create a new entry in the database.
 		entry: A PWManEntry() instance.
 		"""
 		if self.entryExists(entry.category, entry.title):
 			raise PWManError("Entry does already exist")
@@ -459,14 +448,27 @@
 				 "category=?, title=? "
 				 "WHERE id=?;",
 				 (entry.category,
 				  entry.title,
 				  oldEntry.entryId))
 		self.__setDirty()
 
+	def moveEntries(self, fromCategory, toCategory):
+		"""Move all entries from one category to another category.
+		fromCategory: The category to move all entries from.
+		toCategory: The (new) category to move all entries to.
+		"""
+		if not self.categoryExists(fromCategory):
+			raise PWManError("Source category does not exist.")
+		c = self.sqlExec("UPDATE entries SET category=? "
+				 "WHERE category=?;",
+				 (toCategory,
+				  fromCategory))
+		self.__setDirty()
+
 	def delEntry(self, entry):
 		"""Delete an existing entry from the database.
 		entry: The PWManEntry() instance to delete from the database.
 		"""
 		c = self.sqlExec("SELECT id FROM entries WHERE category=? AND title=?;",
 				 (entry.category,
 				  entry.title))
```

### Comparing `pwman-python-2.7/libpwman/dbdiff.py` & `pwman-python-2.8/libpwman/dbdiff.py`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/libpwman/fileobj.py` & `pwman-python-2.8/libpwman/fileobj.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,29 +81,27 @@
 				raise FileObjError("FileObj: Data length extension bit is set, "
 						   "but not supported by this pwman version.")
 			off += 4
 			data = raw[off : off + dataLen]
 			off += dataLen
 		except (IndexError, KeyError) as e:
 			raise FileObjError("Failed to parse file object")
-		return (cls(name, data),
-			off)
+		return (cls(name, data), off)
 
 class FileObjCollection:
 	def __init__(self, *objects):
 		self.objects = objects
 
 	def writeFile(self, filepath):
 		try:
 			with open(filepath, "wb") as f:
 				f.write(self.getRaw())
 				f.flush()
 		except IOError as e:
-			raise FileObjError("Failed to write file: %s" %
-					   e.strerror)
+			raise FileObjError("Failed to write file: %s" % e.strerror)
 
 	def getRaw(self):
 		raw = bytearray()
 		for obj in self.objects:
 			raw += obj.getRaw()
 		return raw
 
@@ -123,23 +121,22 @@
 	@classmethod
 	def parseRaw(cls, raw):
 		assert isinstance(raw, (bytes, bytearray)),\
 		       "FileObjCollection: Invalid 'raw' type."
 		offset = 0
 		objects = []
 		while offset < len(raw):
-			(obj, objLen) = FileObj.parseRaw(raw[offset:])
+			obj, objLen = FileObj.parseRaw(raw[offset:])
 			objects.append(obj)
 			offset += objLen
 		return cls(*objects)
 
 	@classmethod
 	def parseFile(cls, filepath):
 		try:
 			with open(filepath, "rb") as f:
 				rawData = f.read()
-		except (IOError) as e:
+		except IOError as e:
 			if e.errno != errno.ENOENT:
-				raise FileObjError("Failed to read file: %s" %\
-						   e.strerror)
+				raise FileObjError("Failed to read file: %s" % e.strerror)
 			return None
 		return cls.parseRaw(rawData)
```

### Comparing `pwman-python-2.7/libpwman/mlock.py` & `pwman-python-2.8/libpwman/mlock.py`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/libpwman/otp.py` & `pwman-python-2.8/libpwman/otp.py`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/libpwman/ui.py` & `pwman-python-2.8/libpwman/ui.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,95 +5,38 @@
 # Licensed under the GNU/GPL version 2 or later.
 """
 
 from libpwman.database import *
 from libpwman.dbdiff import *
 from libpwman.exception import *
 from libpwman.otp import *
-from libpwman.undo import *
+from libpwman.ui_escape import *
 from libpwman.util import *
 
 import functools
 import os
 import pathlib
 import re
 import readline
 import sys
 import time
 import traceback
-from copy import copy, deepcopy
 from cmd import Cmd
+from copy import copy, deepcopy
 from dataclasses import dataclass, field
+from typing import Optional, Tuple
 
 if osIsPosix:
 	import signal
 
 __all__ = [
 	"PWMan",
 	"PWManTimeout",
 ]
 
-class EscapeError(Exception):
-	pass
-
-def escapeCmd(s):
-	# Commandline escape
-	if s is None:
-		return "\\-"
-	if not s:
-		return "\\~"
-	subst = {
-		'\t'	: '\\t',
-		'\n'	: '\\n',
-		'\\'	: '\\\\',
-		' '	: '\\ ',
-	}
-	ret = []
-	for c in s:
-		try:
-			c = subst[c]
-		except (KeyError) as e:
-			if c.isspace():
-				c = '\\x%02X' % ord(c)
-		ret.append(c)
-	return "".join(ret)
-
-def unescapeCmd(s):
-	# Commandline unescape
-	if s == '\\-':
-		return None
-	if s == '\\~':
-		return ""
-	slashSubst = {
-		't'	: '\t',
-		'n'	: '\n',
-		'\\'	: '\\',
-	}
-	ret = []
-	i = 0
-	while i < len(s):
-		if s[i] == '\\':
-			try:
-				if s[i + 1] == 'x':
-					ret.append(chr(int(s[i + 2 : i + 4], 16)))
-					i += 3
-				elif s[i + 1] == ' ':
-					ret.append(' ')
-					i += 1
-				else:
-					ret.append(slashSubst[s[i + 1]])
-					i += 1
-			except (IndexError, ValueError, KeyError):
-				raise EscapeError("Invalid backslash escape sequence "
-					"at character %d" % i)
-		else:
-			ret.append(s[i])
-		i += 1
-	return "".join(ret)
-
 class PWManTimeout(Exception):
 	def __init__(self, seconds):
 		if seconds is not None and seconds >= 0:
 			self.seconds = seconds
 			if osIsPosix:
 				signal.signal(signal.SIGALRM, self.__timeout)
 				self.poke()
@@ -105,23 +48,239 @@
 	def poke(self):
 		if self.seconds is not None:
 			signal.alarm(self.seconds)
 
 	def __timeout(self, signum, frame):
 		raise self
 
+@dataclass
+class PWManOpts:
+	"""UI command option parser.
+	"""
+	__opts : list = field(default_factory=list)
+	__params : list = field(default_factory=list)
+	__atCmdIndex : dict = field(default_factory=dict)
+	__error : Optional[Tuple[str, str]] = None
+
+	@classmethod
+	def parse(cls,
+		  line,
+		  optTemplates,
+		  ignoreFirst=False,
+		  unescape=True,
+		  softFail=False):
+		"""Parses the command options in 'line' and returns an Opts instance.
+		optTemplates is a tuple of the possible options.
+		"""
+		optTemplatesRaw = cls.rawOptTemplates(optTemplates)
+		opts = cls()
+		i = 0
+		while True:
+			p = cls.parseParam(line, i,
+					   ignoreFirst=ignoreFirst,
+					   unescape=unescape)
+			if not p:
+				break
+			if opts.nrParams:
+				opts._appendParam(i, p)
+			else:
+				try:
+					optIdx = optTemplatesRaw.index(p)
+				except ValueError:
+					opts._appendParam(i, p)
+					i += 1
+					continue
+				if optTemplates[optIdx].endswith(":"):
+					i += 1
+					arg = cls.parseParam(line, i,
+							     ignoreFirst=ignoreFirst,
+							     unescape=unescape)
+					if not arg and softFail:
+						opts._setError(p, "no_arg")
+						break
+					if not arg:
+						PWMan._err(None, "Option '%s' "
+							   "requires an argument." % p)
+					opts._appendOpt(i, p, arg)
+				else:
+					opts._appendOpt(i, p)
+			i += 1
+		return opts
+
+	def _appendOpt(self, cmdIndex, optName, optValue=None):
+		self.__opts.append( (optName, optValue) )
+		self.__atCmdIndex[cmdIndex] = (optName, optValue)
+
+	def _appendParam(self, cmdIndex, param):
+		self.__params.append(param)
+		self.__atCmdIndex[cmdIndex] = (None, param)
+
+	def _setError(self, optName, error):
+		self.__error = (optName, error)
+
+	def __contains__(self, optName):
+		"""Check if we have a specific "-X" style option.
+		"""
+		return optName in (o[0] for o in self.__opts)
+
+	@property
+	def error(self):
+		return self.__error
+
+	@property
+	def hasOpts(self):
+		"""Do we have -X style options?
+		"""
+		return bool(self.__opts)
+
+	def getOpt(self, optName, default=None):
+		"""Get an option value by "-X" style name.
+		"""
+		if optName in self:
+			return [ o[1] for o in self.__opts if o[0] == optName ][-1]
+		return default
+
+	@property
+	def nrParams(self):
+		"""The number of trailing parameters.
+		"""
+		return len(self.__params)
+
+	def getParam(self, index, default=None):
+		"""Get a trailing parameter at index.
+		"""
+		if index < 0 or index >= self.nrParams:
+			return default
+		return self.__params[index]
+
+	def getComplParamIdx(self, complText):
+		"""Get the parameter index in an active completion.
+		complText: The partial parameter text in the completion.
+		"""
+		if complText:
+			paramIdx = self.nrParams - 1
+		else:
+			paramIdx = self.nrParams
+		if paramIdx < 0:
+			return None
+		return paramIdx
+
+	def atCmdIndex(self, cmdIndex):
+		"""Get an item (option or parameter) at command line index cmdIndex.
+		Returns (optName, optValue) if it is an option.
+		Returns (None, parameter) if it is a parameter.
+		Returns (None, None) if it does not exist.
+		"""
+		return self.__atCmdIndex.get(cmdIndex, (None, None))
+
+	@classmethod
+	def skipParams(cls, line, count,
+		       lineIncludesCommand=False, unescape=True):
+		"""Return a parameter string with the first 'count'
+		parameters skipped.
+		"""
+		sline = cls.patchSpaceEscapes(line)
+		if lineIncludesCommand:
+			count += 1
+		i = 0
+		while i < len(sline) and count > 0:
+			while i < len(sline) and not sline[i].isspace():
+				i += 1
+			while i < len(sline) and sline[i].isspace():
+				i += 1
+			count -= 1
+		if i >= len(sline):
+			return ""
+		s = line[i:]
+		if unescape:
+			s = unescapeCmd(s)
+		return s
+
+	@classmethod
+	def calcParamIndex(cls, line, endidx):
+		"""Returns the parameter index into the commandline
+		given the character end-index. This honors space-escape.
+		"""
+		line = cls.patchSpaceEscapes(line)
+		startidx = endidx - 1
+		while startidx > 0 and not line[startidx].isspace():
+			startidx -= 1
+		return len([l for l in line[:startidx].split() if l]) - 1
+
+	@classmethod
+	def patchSpaceEscapes(cls, line):
+		# Patch a commandline for simple whitespace based splitting.
+		# We just replace the space escape sequence by a random
+		# non-whitespace string. The line remains the same size.
+		return line.replace('\\ ', '_S')
+
+	@classmethod
+	def parseParam(cls, line, paramIndex,
+		       ignoreFirst=False, unescape=True):
+		"""Returns the full parameter from the commandline.
+		"""
+		sline = cls.patchSpaceEscapes(line)
+		if ignoreFirst:
+			paramIndex += 1
+		inParam = False
+		idx = 0
+		for startIndex, c in enumerate(sline):
+			if c.isspace():
+				if inParam:
+					idx += 1
+				inParam = False
+			else:
+				inParam = True
+				if idx == paramIndex:
+					break
+		else:
+			return ""
+		endIndex = startIndex
+		while endIndex < len(sline) and not sline[endIndex].isspace():
+			endIndex += 1
+		p = line[startIndex : endIndex]
+		if unescape:
+			p = unescapeCmd(p)
+		return p
+
+	@classmethod
+	def parseComplParam(cls, line, paramIndex, unescape=True):
+		return cls.parseParam(line, paramIndex,
+				      ignoreFirst=True, unescape=unescape)
+
+	@classmethod
+	def parseParams(cls, line, paramIndex, count,
+			ignoreFirst=False, unescape=True):
+		"""Returns a generator of the specified parameters from the commandline.
+		paramIndex: start index.
+		count: Number of paramerts to fetch.
+		"""
+		return ( cls.parseParam(line, i, ignoreFirst, unescape)
+			 for i in range(paramIndex, paramIndex + count) )
+
+	@classmethod
+	def parseComplParams(cls, line, paramIndex, count, unescape=True):
+		return cls.parseParams(line, paramIndex, count,
+				       ignoreFirst=True, unescape=unescape)
+
+	@classmethod
+	def rawOptTemplates(cls, optTemplates):
+		"""Remove the modifiers from opt templates.
+		"""
+		return [ ot.replace(":", "") for ot in optTemplates ]
+
 # PWMan completion decorator that does common things and workarounds.
 def completion(func):
 	@functools.wraps(func)
 	def wrapper(self, text, line, begidx, endidx):
 		try:
 			self._timeout.poke()
 
 			# Find the real begidx that takes space escapes into account.
-			sline = self._patchSpaceEscapes(line)
+			sline = PWManOpts.patchSpaceEscapes(line)
 			realBegidx = endidx
 			while realBegidx > 0:
 				if sline[realBegidx - 1] == " ":
 					break
 				realBegidx -= 1
 
 			if begidx == realBegidx:
@@ -133,16 +292,16 @@
 				# It must be removed from the results.
 				textPrefix = line[realBegidx : begidx]
 				begidx = realBegidx
 
 			# Fixup text.
 			# By fetching the parameter again it is ensured that
 			# it is properly unescaped.
-			paramIdx = self._calcParamIndex(line, endidx)
-			text = self._getComplParam(line, paramIdx)
+			paramIdx = PWManOpts.calcParamIndex(line, endidx)
+			text = PWManOpts.parseComplParam(line, paramIdx)
 
 			# Call the PWMan completion handler.
 			completions = func(self, text, line, begidx, endidx)
 
 			# If we fixed begidx in the workaround above,
 			# we need to remove the additional prefix from the results,
 			# because Cmd/readline won't expect it.
@@ -166,139 +325,166 @@
 			# Fixup command docstrings.
 			if (name.startswith("do_") and
 			    not getattr(attr, "_pwman_fixed", False) and
 			    attr.__doc__):
 				# Remove leading double-tabs.
 				attr.__doc__, n = re.subn("^\t\t", "\t", attr.__doc__,
 							  0, re.MULTILINE)
+				# Remove trailing white space.
+				attr.__doc__ = attr.__doc__.rstrip()
 				# Tabs to spaces.
 				attr.__doc__, n = re.subn("\t", " " * 8, attr.__doc__,
 							  0, re.MULTILINE)
 				attr._pwman_fixed = True
 		return super().__new__(cls, name, bases, dct)
 
 class PWMan(Cmd, metaclass=PWManMeta):
 	class CommandError(Exception): pass
 	class Quit(Exception): pass
 
-	def __init__(self, filename, passphrase,
-		     commitClearsUndo=False, timeout=None):
+	def __init__(self, filename, passphrase, timeout=None):
 		super().__init__()
 
 		self.__isInteractive = False
 
 		if sys.flags.optimize >= 2:
 			# We need docstrings.
 			raise PWManError("pwman does not support "
 					 "Python optimization level 2 (-OO). "
 					 "Please call with python3 -O or less.")
 
 		# argument delimiter shall be space.
 		readline.set_completer_delims(" ")
 
-		self.__db = PWManDatabase(filename, passphrase, readOnly=False)
+		self.__dbs = {
+			"main" : PWManDatabase(filename, passphrase, readOnly=False),
+		}
+		self.__selDbName = "main"
+
 		self.__updatePrompt()
 
 		self._timeout = PWManTimeout(timeout)
-		self.__commitClearsUndo = commitClearsUndo
-		self.__undo = UndoStack()
+
+	@property
+	def __db(self):
+		return self.__dbs[self.__selDbName]
 
 	def __updatePrompt(self):
-		if self.__db.isDirty():
-			self.prompt = "*pwman$ "
+		if len(self.__dbs) > 1:
+			dbName = self.__selDbName
+			lim = 20
+			if len(dbName) > lim - 3:
+				dbName = dbName[:lim-3] + "..."
 		else:
-			self.prompt = "pwman$ "
+			dbName = ""
+		dirty = any(db.isDirty() for db in self.__dbs.values())
+		self.prompt = "%spwman%s%s$ " % (
+			"*" if dirty else "",
+			"/" if dbName else "",
+			dbName
+		)
 
-	def __err(self, source, message):
+	@classmethod
+	def _err(cls, source, message):
 		source = (" " + source + ":") if source else ""
-		raise self.CommandError("***%s %s" % (source, message))
+		raise cls.CommandError("***%s %s" % (source, message))
 
-	def __warn(self, source, message):
+	@classmethod
+	def _warn(cls, source, message):
 		source = (" " + source + ":") if source else ""
 		print("***%s %s" % (source, message))
 
-	def __info(self, source, message):
+	@classmethod
+	def _info(cls, source, message):
 		source = ("+++ " + source + ": ") if source else ""
 		print("%s%s" % (source, message))
 
 	def precmd(self, line):
 		self._timeout.poke()
-		first = self._getParam(line, 0, unescape=False)
+		first = PWManOpts.parseParam(line, 0, unescape=False)
 		if first.endswith('?'):
 			return "help %s" % first[:-1]
 		return line
 
 	def postcmd(self, stop, line):
 		self.__updatePrompt()
 		self._timeout.poke()
 
 	def default(self, line):
 		extra = "\nType 'help' for more help." if self.__isInteractive else ""
-		self.__err(None, "Unknown command: %s%s" % (line, extra))
+		self._err(None, "Unknown command: %s%s" % (line, extra))
 
 	def emptyline(self):
 		self._timeout.poke()
 		# Don't repeat the last command
 
 	@completion
 	def __complete_category_title(self, text, line, begidx, endidx):
 		# Generic [category] [title] completion
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx == 0:
 			# Category completion
 			return self.__getCategoryCompletions(text)
 		elif paramIdx == 1:
 			# Entry title completion
-			return self.__getEntryTitleCompletions(self._getComplParam(line, 0),
+			return self.__getEntryTitleCompletions(PWManOpts.parseComplParam(line, 0),
 							       text)
 		return []
 
 	@completion
 	def __complete_category_title_item(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx in (0, 1):
 			return self.__complete_category_title(text, line, begidx, endidx)
-		category, title, item = self._getComplParams(line, 0, 3)
+		category, title, item = PWManOpts.parseComplParams(line, 0, 3)
 		cmpl = []
 		if paramIdx == 2:
 			cmpl.extend(escapeCmd(n) + " "
 				    for n in ("user", "password", "bulk", "totpkey")
-				    if n.startswith(item.lower()))
+				    if n.startswith(item))
 		cmpl.extend(self.__getEntryAttrCompletions(category, title, item,
 							   doName=(paramIdx == 2),
 							   doData=False,
 							   text=text))
 		return cmpl
 
-	def __getCategoryCompletions(self, text):
+	def __getCategoryCompletions(self, text, db=None):
+		db = db or self.__db
 		return [ escapeCmd(n) + " "
-			 for n in self.__db.getCategoryNames()
-			 if n.lower().startswith(text.lower()) ]
+			 for n in db.getCategoryNames()
+			 if n.startswith(text) ]
 
-	def __getEntryTitleCompletions(self, category, text):
+	def __getEntryTitleCompletions(self, category, text, db=None):
+		db = db or self.__db
 		return [ escapeCmd(t) + " "
-			 for t in self.__db.getEntryTitles(category)
-			 if t.lower().startswith(text.lower()) ]
+			 for t in db.getEntryTitles(category)
+			 if t.startswith(text) ]
 
-	def __getEntryAttrCompletions(self, category, title, name, doName, doData, text):
+	def __getEntryAttrCompletions(self, category, title, name, doName, doData, text, db=None):
+		db = db or self.__db
 		if category and title:
-			entry = self.__db.getEntry(category, title)
+			entry = db.getEntry(category, title)
 			if entry:
 				if doName: # complete name
-					entryAttrs = self.__db.getEntryAttrs(entry)
+					entryAttrs = db.getEntryAttrs(entry)
 					if entryAttrs:
 						return [ escapeCmd(entryAttr.name) + " "
 							 for entryAttr in entryAttrs
-							 if entryAttr.name.lower().startswith(name.lower()) ]
+							 if entryAttr.name.startswith(name) ]
 				elif doData: # complete data
-					entryAttr = self.__db.getEntryAttr(entry, name)
+					entryAttr = db.getEntryAttr(entry, name)
 					if entryAttr:
 						return [ escapeCmd(entryAttr.data) + " " ]
 		return []
 
+	def __getDatabaseCompletions(self, text):
+		return [ escapeCmd(n) + " "
+			 for n in self.__dbs.keys()
+			 if n.startswith(text) ]
+
 	def __getPathCompletions(self, text):
 		"""Return an escaped file system path completion.
 		'text' is the unescaped partial path string.
 		"""
 		try:
 			path = pathlib.Path(text)
 			trailingChar = text[-1] if text else ""
@@ -334,481 +520,752 @@
 		("new", ("n", "add"), "Create new entry"),
 		("edit_user", ("eu",), "Edit the 'user' field of an entry"),
 		("edit_pw", ("ep",), "Edit the 'password' field of an entry"),
 		("edit_bulk", ("eb",), "Edit the 'bulk' field of an entry"),
 		("edit_totp", ("et",), "Edit the TOTP key and parameters"),
 		("edit_attr", ("ea",), "Edit an entry attribute"),
 		("move", ("mv", "rename"), "Move/rename an existing entry"),
+		("copy", ("cp",), "Copy an existing entry or category"),
 		("remove", ("rm", "del"), "Remove an existing entry"),
-		("undo", (), "Undo the last command"),
-		("redo", (), "Redo the last undone command"),
 	)
 
 	cmdHelpDatabase = (
-		("commit", ("c", "w"), "Commit/write database file"),
-		("masterp", (), "Change the master passphrase"),
-		("dbdump", (), "Dump the database"),
+		("database", ("db",), "Open or select another database"),
+		("commit", ("c", "w"), "Commit/write selected db to disk"),
+		("drop", (), "Drop uncommitted changes in selected db"),
+		("close", (), "Close a database"),
+		("dbdump", (), "Dump the selected database"),
 		("dbimport", (), "Import a database dump file"),
-		("drop", (), "Drop all uncommitted changes"),
+		("masterp", (), "Change the master passphrase"),
 	)
 
 	cmdHelpMisc = (
 		("help", ("h",), "Show help about commands"),
 		("quit", ("q", "exit", "^D"), "Quit pwman"),
-		("cls", (), "Clear screen and undo buffers"),
+		("cls", (), "Clear screen"),
 	)
 
 	def do_help(self, params):
-		"""--- Shows help text about a command ---\n
-		Command: help\n
-		Aliases: h"""
+		"""--- Shows help text about a command ---
+		Command: help [COMMAND]
+
+		If COMMAND is not given: Show a command summary.
+		If COMMAND is given: Show detailed help about that command.
+
+		Aliases: h
+		"""
 		if params:
-			super().do_help(params)
+			Cmd.do_help(self, params)
 			return
 		def printCmdHelp(cmdHelp):
 			for cmd, aliases, desc in cmdHelp:
 				spc = " " * (10 - len(cmd))
 				msg = "  %s%s%s" % (cmd, spc, desc)
 				if aliases:
-					msg += " " * (51 - len(msg))
+					msg += " " * (52 - len(msg))
 					msg += " Alias%s: %s" %\
 					("es" if len(aliases) > 1 else "",
 					", ".join(aliases))
-				self.__info(None, msg)
-		self.__info(None, "\nSearching/listing commands:")
+				self._info(None, msg)
+		self._info(None, "\nSearching/listing commands:")
 		printCmdHelp(self.cmdHelpShow)
-		self.__info(None, "\nEditing commands:")
+		self._info(None, "\nEditing commands:")
 		printCmdHelp(self.cmdHelpEdit)
-		self.__info(None, "\nDatabase commands:")
+		self._info(None, "\nDatabase commands:")
 		printCmdHelp(self.cmdHelpDatabase)
-		self.__info(None, "\nMisc commands:")
+		self._info(None, "\nMisc commands:")
 		printCmdHelp(self.cmdHelpMisc)
-		self.__info(None, "\nType 'command?' or 'help command' for more help on a command.")
+		self._info(None, "\nType 'command?' or 'help command' for more help on a command.")
 	do_h = do_help
 
 	def do_quit(self, params):
 		"""--- Exit pwman ---
-		Command: quit [!]\n
-		Use the exclamation mark to force quit and discard changes.\n
-		Aliases: q exit ^D"""
+		Command: quit [!]
+
+		Use the exclamation mark to force quit and discard changes.
+
+		Aliases: q exit ^D
+		"""
 		if params == "!":
-			self.__db.flunkDirty()
+			for db in self.__dbs.values():
+				db.flunkDirty()
 		raise self.Quit()
 	do_q = do_quit
 	do_exit = do_quit
 	do_EOF = do_quit
 
 	def do_cls(self, params):
-		"""--- Clear console screen and undo/redo buffer ---
-		Command: cls\n
-		Clear the console screen and all undo/redo buffers.
+		"""--- Clear console screen ---
+		Command: cls
+
+		Clear the console screen.
 		Note that this does not clear a possibly existing
-		'screen' session buffer or other advanced console buffers.\n
-		Aliases: None"""
+		'screen' session buffer or other advanced console buffers.
+
+		Aliases: None
+		"""
 		clearScreen()
-		self.__undo.clear()
 
+	__commit_opts = ("-a",)
 	def do_commit(self, params):
-		"""--- Write changes to the database file ---\n
-		Command: commit\n
-		Aliases: c w"""
-		self.__db.commit()
-		if self.__commitClearsUndo:
-			self.__undo.clear()
+		"""--- Write changes to the database file(s) ---
+		Command: commit
+
+		Options:
+		  -a   Commit all open databases.
+
+		Aliases: c w
+		"""
+		opts = PWManOpts.parse(params, self.__commit_opts)
+		dbs = self.__dbs.values() if "-a" in opts else [ self.__db ]
+		try:
+			for db in dbs:
+				db.commit()
+		except PWManError as e:
+			self._err("commit", str(e))
 	do_c = do_commit
 	do_w = do_commit
 
+	@completion
+	def complete_commit(self, text, line, begidx, endidx):
+		if text == "-":
+			return PWManOpts.rawOptTemplates(self.__commit_opts)
+		return []
+	complete_c = complete_commit
+	complete_w = complete_commit
+
 	def do_masterp(self, params):
-		"""--- Change the master passphrase ---\n
-		Command: masterp\n
-		Aliases: None"""
+		"""--- Change the master passphrase ---
+		Command: masterp
+
+		Aliases: None
+		"""
 		p = readPassphrase("Current master passphrase")
 		if p != self.__db.getPassphrase():
 			time.sleep(1)
-			self.__warn(None, "Passphrase mismatch! ")
+			self._warn(None, "Passphrase mismatch! ")
 			return
 		p = readPassphrase("Master passphrase", verify=True)
 		if p is None:
-			self.__info(None, "Passphrase not changed.")
+			self._info(None, "Passphrase not changed.")
 			return
 		if p != self.__db.getPassphrase():
 			self.__db.setPassphrase(p)
-			self.__undo.clear()
 
 	def do_list(self, params):
 		"""--- Print a listing ---
-		Command: list [category] [title] [item]\n
+		Command: list [category] [title] [item]
+
 		If a category is given as parameter, list the 
 		contents of the category. If category and entry
 		are given, list the contents of the entry.
 		If item is given, then only list one specific content item.
-		Item may be one of: user, password, bulk, totpkey or any attribute name.\n
-		Aliases: ls cat"""
-		category, title, item = self._getParams(params, 0, 3)
+		Item may be one of: user, password, bulk, totpkey or any attribute name.
+
+		Aliases: ls cat
+		"""
+		category, title, item = PWManOpts.parseParams(params, 0, 3)
 		if not category and not title and not item:
-			self.__info(None, "Categories:")
-			self.__info(None, "\t" + "\n\t".join(self.__db.getCategoryNames()))
+			self._info(None, "Categories:")
+			self._info(None, "\t" + "\n\t".join(self.__db.getCategoryNames()))
 		elif category and not title and not item:
-			self.__info(None, "Entries in category '%s':" % category)
-			self.__info(None, "\t" + "\n\t".join(self.__db.getEntryTitles(category)))
+			self._info(None, "Entries in category '%s':" % category)
+			self._info(None, "\t" + "\n\t".join(self.__db.getEntryTitles(category)))
 		elif category and title and not item:
 			entry = self.__db.getEntry(category, title)
 			if entry:
-				self.__info(None, self.__db.dumpEntry(entry))
+				self._info(None, self.__db.dumpEntry(entry))
 			else:
-				self.__err("list", "'%s/%s' not found" % (category, title))
+				self._err("list", "'%s/%s' not found" % (category, title))
 		elif category and title and item:
 			entry = self.__db.getEntry(category, title)
 			if entry:
 				if item == "user":
 					if not entry.user:
-						self.__err("list", "'%s/%s' has no 'user' field." % (
-							   category, title))
-					self.__info(None, entry.user)
+						self._err("list", "'%s/%s' has no 'user' field." % (
+							  category, title))
+					self._info(None, entry.user)
 				elif item == "password":
 					if not entry.pw:
-						self.__err("list", "'%s/%s' has no 'password' field." % (
-							   category, title))
-					self.__info(None, entry.pw)
+						self._err("list", "'%s/%s' has no 'password' field." % (
+							  category, title))
+					self._info(None, entry.pw)
 				elif item == "bulk":
 					bulk = self.__db.getEntryBulk(entry)
 					if not bulk:
-						self.__err("list", "'%s/%s' has no 'bulk' field." % (
-							   category, title))
-					self.__info(None, bulk.data)
+						self._err("list", "'%s/%s' has no 'bulk' field." % (
+							  category, title))
+					self._info(None, bulk.data)
 				elif item == "totpkey":
 					entryTotp = self.__db.getEntryTotp(entry)
 					if not entryTotp:
-						self.__err("list", "'%s/%s' has no 'TOTP key'." % (
-							   category, title))
-					self.__info(None, "TOTP key:     %s (base32 encoding)" % entryTotp.key)
-					self.__info(None, "TOTP digits:  %d" % entryTotp.digits)
-					self.__info(None, "TOTP hash:    %s" % entryTotp.hmacHash)
+						self._err("list", "'%s/%s' has no 'TOTP key'." % (
+							  category, title))
+					self._info(None, "TOTP key:     %s (base32 encoding)" % entryTotp.key)
+					self._info(None, "TOTP digits:  %d" % entryTotp.digits)
+					self._info(None, "TOTP hash:    %s" % entryTotp.hmacHash)
 				else: # attribute
 					attr = self.__db.getEntryAttr(entry, item)
 					if not attr:
-						self.__err("list", "'%s/%s' has no attribute '%s'." % (
-							   category, title, item))
-					self.__info(None, attr.data)
+						self._err("list", "'%s/%s' has no attribute '%s'." % (
+							  category, title, item))
+					self._info(None, attr.data)
 			else:
-				self.__err("list", "'%s/%s' not found" % (category, title))
+				self._err("list", "'%s/%s' not found" % (category, title))
 		else:
-			self.__err("list", "Invalid parameter")
+			self._err("list", "Invalid parameter")
 	do_ls = do_list
 	do_cat = do_list
 
 	complete_list = __complete_category_title_item
 	complete_ls = complete_list
 	complete_cat = complete_list
 
 	def do_new(self, params):
 		"""--- Create a new entry ---
-		Command: new [category] [title] [user] [password]\n
+		Command: new [category] [title] [user] [password]
+
 		Create a new database entry. If no parameters are given,
-		they are asked for interactively.\n
-		Aliases: n add"""
+		they are asked for interactively.
+
+		Aliases: n add
+		"""
 		if params:
-			category, title, user, pw = self._getParams(params, 0, 4)
+			category, title, user, pw = PWManOpts.parseParams(params, 0, 4)
 		else:
-			self.__info("new", "Create new entry:")
+			self._info("new", "Create new entry:")
 			category = input("\tCategory: ")
 			title = input("\tEntry title: ")
 			user = input("\tUsername: ")
 			pw = input("\tPassword: ")
 		if not category or not title:
-			self.__err("new", "Invalid parameters. "
-				"Need to supply category and title.")
+			self._err("new", "Invalid parameters. "
+				  "Need to supply category and title.")
 		entry = PWManEntry(category=category, title=title, user=user, pw=pw)
 		try:
 			self.__db.addEntry(entry)
 		except (PWManError) as e:
-			self.__err("new", str(e))
-		self.__undo.do("new %s" % params,
-			       "remove %s %s" % (escapeCmd(category), escapeCmd(title)))
+			self._err("new", str(e))
 	do_n = do_new
 	do_add = do_new
 
 	complete_new = __complete_category_title
 	complete_n = complete_new
 	complete_add = complete_new
 
 	def __do_edit_entry(self, params, commandName,
 			    entry2data, data2entry):
-		category, title = self._getParams(params, 0, 2)
+		category, title = PWManOpts.parseParams(params, 0, 2)
 		if not category or not title:
-			self.__err(commandName, "Invalid parameters. "
-				"Need to supply category and title.")
-		oldEntry = self.__db.getEntry(category, title)
-		if not oldEntry:
-			self.__err(commandName, "Entry does not exist")
-		newData = self._skipParams(params, 2).strip()
+			self._err(commandName, "Invalid parameters. "
+				  "Need to supply category and title.")
+		newData = PWManOpts.skipParams(params, 2).strip()
 		try:
 			self.__db.editEntry(data2entry(category, title, newData))
 		except (PWManError) as e:
-			self.__err(commandName, str(e))
-		self.__undo.do("%s %s" % (commandName, params),
-			       "%s %s %s %s" %\
-			       (commandName, escapeCmd(oldEntry.category),
-				escapeCmd(oldEntry.title),
-				escapeCmd(entry2data(oldEntry))))
+			self._err(commandName, str(e))
 
 	def do_edit_user(self, params):
 		"""--- Edit the 'user' field of an existing entry ---
-		Command: edit_user category title NEWDATA...\n
+		Command: edit_user category title NEWDATA...
+
 		Change the 'user' field of an existing database entry.
 		NEWDATA is the new data to write into the 'user' field.
 		The NEWDATA must _not_ be escaped (however, category and
-		title must be escaped).\n
-		Aliases: eu"""
+		title must be escaped).
+
+		Aliases: eu
+		"""
 		self.__do_edit_entry(params, "edit_user",
 			lambda entry: entry.user,
 			lambda cat, tit, data: PWManEntry(cat, tit, user=data))
 	do_eu = do_edit_user
 
 	@completion
 	def complete_edit_user(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx == 0:
 			# Category completion
 			return self.__getCategoryCompletions(text)
 		elif paramIdx == 1:
 			# Entry title completion
-			return self.__getEntryTitleCompletions(self._getComplParam(line, 0),
+			return self.__getEntryTitleCompletions(PWManOpts.parseComplParam(line, 0),
 							       text)
 		elif paramIdx == 2:
 			# User data
-			entry = self.__db.getEntry(self._getComplParam(line, 0),
-						   self._getComplParam(line, 1))
+			entry = self.__db.getEntry(PWManOpts.parseComplParam(line, 0),
+						   PWManOpts.parseComplParam(line, 1))
 			return [ escapeCmd(entry.user) ]
 		return []
 	complete_eu = complete_edit_user
 
 	def do_edit_pw(self, params):
 		"""--- Edit the 'password' field of an existing entry ---
-		Command: edit_pw category title NEWDATA...\n
+		Command: edit_pw category title NEWDATA...
+
 		Change the 'password' field of an existing database entry.
 		NEWDATA is the new data to write into the 'password' field.
 		The NEWDATA must _not_ be escaped (however, category and
-		title must be escaped).\n
-		Aliases: ep"""
+		title must be escaped).
+
+		Aliases: ep
+		"""
 		self.__do_edit_entry(params, "edit_pw",
 			lambda entry: entry.pw,
 			lambda cat, tit, data: PWManEntry(cat, tit, pw=data))
 	do_ep = do_edit_pw
 
 	@completion
 	def complete_edit_pw(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx == 0:
 			# Category completion
 			return self.__getCategoryCompletions(text)
 		elif paramIdx == 1:
 			# Entry title completion
-			return self.__getEntryTitleCompletions(self._getComplParam(line, 0),
+			return self.__getEntryTitleCompletions(PWManOpts.parseComplParam(line, 0),
 							       text)
 		elif paramIdx == 2:
 			# Password data
-			entry = self.__db.getEntry(self._getComplParam(line, 0),
-						   self._getComplParam(line, 1))
+			entry = self.__db.getEntry(PWManOpts.parseComplParam(line, 0),
+						   PWManOpts.parseComplParam(line, 1))
 			return [ escapeCmd(entry.pw) ]
 		return []
 	complete_ep = complete_edit_pw
 
 	def do_edit_bulk(self, params):
 		"""--- Edit the 'bulk' field of an existing entry ---
-		Command: edit_bulk category title NEWDATA...\n
+		Command: edit_bulk category title NEWDATA...
+
 		Change the 'bulk' field of an existing database entry.
 		NEWDATA is the new data to write into the 'bulk' field.
 		The NEWDATA must _not_ be escaped (however, category and
-		title must be escaped).\n
-		Aliases: eb"""
-		category, title = self._getParams(params, 0, 2)
-		data = self._skipParams(params, 2).strip()
+		title must be escaped).
+
+		Aliases: eb
+		"""
+		category, title = PWManOpts.parseParams(params, 0, 2)
+		data = PWManOpts.skipParams(params, 2).strip()
 		if not category:
-			self.__err("edit_bulk", "Category parameter is required.")
+			self._err("edit_bulk", "Category parameter is required.")
 		if not title:
-			self.__err("edit_bulk", "Title parameter is required.")
+			self._err("edit_bulk", "Title parameter is required.")
 		entry = self.__db.getEntry(category, title)
 		if not entry:
-			self.__err("edit_bulk", "'%s/%s' not found" % (category, title))
+			self._err("edit_bulk", "'%s/%s' not found" % (category, title))
 		entryBulk = self.__db.getEntryBulk(entry)
 		if not entryBulk:
 			entryBulk = PWManEntryBulk(entry=entry)
-		origEntryBulk = deepcopy(entryBulk)
 		entryBulk.data = data
 		self.__db.setEntryBulk(entryBulk)
-		self.__undo.do("edit_bulk %s" % params,
-			       "edit_bulk %s %s %s" % (
-			       escapeCmd(category),
-			       escapeCmd(title),
-			       escapeCmd(origEntryBulk.data or "")))
 	do_eb = do_edit_bulk
 
 	@completion
 	def complete_edit_bulk(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx == 0:
 			# Category completion
 			return self.__getCategoryCompletions(text)
 		elif paramIdx == 1:
 			# Entry title completion
-			return self.__getEntryTitleCompletions(self._getComplParam(line, 0),
+			return self.__getEntryTitleCompletions(PWManOpts.parseComplParam(line, 0),
 							       text)
 		elif paramIdx == 2:
 			# Bulk data
-			entry = self.__db.getEntry(self._getComplParam(line, 0),
-						   self._getComplParam(line, 1))
+			entry = self.__db.getEntry(PWManOpts.parseComplParam(line, 0),
+						   PWManOpts.parseComplParam(line, 1))
 			if entry:
 				entryBulk = self.__db.getEntryBulk(entry)
 				if entryBulk:
 					return [ escapeCmd(entryBulk.data) ]
 		return []
 	complete_eb = complete_edit_bulk
 
 	def do_remove(self, params):
 		"""--- Remove an existing entry ---
-		Command: remove category [title]\n
-		Remove an existing database entry.\n
-		Aliases: rm del"""
-		category, title = self._getParams(params, 0, 2)
+		Command: remove category [title]
+
+		Remove an existing database entry.
+
+		Aliases: rm del
+		"""
+		category, title = PWManOpts.parseParams(params, 0, 2)
 		if not category:
-			self.__err("remove", "Category parameter is required.")
+			self._err("remove", "Category parameter is required.")
 		if not title:
 			# Remove whole category
 			for title in self.__db.getEntryTitles(category):
 				p = "%s %s" % (escapeCmd(category),
 					       escapeCmd(title))
-				self.__info("remove", "running: remove %s" % p)
+				self._info("remove", "running command: remove %s" % p)
 				self.do_remove(p)
 			return
-		oldEntry = self.__db.getEntry(category, title)
-		if not oldEntry:
-			self.__err("remove", "Entry does not exist")
-		oldEntryBulk = self.__db.getEntryBulk(oldEntry)
-		oldEntryAttrs = self.__db.getEntryAttrs(oldEntry)
-		oldEntryTotp = self.__db.getEntryTotp(oldEntry)
 		try:
 			self.__db.delEntry(PWManEntry(category, title))
 		except (PWManError) as e:
-			self.__err("remove", str(e))
-		undoCmds = [ "new %s %s %s %s" % (
-			     escapeCmd(oldEntry.category),
-			     escapeCmd(oldEntry.title),
-			     escapeCmd(oldEntry.user),
-			     escapeCmd(oldEntry.pw)) ]
-		if oldEntryBulk:
-			undoCmds.append("edit_bulk %s %s %s" % (
-					escapeCmd(oldEntry.category),
-					escapeCmd(oldEntry.title),
-					escapeCmd(oldEntryBulk.data or "")))
-		for oldEntryAttr in (oldEntryAttrs or []):
-			undoCmds.append("edit_attr %s %s %s %s" % (
-					escapeCmd(oldEntry.category),
-					escapeCmd(oldEntry.title),
-					escapeCmd(oldEntryAttr.name),
-					escapeCmd(oldEntryAttr.data or "")))
-		if oldEntryTotp:
-			undoCmds.append("edit_totp %s %s %s %s %s" % (
-					escapeCmd(oldEntry.category),
-					escapeCmd(oldEntry.title),
-					escapeCmd(oldEntryTotp.key or ""),
-					escapeCmd(("%d" % oldEntryTotp.digits) if oldEntryTotp.digits else ""),
-					escapeCmd(oldEntryTotp.hmacHash or "")))
-		self.__undo.do("remove %s" % params, undoCmds)
+			self._err("remove", str(e))
 	do_rm = do_remove
 	do_del = do_remove
 
 	complete_remove = __complete_category_title
 	complete_rm = complete_remove
 	complete_del = complete_remove
 
+	__move_opts = ("-s:", "-d:")
 	def do_move(self, params):
-		"""--- Move/rename an existing entry or a category ---\n
+		"""--- Move/rename an existing entry or a category ---
+
 		Move/rename an existing entry:
-		Command: move category title newCategory [newTitle]\n
-		Rename an existing category:
-		Command: move category newCategory\n
-		Aliases: mv rename"""
-		p0, p1, p2, p3 = self._getParams(params, 0, 4)
-		if p0 and p1 and p2:
-			# Entry move
-			fromCategory, fromTitle, toCategory, toTitle = p0, p1, p2, p3
-			if not toTitle:
-				toTitle = fromTitle
-			if fromCategory == toCategory and fromTitle == toTitle:
-				self.__info("move", "Nothing changed. Not moving anything.")
+		Command: move CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+		(NEW_TITLE defaults to TITLE)
+
+		Move all entries from one category into another category.
+		Command: move FROM_CATEGORY TO_CATEGORY
+
+		Move an entry from one database to another:
+		Command: move -s main -d other CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+		(NEW_TITLE defaults to TITLE)
+
+		Move all entries from a category from one database into another database:
+		Command: move -s main -d other FROM_CATEGORY [TO_CATEGORY]
+		(TO_CATEGORY defaults to FROM_CATEGORY)
+
+		Options:
+		  -s SOURCE_DATABASE_NAME
+		  -d DESTINATION_DATABASE_NAME
+		  Databases default to the currently selected database.
+		  The named databases must be open. See 'database' command.
+
+		Aliases: mv rename
+		"""
+		opts = PWManOpts.parse(params, self.__move_opts)
+
+		sourceDbName = opts.getOpt("-s", default=self.__selDbName)
+		sourceDb = self.__dbs.get(sourceDbName, None)
+		if sourceDb is None:
+			self._err("move", "Source database '%s' does not exist" % sourceDbName)
+		destDbName = opts.getOpt("-d", default=self.__selDbName)
+		destDb = self.__dbs.get(destDbName, None)
+		if destDb is None:
+			self._err("move", "Destination database '%s' does not exist" % destDbName)
+
+		if opts.nrParams in (3, 4):
+			# Entry rename/move
+			fromCategory, fromTitle, toCategory, toTitle =\
+				(opts.getParam(0), opts.getParam(1),
+				 opts.getParam(2), opts.getParam(3))
+			toTitle = toTitle or fromTitle
+			if sourceDb is destDb and fromCategory == toCategory and fromTitle == toTitle:
+				self._info("move", "Nothing changed. Not moving anything.")
 				return
-			entry = self.__db.getEntry(fromCategory, fromTitle)
-			if not entry:
-				self.__err("move", "Source entry does not exist.")
+			entry = sourceDb.getEntry(fromCategory, fromTitle)
 			oldEntry = deepcopy(entry)
+			if not entry:
+				self._err("move", "Source entry does not exist.")
 			try:
-				self.__db.moveEntry(entry, toCategory, toTitle)
+				if sourceDb is destDb:
+					# Move in one DB.
+					sourceDb.moveEntry(entry, toCategory, toTitle)
+				else:
+					# Move between different DBs.
+					entry.entryId = None
+					entry.category = toCategory
+					entry.title = toTitle
+					destDb.addEntry(entry)
+					sourceDb.delEntry(oldEntry)
 			except (PWManError) as e:
-				self.__err("move", str(e))
-			self.__undo.do("move %s" % params,
-				       "move %s %s %s %s" % (
-				       escapeCmd(entry.category), escapeCmd(entry.title),
-				       escapeCmd(oldEntry.category), escapeCmd(oldEntry.title)))
-		elif p0 and p1:
-			# Category rename
-			fromCategory, toCategory = p0, p1
+				self._err("move", str(e))
+		elif (sourceDb is destDb and opts.nrParams == 2) or\
+		     (sourceDb is not destDb and opts.nrParams in (1, 2)):
+			# Whole category move.
+			fromCategory, toCategory = opts.getParam(0), opts.getParam(1)
+			toCategory = toCategory or fromCategory
 			try:
-				self.__db.renameCategory(fromCategory, toCategory)
+				if sourceDb is destDb:
+					# Category move in one DB.
+					sourceDb.moveEntries(fromCategory, toCategory)
+				else:
+					# Category move between DBs.
+					if not sourceDb.categoryExists(fromCategory):
+						self._err("move", "Source category does not exist.")
+					for fromTitle in sourceDb.getEntryTitles(fromCategory):
+						self._info("move",
+							"running command: move -s %s -d %s %s %s %s %s" % (
+							escapeCmd(sourceDbName), escapeCmd(destDbName),
+							escapeCmd(fromCategory), escapeCmd(fromTitle),
+							escapeCmd(toCategory), escapeCmd(fromTitle)))
+						entry = sourceDb.getEntry(fromCategory, fromTitle)
+						oldEntry = deepcopy(entry)
+						entry.entryId = None
+						entry.category = toCategory
+						destDb.addEntry(entry)
+						sourceDb.delEntry(oldEntry)
 			except (PWManError) as e:
-				self.__err("move", str(e))
-			self.__undo.do("move %s" % params,
-				       "move %s %s" % (
-				       escapeCmd(toCategory), escapeCmd(fromCategory)))
+				self._err("move", str(e))
 		else:
-			self.__err("move", "Invalid parameters.")
+			self._err("move", "Invalid parameters.")
 	do_mv = do_move
 	do_rename = do_move
 
 	@completion
 	def complete_move(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
-		if paramIdx in (0, 2):
+		if text == "-":
+			return PWManOpts.rawOptTemplates(self.__move_opts)
+		if len(text) == 2 and text.startswith("-"):
+			return [ text + " " ]
+		dbOpts = ("-s", "-d")
+		opts = PWManOpts.parse(line, self.__move_opts, ignoreFirst=True, softFail=True)
+		if opts.error:
+			opt, error = opts.error
+			if error == "no_arg" and opt in dbOpts:
+				return self.__getDatabaseCompletions(text)
+			return []
+		optName, value = opts.atCmdIndex(PWManOpts.calcParamIndex(line, endidx))
+		if optName in dbOpts:
+			return self.__getDatabaseCompletions(text)
+
+		sourceDbName = opts.getOpt("-s", default=self.__selDbName)
+		sourceDb = self.__dbs.get(sourceDbName, None)
+		if sourceDb is None:
+			return []
+		destDbName = opts.getOpt("-d", default=self.__selDbName)
+		destDb = self.__dbs.get(destDbName, None)
+		if destDb is None:
+			return []
+
+		paramIdx = opts.getComplParamIdx(text)
+		if paramIdx == 0:
 			# Category completion
-			return self.__getCategoryCompletions(text)
-		elif paramIdx in (1, 3):
+			return self.__getCategoryCompletions(text, db=sourceDb)
+		elif paramIdx == 1:
+			# Entry title completion
+			category = opts.getParam(0)
+			if category:
+				compl = self.__getEntryTitleCompletions(category, text, db=sourceDb)
+				if compl:
+					return compl
+				# Category completion
+				return self.__getCategoryCompletions(text, db=destDb)
+		elif paramIdx == 2:
+			# Category completion
+			return self.__getCategoryCompletions(text, db=destDb)
+		elif paramIdx == 3:
 			# Entry title completion
-			category = self._getComplParam(line, 0 if paramIdx == 1 else 2)
-			return self.__getEntryTitleCompletions(category, text)
+			category = opts.getParam(2)
+			if category:
+				return self.__getEntryTitleCompletions(category, text, db=destDb)
 		return []
 	complete_mv = complete_move
 	complete_rename = complete_move
 
+	__copy_opts = ("-s:", "-d:")
+	def do_copy(self, params):
+		"""--- Copy an entry or a category ---
+
+		Copy an existing entry:
+		Command: copy CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+		(NEW_TITLE defaults to TITLE)
+
+		Copy all entries from a category into another category:
+		Command: copy FROM_CATEGORY TO_CATEGORY
+
+		Copy an entry from one database to another:
+		Command: copy -s main -d other CATEGORY TITLE TO_CATEGORY [NEW_TITLE]
+		(NEW_TITLE defaults to TITLE)
+
+		Copy all entries from a category from one database into another database:
+		Command: copy -s main -d other FROM_CATEGORY [TO_CATEGORY]
+		(TO_CATEGORY defaults to FROM_CATEGORY)
+
+		Options:
+		  -s SOURCE_DATABASE_NAME
+		  -d DESTINATION_DATABASE_NAME
+		  Databases default to the currently selected database.
+		  The named databases must be open. See 'database' command.
+
+		Aliases: cp
+		"""
+		opts = PWManOpts.parse(params, self.__copy_opts)
+
+		sourceDbName = opts.getOpt("-s", default=self.__selDbName)
+		sourceDb = self.__dbs.get(sourceDbName, None)
+		if sourceDb is None:
+			self._err("copy", "Source database '%s' does not exist" % sourceDbName)
+		destDbName = opts.getOpt("-d", default=self.__selDbName)
+		destDb = self.__dbs.get(destDbName, None)
+		if destDb is None:
+			self._err("copy", "Destination database '%s' does not exist" % destDbName)
+
+		if opts.nrParams in (3, 4):
+			# Entry copy
+			fromCategory, fromTitle, toCategory, toTitle =\
+				(opts.getParam(0), opts.getParam(1),
+				 opts.getParam(2), opts.getParam(3))
+			toTitle = toTitle or fromTitle
+			if sourceDb is destDb and fromCategory == toCategory and fromTitle == toTitle:
+				self._info("copy", "Copy source and target are identical.")
+				return
+			entry = sourceDb.getEntry(fromCategory, fromTitle)
+			if not entry:
+				self._err("copy", "Source entry does not exist.")
+			try:
+				entry.entryId = None
+				entry.category = toCategory
+				entry.title = toTitle
+				destDb.addEntry(entry)
+			except (PWManError) as e:
+				self._err("copy", str(e))
+		elif (sourceDb is destDb and opts.nrParams == 2) or\
+		     (sourceDb is not destDb and opts.nrParams in (1, 2)):
+			# Category copy
+			fromCategory, toCategory = opts.getParam(0), opts.getParam(1)
+			toCategory = toCategory or fromCategory
+			try:
+				if not sourceDb.categoryExists(fromCategory):
+					self._err("copy", "Source category does not exist.")
+				for fromTitle in sourceDb.getEntryTitles(fromCategory):
+					self._info("copy",
+						"running command: copy -s %s -d %s %s %s %s %s" % (
+						escapeCmd(sourceDbName), escapeCmd(destDbName),
+						escapeCmd(fromCategory), escapeCmd(fromTitle),
+						escapeCmd(toCategory), escapeCmd(fromTitle)))
+					entry = sourceDb.getEntry(fromCategory, fromTitle)
+					entry.entryId = None
+					entry.category = toCategory
+					destDb.addEntry(entry)
+			except (PWManError) as e:
+				self._err("copy", str(e))
+		else:
+			self._err("copy", "Invalid parameters.")
+	do_cp = do_copy
+
+	complete_copy = complete_move # copy and move are equal w.r.t. completion
+	complete_cp = complete_copy
+
+	__database_opts = ("-f:",)
+	def do_database(self, params):
+		"""--- Open a database or switch to an already opened database ---
+		Command: database [-f FILEPATH] [NAME]
+
+		If neither FILEPATH nor NAME are given, then
+		a list of all currently opened databases will be printed.
+		The currently selected database will be marked with [@].
+		All databases with uncommitted changes will be marked with [*].
+
+		If only NAME is given, then the selected database will
+		be switched to the named one. NAME must already be open.
+
+		A new database can be opened with -f FILEPATH.
+		NAME is optional in this case.
+		The selected database will be switched to the newly opened one.
+
+		Aliases: db
+		"""
+		opts = PWManOpts.parse(params, self.__database_opts)
+		path = opts.getOpt("-f")
+		name = opts.getParam(0)
+		if path:
+			if opts.nrParams not in (0, 1):
+				self._err("database", "Invalid parameters.")
+			# Open a new db.
+			path = pathlib.Path(path)
+			name = name or path.name
+			if name == "main":
+				self._err("database",
+					  "The database name 'main' is reserved. "
+					  "Please select another name.")
+			if name in self.__dbs:
+				self._err("database",
+					  ("The database name '%' is already used. "
+					   "Please select another name.") % name)
+			try:
+				passphrase = readPassphrase(
+					"Master passphrase of '%s'" % path,
+					verify=not path.exists())
+				if passphrase is None:
+					self._err("database", "Could not get passphrase.")
+				db = PWManDatabase(filename=path,
+						   passphrase=passphrase,
+						   readOnly=False)
+			except PWManError as e:
+				self._err("database", str(e))
+			self.__dbs[name] = db
+			self.__selDbName = name
+		elif opts.nrParams == 1:
+			# Switch selected db to NAME.
+			if name not in self.__dbs:
+				self._err("database", "The database '%s' does not exist." % name)
+			if name != self.__selDbName:
+				self.__selDbName = name
+		elif opts.nrParams == 0:
+			# Print db list.
+			for name, db in self.__dbs.items():
+				flags = "@" if db is self.__db else " "
+				flags += "*" if db.isDirty() else " "
+				path = db.getFilename()
+				self._info(None, "[%s] %s: %s" % (
+					   flags, name, path))
+		else:
+			self._err("database", "Invalid parameters.")
+	do_db = do_database
+
+	@completion
+	def complete_database(self, text, line, begidx, endidx):
+		if text == "-":
+			return PWManOpts.rawOptTemplates(self.__database_opts)
+		if len(text) == 2 and text.startswith("-"):
+			return [ text + " " ]
+		opts = PWManOpts.parse(line, self.__database_opts, ignoreFirst=True, softFail=True)
+		if opts.error:
+			opt, error = opts.error
+			if error == "no_arg" and opt == "-f":
+				return self.__getPathCompletions(text)
+			return []
+		optName, value = opts.atCmdIndex(PWManOpts.calcParamIndex(line, endidx))
+		if optName == "-f":
+			return self.__getPathCompletions(text)
+		paramIdx = opts.getComplParamIdx(text)
+		if paramIdx == 0:
+			# Database name
+			return self.__getDatabaseCompletions(text)
+		return []
+	complete_db = complete_database
+
 	__dbdump_opts = ("-s", "-h", "-c")
 	def do_dbdump(self, params):
 		"""--- Dump the pwman SQL database ---
-		Command: dbdump [OPTS] [FILEPATH]\n
+		Command: dbdump [OPTS] [FILEPATH]
+
 		If FILEPATH is given, the database is dumped
 		unencrypted to the file.
 		If FILEPATH is omitted, the database is dumped
-		unencrypted to stdout.\n
+		unencrypted to stdout.
+
 		OPTS may be one of:
 		  -s   Dump format SQL. (default)
 		  -h   Dump format human readable text.
-		  -c   Dump format CSV.\n
-		WARNING: The database dump is not encrypted.\n
-		Aliases: None"""
-		opts = self._getOpts(params, self.__dbdump_opts)
+		  -c   Dump format CSV.
+
+		WARNING: The database dump is not encrypted.
+
+		Aliases: None
+		"""
+		opts = PWManOpts.parse(params, self.__dbdump_opts)
 		if opts.nrParams > 1:
-			self.__err("dbdump", "Too many arguments.")
+			self._err("dbdump", "Too many arguments.")
 		optFmtSqlDump = "-s" in opts
 		optFmtHumanReadable = "-h" in opts
 		optFmtCsv = "-c" in opts
 		numFmtOpts = int(optFmtSqlDump) + int(optFmtHumanReadable) + int(optFmtCsv)
 		if not 0 <= numFmtOpts <= 1:
-			self.__err("dbdump", "Multiple format OPTions. "
+			self._err("dbdump", "Multiple format OPTions. "
 					     "Only one is allowed.")
 		if numFmtOpts == 0:
 			optFmtSqlDump = True
-		dumpFile = opts.getParam(0) if opts.nrParams > 0 else None
+		dumpFile = opts.getParam(0)
 		try:
 			if optFmtSqlDump:
 				dump = self.__db.sqlPlainDump() + b"\n"
 			elif optFmtHumanReadable:
 				dump = self.__db.dumpEntries(showTotpKey=True)
 				dump = dump.encode("UTF-8") + b"\n"
 			elif optFmtCsv:
@@ -818,211 +1275,281 @@
 				assert(0)
 			if dumpFile:
 				with open(dumpFile, "wb") as f:
 					f.write(dump)
 			else:
 				stdout(dump)
 		except UnicodeError as e:
-			self.__err("dbdump", "Unicode error.")
+			self._err("dbdump", "Unicode error.")
 		except IOError as e:
-			self.__err("dbdump", "Failed to write dump: %s" % e.strerror)
+			self._err("dbdump", "Failed to write dump: %s" % e.strerror)
 
 	@completion
 	def complete_dbdump(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
 		if text == "-":
-			return self.__dbdump_opts
-		opts = self._getOpts(line, self.__dbdump_opts, ignoreFirst=True)
-		optName, value = opts.atCmdIndex(paramIdx)
-		if optName: # -... option
+			return PWManOpts.rawOptTemplates(self.__dbdump_opts)
+		if len(text) == 2 and text.startswith("-"):
 			return [ text + " " ]
-		if (opts.nrParams == 0 and not text) or (opts.nrParams == 1 and text): # trailing param
+		opts = PWManOpts.parse(line, self.__dbdump_opts, ignoreFirst=True, softFail=True)
+		if opts.error:
+			return []
+		paramIdx = opts.getComplParamIdx(text)
+		if paramIdx == 0:
+			# filepath
 			return self.__getPathCompletions(text)
 		return []
 
 	def do_dbimport(self, params):
 		"""--- Import an SQL database dump ---
-		Command: dbimport FILEPATH\n
+		Command: dbimport FILEPATH
+
 		Import the FILEPATH into the current database.
-		The database is cleared before importing the file!\n
-		Aliases: None"""
+		The database is cleared before importing the file!
+
+		Aliases: None
+		"""
 		try:
 			if not params.strip():
 				raise IOError("FILEPATH is empty.")
 			with open(params, "rb") as f:
 				data = f.read().decode("UTF-8")
 			self.__db.importSqlScript(data)
-			self.__info("dbimport", "success.")
+			self._info("dbimport", "success.")
 		except (CSQLError, IOError, UnicodeError) as e:
-			self.__err("dbimport", "Failed to import dump: %s" % str(e))
+			self._err("dbimport", "Failed to import dump: %s" % str(e))
 
 	@completion
 	def complete_dbimport(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx == 0:
 			return self.__getPathCompletions(text)
 		return []
 
 	def do_drop(self, params):
 		"""--- Drop all uncommitted changes ---
-		Command: drop\n
-		Aliases: None"""
+		Command: drop
+
+		Aliases: None
+		"""
 		self.__db.dropUncommitted()
 
+	def do_close(self, params):
+		"""--- Close a database ---
+		Command: close [!] [NAME]
+
+		If NAME is not given, then this closes the currently selected database.
+		If NAME is given, then this closes the named database.
+
+		If ! is specified, then the uncommitted changes will be dropped.
+
+		If the currently used database is closed, the selected database
+		will be switched to 'main'.
+
+		The 'main' database can only be closed last,
+		which in turn closes the application.
+
+		Aliases: None
+		"""
+		flunk = params.startswith("!")
+		if flunk:
+			params = params[1:].strip()
+		name = params if params else self.__selDbName
+		if name == "main" and len(self.__dbs) > 1:
+			self._err("close", "The 'main' database can only be closed last")
+		db = self.__dbs.get(name, None)
+		if db is None:
+			self._err("close", "The database '%s' does not exist" % name)
+		if db.isDirty():
+			if not flunk:
+				self._err("close", "The database '%s' contains "
+					  "uncommitted changes" % name)
+			db.flunkDirty()
+		if len(self.__dbs) > 1:
+			self.__dbs.pop(name)
+			if self.__selDbName == name:
+				self.__selDbName = "main"
+		else:
+			raise self.Quit()
+
+	@completion
+	def complete_close(self, text, line, begidx, endidx):
+		if text == "!":
+			return [ text + " " ]
+		opts = PWManOpts.parse(line, (), ignoreFirst=True, softFail=True)
+		if opts.error:
+			return []
+		paramIdx = opts.getComplParamIdx(text)
+		if paramIdx == 0 or (paramIdx == 1 and opts.getParam(0) == "!"):
+			# Database name
+			return self.__getDatabaseCompletions(text)
+		return []
+
 	__find_opts = ("-c", "-t", "-u", "-p", "-b", "-a", "-A", "-r")
 	def do_find(self, params):
 		"""--- Search the database ---
-		Command: find [OPTS] [IN_CATEGORY] PATTERN\n
+		Command: find [OPTS] [IN_CATEGORY] PATTERN
+
 		Searches the database for patterns. If 'IN_CATEGORY' is given, only search
 		in the specified category.
 		PATTERN may either use SQL LIKE wildcards (without -r)
-		or Python Regular Expression special characters (with -r).\n
+		or Python Regular Expression special characters (with -r).
+
 		OPTS may be one or multiple of:
 		  -c   Match 'category'       (only if no IN_CATEGORY parameter)
 		  -t   Match 'title'          (*)
 		  -u   Match 'user'           (*)
 		  -p   Match 'password'       (*)
 		  -b   Match 'bulk'           (*)
 		  -a   Match 'attribute data' (*)
 		  -A   Match 'attribute name'
-		  -r   Use Python Regular Expression matching\n
+		  -r   Use Python Regular Expression matching
+
 		(*) = These OPTS are enabled by default, if and only if
-		      none of them are specified by the user.\n
-		Aliases: f"""
-		opts = self._getOpts(params, self.__find_opts)
+		      none of them are specified by the user.
+
+		Aliases: f
+		"""
+		opts = PWManOpts.parse(params, self.__find_opts)
 		mCategory = "-c" in opts
 		mTitle = "-t" in opts
 		mUser = "-u" in opts
 		mPw = "-p" in opts
 		mBulk = "-b" in opts
 		mAttrData = "-a" in opts
 		mAttrName = "-A" in opts
 		regexp = "-r" in opts
 		if not any( (mTitle, mUser, mPw, mBulk, mAttrData) ):
 			mTitle, mUser, mPw, mBulk, mAttrData = (True,) * 5
 		if opts.nrParams < 1 or opts.nrParams > 2:
-			self.__err("find", "Invalid parameters.")
+			self._err("find", "Invalid parameters.")
 		inCategory = opts.getParam(0) if opts.nrParams > 1 else None
 		pattern = opts.getParam(1) if opts.nrParams > 1 else opts.getParam(0)
 		if inCategory and mCategory:
-			self.__err("find", "-c and [IN_CATEGORY] cannot be used at the same time.")
+			self._err("find", "-c and [IN_CATEGORY] cannot be used at the same time.")
 		entries = self.__db.findEntries(pattern=pattern,
 						useRegexp=regexp,
 						inCategory=inCategory,
 						matchCategory=mCategory,
 						matchTitle=mTitle,
 						matchUser=mUser,
 						matchPw=mPw,
 						matchBulk=mBulk,
 						matchAttrName=mAttrName,
 						matchAttrData=mAttrData)
 		if not entries:
-			self.__err("find", "'%s' not found" % pattern)
+			self._err("find", "'%s' not found" % pattern)
 		for entry in entries:
-			self.__info(None, self.__db.dumpEntry(entry))
+			self._info(None, self.__db.dumpEntry(entry))
 	do_f = do_find
 
 	@completion
 	def complete_find(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
 		if text == "-":
-			return self.__find_opts
-		opts = self._getOpts(line, self.__find_opts, ignoreFirst=True)
-		optName, value = opts.atCmdIndex(paramIdx)
-		if optName: # -... option
+			return PWManOpts.rawOptTemplates(self.__find_opts)
+		if len(text) == 2 and text.startswith("-"):
 			return [ text + " " ]
-		if (opts.nrParams == 0 and not text) or (opts.nrParams == 1 and text): # category
+		opts = PWManOpts.parse(line, self.__find_opts, ignoreFirst=True, softFail=True)
+		if opts.error:
+			return []
+		paramIdx = opts.getComplParamIdx(text)
+		if paramIdx == 0:
+			# category
 			return self.__getCategoryCompletions(text)
 		return []
 	complete_f = complete_find
 
 	def do_totp(self, params):
 		"""--- Generate a TOTP token ---
-		Command: totp [CATEGORY TITLE] OR [TITLE]\n
-		Generates a token using the Time-Based One-Time Password Algorithm.\n
-		Aliases: t"""
-		first, second = self._getParams(params, 0, 2)
+		Command: totp [CATEGORY TITLE] OR [TITLE]
+
+		Generates a token using the Time-Based One-Time Password Algorithm.
+
+		Aliases: t
+		"""
+		first, second = PWManOpts.parseParams(params, 0, 2)
 		if not first:
-			self.__err("totp", "First parameter is required.")
+			self._err("totp", "First parameter is required.")
 		if second:
 			category, title = first, second
 		else:
 			entries = self.__db.findEntries(first, matchTitle=True)
 			if not entries:
-				self.__err("totp", "Entry title not found.")
+				self._err("totp", "Entry title not found.")
 				return
 			elif len(entries) == 1:
 				category = entries[0].category
 				title = entries[0].title
 			else:
-				self.__err("totp", "Entry title ambiguous.")
+				self._err("totp", "Entry title ambiguous.")
 				return
 		entry = self.__db.getEntry(category, title)
 		if not entry:
-			self.__err("totp", "'%s/%s' not found" % (category, title))
+			self._err("totp", "'%s/%s' not found" % (category, title))
 		entryTotp = self.__db.getEntryTotp(entry)
 		if not entryTotp:
-			self.__err("totp", "'%s/%s' does not have "
+			self._err("totp", "'%s/%s' does not have "
 				   "TOTP key information" % (category, title))
 		try:
 			token = totp(key=entryTotp.key,
 				     nrDigits=entryTotp.digits,
 				     hmacHash=entryTotp.hmacHash)
 		except OtpError as e:
-			self.__err("totp", "Failed to generate TOTP: %s" % str(e))
-		self.__info(None, "%s" % token)
+			self._err("totp", "Failed to generate TOTP: %s" % str(e))
+		self._info(None, "%s" % token)
 	do_t = do_totp
 
 	complete_totp = __complete_category_title
 	complete_t = complete_totp
 
 	def do_edit_totp(self, params):
 		"""--- Edit TOTP key and parameters ---
-		Command: edit_totp category title [KEY] [DIGITS] [HASH]\n
+		Command: edit_totp category title [KEY] [DIGITS] [HASH]
+
 		Set Time-Based One-Time Password Algorithm key and parameters.
 		If KEY is not provided, the TOTP parameters for this entry are deleted.
 		DIGITS default to 6, if not provided.
-		HASH defaults to SHA1, if not provided.\n
-		Aliases: et"""
-		category, title, key, digits, _hash = self._getParams(params, 0, 5)
+		HASH defaults to SHA1, if not provided.
+
+		Aliases: et
+		"""
+		category, title, key, digits, _hash = PWManOpts.parseParams(params, 0, 5)
 		if not category:
-			self.__err("edit_totp", "Category parameter is required.")
+			self._err("edit_totp", "Category parameter is required.")
 		if not title:
-			self.__err("edit_totp", "Title parameter is required.")
+			self._err("edit_totp", "Title parameter is required.")
 		entry = self.__db.getEntry(category, title)
 		if not entry:
-			self.__err("edit_totp", "'%s/%s' not found" % (category, title))
+			self._err("edit_totp", "'%s/%s' not found" % (category, title))
 		entryTotp = self.__db.getEntryTotp(entry)
 		if not entryTotp:
 			entryTotp = PWManEntryTOTP(key=None, entry=entry)
-		origEntryTotp = deepcopy(entryTotp)
 		entryTotp.key = key
 		if digits:
 			try:
 				entryTotp.digits = int(digits)
 			except ValueError:
-				self.__err("edit_totp", "Invalid digits parameter.")
+				self._err("edit_totp", "Invalid digits parameter.")
 		if _hash:
 			entryTotp.hmacHash = _hash
+		try:
+			# Check parameters.
+			totp(key=entryTotp.key,
+			     nrDigits=entryTotp.digits,
+			     hmacHash=entryTotp.hmacHash)
+		except OtpError as e:
+			self._err("edit_totp", "TOTP error: %s" % str(e))
 		self.__db.setEntryTotp(entryTotp)
-		self.__undo.do("edit_totp %s" % params,
-			       "edit_totp %s %s %s %s %s" % (
-			       escapeCmd(category),
-			       escapeCmd(title),
-			       escapeCmd(origEntryTotp.key or ""),
-			       escapeCmd(("%d" % origEntryTotp.digits) if origEntryTotp.digits else ""),
-			       escapeCmd(origEntryTotp.hmacHash or "")))
 	do_et = do_edit_totp
 
 	@completion
 	def complete_edit_totp(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx in (0, 1):
 			return self.__complete_category_title(text, line, begidx, endidx)
-		category, title = self._getComplParams(line, 0, 2)
+		category, title = PWManOpts.parseComplParams(line, 0, 2)
 		if category and title:
 			entry = self.__db.getEntry(category, title)
 			if entry:
 				entryTotp = self.__db.getEntryTotp(entry)
 				if entryTotp:
 					if paramIdx == 2: # key
 						return [ escapeCmd(entryTotp.key) + " " ]
@@ -1031,333 +1558,128 @@
 					elif paramIdx == 4: # hash
 						return [ escapeCmd(entryTotp.hmacHash) + " " ]
 		return []
 	complete_et = complete_edit_totp
 
 	def do_edit_attr(self, params):
 		"""--- Edit an entry attribute ---
-		Command: edit_attr category title NAME [DATA]\n
-		Edit or delete an entry attribute.\n
-		Aliases: ea"""
-		category, title, name, data = self._getParams(params, 0, 4)
+		Command: edit_attr category title NAME [DATA]
+
+		Edit or delete an entry attribute.
+
+		Aliases: ea
+		"""
+		category, title, name, data = PWManOpts.parseParams(params, 0, 4)
 		if not category:
-			self.__err("edit_attr", "Category parameter is required.")
+			self._err("edit_attr", "Category parameter is required.")
 		if not title:
-			self.__err("edit_attr", "Title parameter is required.")
+			self._err("edit_attr", "Title parameter is required.")
 		entry = self.__db.getEntry(category, title)
 		if not entry:
-			self.__err("edit_attr", "'%s/%s' not found" % (category, title))
+			self._err("edit_attr", "'%s/%s' not found" % (category, title))
 		entryAttr = self.__db.getEntryAttr(entry, name)
 		if not entryAttr:
 			entryAttr = PWManEntryAttr(name=name, entry=entry)
-		origEntryAttr = deepcopy(entryAttr)
 		entryAttr.data = data
 		self.__db.setEntryAttr(entryAttr)
-		self.__undo.do("edit_attr %s" % params,
-			       "edit_attr %s %s %s %s" % (
-			       escapeCmd(category),
-			       escapeCmd(title),
-			       escapeCmd(origEntryAttr.name or ""),
-			       escapeCmd(origEntryAttr.data or "")))
 	do_ea = do_edit_attr
 
 	@completion
 	def complete_edit_attr(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
+		paramIdx = PWManOpts.calcParamIndex(line, endidx)
 		if paramIdx in (0, 1):
 			return self.__complete_category_title(text, line, begidx, endidx)
-		category, title, name = self._getComplParams(line, 0, 3)
+		category, title, name = PWManOpts.parseComplParams(line, 0, 3)
 		return self.__getEntryAttrCompletions(category, title, name,
 						      doName=(paramIdx == 2),
 						      doData=(paramIdx == 3),
 						      text=text)
 	complete_ea = complete_edit_attr
 
 	__diff_opts = ("-u", "-c", "-n")
 	def do_diff(self, params):
 		"""--- Diff the current database to another database ---
-		Command: diff [OPTS] [DATABASE_FILE]\n
+		Command: diff [OPTS] [DATABASE_FILE]
+
 		If no DATABASE_FILE is provided: Diffs the latest changes in the
 		currently open database to the committed changes in the current database.
-		This can be used to review changes before commit.\n
+		This can be used to review changes before commit.
+
 		If DATABASE_FILE is provided: Diffs the latest changes in the
-		currently opened database to the contents of DATABASE_FILE.\n
+		currently opened database to the contents of DATABASE_FILE.
+
 		OPTS may be one of:
 		-u  Generate a unified diff (default if no OPT is given).
 		-c  Generate a context diff
-		-n  Generate an ndiff\n
-		Aliases: None"""
-		opts = self._getOpts(params, self.__diff_opts)
+		-n  Generate an ndiff
+
+		Aliases: None
+		"""
+		opts = PWManOpts.parse(params, self.__diff_opts)
 		if opts.nrParams > 1:
-			self.__err("diff", "Too many arguments.")
+			self._err("diff", "Too many arguments.")
 		optUnified = "-u" in opts
 		optContext = "-c" in opts
 		optNdiff = "-n" in opts
 		numFmtOpts = int(optUnified) + int(optContext) + int(optNdiff)
 		if not 0 <= numFmtOpts <= 1:
-			self.__err("diff", "Multiple format OPTions. "
+			self._err("diff", "Multiple format OPTions. "
 					   "Only one is allowed.")
 		if numFmtOpts == 0:
 			optUnified = True
-		dbFile = opts.getParam(0) if opts.nrParams > 0 else None
+		dbFile = opts.getParam(0)
 		try:
 			if dbFile:
 				path = pathlib.Path(dbFile)
 				if not path.exists():
-					self.__err("diff", "'%s' does not exist." % dbFile)
+					self._err("diff", "'%s' does not exist." % path)
 				passphrase = readPassphrase(
-						"Master passphrase of '%s'" % dbFile,
-						verify=False)
+					"Master passphrase of '%s'" % path,
+					verify=False)
 				if passphrase is None:
-					self.__err("diff", "Could not get passphrase.")
+					self._err("diff", "Could not get passphrase.")
 				oldDb = PWManDatabase(filename=path,
 						      passphrase=passphrase,
 						      readOnly=True)
 			else:
 				oldDb = self.__db.getOnDiskDb()
 			diff = PWManDatabaseDiff(db=self.__db, oldDb=oldDb)
 			if optUnified:
 				diffText = diff.getUnifiedDiff()
 			elif optContext:
 				diffText = diff.getContextDiff()
 			elif optNdiff:
 				diffText = diff.getNdiffDiff()
 			else:
 				assert(0)
-			self.__info(None, diffText)
+			self._info(None, diffText)
 		except PWManError as e:
-			self.__err("diff", "Failed: %s" % str(e))
+			self._err("diff", "Failed: %s" % str(e))
 
 	@completion
 	def complete_diff(self, text, line, begidx, endidx):
-		paramIdx = self._calcParamIndex(line, endidx)
 		if text == "-":
-			return self.__diff_opts
-		opts = self._getOpts(line, self.__diff_opts, ignoreFirst=True)
-		optName, value = opts.atCmdIndex(paramIdx)
-		if optName: # -... option
+			return PWManOpts.rawOptTemplates(self.__diff_opts)
+		if len(text) == 2 and text.startswith("-"):
 			return [ text + " " ]
-		if (opts.nrParams == 0 and not text) or (opts.nrParams == 1 and text): # trailing param
+		opts = PWManOpts.parse(line, self.__diff_opts, ignoreFirst=True, softFail=True)
+		if opts.error:
+			return []
+		paramIdx = opts.getComplParamIdx(text)
+		if paramIdx == 0:
+			# database file path
 			return self.__getPathCompletions(text)
 		return []
 
-	def do_undo(self, params):
-		"""--- Undo the last command ---
-		Command: undo\n
-		Rewinds the last command that changed the database.\n
-		Aliases: None"""
-		cmd = self.__undo.undo()
-		if not cmd:
-			self.__err("undo", "There is no command to be undone.")
-		self.__undo.freeze()
-		try:
-			for undoCommand in cmd.undoCommands:
-				self.onecmd(undoCommand)
-		finally:
-			self.__undo.thaw()
-		self.__info("undo",
-			    "\n    " + "\n    ".join(cmd.doCommands) +
-			    "\nsuccessfully undone with:\n" +
-			    "    " + "\n    ".join(cmd.undoCommands))
-
-	def do_redo(self, params):
-		"""--- Redo the last undone command ---
-		Command: redo\n
-		Redoes the last undone command.
-		Also see 'undo' help.\n
-		Aliases: None"""
-		cmd = self.__undo.redo()
-		if not cmd:
-			self.__err("redo", "There is no undone command to be redone.")
-		self.__undo.freeze()
-		try:
-			for doCommand in cmd.doCommands:
-				self.onecmd(doCommand)
-		finally:
-			self.__undo.thaw()
-		self.__info("redo",
-			    "\n    " + "\n    ".join(cmd.undoCommands) +
-			    "\nsuccessfully redone with:\n" +
-			    "    " + "\n    ".join(cmd.doCommands))
-
-	def _skipParams(self, line, count,
-			 lineIncludesCommand=False, unescape=True):
-		# Return a parameter string with the first 'count'
-		# parameters skipped.
-		sline = self._patchSpaceEscapes(line)
-		if lineIncludesCommand:
-			count += 1
-		i = 0
-		while i < len(sline) and count > 0:
-			while i < len(sline) and not sline[i].isspace():
-				i += 1
-			while i < len(sline) and sline[i].isspace():
-				i += 1
-			count -= 1
-		if i >= len(sline):
-			return ""
-		s = line[i:]
-		if unescape:
-			s = unescapeCmd(s)
-		return s
-
-	def _calcParamIndex(self, line, endidx):
-		# Returns the parameter index into the commandline
-		# given the character end-index. This honors space-escape.
-		line = self._patchSpaceEscapes(line)
-		startidx = endidx - 1
-		while startidx > 0 and not line[startidx].isspace():
-			startidx -= 1
-		return len([l for l in line[:startidx].split() if l]) - 1
-
-	def _patchSpaceEscapes(self, line):
-		# Patch a commandline for simple whitespace based splitting.
-		# We just replace the space escape sequence by a random
-		# non-whitespace string. The line remains the same size.
-		return line.replace('\\ ', '_S')
-
-	def _getParam(self, line, paramIndex,
-		       ignoreFirst=False, unescape=True):
-		"""Returns the full parameter from the commandline.
-		"""
-		sline = self._patchSpaceEscapes(line)
-		if ignoreFirst:
-			paramIndex += 1
-		inParam = False
-		idx = 0
-		for startIndex, c in enumerate(sline):
-			if c.isspace():
-				if inParam:
-					idx += 1
-				inParam = False
-			else:
-				inParam = True
-				if idx == paramIndex:
-					break
-		else:
-			return ""
-		endIndex = startIndex
-		while endIndex < len(sline) and not sline[endIndex].isspace():
-			endIndex += 1
-		p = line[startIndex : endIndex]
-		if unescape:
-			p = unescapeCmd(p)
-		return p
-
-	def _getComplParam(self, line, paramIndex, unescape=True):
-		return self._getParam(line, paramIndex,
-				      ignoreFirst=True, unescape=unescape)
-
-	def _getParams(self, line, paramIndex, count,
-		       ignoreFirst=False, unescape=True):
-		"""Returns a generator of the specified parameters from the commandline.
-		paramIndex: start index.
-		count: Number of paramerts to fetch.
-		"""
-		return ( self._getParam(line, i, ignoreFirst, unescape)
-			 for i in range(paramIndex, paramIndex + count) )
-
-	def _getComplParams(self, line, paramIndex, count, unescape=True):
-		return self._getParams(line, paramIndex, count,
-				       ignoreFirst=True, unescape=unescape)
-
-	@dataclass
-	class Opts:
-		__opts : list = field(default_factory=list)
-		__params : list = field(default_factory=list)
-		__atCmdIndex : dict = field(default_factory=dict)
-
-		def _appendOpt(self, cmdIndex, optName, optValue=None):
-			self.__opts.append( (optName, optValue) )
-			self.__atCmdIndex[cmdIndex] = (optName, optValue)
-
-		def _appendParam(self, cmdIndex, param):
-			self.__params.append(param)
-			self.__atCmdIndex[cmdIndex] = (None, param)
-
-		def __contains__(self, optName):
-			"""Check if we have a specific "-X" style option.
-			"""
-			return optName in (o[0] for o in self.__opts)
-
-		@property
-		def hasOpts(self):
-			"""Do we have -X style options?
-			"""
-			return bool(self.__opts)
-
-		def getOpt(self, optName):
-			"""Get an option value by "-X" style name.
-			"""
-			if optName in self:
-				return [ o[1] for o in self.__opts if o[0] == optName ][-1]
-			return None
-
-		@property
-		def nrParams(self):
-			"""The number of trailing parameters.
-			"""
-			return len(self.__params)
-
-		def getParam(self, index):
-			"""Get a trailing parameter at index.
-			"""
-			return self.__params[index]
-
-		def atCmdIndex(self, cmdIndex):
-			"""Get an item (option or parameter) at command line index cmdIndex.
-			Returns (optName, optValue) if it is an option.
-			Returns (None, parameter) if it is a parameter.
-			Returns (None, None) if it does not exist.
-			"""
-			return self.__atCmdIndex.get(cmdIndex, (None, None))
-
-	def _getOpts(self, line, possibleOpts,
-		     ignoreFirst=False, unescape=True):
-		"""Parses the command options in 'line' and returns an Opts instance.
-		possibleOpts is a tuple of the possible options.
-		"""
-		possibleOptsPlain = [ o.replace(":", "") for o in possibleOpts ]
-		opts = self.Opts()
-		i = 0
-		while True:
-			p = self._getParam(line, i,
-					   ignoreFirst=ignoreFirst,
-					   unescape=unescape)
-			if not p:
-				break
-			if opts.nrParams:
-				opts._appendParam(i, p)
-			else:
-				try:
-					optIdx = possibleOptsPlain.index(p)
-				except ValueError:
-					opts._appendParam(i, p)
-					i += 1
-					continue
-				if possibleOpts[optIdx].endswith(":"):
-					i += 1
-					arg = self._getParam(line, i,
-							     ignoreFirst=ignoreFirst,
-							     unescape=unescape)
-					if not arg:
-						self.__err(None, "Option '%s' "
-							   "requires an argument." % p)
-					opts._appendOpt(i, p, arg)
-				else:
-					opts._appendOpt(i, p)
-			i += 1
-		return opts
-
 	def __mayQuit(self):
 		if self.__db.isDirty():
-			self.__warn(None,
-				    "Warning: Uncommitted changes. Operation not performed.\n"
-				    "Use command 'commit' to write the changes to the database.\n"
-				    "Use command 'quit!' to quit without saving.")
+			self._warn(None,
+				   "Warning: Uncommitted changes. Operation not performed.\n"
+				   "Use command 'commit' to write the changes to the database.\n"
+				   "Use command 'quit!' to quit without saving.")
 			return False
 		return True
 
 	def flunkDirty(self):
 		self.__db.flunkDirty()
 
 	def interactive(self):
@@ -1368,21 +1690,21 @@
 					self.cmdloop()
 					break
 				except self.Quit as e:
 					if self.__mayQuit():
 						self.do_cls("")
 						break
 				except EscapeError as e:
-					self.__warn(None, str(e))
+					self._warn(None, str(e))
 				except self.CommandError as e:
 					print(str(e), file=sys.stderr)
 				except (KeyboardInterrupt, EOFError) as e:
 					print("")
 				except CSQLError as e:
-					self.__warn(None, "SQL error: %s" % str(e))
+					self._warn(None, "SQL error: %s" % str(e))
 		finally:
 			self.__isInteractive = False
 
 	def runOneCommand(self, command):
 		self.__isInteractive = False
 		try:
 			self.onecmd(command)
```

### Comparing `pwman-python-2.7/libpwman/util.py` & `pwman-python-2.8/libpwman/util.py`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/maintenance/gen-doc.sh` & `pwman-python-2.8/maintenance/gen-doc.sh`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/maintenance/win-install-dependencies.cmd` & `pwman-python-2.8/maintenance/win-install-dependencies.cmd`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/maintenance/win-standalone-build.cmd` & `pwman-python-2.8/maintenance/win-standalone-build.cmd`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/pwman.cmd` & `pwman-python-2.8/pwman.cmd`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/pwman_python.egg-info/PKG-INFO` & `pwman-python-2.8/pwman_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwman-python
-Version: 2.7
+Version: 2.8
 Summary: Commandline password manager
 Home-page: https://bues.ch/h/pwman
 Author: Michael Büsch
 Author-email: m@bues.ch
 Keywords: password manager command line TOTP 2FA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pwman-python-2.7/pwman_python.egg-info/SOURCES.txt` & `pwman-python-2.8/pwman_python.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 doc/api/libpwman/database.html
 doc/api/libpwman/dbdiff.html
 doc/api/libpwman/exception.html
 doc/api/libpwman/fileobj.html
 doc/api/libpwman/mlock.html
 doc/api/libpwman/otp.html
 doc/api/libpwman/ui.html
-doc/api/libpwman/undo.html
+doc/api/libpwman/ui_escape.html
 doc/api/libpwman/util.html
 doc/api/libpwman/version.html
 doc/foreign-licenses/PYTHON-LICENSE.txt
 doc/foreign-licenses/README
 libpwman/__init__.py
 libpwman/__main__.py
 libpwman/aes.py
@@ -30,15 +30,15 @@
 libpwman/database.py
 libpwman/dbdiff.py
 libpwman/exception.py
 libpwman/fileobj.py
 libpwman/mlock.py
 libpwman/otp.py
 libpwman/ui.py
-libpwman/undo.py
+libpwman/ui_escape.py
 libpwman/util.py
 libpwman/version.py
 maintenance/cleantree.sh
 maintenance/deb-dependencies-install.sh
 maintenance/gen-doc.sh
 maintenance/win-install-dependencies.cmd
 maintenance/win-standalone-build.cmd
```

### Comparing `pwman-python-2.7/setup.py` & `pwman-python-2.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,27 +3,23 @@
 
 from setuptools import setup
 try:
 	from cx_Freeze import setup, Executable
 	cx_Freeze = True
 except ImportError:
 	cx_Freeze = False
-import warnings
 import os
 import sys
 
 from libpwman import __version__
 
 basedir = os.path.abspath(os.path.dirname(__file__))
 for base in (os.getcwd(), basedir):
 	sys.path.insert(0, base)
 
-isWindows = os.name.lower() in {"nt", "ce"}
-isPosix = os.name.lower() == "posix"
-
 # Create freeze executable list.
 extraKeywords = {}
 if cx_Freeze:
 	extraKeywords["executables"] = [ Executable(script="pwman") ]
 	extraKeywords["options"] = {
 		"build_exe" : {
 			"packages" : [ "readline",
@@ -32,18 +28,14 @@
 				       "_curses",
 				       "sqlite3",
 				       "sqlite3.dump", ],
 			"excludes" : [ "tkinter", ],
 		}
 	}
 
-warnings.filterwarnings("ignore", r".*'python_requires'.*")
-warnings.filterwarnings("ignore", r".*'install_requires'.*")
-warnings.filterwarnings("ignore", r".*'long_description_content_type'.*")
-
 with open(os.path.join(basedir, "README.rst"), "rb") as fd:
 	readmeText = fd.read().decode("UTF-8")
 
 setup(
 	name		= "pwman-python",
 	version		= __version__,
 	description	= "Commandline password manager",
```

### Comparing `pwman-python-2.7/tests/run.sh` & `pwman-python-2.8/tests/run.sh`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	(
 		echo
 		echo "==="
 		echo "= Running $interpreter, PWMAN_CRYPTOLIB=\"$PWMAN_CRYPTOLIB\""
 		echo "==="
 		export PYTHONPATH="$rootdir/tests:$PYTHONPATH"
 		cd "$rootdir" || die "Failed to cd to rootdir."
-		"$interpreter" -m unittest --failfast --buffer --catch "$test_dir" ||\
+		"$interpreter" -m unittest --failfast --buffer --catch --verbose "$test_dir" ||\
 			die "Test failed"
 	) || die
 }
 
 # $1=test_dir
 run_testdir()
 {
```

### Comparing `pwman-python-2.7/tests/test_database_v0.db` & `pwman-python-2.8/tests/test_database_v0.db`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/tests/test_database_v0.py` & `pwman-python-2.8/tests/test_database_v0.py`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/tests/test_database_v1.db` & `pwman-python-2.8/tests/test_database_v1.db`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/tests/test_database_v1.py` & `pwman-python-2.8/tests/test_database_v1.py`

 * *Files identical despite different names*

### Comparing `pwman-python-2.7/tests/test_otp.py` & `pwman-python-2.8/tests/test_otp.py`

 * *Files identical despite different names*

