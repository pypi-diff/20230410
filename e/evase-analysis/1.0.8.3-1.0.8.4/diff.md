# Comparing `tmp/evase-analysis-1.0.8.3.tar.gz` & `tmp/evase-analysis-1.0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evase-analysis-1.0.8.3.tar", last modified: Thu Apr  6 19:25:08 2023, max compression
+gzip compressed data, was "evase-analysis-1.0.8.4.tar", last modified: Mon Apr 10 20:18:01 2023, max compression
```

## Comparing `evase-analysis-1.0.8.3.tar` & `evase-analysis-1.0.8.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.860700 evase-analysis-1.0.8.3/
--rw-rw-rw-   0        0        0     7073 2023-04-06 19:25:08.859699 evase-analysis-1.0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     6230 2023-04-04 20:11:33.000000 evase-analysis-1.0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.810588 evase-analysis-1.0.8.3/docs/
--rw-rw-rw-   0        0        0     1166 2023-03-30 01:19:57.000000 evase-analysis-1.0.8.3/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.811591 evase-analysis-1.0.8.3/evase/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/evase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.815587 evase-analysis-1.0.8.3/evase/depanalyze/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/evase/depanalyze/__init__.py
--rw-rw-rw-   0        0        0     9152 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.3/evase/depanalyze/codetraversalnode.py
--rw-rw-rw-   0        0        0    12059 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.3/evase/depanalyze/importresolver.py
--rw-rw-rw-   0        0        0     3829 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.3/evase/depanalyze/scoperesolver.py
--rw-rw-rw-   0        0        0    15873 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.3/evase/depanalyze/searching.py
--rw-rw-rw-   0        0        0     1450 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.3/evase/depanalyze/surfacedetector.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.816588 evase-analysis-1.0.8.3/evase/exceptions/
--rw-rw-rw-   0        0        0        0 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.3/evase/exceptions/__init__.py
--rw-rw-rw-   0        0        0      626 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.3/evase/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.818094 evase-analysis-1.0.8.3/evase/sql_injection/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/evase/sql_injection/__init__.py
--rw-rw-rw-   0        0        0     4242 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/evase/sql_injection/injectionutil.py
--rw-rw-rw-   0        0        0     6537 2023-04-06 16:36:00.000000 evase-analysis-1.0.8.3/evase/sql_injection/injectionvisitor.py
--rw-rw-rw-   0        0        0    10947 2023-04-06 16:39:55.000000 evase-analysis-1.0.8.3/evase/sql_injection/vulnerabletraversal.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.820107 evase-analysis-1.0.8.3/evase/structures/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/evase/structures/__init__.py
--rw-rw-rw-   0        0        0    15131 2023-04-06 17:45:27.000000 evase-analysis-1.0.8.3/evase/structures/analysisperformer.py
--rw-rw-rw-   0        0        0     5410 2023-04-06 16:21:46.000000 evase-analysis-1.0.8.3/evase/structures/modulestructure.py
--rw-rw-rw-   0        0        0     6608 2023-04-06 16:28:41.000000 evase-analysis-1.0.8.3/evase/structures/projectstructure.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.822107 evase-analysis-1.0.8.3/evase/util/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:19:57.000000 evase-analysis-1.0.8.3/evase/util/__init__.py
--rw-rw-rw-   0        0        0     3012 2023-04-06 16:44:37.000000 evase-analysis-1.0.8.3/evase/util/fileutil.py
--rw-rw-rw-   0        0        0     1411 2023-04-06 19:23:47.000000 evase-analysis-1.0.8.3/evase/util/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.837623 evase-analysis-1.0.8.3/evase_analysis.egg-info/
--rw-rw-rw-   0        0        0     7073 2023-04-06 19:25:08.000000 evase-analysis-1.0.8.3/evase_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2685 2023-04-06 19:25:08.000000 evase-analysis-1.0.8.3/evase_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 19:25:08.000000 evase-analysis-1.0.8.3/evase_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-06 19:25:08.000000 evase-analysis-1.0.8.3/evase_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-06 19:25:08.000000 evase-analysis-1.0.8.3/evase_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1345 2023-04-06 19:24:25.000000 evase-analysis-1.0.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 19:25:08.860700 evase-analysis-1.0.8.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.840148 evase-analysis-1.0.8.3/tests/
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.844659 evase-analysis-1.0.8.3/tests/resources/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.807946 evase-analysis-1.0.8.3/tests/resources/demo/
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.848165 evase-analysis-1.0.8.3/tests/resources/demo/backend/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/demo/backend/__init__.py
--rw-rw-rw-   0        0        0     1108 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/demo/backend/app.py
--rw-rw-rw-   0        0        0     1098 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/demo/backend/vul.py
--rw-rw-rw-   0        0        0     1140 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/demo/backend/vul_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.807946 evase-analysis-1.0.8.3/tests/resources/demo2/
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.846660 evase-analysis-1.0.8.3/tests/resources/demo2/demonstration/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/demo2/demonstration/__init__.py
--rw-rw-rw-   0        0        0      185 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/demo2/demonstration/api.py
--rw-rw-rw-   0        0        0      183 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/demo2/demonstration/controller.py
--rw-rw-rw-   0        0        0      458 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/demo2/demonstration/model.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.849172 evase-analysis-1.0.8.3/tests/resources/prjstructtest/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/prjstructtest/__init__.py
--rw-rw-rw-   0        0        0      290 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/prjstructtest/runner.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.850179 evase-analysis-1.0.8.3/tests/resources/prjstructtest/test/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/prjstructtest/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.851181 evase-analysis-1.0.8.3/tests/resources/prjstructtest/util/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/prjstructtest/util/__init__.py
--rw-rw-rw-   0        0        0      163 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/prjstructtest/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.852179 evase-analysis-1.0.8.3/tests/resources/prjstructtest/util/moreutil/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/prjstructtest/util/moreutil/__init__.py
--rw-rw-rw-   0        0        0       79 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/prjstructtest/util/moreutil/helper2.py
--rw-rw-rw-   0        0        0      306 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/screstest.py
--rw-rw-rw-   0        0        0      108 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_safe1.py
--rw-rw-rw-   0        0        0      150 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_safe2.py
--rw-rw-rw-   0        0        0      128 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_vul1.py
--rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_vul2.py
--rw-rw-rw-   0        0        0      130 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_vul3.py
--rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_vul4.py
--rw-rw-rw-   0        0        0      535 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_vul5.py
--rw-rw-rw-   0        0        0     5135 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/sql_injection_vul6.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.854179 evase-analysis-1.0.8.3/tests/resources/type_demo/
--rw-rw-rw-   0        0        0      911 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/type_demo/app.py
--rw-rw-rw-   0        0        0      280 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/type_demo/create_db.py
--rw-rw-rw-   0        0        0      759 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/type_demo/user_db_handler.py
--rw-rw-rw-   0        0        0      700 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/type_demo/vul.py
--rw-rw-rw-   0        0        0      732 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.3/tests/resources/type_demo/vul_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.809588 evase-analysis-1.0.8.3/tests/resources/webgoat/
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.857685 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/
--rw-rw-rw-   0        0        0     1534 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/__init__.py
--rw-rw-rw-   0        0        0     2063 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/actions.py
--rw-rw-rw-   0        0        0     1633 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/auth.py
--rw-rw-rw-   0        0        0      232 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/status.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:25:08.859699 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/templates/
--rw-rw-rw-   0        0        0       89 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/templates/__init__.py
--rw-rw-rw-   0        0        0       32 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/templates/hello.py
--rw-rw-rw-   0        0        0       77 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/templates/helper.py
--rw-rw-rw-   0        0        0      850 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/ui.py
--rw-rw-rw-   0        0        0     1488 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/users.py
--rw-rw-rw-   0        0        0     2026 2023-04-06 19:23:32.000000 evase-analysis-1.0.8.3/tests/test_analysisperformer.py
--rw-rw-rw-   0        0        0     2593 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.3/tests/test_fileutil.py
--rw-rw-rw-   0        0        0     1618 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.3/tests/test_projectstructure.py
--rw-rw-rw-   0        0        0     1639 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.3/tests/test_scoperesolver.py
--rw-rw-rw-   0        0        0     1714 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.3/tests/testutil.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.534396 evase-analysis-1.0.8.4/
+-rw-rw-rw-   0        0        0     7073 2023-04-10 20:18:01.534396 evase-analysis-1.0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6230 2023-04-04 20:11:33.000000 evase-analysis-1.0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.466239 evase-analysis-1.0.8.4/docs/
+-rw-rw-rw-   0        0        0     1166 2023-04-10 18:09:48.000000 evase-analysis-1.0.8.4/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.467240 evase-analysis-1.0.8.4/evase/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.471239 evase-analysis-1.0.8.4/evase/depanalyze/
+-rw-rw-rw-   0        0        0        0 2023-04-10 01:10:48.000000 evase-analysis-1.0.8.4/evase/depanalyze/__init__.py
+-rw-rw-rw-   0        0        0     9152 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/codetraversalnode.py
+-rw-rw-rw-   0        0        0    12059 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/importresolver.py
+-rw-rw-rw-   0        0        0     3829 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/scoperesolver.py
+-rw-rw-rw-   0        0        0    15873 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/searching.py
+-rw-rw-rw-   0        0        0     1450 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/surfacedetector.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.471745 evase-analysis-1.0.8.4/evase/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.473758 evase-analysis-1.0.8.4/evase/sql_injection/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/sql_injection/__init__.py
+-rw-rw-rw-   0        0        0     4242 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/sql_injection/injectionutil.py
+-rw-rw-rw-   0        0        0     6537 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.4/evase/sql_injection/injectionvisitor.py
+-rw-rw-rw-   0        0        0    10947 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.4/evase/sql_injection/vulnerabletraversal.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.475758 evase-analysis-1.0.8.4/evase/structures/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/structures/__init__.py
+-rw-rw-rw-   0        0        0    14911 2023-04-10 20:13:56.000000 evase-analysis-1.0.8.4/evase/structures/analysisperformer.py
+-rw-rw-rw-   0        0        0     5410 2023-04-10 18:09:51.000000 evase-analysis-1.0.8.4/evase/structures/modulestructure.py
+-rw-rw-rw-   0        0        0     6608 2023-04-10 18:09:51.000000 evase-analysis-1.0.8.4/evase/structures/projectstructure.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.477758 evase-analysis-1.0.8.4/evase/util/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:19:57.000000 evase-analysis-1.0.8.4/evase/util/__init__.py
+-rw-rw-rw-   0        0        0     3012 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.4/evase/util/fileutil.py
+-rw-rw-rw-   0        0        0     1411 2023-04-06 19:27:20.000000 evase-analysis-1.0.8.4/evase/util/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.492798 evase-analysis-1.0.8.4/evase_analysis.egg-info/
+-rw-rw-rw-   0        0        0     7073 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2685 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1345 2023-04-10 20:15:15.000000 evase-analysis-1.0.8.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 20:18:01.534396 evase-analysis-1.0.8.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.513347 evase-analysis-1.0.8.4/tests/
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.518356 evase-analysis-1.0.8.4/tests/resources/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.463231 evase-analysis-1.0.8.4/tests/resources/demo/
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.521860 evase-analysis-1.0.8.4/tests/resources/demo/backend/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/__init__.py
+-rw-rw-rw-   0        0        0     1108 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/app.py
+-rw-rw-rw-   0        0        0     1098 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/vul.py
+-rw-rw-rw-   0        0        0     1140 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/vul_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.462231 evase-analysis-1.0.8.4/tests/resources/demo2/
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.520355 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/api.py
+-rw-rw-rw-   0        0        0      183 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/controller.py
+-rw-rw-rw-   0        0        0      458 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/model.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.522869 evase-analysis-1.0.8.4/tests/resources/prjstructtest/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/__init__.py
+-rw-rw-rw-   0        0        0      290 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/runner.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.523877 evase-analysis-1.0.8.4/tests/resources/prjstructtest/test/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.524875 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.525876 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/moreutil/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/moreutil/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/moreutil/helper2.py
+-rw-rw-rw-   0        0        0      306 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/screstest.py
+-rw-rw-rw-   0        0        0      108 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_safe1.py
+-rw-rw-rw-   0        0        0      150 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_safe2.py
+-rw-rw-rw-   0        0        0      128 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul1.py
+-rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul2.py
+-rw-rw-rw-   0        0        0      130 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul3.py
+-rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul4.py
+-rw-rw-rw-   0        0        0      535 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul5.py
+-rw-rw-rw-   0        0        0     5135 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul6.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.527876 evase-analysis-1.0.8.4/tests/resources/type_demo/
+-rw-rw-rw-   0        0        0      911 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/app.py
+-rw-rw-rw-   0        0        0      280 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/create_db.py
+-rw-rw-rw-   0        0        0      759 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/user_db_handler.py
+-rw-rw-rw-   0        0        0      700 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/vul.py
+-rw-rw-rw-   0        0        0      732 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/vul_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.464237 evase-analysis-1.0.8.4/tests/resources/webgoat/
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.532391 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/
+-rw-rw-rw-   0        0        0     1534 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/__init__.py
+-rw-rw-rw-   0        0        0     2063 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/actions.py
+-rw-rw-rw-   0        0        0     1633 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/auth.py
+-rw-rw-rw-   0        0        0      232 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/status.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.533390 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/
+-rw-rw-rw-   0        0        0       89 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/hello.py
+-rw-rw-rw-   0        0        0       77 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/helper.py
+-rw-rw-rw-   0        0        0      850 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/ui.py
+-rw-rw-rw-   0        0        0     1488 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/users.py
+-rw-rw-rw-   0        0        0     2172 2023-04-10 20:14:52.000000 evase-analysis-1.0.8.4/tests/test_analysisperformer.py
+-rw-rw-rw-   0        0        0     2593 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/test_fileutil.py
+-rw-rw-rw-   0        0        0     1618 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/test_projectstructure.py
+-rw-rw-rw-   0        0        0     1639 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/test_scoperesolver.py
+-rw-rw-rw-   0        0        0     1714 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/testutil.py
```

### Comparing `evase-analysis-1.0.8.3/PKG-INFO` & `evase-analysis-1.0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evase-analysis
-Version: 1.0.8.3
+Version: 1.0.8.4
 Summary: A Python package with tools for the detection of SQL injection vulnerabilities in projects.
 Author-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Maintainer-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Keywords: attack,security,SQL,injection
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `evase-analysis-1.0.8.3/README.md` & `evase-analysis-1.0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/docs/conf.py` & `evase-analysis-1.0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/depanalyze/codetraversalnode.py` & `evase-analysis-1.0.8.4/evase/depanalyze/codetraversalnode.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/depanalyze/importresolver.py` & `evase-analysis-1.0.8.4/evase/depanalyze/importresolver.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/depanalyze/scoperesolver.py` & `evase-analysis-1.0.8.4/evase/depanalyze/scoperesolver.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/depanalyze/searching.py` & `evase-analysis-1.0.8.4/evase/depanalyze/searching.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/depanalyze/surfacedetector.py` & `evase-analysis-1.0.8.4/evase/depanalyze/surfacedetector.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/exceptions/exceptions.py` & `evase-analysis-1.0.8.4/evase/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/sql_injection/injectionutil.py` & `evase-analysis-1.0.8.4/evase/sql_injection/injectionutil.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/sql_injection/injectionvisitor.py` & `evase-analysis-1.0.8.4/evase/sql_injection/injectionvisitor.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/sql_injection/vulnerabletraversal.py` & `evase-analysis-1.0.8.4/evase/sql_injection/vulnerabletraversal.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/structures/analysisperformer.py` & `evase-analysis-1.0.8.4/evase/structures/analysisperformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,72 +71,58 @@
 }
 
 
 class BehaviourAnalyzer(ABC):
 
     def __init__(
             self,
-            project_struct: ProjectAnalysisStruct = None,
-            executor=None
+            project_struct: ProjectAnalysisStruct = None
     ):
         """
         An abstract class of an analyzer that detects specific attack behaviours within a project.
 
         :param project_struct: The project structure to analyze
-        :param executor: The execution function to run for analysis
         """
 
-        self.project_struct = project_struct
-        self.analysis_results = dict(vulnerabilities=[], found_any=False)
-        self.executor = executor
+        self._project_struct = project_struct
+        self._analysis_results = dict()
 
-    def get_project_struct(self) -> ProjectAnalysisStruct:
+    @property
+    def analysis_results(self) -> Dict:
         """
-        Retrieve the project analysis structure.
+        Retrieve the analysis result of the analyzer.
 
-        :return: The analysis structure being analyzed
+        :return: The mapping of analysis results
         """
-        return self.project_struct
+        return self._analysis_results
 
-    def get_analysis_results(self) -> Dict:
+    @property
+    def project_struct(self) -> ProjectAnalysisStruct:
         """
-        Retrieve the analysis result of the analyzer.
+        Retrieve the project analysis structure.
 
-        :return: The mapping of analysis results
+        :return: The analysis structure being analyzed
         """
+        return self._project_struct
 
-        return self.analysis_results
-
-    def set_project_struct(self, project_struct: ProjectAnalysisStruct):
+    @project_struct.setter
+    def project_struct(self, project_struct: ProjectAnalysisStruct):
         """
         Set the project structure to analyze.
 
         :param project_struct: The project structure to analyze
         """
 
-        self.project_struct = project_struct
-
-    def set_executor(self, executor):
-        """
-        Set the executor function of this analyzer.
-
-        :param executor: The executor function.
-        """
-        self.executor = executor
+        self._project_struct = project_struct
 
     @abstractmethod
     def do_analysis(self):
         """
         Abstract method to do the analysis and output a result.
         """
-
-        if self.project_struct is None:
-            raise ValueError("Project structure needs to be set before performing analysis.")
-        if self.executor is None:
-            raise ValueError("An executor function needs to be set before performing analysis.")
         pass
 
 
 class SQLInjectionBehaviourAnalyzer(BehaviourAnalyzer):
 
     def __init__(self, project_struct: ProjectAnalysisStruct = None):
         """
@@ -153,18 +139,17 @@
         :return: A dictionary of the analysis results
         """
         for m_name, m_struct in self.project_struct.structure.items():
             visitor = InjectionNodeVisitor(self.project_struct, m_name)
             visitor.visit(m_struct.tree)
             results = visitor.vulnerable_funcs
             if len(results) > 0:
-                self.analysis_results['found_any'] = True
-                self.analysis_results['graph'] = results
+                self._analysis_results = results
 
-        return self.analysis_results
+        return self._analysis_results
 
 
 class AnalysisPerformer:
 
     def __init__(
             self,
             project_name: str = None,
@@ -185,30 +170,48 @@
             print("HERE")
             output_path = check_path(output_path, file_ok=False, file_req=False, absolute_req=False, ret_absolute=True)
             AnalysisLogger.log_path = Path(output_path, 'analysis-log.log')
             print(output_path)
 
         self.analysis_results = {}
 
-        self.sql_injection_detector = SQLInjectionBehaviourAnalyzer()
+        self._strategy: BehaviourAnalyzer = None
+
+    @property
+    def strategy(self) -> BehaviourAnalyzer:
+        """
+        Retrieve the strategy that the analysis performer will use to conduct analysis.
+
+        :return: Analysis strategy
+        """
+        return self._strategy
+
+    @strategy.setter
+    def strategy(self, strategy: BehaviourAnalyzer):
+        """
+        Retrieve the strategy that the analysis performer will use to conduct analysis.
+
+        :param strategy: Analysis strategy
+        """
+        self._strategy = strategy
 
     def perform_analysis(self):
         """
         Performs analysis on the code structure that is currently loaded.
         Results are stored in the analysis_results field.
         """
 
         prj_struct = ProjectAnalysisStruct(self.project_name, self.project_root)
         graph, groups = get_mdl_depdigraph(prj_struct)
 
-        if self.sql_injection_detector is not None:
-            self.sql_injection_detector.set_project_struct(prj_struct)
-            sql_injection_results = self.sql_injection_detector.do_analysis()
+        if self._strategy is not None:
+            self._strategy.project_struct = prj_struct
+            analysis_results = self._strategy.do_analysis()
 
-            graph, groups = extend_depgraph_attackvectors(graph, groups, sql_injection_results['graph'])
+            graph, groups = extend_depgraph_attackvectors(graph, groups, analysis_results)
 
             graph_data = nx.node_link_data(graph, source='from', target='to', link='edges')
 
             self.analysis_results['graph'] = {}
             self.analysis_results['graph']['total'] = graph_data
 
     def get_results(self):
```

### Comparing `evase-analysis-1.0.8.3/evase/structures/modulestructure.py` & `evase-analysis-1.0.8.4/evase/structures/modulestructure.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/structures/projectstructure.py` & `evase-analysis-1.0.8.4/evase/structures/projectstructure.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/util/fileutil.py` & `evase-analysis-1.0.8.4/evase/util/fileutil.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase/util/logger.py` & `evase-analysis-1.0.8.4/evase/util/logger.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/evase_analysis.egg-info/PKG-INFO` & `evase-analysis-1.0.8.4/evase_analysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evase-analysis
-Version: 1.0.8.3
+Version: 1.0.8.4
 Summary: A Python package with tools for the detection of SQL injection vulnerabilities in projects.
 Author-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Maintainer-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Keywords: attack,security,SQL,injection
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `evase-analysis-1.0.8.3/evase_analysis.egg-info/SOURCES.txt` & `evase-analysis-1.0.8.4/evase_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/pyproject.toml` & `evase-analysis-1.0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     {name = "Shaopeng Liu", email="shaopengliu@cmail.carleton.ca"},
     {name = "Jason Jaskolka", email="jason.jaskolka@carleton.ca"}
 ]
 description = "A Python package with tools for the detection of SQL injection vulnerabilities in projects."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["attack", "security", "SQL", "injection"]
-version="1.0.8.3"
+version="1.0.8.4"
 classifiers=[
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3"
 ]
 dependencies = [
     'Flask~=2.2.2',
     'Jinja2~=3.1.2',
```

### Comparing `evase-analysis-1.0.8.3/tests/resources/demo/backend/app.py` & `evase-analysis-1.0.8.4/tests/resources/demo/backend/app.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/demo/backend/vul.py` & `evase-analysis-1.0.8.4/tests/resources/demo/backend/vul.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/demo/backend/vul_wrapper.py` & `evase-analysis-1.0.8.4/tests/resources/demo/backend/vul_wrapper.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/sql_injection_vul5.py` & `evase-analysis-1.0.8.4/tests/resources/sql_injection_vul5.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/sql_injection_vul6.py` & `evase-analysis-1.0.8.4/tests/resources/sql_injection_vul6.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/type_demo/app.py` & `evase-analysis-1.0.8.4/tests/resources/type_demo/app.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/type_demo/user_db_handler.py` & `evase-analysis-1.0.8.4/tests/resources/type_demo/user_db_handler.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/type_demo/vul.py` & `evase-analysis-1.0.8.4/tests/resources/type_demo/vul.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/type_demo/vul_wrapper.py` & `evase-analysis-1.0.8.4/tests/resources/type_demo/vul_wrapper.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/__init__.py` & `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/__init__.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/actions.py` & `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/actions.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/auth.py` & `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/auth.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/ui.py` & `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/ui.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/resources/webgoat/flask_webgoat/users.py` & `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/users.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/test_analysisperformer.py` & `evase-analysis-1.0.8.4/tests/test_analysisperformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         )
 
     def test_dependency_graph(self):
         """
         Tests the ability of the analysis performer to construct the proper graph.
         """
 
+        self.test_struct1.strategy = ap.SQLInjectionBehaviourAnalyzer()
         self.test_struct1.perform_analysis()
         results = self.test_struct1.get_results()
 
         dirpath = Path(prjroot3_filename)
         all_package_names = [name for name, _ in futil.get_project_module_names(dirpath)]
         nodes_present = [x['id'] for x in results['graph']['total']['nodes']]
 
@@ -41,14 +42,15 @@
             all_package_names.remove(exc)
 
         # exclude files when they have no incoming or outgoing dependencies
         self.assertTrue(
             all([x in nodes_present for x in all_package_names])
         )
 
+        self.test_struct2.strategy = ap.SQLInjectionBehaviourAnalyzer()
         self.test_struct2.perform_analysis()
         results = self.test_struct2.get_results()
 
         dirpath = Path(prjroot2_filename)
         all_package_names = [name for name, _ in futil.get_project_module_names(dirpath)]
         nodes_present = [x['id'] for x in results['graph']['total']['nodes']]
```

### Comparing `evase-analysis-1.0.8.3/tests/test_fileutil.py` & `evase-analysis-1.0.8.4/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/test_projectstructure.py` & `evase-analysis-1.0.8.4/tests/test_projectstructure.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/test_scoperesolver.py` & `evase-analysis-1.0.8.4/tests/test_scoperesolver.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.3/tests/testutil.py` & `evase-analysis-1.0.8.4/tests/testutil.py`

 * *Files identical despite different names*

