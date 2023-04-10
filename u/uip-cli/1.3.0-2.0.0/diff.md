# Comparing `tmp/uip-cli-1.3.0.tar.gz` & `tmp/uip-cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\uip-cli-1.3.0.tar", last modified: Mon Oct  3 15:17:08 2022, max compression
+gzip compressed data, was "dist\uip-cli-2.0.0.tar", last modified: Mon Apr 10 12:01:50 2023, max compression
```

## Comparing `uip-cli-1.3.0.tar` & `uip-cli-2.0.0.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/
--rw-rw-rw-   0        0        0    35821 2021-09-30 19:23:27.000000 uip-cli-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      159 2021-09-07 18:15:28.000000 uip-cli-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    27057 2022-10-03 15:17:08.000000 uip-cli-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    20565 2022-06-16 18:04:41.000000 uip-cli-1.3.0/README.rst
--rw-rw-rw-   0        0        0       42 2022-10-03 15:17:08.000000 uip-cli-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1452 2021-10-04 22:33:26.000000 uip-cli-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/cliapis/
--rw-rw-rw-   0        0        0    15499 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/cliapis/apis.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/cliapis/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/cliconfig/
--rw-rw-rw-   0        0        0     3654 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/cliconfig/customformatter.py
--rw-rw-rw-   0        0        0    17836 2022-06-16 18:04:41.000000 uip-cli-1.3.0/uip/cliconfig/setupcli.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/cliconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/config/
--rw-rw-rw-   0        0        0     3511 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/config/config.py
--rw-rw-rw-   0        0        0     3390 2022-06-16 18:04:41.000000 uip-cli-1.3.0/uip/config/configoptions.py
--rw-rw-rw-   0        0        0     3746 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/config/mergeconfig.py
--rw-rw-rw-   0        0        0     6836 2022-03-03 17:44:42.000000 uip-cli-1.3.0/uip/config/uip.yml
--rw-rw-rw-   0        0        0     6312 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/config/verifyconfig.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/config/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/constants/
--rw-rw-rw-   0        0        0     1966 2022-09-26 15:32:31.000000 uip-cli-1.3.0/uip/constants/constants.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/exceptions/
--rw-rw-rw-   0        0        0     4204 2022-02-11 17:58:00.000000 uip-cli-1.3.0/uip/exceptions/customexceptions.py
--rw-rw-rw-   0        0        0     2458 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/exceptions/errormessages.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/exceptions/__init__.py
--rw-rw-rw-   0        0        0      251 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/main.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/parsecli/
--rw-rw-rw-   0        0        0    20394 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/parsecli/parsecli.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/parsecli/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uipproject/
--rw-rw-rw-   0        0        0    17634 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/uipproject/uipproject.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/uipproject/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/
--rw-rw-rw-   0        0        0     2074 2022-03-24 16:21:06.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/extension.py
--rw-rw-rw-   0        0        0      302 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/extension.yml
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/templates/
--rw-rw-rw-   0        0        0     3266 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/templates/template.json
--rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/__init__.py
--rw-rw-rw-   0        0        0     1180 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/template_config.yml
--rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/resources/
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/resources/setupscripts/
--rw-rw-rw-   0        0        0       43 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/uiptemplates/resources/setupscripts/setup.cfg
--rw-rw-rw-   0        0        0     3867 2022-03-02 14:49:03.000000 uip-cli-1.3.0/uip/uiptemplates/resources/setupscripts/setup.py
--rw-rw-rw-   0        0        0        0 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/uiptemplates/resources/setupscripts/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/
--rw-rw-rw-   0        0        0     1599 2022-03-03 17:44:42.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/extension.py
--rw-rw-rw-   0        0        0      297 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/extension.yml
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/templates/
--rw-rw-rw-   0        0        0     3321 2022-03-03 17:44:42.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/templates/template.json
--rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/__init__.py
--rw-rw-rw-   0        0        0     1090 2022-03-03 17:44:42.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/template_config.yml
--rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/__init__.py
--rw-rw-rw-   0        0        0     2718 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/uiptemplates/template.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/uiptemplates/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/uiptemplates/__pycache__/
--rw-rw-rw-   0        0        0     2228 2022-10-03 15:16:43.000000 uip-cli-1.3.0/uip/uiptemplates/__pycache__/template.cpython-36.pyc
--rw-rw-rw-   0        0        0      181 2022-10-03 15:16:43.000000 uip-cli-1.3.0/uip/uiptemplates/__pycache__/__init__.cpython-36.pyc
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip/utils/
--rw-rw-rw-   0        0        0     3615 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/utils/custom_io.py
--rw-rw-rw-   0        0        0     2945 2022-09-22 14:39:23.000000 uip-cli-1.3.0/uip/utils/formatting.py
--rw-rw-rw-   0        0        0      662 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/utils/generic.py
--rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-1.3.0/uip/utils/__init__.py
--rw-rw-rw-   0        0        0       98 2022-09-30 20:20:04.000000 uip-cli-1.3.0/uip/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip_cli.egg-info/
--rw-rw-rw-   0        0        0        1 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    27057 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      141 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1928 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        4 2022-10-03 15:17:08.000000 uip-cli-1.3.0/uip_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2021-09-03 01:31:50.000000 uip-cli-1.3.0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/
+-rw-rw-rw-   0        0        0    35821 2021-09-30 19:23:27.000000 uip-cli-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      159 2021-09-07 18:15:28.000000 uip-cli-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    41370 2023-04-10 12:01:50.000000 uip-cli-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    31971 2023-04-06 20:55:29.000000 uip-cli-2.0.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-10 12:01:50.000000 uip-cli-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1520 2023-04-03 16:22:07.000000 uip-cli-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/cliapis/
+-rw-rw-rw-   0        0        0    15499 2022-09-22 14:39:23.000000 uip-cli-2.0.0/uip/cliapis/apis.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/cliapis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/cliconfig/
+-rw-rw-rw-   0        0        0     3654 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/cliconfig/customformatter.py
+-rw-rw-rw-   0        0        0    26560 2023-04-04 17:20:33.000000 uip-cli-2.0.0/uip/cliconfig/setupcli.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/cliconfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/config/
+-rw-rw-rw-   0        0        0     3532 2023-02-01 17:56:49.000000 uip-cli-2.0.0/uip/config/config.py
+-rw-rw-rw-   0        0        0     4458 2023-03-13 01:56:34.000000 uip-cli-2.0.0/uip/config/configoptions.py
+-rw-rw-rw-   0        0        0     3746 2022-09-22 14:39:23.000000 uip-cli-2.0.0/uip/config/mergeconfig.py
+-rw-rw-rw-   0        0        0     8081 2023-03-13 01:56:34.000000 uip-cli-2.0.0/uip/config/uip.yml
+-rw-rw-rw-   0        0        0     7537 2023-03-13 01:56:34.000000 uip-cli-2.0.0/uip/config/verifyconfig.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/constants/
+-rw-rw-rw-   0        0        0     5626 2023-03-23 14:08:25.000000 uip-cli-2.0.0/uip/constants/constants.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/exceptions/
+-rw-rw-rw-   0        0        0     4204 2022-02-11 17:58:00.000000 uip-cli-2.0.0/uip/exceptions/customexceptions.py
+-rw-rw-rw-   0        0        0     3461 2023-03-23 14:08:25.000000 uip-cli-2.0.0/uip/exceptions/errormessages.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      251 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/main.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/parsecli/
+-rw-rw-rw-   0        0        0    26306 2023-03-23 14:08:25.000000 uip-cli-2.0.0/uip/parsecli/parsecli.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/parsecli/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uipproject/
+-rw-rw-rw-   0        0        0    30529 2023-03-28 20:27:23.000000 uip-cli-2.0.0/uip/uipproject/uipproject.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/uipproject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/
+-rw-rw-rw-   0        0        0      306 2023-03-17 20:26:38.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/
+-rw-rw-rw-   0        0        0     2074 2022-03-24 16:21:06.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/extension.py
+-rw-rw-rw-   0        0        0      646 2023-03-06 16:58:43.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/extension.yml
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/templates/
+-rw-rw-rw-   0        0        0     3190 2023-02-01 17:56:49.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/templates/template.json
+-rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-17 20:26:38.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/template_config.yml
+-rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/resources/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/resources/setupscripts/
+-rw-rw-rw-   0        0        0       43 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/uiptemplates/resources/setupscripts/setup.cfg
+-rw-rw-rw-   0        0        0    12088 2023-03-28 20:27:23.000000 uip-cli-2.0.0/uip/uiptemplates/resources/setupscripts/setup.py
+-rw-rw-rw-   0        0        0        0 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/uiptemplates/resources/setupscripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/
+-rw-rw-rw-   0        0        0      306 2023-03-17 20:26:38.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/
+-rw-rw-rw-   0        0        0     1776 2023-03-17 20:26:38.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/extension.py
+-rw-rw-rw-   0        0        0      641 2023-03-06 16:58:43.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/extension.yml
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/templates/
+-rw-rw-rw-   0        0        0     3213 2023-02-01 17:56:49.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/templates/template.json
+-rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/__init__.py
+-rw-rw-rw-   0        0        0     1087 2023-03-17 20:26:38.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/template_config.yml
+-rw-rw-rw-   0        0        0        0 2022-03-01 19:15:42.000000 uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/__init__.py
+-rw-rw-rw-   0        0        0     8937 2023-03-23 14:08:25.000000 uip-cli-2.0.0/uip/uiptemplates/template.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/uiptemplates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/uiptemplates/__pycache__/
+-rw-rw-rw-   0        0        0     4972 2023-04-10 11:59:38.000000 uip-cli-2.0.0/uip/uiptemplates/__pycache__/template.cpython-36.pyc
+-rw-rw-rw-   0        0        0      181 2023-04-10 11:59:38.000000 uip-cli-2.0.0/uip/uiptemplates/__pycache__/__init__.cpython-36.pyc
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip/utils/
+-rw-rw-rw-   0        0        0     4915 2023-02-01 17:56:49.000000 uip-cli-2.0.0/uip/utils/custom_io.py
+-rw-rw-rw-   0        0        0     4519 2023-03-23 14:08:25.000000 uip-cli-2.0.0/uip/utils/formatting.py
+-rw-rw-rw-   0        0        0     2008 2023-02-08 21:46:46.000000 uip-cli-2.0.0/uip/utils/generic.py
+-rw-rw-rw-   0        0        0       41 2021-09-03 01:31:50.000000 uip-cli-2.0.0/uip/utils/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-04-03 16:22:07.000000 uip-cli-2.0.0/uip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip_cli.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    41370 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     2046 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        4 2023-04-10 12:01:50.000000 uip-cli-2.0.0/uip_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2021-09-03 01:31:50.000000 uip-cli-2.0.0/__init__.py
```

### Comparing `uip-cli-1.3.0/LICENSE.txt` & `uip-cli-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uip-cli-1.3.0/PKG-INFO` & `uip-cli-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uip-cli
-Version: 1.3.0
+Version: 2.0.0
 Summary: Universal Extension CLI for interfacing with Controller Web Services
 Home-page: UNKNOWN
 Author: Stonebranch
 License: GNU General Public License
 Description: Universal Integration Platform Command Line Utility
         ===================================================
         
@@ -14,33 +14,35 @@
         to interface with the Universal Extension Web Service APIs. The goal of
         the CLI is to make the process of creating, editing, and deploying
         Extensions convenient and fast.
         
         Features
         --------
         
-        -  Quickly prototype Extensions using starter Extension Templates
+        -  Quickly prototype Extensions using starter (or custom) Extension Templates
         -  Build and upload Extensions and/or Universal Templates
         -  Pull the latest Universal Template source files from the Controller
         -  Download the full Universal Template package 
         
         Getting Started
         ===============
         Requirements
         ------------
         
-        ``uip-cli`` works with Python 2.7 and greater on Windows, Linux, and
+        ``uip-cli`` works with Python 3.6 and greater on Windows, Linux, and
         MacOS, and uses the following third party libraries:
         
+        - ``jsonschema`` (3.2.0)
         - ``colorama`` (0.4.4)
         - ``requests`` (2.26.0) 
         - ``jinja2`` (2.11.3) 
         - ``prettytable`` (1.0.1)
         - ``pyyaml`` (5.4.1)
         - ``setuptools`` (44.1.1)
+        - ``wheel`` (0.37.1)
         
         All the required libraries listed above are automatically installed
         during the installation process
         
         Installation
         ------------
         
@@ -77,71 +79,80 @@
             usage: uip [-h] <command> ...
         
             optional arguments:
             -h --help
                             show this help message and exit
         
             commands:
-            <command>
+              <command>
                 init         initialize a new project with starter Extension templates
-                template-list
-                             list of available Extension templates
+                template     used to perform actions on built-in (and external) templates
                 build        used to build Extension or full package
                 upload       upload Extension (or full package) to the Controller
                 push         build and upload Extension (or full package) to the Controller
                 pull         pulls the latest template.json (and template_icon.png, if
-                             present)
+                            present)
                 download     downloads the full Universal Template package
                 clean        used to purge build artifacts
                 task         used to perform actions on Universal Extension tasks
+                template-list
+                            list of available Extension templates. Note: this command will
+                            be deprecated in two releases
         
             examples:
             uip <command>
             uip init
             uip download
         
         Basic Usage 
         ===========
         ``uip-cli`` currently supports the following commands:
         
         - init 
-        - template-list
+        - template
+        
+          - list
+          - add
+          - delete
+          - export
         - build 
         - upload 
         - push 
         - pull 
         - download
         - clean
         - task
         
           - launch
           - status   
           - output
+        - template-list (will be deprecated in two releases. replaced by the ``template list`` command)
+        
         
         A brief overview of each of the commands is provided below along with 
-        some examples. For a more detailed demonstration of the commands, 
-        refer to the 'How-To/Getting Started' Document. 
+        some examples. It is highly recommended to go through the `Extension Development <https://docs.stonebranch.com/confluence/display/UC73/Extension+Development>`_
+        document for a more detailed demonstration.
         
         ``init`` 
         --------
-        This command is used to initialize a new project using one of the provided 
-        starter Extension templates. It can also be used to initialize an existing,
-        *partially valid* Extension project.
+        This command is used to initialize a new project using a custom, user-specified
+        template or one of the provided starter Extension templates. It can also be used
+        to initialize an existing, *partially valid* Extension project.
         
         **To initialize a brand new project using a starter Extension template, issue the 
         following command**:
         :: 
         
             $ uip init -t ue-task -e 'extension_name=my_sample_extension'
         
         
         - The ``-t`` option accepts the name of the starter Extension template. For a full 
-          list of the available Extension templates, see the ``template-list`` command below. 
+          list of the available Extension templates, see the ``template list`` command below. 
         - The ``-e`` option is used to configure the starter Extension template with user-defined 
-          variables. See the ``template-list`` command for instructions on obtaining 
+          variables. See the ``template list`` command for instructions on obtaining 
           a full list of configurable variables. 
         
         Once the CLI executes the command, a project will be initialized in the current 
         working directory with the following structure:
         ::
         
             |   setup.cfg
@@ -173,44 +184,229 @@
         
         :: 
         
             $ uip init 
         
         The CLI will first check to make sure ``extension.py``, ``extension.yml``, and ``template.json``
         exist in their respective directories shown above. If so, the CLI will create the ``.uip`` folder.
-        Additionally, if ``setup.py`` and ``setup.cfg`` are not present, they will be created along with the
-        ``.uip`` folder.
+        Additionally, if ``setup.py`` and ``setup.cfg`` are not present, they will be
+        created along with the ``.uip`` folder.
+        
+        **How to create a custom/configurable Extension template**:
+        
+        The CLI is equipped with two built-in, configurable Extension templates:
+        ``ue-task`` and ``ue-publisher``. These two templates may not be enough for some
+        users. To get around this, the CLI supports initializing from external, user-built
+        Extension templates. 
+        
+        This section will outline the basic requirements for creating a custom, configurable
+        Extension template.
+        
+        Assuming a folder named ``my_template`` exists, it must contain (at minimum) the following
+        files/folders to be considered a valid Extension template:
+        
+        ::
+        
+            my_template
+            â”œâ”€â”€ template_config.yml
+            â””â”€â”€ src/
+                â”œâ”€â”€ extension.py
+                â”œâ”€â”€ extension.yml
+                â””â”€â”€ templates/
+                    â””â”€â”€ template.json 
+        
+        Aside from the usual Extension related files, ``template_config.yml`` is also needed to make
+        the template configurable. 
+        
+        The file must contain:
+        
+        - ``name``: a string that identifies the name of the template (this is NOT referring to the Universal Template name).
+        - ``version``: a string that identifies the template version. Not restricted to ``x.y.z`` (SemVer); it could be anything (e.g. ``v1``). 
+        - ``description``: a string describing the template.
+        
+        and can optionally contain:
+        
+        - ``files_to_template``: an array containing paths to files that will be "templated" using ``Jinja2``. All files must be specified relative to ``template_config.yml``.
+        - ``variables``: a mapping/dictionary of variables that will be substituted in the relevant files specified by ``files_to_template``. The value of each key/variable is another mapping/dictionary that must contain ``default`` and ``description``.
+        
+        Shown below is a sample ``template_config.yml``:
+        
+        ::
+        
+            name: my_template
+        
+            version: 1.0.0
+        
+            description: this is the description for my_template
+        
+            files_to_template: 
+              - src/extension.py
+              - src/templates/template.json
+        
+            variables:
+              msg:
+                default: test_message
+                description: message to print to STDOUT and STDERR
+              log_level:
+                default: Info
+                description: Universal Template Log Level 
+        
+        As mentioned, the CLI uses the ``Jinja2`` module to substitute the variables in each file from ``files_to_template``. For instance,
+        if ``src/extension.py`` or ``src/templates/template.json`` mention ``{{ msg }}`` or ``{{ log_level }}``, the entirety of
+        ``{{ msg }}``/``{ log_level }}`` will be replaced with the user-specified value (or the default, if nothing is specified).
+        
+        Once the custom Extension template is created, it can be zipped up or pushed out to a Git repository. The CLI supports initializing from both
+        of these ways, which makes the custom template easy to distribute. The next section will outline the details regarding this functionality.
+        
+        **Packaging custom-built Extension Templates**:
+        
+        Once a custom template has been created, it must be packaged into either a
+        zip file or a Git repository.
+        
+        Shown below is the structure of a valid, custom template zip called ``my_template.zip``:
+        
+        ::
+        
+            my_template.zip
+            â”œâ”€â”€ template_config.yml
+            â””â”€â”€ src/
+                â”œâ”€â”€ extension.py
+                â”œâ”€â”€ extension.yml
+                â””â”€â”€ templates/
+                    â””â”€â”€ template.json 
+        
+        The custom template can also be pushed out to a Git repository. In this case, the zip file
+        won't be part of the repository. In other words, the top-level file and folder should be ``template_config.yml``
+        and ``src/``, respectively.
+        
+        **Initializing a custom-built Extension Template**:
+        
+        Assuming a custom template has been packaged based on the guidelines from the previous
+        section, it is ready to be used!
+        
+        The CLI supports initializing custom-built templates from:
+        
+        - a zip file
+        - a http(s) link to a zip file
+        - a Git repository
+        
+        **Initializing from a zip file**:
+        
+        To initialize the template zip without saving it:
+        ::
+        
+            $ uip init -t <path to zip file>
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t <path to zip file> --save
+        
+        Once saved, the template will be available in the ``template list`` command. At this point, the template can be
+        initialized similarly to ``ue-task`` and ``ue-publisher``.
         
+        **Initializing from a http(s) link**:
         
-        ``template-list`` 
+        The CLI supports initializing from both HTTP and HTTPS links that point to a zip file (link normally ends in .zip).
+        
+        It also supports basic authentication. The syntax is ``http://<username>:<password>@<actual url>`` (applies to HTTPS as well). For instance, if the url is ``http://mytestserver/test/my_template.zip``, the username is ``testuser``, and password is ``testpwd``, the formatted URL would be ``http://testuser:testpwd@mytestserver/test/my_template.zip``.
+        
+        To initialize the template without saving it:
+        ::
+        
+            $ uip init -t <link to http(s) url>
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t <link to http(s) url> --save
+        
+        **Initializing from a Git repository**:
+        
+        The CLI also supports initializing directly from a Git repository (similar to how pip installs work from a Git repo). The repo should not contain the zip file, just the raw files/folders that make up the template.
+        
+        The CLI relies on Git being installed on the system. If it is not, the CLI will issue an error.
+        
+        Both SSH and HTTPS protocols are supported.
+        
+        For HTTPS protocol, the url must start with ``git+`` followed by the HTTPS clone url. For instance, if the HTTPS Clone URL is ``https://gitlab-tst.com/test/templates/my_template.git``, then the syntax:
+        
+        To initialize the template without saving it:
+        ::
+        
+            $ uip init -t git+https://gitlab-tst.com/test/templates/my_template.git
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t git+https://gitlab-tst.com/test/templates/my_template.git --save
+        
+        If the repository is private and requires a username and access token to clone it, the URL should be specified as: ``git+https://<USERNAME>:<ACCESS TOKEN>@gitlab-tst.com/test/templates/my_template.git``.
+        
+        
+        For the SSH protocol, the url must start with ``git+`` followed by the SSH clone url. For instance, if the SSH Clone URL is ``git@gitlab-tst.com:test/templates/my_template.git``, then the syntax:
+        
+        To initialize the template without saving it:
+        ::
+        
+            $ uip init -t git+git@gitlab-tst.com:test/templates/my_template.git
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t git+git@gitlab-tst.com:test/templates/my_template.git --save
+        
+        The CLI also supports cloning a specific branch/commit/tag. This can be done by appending the branch/commit SHA/tag at the end of the URL using ``@branch``, ``@commit``, or ``@tag``. For instance, to clone
+        
+        a branch named ``test1``
+        ::
+        
+            HTTPS URL: git+https://gitlab-tst.com/test/templates/my_template.git@branch:test1
+            SSH URL: git+git@gitlab-tst.com:test/templates/my_template.git@branch:test1
+        
+        a commit with SHA ``9ab454ef``:
+        ::
+        
+            HTTPS URL: git+https://gitlab-tst.com/test/templates/my_template.git@commit:9ab454ef
+            SSH URL: git+git@gitlab-tst.com:test/templates/my_template.git@commit:9ab454ef
+        
+        a tag named ``v1``:
+        ::
+        
+            HTTPS URL: git+https://gitlab-tst.com/test/templates/my_template.git@tag:v1
+            SSH URL: git+git@gitlab-tst.com:test/templates/my_template.git@tag:v1
+        
+        
+        ``template`` 
         -----------------
-        This command is used to list all the available starter Extension templates as well as 
-        the variables used to configure the templates. 
+        This command is used to perform actions on all the available, custom-built and 
+        starter Extension templates. As of now, four actions/subcommands are supported: 
+        ``list``, ``add``, ``delete``, and ``export``.
         
         To see the list of available templates, type the following:
         ::
         
-            $ uip template-list 
+            $ uip template list
         
         Something similar to the output below should be shown:
         :: 
         
-            +--------------------+---------------------------------------------------------+
-            | Extension Template | Description                                             |
-            +--------------------+---------------------------------------------------------+
-            | ue-publisher       | starter Extension with a local Universal Event template |
-            +--------------------+---------------------------------------------------------+
-            | ue-task            | starter Extension with minimal code                     |
-            +--------------------+---------------------------------------------------------+
+            +--------------------+---------+---------------------------------------------------------+
+            | Extension Template | Version | Description                                             |
+            +--------------------+---------+---------------------------------------------------------+
+            | ue-task            | 1.0.0   | starter Extension with minimal code                     |
+            +--------------------+---------+---------------------------------------------------------+
+            | ue-publisher       | 1.0.0   | starter Extension with a local Universal Event template |
+            +--------------------+---------+---------------------------------------------------------+
         
         To see the list of configurable variables for one of the templates shown above, 
         type the following (same process applies to ``ue-publisher``): 
         :: 
         
-            $ uip template-list ue-task 
+            $ uip template list ue-task 
         
         and a table of variables will be shown: 
         :: 
         
             +---------------------------+------------------+--------------------------------+
             | Variable Name             | Default          | Description                    |
             +---------------------------+------------------+--------------------------------+
@@ -220,31 +416,71 @@
             | extension_requires_python | >=2.6            | Extension Python requirement   |
             | owner_name                | Stonebranch      | Extension owner's name         |
             | owner_organization        | Stonebranch Inc. | Extension owner's organization |
             | universal_template_name   | UE Task          | Universal Template name        |
             +---------------------------+------------------+--------------------------------+
         
         
+        To add a custom-built Extension template:
+        :: 
+        
+            $ uip template add <path to zip / link to zip / link to Git repository>
+        
+        Similar to the ``init`` command, the ``template add`` command also supports
+        adding/saving custom-built templates from:
+        
+        - a zip file
+        - a http(s) link to a zip file
+        - a Git repository
+        
+        In fact, it does so in the same exact manner. See the ``init`` section for details.
+        
+        Once the template is added, it will be available for use just like ``ue-task``
+        and ``ue-publisher``.
+        
+        
+        To delete a custom-built Extension template:
+        :: 
+        
+            $ uip template delete <template name>
+        
+        
+        To export an Extension template:
+        :: 
+        
+            $ uip template export <template name>
+        
+        
         ``build`` 
         ---------
-        This command is used to build an Extension or the full package.
-        
+        This command is used to build an Extension or the full package. 
         A full package build consists of the Universal Template and the Extension. 
         
+        The command also supports building extensions with third-party Python packages.
+        To do so, create a file called ``requirements.txt`` in the Extension folder.
+        Running ``uip build`` will then create a ``3pp`` folder, install all PyPi packages
+        specified in ``requirements.txt`` to ``3pp``, and package it in the extension zip
+        (or the full package).
+        
         
         To build the Extension only:
         :: 
         
             $ uip build 
         
         To build the full package:
         :: 
         
             $ uip build -a 
         
+        To build the dependency wheel file only:
+        :: 
+        
+            $ uip build -d
+        
         
         ``upload`` 
         ----------
         This command is used to upload an Extension or the full package to the 
         Controller. 
         
         To upload the Extension only:
@@ -329,14 +565,19 @@
         (including the folders themselves).
         
         To purge the build artifacts:
         :: 
         
             $ uip clean
         
+        Optionally, it is also possible to purge the 3pp folder (if it exists) using:
+        :: 
+        
+            $ uip clean --all
+        
         
         ``task``
         ------------
         This command is used to perform actions on Universal Extension tasks. 
         As of now, three actions/subcommands are supported: ``launch``, ``status``, 
         and ``output`` which allow the CLI to launch, get status, and get output of
         Universal Extension tasks. 
@@ -485,14 +726,28 @@
            * - Variables 
              - ``-e``
              - ``--variables``
              - UIP_TEMPLATE_VARIABLES 
              - variables 
              - NO 
              - None 
+           * - Save
+             - ``-s``
+             - ``--save``
+             - None
+             - None
+             - NO 
+             - False 
+           * - Upgrade
+             - ``-u``
+             - ``--upgrade``
+             - None
+             - None
+             - NO
+             - False
         
         
         Values for the **variables** option can be specified in three different ways:
         
         - Using the ``-e`` option multiple times:
           ::
         
@@ -529,30 +784,94 @@
              - NO 
              - Current Working Directory 
              - Where to initialize the Extension template. For example, in the following command:
                ``uip init -t ue-task -e '@vars.yml' my_extension_dir``, ``my_extension_dir`` is 
                where the ``ue-task`` Extension template will be initialized.
         
         
-        ``template-list`` command options  
+        ``template list`` command options  
         ---------------------------------
         .. list-table:: Positional Arguments 
            :header-rows: 1
         
            * - Option Name 
              - Required 
              - Default
              - Description
            * - <extension template name> 
              - NO 
              - None 
              - The name of the Extension template to get more details of. For example, in the 
-               following command: ``uip template-list ue-task``, ``ue-task`` is the value of 
+               following command: ``uip template list ue-task``, ``ue-task`` is the value of 
                ``<extension template name>``. 
         
+        .. list-table:: Optional Arguments 
+           :header-rows: 1
+        
+           * - Option Name
+             - Short Arg
+             - Long Arg
+             - Environment Variable
+             - Configuration File Arg
+             - Required
+             - Default
+           * - JSON
+             - ``-j``
+             - ``--json``
+             - None
+             - None
+             - NO
+             - False
+        
+        
+        ``template add`` command options  
+        --------------------------------
+        .. list-table:: Positional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Required 
+             - Default
+             - Description
+           * - <extension template> 
+             - YES 
+             - None 
+             - The name of the Extension template to add. Valid values include path to a zip
+               file, HTTP(S) url pointing to a zip file, or a Git repository clone url.
+        
+        
+        ``template delete`` command options  
+        -----------------------------------
+        .. list-table:: Positional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Required 
+             - Default
+             - Description
+           * - <extension template> 
+             - YES 
+             - None 
+             - The name of the Extension template to delete
+        
+        
+        ``template export`` command options  
+        -----------------------------------
+        .. list-table:: Positional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Required 
+             - Default
+             - Description
+           * - <extension template> 
+             - YES 
+             - None 
+             - The name of the Extension template to export
+        
         
         ``build`` command options  
         -------------------------
         .. list-table:: Optional Arguments 
            :header-rows: 1
         
            * - Option Name 
@@ -565,14 +884,21 @@
            * - Build All  
              - ``-a``
              - ``--all``
              - UIP_BUILD_ALL 
              - build-all 
              - NO 
              - False
+           * - Build Dependency Wheel Only 
+             - ``-d``
+             - ``--dep-whl-only``
+             - UIP_BUILD_DEPENDENCY_WHEEL_ONLY 
+             - dep-whl-only 
+             - NO 
+             - False
         
         
         ``upload`` command options  
         --------------------------
         .. list-table:: Optional Arguments 
            :header-rows: 1
         
@@ -630,14 +956,35 @@
              - ``--template-name``
              - UIP_TEMPLATE_NAME 
              - template-name 
              - NO 
              - Name from ``template.json``
         
         
+        ``clean`` command options  
+        -------------------------
+        .. list-table:: Optional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Short Arg 
+             - Long Arg
+             - Environment Variable
+             - Configuration File Arg 
+             - Required 
+             - Default
+           * - Clean All  
+             - ``-a``
+             - ``--all``
+             - UIP_CLEAN_ALL 
+             - clean-all 
+             - NO 
+             - False
+        
+        
         ``task launch`` command options  
         -------------------------------
         .. list-table:: Positional Arguments 
            :header-rows: 1
           
            * - Option Name 
              - Required 
@@ -739,23 +1086,23 @@
         Acknowledgements
         ================
         ``uip-cli`` acknowledges the use of the following open source Python modules:
         
         - `colorama <https://pypi.org/project/colorama/>`_ (BSD License)
         - `Jinja2 <https://pypi.org/project/Jinja2/>`_ (BSD-3-Clause License)
         - `prettytable <https://pypi.org/project/prettytable/>`_ (BSD-3-Clause License)
+        - `jsonschema <https://pypi.org/project/jsonschema/>`_ (MIT)
         - `PyYAML <https://pypi.org/project/PyYAML/>`_ (MIT)
         - `requests <https://pypi.org/project/requests/>`_ (Apache 2.0)
         - `setuptools <https://pypi.org/project/setuptools/>`_ (MIT)
         
         Copyright
         =========
-        Copyright (c) 2022. Stonebranch, Inc. All rights reserved.
+        Copyright (c) 2023. Stonebranch, Inc. All rights reserved.
         
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uip-cli-1.3.0/setup.py` & `uip-cli-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,38 +6,40 @@
         long_description = readme.read()
     setup(
         name='uip-cli',
         version=UIP_CLI_VERSION,
         packages=find_packages(exclude=['*test*']),
         include_package_data=True,
         install_requires=[
+            "jsonschema >= 3.2.0",
             "colorama >= 0.4.4",
             "requests >= 2.26.0",
             "jinja2 >= 2.11.3",
             "prettytable >= 1.0.1",
             "pyyaml >= 5.4.1",
-            "setuptools >= 44.1.1"
+            "setuptools >= 44.1.1",
+            "wheel >= 0.37.1"
         ],
         extras_require={
-            'tests': ['configparser', 'mock', 'pyyaml', 'pytest']
+            'tests': ['configparser', 'mock', 'pyyaml', 'pytest',
+                      'parameterized', 'pytest-cov']
         },
         author='Stonebranch',
         license="GNU General Public License",
         license_files='LICENSE.txt',
         description='Universal Extension CLI for interfacing with Controller Web Services',
         entry_points={
             'console_scripts': [
                 'uip=uip.main:main'
             ]
         },
-        python_requires='>=2.7',
+        python_requires='>=3.6',
         classifiers=[
             'Operating System :: POSIX :: Linux',
             'Operating System :: Microsoft :: Windows',
-            'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3'
         ],
         long_description=long_description,
         long_description_content_type="text/x-rst"
     )
```

### Comparing `uip-cli-1.3.0/uip/cliapis/apis.py` & `uip-cli-2.0.0/uip/cliapis/apis.py`

 * *Files identical despite different names*

### Comparing `uip-cli-1.3.0/uip/cliconfig/customformatter.py` & `uip-cli-2.0.0/uip/cliconfig/customformatter.py`

 * *Files identical despite different names*

### Comparing `uip-cli-1.3.0/uip/cliconfig/setupcli.py` & `uip-cli-2.0.0/uip/cliconfig/setupcli.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,31 +6,33 @@
 from uip.cliconfig.customformatter import CustomHelpFormatter
 from uip.config.configoptions import get_default_value as gdv
 from uip.config.configoptions import get_env_var_name as gevn
 from uip.config.configoptions import get_long_arg as gla
 from uip.config.configoptions import get_short_arg as gsa
 from uip.constants import constants
 from uip.parsecli.parsecli import parse_cli_args
-from uip.utils.formatting import wrap_text
+from uip.utils.formatting import wrap_text, join_list_of_strings
 from .. import UIP_CLI_VERSION
 
+prog_ref = "%(prog)s"
+
 def add_example_epilog(cmd_arg, example_usage, title="examples"):
     """
     Adds examples section at the end of the help menu
 
     Parameters
     ----------
     cmd_arg : parser, subparser
         The parser or subparser to add the examples to
     example_usage : str
         The examples to add
     """
     # At this point, example_usage contains %(prog)s instead of the actual program name (which is substituted later).
     # Thus, effective_width needs to account for this as shown below.
-    effective_width = 80 - (len(cmd_arg.prog) - len('%(prog)s'))
+    effective_width = 80 - (len(cmd_arg.prog) - len(prog_ref))
     wrapped_usage = wrap_text(example_usage, effective_width, initial_indent=2, subsequent_indent=4)
     title = wrap_text(title, effective_width, initial_indent=0, subsequent_indent=2)
     wrapped_usage = '\n%s: \n%s\n' % (title, wrapped_usage)
     cmd_arg.formatter_class = CustomHelpFormatter
     if cmd_arg.epilog:
         cmd_arg.epilog += wrapped_usage
     else:
@@ -45,14 +47,17 @@
     cmd_arg.formatter_class = CustomHelpFormatter
     if cmd_arg.description:
         cmd_arg.description += wrapped_description
     else:
         cmd_arg.description = wrapped_description
 
 
+validation_funcs = []
+
+
 def add_login_args(cmd_arg):
     """
     Adds login related arguments to cmd_arg
 
     Parameters
     ----------
     cmd_arg : parser, subparser
@@ -85,82 +90,228 @@
     add_command_description(init_arg,
                             "The 'init' command provides starter Extension templates to start a new project")
 
     # Add positional arguments
     init_arg.add_argument('dir', metavar='<dir>', default=gdv('init.dir'), nargs='?', type=str,
                           help='where to initialize the Extension template (default: %(default)s)')
 
+
+    extension_template_arg_ref = 'init.extension_template'
+    variables_arg_ref = 'init.variables'
+    save_arg_ref = 'init.save'
+    upgrade_arg_ref = 'init.upgrade'
+
     # Add optional arguments
-    init_arg.add_argument(gsa('init.extension_template'), gla('init.extension_template'), metavar='<name>',
-                          default=gdv('init.extension_template'), type=str,
-                          help='name of the Extension template to initialize in the specified directory. If no name is '
-                               'specified, an empty .uip project will be created.')
-    init_arg.add_argument(gsa('init.variables'), gla('init.variables'), metavar='<variables>',
-                          default=gdv('init.variables'), action='append',
+    init_arg.add_argument(gsa(extension_template_arg_ref), gla(extension_template_arg_ref), metavar='<name>',
+                          default=gdv(extension_template_arg_ref), type=str,
+                          help='name of the Extension template to initialize in the specified directory. '
+                               'If there are multiple templates with the same name, the version must also '
+                               'be specified as <template>@<version>. If no name is specified, an empty '
+                               '.uip project will be created.')
+    init_arg.add_argument(gsa(variables_arg_ref), gla(variables_arg_ref), metavar='<variables>',
+                          default=gdv(variables_arg_ref), action='append',
                           help='user defined variables used to configure templates before creating them. '
-                               '(environment variable: %s)' % gevn('init.variables'))
+                               '(environment variable: %s)' % gevn(variables_arg_ref))
+    init_arg.add_argument(gsa(save_arg_ref), gla(save_arg_ref), default=None,
+                           action='store_true', help='if specified, the user specified template will be saved for future use. ')
+    init_arg.add_argument(gsa(upgrade_arg_ref), gla(upgrade_arg_ref), default=None,
+                           action='store_true',
+                           help="if specified, the existing Extension project will be "
+                                "upgraded to meet the CLI's new requirements. "
+                                "For now, this involves upgrading the setup scripts "
+                                "(script.py and setup.cfg).")
+    
+    def validate_init_args(parser, args):
+        if args and args.command_type == 'init':
+            if args.upgrade and (args.extension_template is not None or \
+                                 args.variables is not None or \
+                                 args.save is not None):
+                parser.error('The {0} option cannot be specified with {1}'.
+                             format(gla(upgrade_arg_ref), join_list_of_strings([
+                                gla(extension_template_arg_ref),
+                                gla(variables_arg_ref),
+                                gla(save_arg_ref)], 'or')))
+
+    validation_funcs.append(validate_init_args)
 
     # Add examples
     add_example_epilog(init_arg, """
         {prog}
+        {prog} {ula}
+        {prog} {ietsa} <template name>@<template version>
         {prog} {ietsa} <template name> {itvsa} '{{"extension_name": "myext", "version": "1.0.0"}}'
         {prog} {ietsa} <template name> {itvsa} 'extension_name=myext' {itvsa} 'version=1.0.0'
         {prog} {ietsa} <template name> {itvsa} @vars.json
         {prog} {ietsa} <template name> {itvsa} @vars.yml
-    """.format(prog="%(prog)s", ietsa=gsa('init.extension_template'), itvsa=gsa('init.variables')))
+        {prog} {ietsa} <template name>@<template version>
+        {prog} {ietsa} <template zip> {itvsa} @vars.yml {itsla}
+        {prog} {ietsa} <HTTP(S) link to zip> {itssa}
+    """.format(prog=prog_ref, ietsa=gsa(extension_template_arg_ref), itvsa=gsa(variables_arg_ref),
+        itssa=gsa(save_arg_ref), itsla=gla(save_arg_ref), ula=gla(upgrade_arg_ref)))
 
 
-def setup_template_list_arg(cmd_subparsers):
+def setup_template_list_arg_deprecated(cmd_subparsers):
     """
-    Sets up the init command and it's arguments
-
-    Parameters
-    ----------
-    cmd_subparsers : subparsers
-        The subparser to add the init arg to
+    NOTE: This command will be deprecated in two releases. Currently, replace by
+    'template' command.
     """
     template_list = cmd_subparsers.add_parser('template-list',
-                                              help='list of available Extension templates')
-    add_command_description(template_list, "List of available Extension templates")
+                                              help='list of available Extension templates. Note: this command will be deprecated in two releases')
+    add_command_description(template_list, "List of available Extension templates. \nNote: this command will be deprecated in two releases. Use the 'template' command instead.")
 
     # Add positional arguments
-    template_list.add_argument('extension_template_name', metavar="<extension template name>", nargs='?', type=str,
-                               default=None, help='name of the Extension template to get more details of')
+    template_list.add_argument('extension_template', metavar="<extension template>", nargs='?', type=str,
+                               default=None, help='Extension template to list variables of')
 
     # Add examples
     add_example_epilog(template_list, """
         %(prog)s
         %(prog)s <template name>
     """)
 
 
+def setup_template_list_arg(template_subparser):
+    template_list_arg = template_subparser.add_parser('list', help='list available Extension templates (and their variables)')
+    add_command_description(template_list_arg, 
+                            "used to list available Extension templates. If a template name isn't specified, the CLI will "
+                            "print all the available templates. Specifying the template name will print the template's "
+                            "variables.")
+
+    # Add positional arguments
+    template_list_arg.add_argument('extension_template', metavar="<extension template>", nargs='?', type=str,
+                               default=None, help='Extension template to list variables of. If there are multiple '
+                                                  'templates with the same name, the version must also be specified '
+                                                  'as <template>@<version>')
+
+    # Add optional arguments
+    template_list_arg.add_argument(gsa('template_list.json'), gla('template_list.json'), default=None,
+                           action='store_true', help='if specified, the output will be printed as a JSON string. ')
+
+    # Add examples
+    add_example_epilog(template_list_arg, """
+        {prog}
+        {prog} {tljla}
+        {prog} <template name>
+        {prog} <template name>@<template version>
+        {prog} <template name> {tljla}
+    """.format(prog=prog_ref, tljla=gla('template_list.json')))
+
+
+def setup_template_add_arg(template_subparser):
+    template_add_arg = template_subparser.add_parser('add', help='add an external Extension template')
+    add_command_description(template_add_arg, 
+                            "used to add external Extension templates. Valid values include path to a zip file, "
+                            "HTTP(S) url pointing to a zip file, or a Git repository clone url. "
+                            "See the full documentation for details.")
+
+    # Add positional arguments
+    template_add_arg.add_argument('extension_template', metavar="<extension template>", type=str,
+                               default=None, help='Extension template to add')
+
+    # Add examples
+    add_example_epilog(template_add_arg, """
+        %(prog)s <path to zip file>
+        %(prog)s <HTTP(S) url to a zip file>
+        %(prog)s <Git Repository Clone url>
+    """)
+
+
+def setup_template_delete_arg(template_subparser):
+    template_delete_arg = template_subparser.add_parser('delete', help='delete an Extension template')
+    add_command_description(template_delete_arg, 
+                            "the specified Extension template will be deleted.")
+
+    # Add positional arguments
+    template_delete_arg.add_argument('extension_template', metavar="<extension template>", type=str,
+                               default=None, help='Extension template to delete. If there are multiple '
+                                                  'templates with the same name, the version must also be specified '
+                                                  'as <template>@<version>')
+
+    # Add examples
+    add_example_epilog(template_delete_arg, """
+        %(prog)s <template name>
+        %(prog)s <template name>@<template version>
+    """)
+
+
+def setup_template_export_arg(template_subparser):
+    template_export_arg = template_subparser.add_parser('export', help='export an Extension template')
+    add_command_description(template_export_arg, 
+                            "the specified Extension template will be exported.")
+
+    # Add positional arguments
+    template_export_arg.add_argument('extension_template', metavar="<extension template>", type=str,
+                               default=None, help='Extension template to export. If there are multiple '
+                                                  'templates with the same name, the version must also be specified '
+                                                  'as <template>@<version>')
+
+    # Add examples
+    add_example_epilog(template_export_arg, """
+        %(prog)s <template name>
+        %(prog)s <template name>@<template version>
+    """)
+
+
+def setup_template_arg(cmd_subparsers):
+    template_arg = cmd_subparsers.add_parser('template', help='used to perform actions on built-in (and external) templates')
+    template_subparser = template_arg.add_subparsers(title="template action", dest='template_action', metavar='')
+    template_subparser.required = True
+
+    add_command_description(template_arg,
+                            'used to perform actions on built-in (and external) templates.')
+
+    setup_template_list_arg(template_subparser)
+    setup_template_add_arg(template_subparser)
+    setup_template_delete_arg(template_subparser)
+    setup_template_export_arg(template_subparser)
+
+    # Add examples
+    add_example_epilog(template_arg, """
+        %(prog)s list
+        %(prog)s list <template name>
+        %(prog)s add <template zip / HTTP(S) link to zip / Git Repo>
+        %(prog)s delete <template name>
+        %(prog)s delete <template name>@<template version>
+        %(prog)s export <template name>
+    """)
+
+
 def setup_build_arg(cmd_subparsers):
     """
     Sets up the build command and it's arguments
 
     Parameters
     ----------
     cmd_subparsers : subparsers
         The subparser to add the build arg to
     """
+    build_all_arg_ref = 'build.all'
+    build_dep_whl_only_arg_ref = 'build.dep_whl_only'
+
     build_arg = cmd_subparsers.add_parser('build', help='used to build Extension or full package')
     add_command_description(build_arg,
                             "The 'build' command is used to build the Extension or the full package. By default, "
                             "only the Extension will be built.")
 
     # Add optional arguments
-    build_arg.add_argument(gsa('build.all'), gla('build.all'), default=None,
+    mutually_exclusive_args = build_arg.add_mutually_exclusive_group()
+    mutually_exclusive_args.add_argument(gsa(build_all_arg_ref), gla(build_all_arg_ref), default=None,
                            action='store_true', help='if specified, the full package will be built '
-                                                     '(environment variable: %s)' % gevn('build.all'))
+                                                     '(environment variable: %s)' % gevn(build_all_arg_ref))
+    mutually_exclusive_args.add_argument(gsa(build_dep_whl_only_arg_ref), gla(build_dep_whl_only_arg_ref), default=None,
+                           action='store_true', help='if specified, only the dependency wheel file will be built '
+                                                     '(environment variable: %s)' % gevn(build_dep_whl_only_arg_ref))
 
     # Add examples
     add_example_epilog(build_arg, """
         {prog} 
         {prog} {basa}
-    """.format(prog="%(prog)s", basa=gsa('build.all')))
+        {prog} {bdwola}
+    """.format(prog=prog_ref, basa=gsa(build_all_arg_ref),
+               bdwola=gla(build_dep_whl_only_arg_ref)))
 
 
 def setup_upload_arg(cmd_subparsers):
     upload_arg = cmd_subparsers.add_parser('upload', help='upload Extension (or full package) to the Controller')
     add_command_description(upload_arg, "upload Extension (or full package) to the Controller. By default, only the "
                                         "Extension will be uploaded.")
 
@@ -171,15 +322,15 @@
     # Add required arguments related to login
     add_login_args(upload_arg)
 
     # Add examples
     add_example_epilog(upload_arg, """
         {prog}
         {prog} {uala}
-    """.format(prog="%(prog)s", uala=gla('upload.all')))
+    """.format(prog=prog_ref, uala=gla('upload.all')))
 
 
 def setup_push_arg(cmd_subparsers):
     push_arg = cmd_subparsers.add_parser('push', help='build and upload Extension (or full package) to the Controller')
     add_command_description(push_arg,
                             "build and upload Extension (or full package) to the Controller. By default, only the "
                             "Extension will be built and uploaded.")
@@ -191,30 +342,30 @@
     # Add required arguments related to login
     add_login_args(push_arg)
 
     # Add examples
     add_example_epilog(push_arg, """
         {prog}
         {prog} {pala}
-    """.format(prog="%(prog)s", pala=gla('push.all')))
+    """.format(prog=prog_ref, pala=gla('push.all')))
 
 
 def setup_pull_arg(cmd_subparsers):
     pull_arg = cmd_subparsers.add_parser('pull',
                                          help='pulls the latest template.json (and template_icon.png, if present)')
     add_command_description(pull_arg, "pulls the latest template.json (and template_icon.png, if present)")
 
     # Add required arguments related to login
     add_login_args(pull_arg)
 
     # Add examples
     add_example_epilog(pull_arg, """
         {prog}
         {prog} {sula} admin {spla} admin
-    """.format(prog="%(prog)s", sula=gla('shared.userid'), spla=gla('shared.password')))
+    """.format(prog=prog_ref, sula=gla('shared.userid'), spla=gla('shared.password')))
 
 
 def setup_download_arg(cmd_subparsers):
     download_arg = cmd_subparsers.add_parser('download', help='downloads the full Universal Template package')
     add_command_description(download_arg,
                             'downloads the full Universal Template package and saves the zip in the "dist" folder')
 
@@ -227,35 +378,43 @@
     # Add required arguments related to login
     add_login_args(download_arg)
 
     # Add examples
     add_example_epilog(download_arg, """
           {prog} {dtnsa} <template name>
           {prog} {susa} admin {spsa} admin
-      """.format(prog="%(prog)s", dtnsa=gsa('download.template_name'), susa=gsa('shared.userid'),
+      """.format(prog=prog_ref, dtnsa=gsa('download.template_name'), susa=gsa('shared.userid'),
                  spsa=gsa('shared.password')))
 
 def setup_clean_arg(cmd_subparsers):
     """
     Sets up the clean command and it's arguments
 
     Parameters
     ----------
     cmd_subparsers : subparsers
         The subparser to add the clean arg to
     """
+    clean_all_arg_ref = 'clean.all'
+
     clean_arg = cmd_subparsers.add_parser('clean', help='used to purge build artifacts')
     add_command_description(clean_arg,
                             "The 'clean' command is used to purge build artifacts which "
                             "includes anything inside the dist, build, and temp folders.")
+    
+    # Add optional arguments
+    clean_arg.add_argument(gsa(clean_all_arg_ref), gla(clean_all_arg_ref), default=None,
+                          action='store_true', help='if specified, the 3pp folder will also be purged '
+                                                    '(environment variable: %s)' % gevn(clean_all_arg_ref))
 
     # Add examples
     add_example_epilog(clean_arg, """
         {prog} 
-    """.format(prog="%(prog)s"))
+        {prog} {cala}
+    """.format(prog=prog_ref, cala=gla(clean_all_arg_ref)))
 
 def setup_task_launch_arg(task_subparser):
     launch_task_arg = task_subparser.add_parser('launch', help='launch an Universal Extension task')
     add_command_description(launch_task_arg, 
                             'used to launch an Universal Extension task. By default, the CLI will '
                             'launch the task and continously print the status. Once the task '
                             'succeeds/fails, it will print the task output.')
@@ -374,16 +533,16 @@
 
     cmd_type_subparsers = parser.add_subparsers(title="commands", dest='command_type', metavar='<command>')
     cmd_type_subparsers.required = True
 
     # init command setup
     setup_init_arg(cmd_type_subparsers)
 
-    # template-list command setup
-    setup_template_list_arg(cmd_type_subparsers)
+    # template command setup
+    setup_template_arg(cmd_type_subparsers)
 
     # build command setup
     setup_build_arg(cmd_type_subparsers)
 
     # upload command setup
     setup_upload_arg(cmd_type_subparsers)
 
@@ -398,15 +557,20 @@
 
     # clean command setup
     setup_clean_arg(cmd_type_subparsers)
 
     # task command setup
     setup_task_arg(cmd_type_subparsers)
 
+    # template-list command setup (will be deprecated in two releases)
+    setup_template_list_arg_deprecated(cmd_type_subparsers)
+
     num_args = len(sys.argv)
     if num_args == 1:
         parser.print_help()
     else:
         init()
         args = parser.parse_args()
+        for f in validation_funcs:
+            f(parser, args)
         parse_cli_args(args)
         deinit()
```

### Comparing `uip-cli-1.3.0/uip/config/config.py` & `uip-cli-2.0.0/uip/config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,22 +65,22 @@
             rendered_config_file = formatting.jinja_render_file(config_file_dir, constants.CONFIG_FILE_NAME, variables)
             custom_io.write_to_file(os.path.join(dest, constants.CONFIG_FILE_NAME), rendered_config_file)
     else:
         #TODO: implement configuration file upgrade logic
         # import linecache
         # current_version = linecache.getline(global_config_file, 6).strip()
         # if current_version != ('# %s' % UIP_CLI_VERSION):
-        #     current_config = io.read_yaml(global_config_file)
+        #     current_config = custom_io.read_yaml(global_config_file)
         #     dest = get_global_config_file_dir()
         #     if dest:
-        #         io.make_dir(dest)
+        #         custom_io.make_dir(dest)
         #         config_file_dir = os.path.join(package_dir, constants.CONFIG_FILE_DIR_NAME)
         #         variables = {'UIP_CLI_VERSION': UIP_CLI_VERSION}
         #         rendered_config_file = formatting.jinja_render_file(config_file_dir, constants.CONFIG_FILE_NAME, variables)
-        #         io.write_to_file(os.path.join(dest, constants.CONFIG_FILE_NAME), rendered_config_file)
+        #         custom_io.write_to_file(os.path.join(dest, constants.CONFIG_FILE_NAME), rendered_config_file)
         #         if current_config:
         #             with open(os.path.join(dest, constants.CONFIG_FILE_NAME), 'a') as yml_file:
         #                 import yaml 
         #                 yml_file.write('\n')
         #                 yaml.safe_dump(current_config, yml_file)
         pass
```

### Comparing `uip-cli-1.3.0/uip/config/configoptions.py` & `uip-cli-2.0.0/uip/config/configoptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,18 +14,38 @@
         # options that are shared across the various commands
     },
     'init': {
         'extension_template': {'short_arg': '-t', 'long_arg': '--extension-template', 'env_var': None,
                                'config_arg': None, 'default': None},
         'variables': {'short_arg': '-e', 'long_arg': '--variables', 'env_var': 'UIP_TEMPLATE_VARIABLES',
                       'config_arg': 'variables', 'default': None},
-        'dir': {'default': os.getcwd()}
+        'dir': {'default': os.getcwd()},
+        'save': {'short_arg': '-s', 'long_arg': '--save', 'env_var': None, 'config_arg': None,
+                'default': False},
+        'upgrade': {'short_arg': '-u', 'long_arg': '--upgrade', 'env_var': None, 'config_arg': None,
+                'default': False},
+    },
+    'template_list': {
+        'extension_template': {'default': None},
+        'json': {'short_arg': '-j', 'long_arg': '--json', 'env_var': None, 'config_arg': None,
+                'default': False}
+    },
+    'template_add': {
+        'extension_template': {'default': None},
+    },
+    'template_delete': {
+        'extension_template': {'default': None},
+    },
+    'template_export': {
+        'extension_template': {'default': None},
     },
     'build': {
         'all': {'short_arg': '-a', 'long_arg': '--all', 'env_var': 'UIP_BUILD_ALL', 'config_arg': 'build-all',
+                'default': False},
+        'dep_whl_only': {'short_arg': '-d', 'long_arg': '--dep-whl-only', 'env_var': 'UIP_BUILD_DEPENDENCY_WHEEL_ONLY', 'config_arg': 'dep-whl-only',
                 'default': False}
     },
     'upload': {
         'all': {'short_arg': '-a', 'long_arg': '--all', 'env_var': 'UIP_UPLOAD_ALL', 'config_arg': 'upload-all',
                 'default': False},
     },
     'push': {
@@ -50,14 +70,16 @@
     },
     'task_output': {
         'task_name': {'default': None},
         'instance_number': {'short_arg': '-s', 'long_arg': '--instance-number', 'env_var': 'UIP_INSTANCE_NUMBER', 'config_arg': 'instance-number',
                     'default': 'most_recent_task_instance'},
     },
     'clean': {   
+        'all': {'short_arg': '-a', 'long_arg': '--all', 'env_var': 'UIP_CLEAN_ALL', 'config_arg': 'clean-all',
+                'default': False},
     }
 }
 
 for config_option in ['shared', 'upload', 'push', 'pull', 'download', 'task_launch', 'task_status', 'task_output']:
     config_options[config_option].update(login_options)
```

### Comparing `uip-cli-1.3.0/uip/config/mergeconfig.py` & `uip-cli-2.0.0/uip/config/mergeconfig.py`

 * *Files identical despite different names*

### Comparing `uip-cli-1.3.0/uip/config/uip.yml` & `uip-cli-2.0.0/uip/config/uip.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# (c) Copyright 2022 Stonebranch, Inc., All rights reserved.
+# (c) Copyright 2023 Stonebranch, Inc., All rights reserved.
 #
 # Stonebranch, Inc.
 # Universal Integration Platform Command Line Utility Configuration File
 # {{ UIP_CLI_VERSION }}
 #
 # This configuration file specifies options used by the UIP CLI. The options
 # and their values must be specified in proper YAML format as shown below.
@@ -69,14 +69,32 @@
 #
 #   Examples:
 #     build-all: false
 #     build-all: yes
 #     build-all: TRUE
 #     build-all: NO
 #
+# Option: dep-whl-only
+# Default: False
+#
+#   If specified, only the dependency wheel file will be generated. This option
+#   is applicable only if the 'zip_safe' option is 'False' in extension.yml
+#
+#   There are multiple ways to specify the option:
+#     - True/yes
+#     - False/no
+#
+#   Note that 'True/yes' and 'False/no' are case-insensitive
+#
+#   Examples:
+#     dep-whl-only: false
+#     dep-whl-only: yes
+#     dep-whl-only: TRUE
+#     dep-whl-only: NO
+#
 ###############################################################################
 ###############################################################################
 #
 # 'upload' command options:
 #############################
 # Option: upload-all
 # Default: False
@@ -193,14 +211,38 @@
 #   Examples:
 #     instance-number: 5
 #     instance-number: 132
 #
 ###############################################################################
 ###############################################################################
 #
+# 'clean' command options:
+###########################
+# Option: clean-all
+# Default: False
+#
+#   The 'clean-all' option is used to specify whether the 3pp folder should be
+#   purged or not. By itself, the clean purges the build, dist, and temp folder.
+#   If 'clean-all' is specified, the 3pp folder will also be purged.
+#
+#   There are multiple ways to specify the option:
+#     - True/yes
+#     - False/no
+#
+#   Note that 'True/yes' and 'False/no' are case-insensitive
+#
+#   Examples:
+#     clean-all: false
+#     clean-all: yes
+#     clean-all: TRUE
+#     clean-all: NO
+#
+###############################################################################
+###############################################################################
+#
 # Configuration Options Section
 #
 ###############################################################################
 #
 # userid: <userid>
 # url: <url>
 # variables: <JSON string | JSON/YAML file>
```

### Comparing `uip-cli-1.3.0/uip/exceptions/customexceptions.py` & `uip-cli-2.0.0/uip/exceptions/customexceptions.py`

 * *Files identical despite different names*

### Comparing `uip-cli-1.3.0/uip/exceptions/errormessages.py` & `uip-cli-2.0.0/uip/exceptions/errormessages.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     201: '"{0}" must be specified',
     202: 'Universal Template name must be specified',
     203: '"{0}" option cannot be None',
     204: '"{0}" configuration file not found',
     205: 'Universal Extension task name must be specified',
     206: '"{0}" is not a valid integer value',
     207: 'value must be a positive integer',
-    208: '"{0}" is not a supported platform. Only Windows, Linux, and MacOS are supported'
+    208: '"{0}" is not a supported platform. Only Windows, Linux, and MacOS are supported',
+    209: 'value cannot be empty'
 }
 
 # uipproject errors (301-400)
 uipproject_errors = {
     301: '"{0}" is not a valid JSON or YAML file',
     302: '"{0}" is incorrectly formatted',
     303: '{0} folder already exists in "{1}"',
@@ -41,15 +42,26 @@
     307: '"{0}" already contains an Extension template',
     308: '"{0}" does not contain a valid Extension template',
     309: '"{0}" is not a valid Extension template directory',
     310: 'No zip files were found in "{0}"',
     311: '"{0}" is not a valid Extension template',
     312: 'template.json is corrupted. The "name" field must be non-empty',
     313: '"{0}" not found',
-    314: 'extension version must be SemVer compliant'
+    314: '"{0}" is invalid. {1}',
+    315: 'template name must be something other than {0}',
+    316: 'multiple matching templates found. Specify one of the following versions: {0}.',
+    317: 'template must be specified.',
+    318: 'Unable to clone the specified Git repository. Ensure the URL is valid.',
+    319: 'HTTP(S) request failed with code {0}: {1}.',
+    320: 'URL must point to a valid zip file.',
+    321: 'extension version must be SemVer compliant',
+    322: 'Unable to add "{0}"',
+    323: '"{0}" contains invalid jinja2 syntax: {1}',
+    324: 'Dependency wheel cannot be built if zip_safe is True',
+    325: 'setup.py is incompatible with this version of uip-cli. Run "uip init --upgrade"'
 }
 
 # utils errors (401-500)
 utils_errors = {
     401: '"{0}" is not a valid JSON string'
 }
 
@@ -57,14 +69,24 @@
 parsecli_errors = {
     501: '"{0}" is not a valid folder name',
     502: '"{0}" is not a valid Extension template',
     503: '"{0}" is not a valid Universal Extension task',
     504: '"{0}" is not a valid task instance number'
 }
 
+# Generic errors (601-700)
+generic_errors = {
+    601: 'Unable to create "{0}"',
+    602: '{0}',  # Can be used if error is coming from an external source
+    603: '{0} not found',
+    604: '{0} expected to be one of {1}',
+    605: '"{0}" is not valid'
+}
+
 error_messages = {}
 error_messages.update(cliapis_errors)
 error_messages.update(cliconfig_errors)
 error_messages.update(config_errors)
 error_messages.update(uipproject_errors)
 error_messages.update(utils_errors)
-error_messages.update(parsecli_errors)
+error_messages.update(parsecli_errors)
+error_messages.update(generic_errors)
```

### Comparing `uip-cli-1.3.0/uip/parsecli/parsecli.py` & `uip-cli-2.0.0/uip/parsecli/parsecli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import print_function
 import argparse
 import os
 import sys
 from datetime import datetime
+import functools
 
 from colorama import Fore
 from uip.cliapis import apis
 from uip.config.mergeconfig import get_merged_config
 from uip.exceptions import customexceptions
 from uip.uipproject import uipproject
 from uip.uiptemplates import template
+from uip.constants import constants
 from uip.utils import custom_io, formatting
-from uip.constants.constants import TASK_STATUSES
 
 
 def pack_login_info(userid, password, url):
     """
     Packs the login information into a tuple
 
     Parameters
@@ -55,63 +56,195 @@
 
     Parameters
     ----------
     args : argparse.Namespace
         The args read by argparser
     """
     mc = get_merged_config('init', args)
-    msg = uipproject.initialize_uip(mc.extension_template, mc.variables, mc.dir)
+    if mc.upgrade:
+        msg = uipproject.upgrade_extension_repo(mc.dir)
+    else:
+        msg = uipproject.initialize_uip(mc.extension_template, mc.variables, mc.dir,
+            mc.save)
     return {
         'msg': msg
     }
 
 
 def parse_template_list_command(args):
     mc = get_merged_config('template_list', args)
-    chosen_template_name = mc.extension_template_name
+    chosen_template_name = mc.extension_template
 
     if chosen_template_name:
-        extension_templates = template.get_extension_templates([chosen_template_name])
+        extension_templates = template.get_extension_templates(chosen_template_name)
         if len(extension_templates) == 0:
             raise customexceptions.InvalidValueError(502, chosen_template_name)
+        elif len(extension_templates) > 1:
+            raise customexceptions.InvalidValueError(316, formatting.join_list_of_strings(
+                list(map(lambda t: t['template_version'], extension_templates)), 'or'))
     else:
         extension_templates = template.get_all_extension_templates()
+
     table_data = []
     table_headers = None
     separate_each_entry = True
     for extension_template in extension_templates:
-        template_name = extension_template.get('template_name')
-        template_path = extension_template.get('template_path')
-        template_details = template.get_extension_template_details(template_path)
-        template_description = template_details['template_description']
-
-        if chosen_template_name == template_name:
-            for template_variable in template_details.get('user_defined_variables'):
-                variable_name = list(template_variable.keys())[0]
-                variable_default = template_variable[variable_name]['default']
-                variable_description = template_variable[variable_name]['description']
-                table_data.append([variable_name, variable_default, variable_description])
+        template_name = extension_template['template_name']
+        template_version = extension_template['template_version']
+        template_description = extension_template['template_description']
+        template_variables = extension_template['template_variables']
+
+        if chosen_template_name and chosen_template_name.startswith(template_name):
+            # Found the matching template
+
+            if not template_variables:
+                return {
+                    'msg': '"%s (%s)" does not contain any variables' % (template_name, template_version)
+                }
+
+            for var_name, var_details in template_variables.items():
+                variable_default = var_details['default']
+                variable_description = var_details['description']
+                table_data.append([var_name, variable_default, variable_description])
             table_headers = ['Variable Name', 'Default', 'Description']
             separate_each_entry = False
             break
         else:
-            table_data.append([template_name, template_description])
-            table_headers = ['Extension Template', 'Description'] if table_headers is None else table_headers
+            table_data.append([template_name, template_version, template_description])
+            table_headers = ['Extension Template', 'Version', 'Description'] if table_headers is None else table_headers
 
-    formatting.print_table(table_headers, table_data, separate_each_entry=separate_each_entry)
+    formatting.print_table(table_headers, table_data, separate_each_entry=separate_each_entry,
+        as_json=mc.json)
+
+
+def parse_template_add_command(args):
+    mc = get_merged_config('template_add', args)
+    extension_template = mc.extension_template
+
+    temp_folder = custom_io.get_temp_dir(prefix=constants.TEMP_DIRECTORY_PREFIX)
+    try:
+        success = uipproject.process_user_specified_template(extension_template,
+            temp_folder)
+        if not success:
+            raise customexceptions.InvalidValueError(322, extension_template)
+
+        # Verify template before saving
+        template_details = template.get_extension_template_details(temp_folder)
+
+        if template_details is None:
+            # 'template_config.yml' must not exist
+            raise customexceptions.FileNotFoundError(313, constants.TEMPLATE_CONFIG_YAML)
+
+        # validate 'template_config.yml'
+        error = template.validate_template_config(template_details)
+        if error:
+            raise customexceptions.CorruptedFileError(314,
+                        constants.TEMPLATE_CONFIG_YAML, error)
+
+        template_name = template_details['name']
+        if template_name in constants.BUILT_IN_TEMPLATES:
+            raise customexceptions.InvalidValueError(315,
+                formatting.join_list_of_strings(constants.BUILT_IN_TEMPLATES,
+                    'or'))
+
+        # ensure 'files_to_template' have correct jinja2 syntax
+        template.validate_jinja2_syntax(temp_folder, 
+            template_details.get('files_to_template', []))
+
+        # Save the template
+        name, version, updating_template = uipproject.save_user_specified_template(temp_folder,
+            template_details)
+        return {
+            'msg': 'Successfully %s "%s (%s)"' % 
+                ("updated" if updating_template else "added", name, version)
+        }
+    finally:
+        if temp_folder:
+            custom_io.remove_dir(temp_folder)
+
+
+def parse_template_delete_command(args):
+    mc = get_merged_config('template_delete', args)
+    extension_template = mc.extension_template
+
+    extension_templates = template.get_extension_templates(extension_template)
+    if len(extension_templates) == 0:
+        raise customexceptions.InvalidValueError(502, extension_template)
+    elif len(extension_templates) > 1:
+        raise customexceptions.InvalidValueError(316, formatting.join_list_of_strings(
+            list(map(lambda t: t['template_version'], extension_templates)), 'or'))
+    else:
+        # Found the matching template
+        ext_template = extension_templates[0]
+        template_path = ext_template['template_path']
+        template_name = ext_template['template_name']
+        template_version = ext_template['template_version']
+
+        if ext_template['is_user_template']:
+            custom_io.remove_dir(template_path)
+            return {
+                'msg': 'Successfully deleted "%s (%s)"' % (template_name, template_version)
+            }
+        else:
+            # Cannot delete built-in templates
+            raise customexceptions.InvalidValueError(315, 
+                formatting.join_list_of_strings(constants.BUILT_IN_TEMPLATES))
+
+
+def parse_template_export_command(args):
+    mc = get_merged_config('template_export', args)
+    extension_template = mc.extension_template
+
+    extension_templates = template.get_extension_templates(extension_template)
+    if len(extension_templates) == 0:
+        raise customexceptions.InvalidValueError(502, extension_template)
+    elif len(extension_templates) > 1:
+        raise customexceptions.InvalidValueError(316, formatting.join_list_of_strings(
+            list(map(lambda t: t['template_version'], extension_templates)), 'or'))
+    else:
+        # Found the matching template
+        ext_template = extension_templates[0]
+        template_path = ext_template['template_path']
+        template_name = ext_template['template_name']
+        template_version = ext_template['template_version']
+
+        filename = '%s-%s.zip' % (formatting.replace_nonalphanum_chars(template_name), 
+            formatting.replace_nonalphanum_chars(template_version, replace_with='.'))
+        success = custom_io.zip_directory(filename, template_path)
+        if not success:
+            raise customexceptions.Error(601, filename)
+
+        return {
+            'msg': 'Successfully exported "%s"' % filename
+        }
 
 
 def parse_build_command(args):
     mc = get_merged_config('build', args)
-    generated_file = uipproject.generate_build(build_all=mc.all)
-    filename = os.path.basename(generated_file)
-    buildpath = os.path.relpath(os.path.dirname(generated_file))
+    generated_files = uipproject.generate_build(build_all=mc.all,
+                                               dep_whl_only=mc.dep_whl_only)
+    
+    # Remove all the 'None' items
+    generated_files = [f for f in generated_files if f is not None]
 
-    msg = formatting.format_list_for_printing([filename],
-                                              header='The following files were built in "%s"' % buildpath)
+    if len(generated_files) == 0:
+        msg = 'No build artifacts generated'
+    else:
+        header = 'The following files were built'
+        all_files_in_same_dir = functools.reduce(
+            lambda f1, f2: os.path.dirname(f1) == os.path.dirname(f2),
+            generated_files)
+        
+        if all_files_in_same_dir:
+            header += ' in "%s"' % os.path.relpath(os.path.dirname(generated_files[0]))
+            generated_files = [os.path.basename(f) for f in generated_files]
+        else:
+            generated_files = [os.path.relpath(f) for f in generated_files]
+
+        msg = formatting.format_list_for_printing(generated_files, header)
     return {
         'msg': msg
     }
 
 
 def parse_upload_command(args):
     mc = get_merged_config('upload', args)
@@ -129,15 +262,15 @@
     return return_dict
 
 
 def parse_push_command(args):
     mc = get_merged_config('push', args)
     login_info = pack_login_info(mc.userid, mc.password, mc.url)
 
-    generated_file = uipproject.generate_build(build_all=mc.all)
+    uipproject.generate_build(build_all=mc.all)
 
     return_dict = {}
     if mc.all:
         full_package_zip_path = uipproject.get_built_full_package_zip_path()
         return_dict = apis.import_template(template=full_package_zip_path, login_info=login_info)
     else:
         extension_zip_path = uipproject.get_built_extension_zip_path()
@@ -260,19 +393,19 @@
 
                                 if status is None:
                                     continue
                                 else:
                                     status = status.title()
 
                                 keep_printing = False 
-                                if status in [TASK_STATUSES.success, TASK_STATUSES.finished]:
+                                if status in [constants.TASK_STATUSES.success, constants.TASK_STATUSES.finished]:
                                     status = Fore.GREEN + status
-                                elif status in [TASK_STATUSES.failed, TASK_STATUSES.cancelled, TASK_STATUSES.start_failure, TASK_STATUSES.undeliverable]:
+                                elif status in [constants.TASK_STATUSES.failed, constants.TASK_STATUSES.cancelled, constants.TASK_STATUSES.start_failure, constants.TASK_STATUSES.undeliverable]:
                                     status = Fore.RED + status 
-                                elif status in [TASK_STATUSES.in_doubt, TASK_STATUSES.skipped]:
+                                elif status in [constants.TASK_STATUSES.in_doubt, constants.TASK_STATUSES.skipped]:
                                     status = Fore.CYAN + status 
                                 else:
                                     status = Fore.YELLOW + status 
                                     keep_printing = True 
 
                                 status = status + Fore.RESET 
 
@@ -343,19 +476,19 @@
                     table_headers = ['Instance Number', 'Instance Id', 'Launch Time', 'Status (Exit Code)', 'Status Description']
                     table_data = []
 
                     num_instances = len(result) if num_instances <= 0 else num_instances
 
                     for data in result[:num_instances]:
                         status = data['status']
-                        if status in [TASK_STATUSES.success, TASK_STATUSES.finished]:
+                        if status in [constants.TASK_STATUSES.success, constants.TASK_STATUSES.finished]:
                             status = Fore.GREEN + status
-                        elif status in [TASK_STATUSES.failed, TASK_STATUSES.cancelled, TASK_STATUSES.start_failure, TASK_STATUSES.undeliverable]:
+                        elif status in [constants.TASK_STATUSES.failed, constants.TASK_STATUSES.cancelled, constants.TASK_STATUSES.start_failure, constants.TASK_STATUSES.undeliverable]:
                             status = Fore.RED + status 
-                        elif status in [TASK_STATUSES.in_doubt, TASK_STATUSES.skipped]:
+                        elif status in [constants.TASK_STATUSES.in_doubt, constants.TASK_STATUSES.skipped]:
                             status = Fore.CYAN + status 
                         else:
                             status = Fore.YELLOW + status 
 
                         status = status + Fore.RESET + (' (%s)' % data['exitCode'])
                         statusDescription = data['statusDescription'] or 'N/A'
                         table_data.append([data['instanceNumber'], data['sysId'], data['launchTime'], status, statusDescription])
@@ -420,26 +553,34 @@
     task_action = args.task_action 
     function_name = 'parse_task_%s_command' % task_action
     func = getattr(sys.modules[__name__], function_name, None)
     call_func(func, args)
 
 
 def parse_clean_command(args):
-    purged_files = uipproject.purge_build_artifacts()
+    mc = get_merged_config('clean', args)
+    purged_files = uipproject.purge_build_artifacts(mc.all)
 
     if len(purged_files) == 0:
         msg = "No build artifacts found"
     else:
         msg = formatting.format_list_for_printing(purged_files,
                                               header='The following build artifacts were purged')
     return {
         'msg': msg
     }
 
 
+def parse_template_command(args):
+    template_action = args.template_action 
+    function_name = 'parse_template_%s_command' % template_action
+    func = getattr(sys.modules[__name__], function_name, None)
+    call_func(func, args)
+
+
 def parse_cli_args(args):
     """
     Parses the cli arguments based on the command_type
     argument which is guaranteed to be one of 'extension'
     or 'template', and calls the appropriate function with
     the name 'parse_%s_command' where %s is one of 'extension'
     or 'template'
```

### Comparing `uip-cli-1.3.0/uip/uipproject/uipproject.py` & `uip-cli-2.0.0/uip/uipproject/uipproject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
+from subprocess import CalledProcessError
 import zipfile
+import json
 import re
+import requests
 
-from jinja2 import Environment, FileSystemLoader
 from setuptools import sandbox
 from uip.constants import constants
 from uip.exceptions import customexceptions
 from uip.uiptemplates import template
 from uip.utils import custom_io, formatting, generic
 
 from .. import package_dir, UIP_CLI_VERSION
@@ -30,99 +32,233 @@
 
 def is_valid_dot_uip_dir(dir):
     config_file_path = os.path.join(dir, constants.DOT_UIP_FOLDER_NAME, constants.CONFIG_FILE_DIR_NAME,
                                     constants.CONFIG_FILE_NAME)
     return os.path.exists(config_file_path)
 
 
-def is_valid_dot_uip_and_extension_template_dir(dir):
-    return is_valid_extension_template_dir(dir) and is_valid_dot_uip_dir(dir)
+def is_valid_dot_uip_and_extension_template_dir(dir, require_setup_files=True):
+    return is_valid_extension_template_dir(dir, require_setup_files) and is_valid_dot_uip_dir(dir)
 
 
 def create_dot_uip_dir(dir, overwrite=False):
     if overwrite or not is_valid_dot_uip_dir(dir):
         dst_config_file_dir = os.path.join(dir, constants.DOT_UIP_FOLDER_NAME, constants.CONFIG_FILE_DIR_NAME)
         custom_io.make_dir(dst_config_file_dir)
 
         config_file_dir = os.path.join(package_dir, constants.CONFIG_FILE_DIR_NAME)
         variables = {'UIP_CLI_VERSION': UIP_CLI_VERSION}
         rendered_config_file = formatting.jinja_render_file(config_file_dir, constants.CONFIG_FILE_NAME, variables)
         custom_io.write_to_file(os.path.join(dst_config_file_dir, constants.CONFIG_FILE_NAME), rendered_config_file)
 
 
-def handle_internal_variables(internal_variables):
-    parsed_internal_variables = {}
-    for variable in internal_variables:
-        variable_type = list(variable.keys())[0]
-        if variable_type == constants.UUID_INTERNAL_VARIABLES:
-            uuid_variables = variable.get(variable_type)
-            for uuid_variable in uuid_variables:
-                parsed_internal_variables[uuid_variable] = generic.generate_uuid()
-    return parsed_internal_variables
+def process_user_specified_template(user_specified_template, folder_to_save_in):
+    success = True
 
+    if user_specified_template.startswith('git+'):        
+        url = user_specified_template[4:] # everything after "git+"
 
-def initialize_uip(starter_template_name, variables, dir):
+        if len(url) == 0:
+            raise customexceptions.InvalidValueError(318)
+
+        groups = re.findall(constants.GIT_BRANCH_COMMIT_TAG_REGEX,
+            url)
+        # groups should be [(branch/commit/tag, branch/commit/tag value)] if the
+        # user specified a branch/commit/tag
+
+        branch_commit_tag = ""
+        if len(groups) == 1 and len(groups[0]) == 2:
+            # User specified a branch/commit/tag
+            branch_commit_tag = groups[0][1]
+            # Update the url to no longer contain "@branch/@commit/@tag"
+            url = url[0:url.index("@"+groups[0][0])]
+
+        try:
+            generic.git_clone(url, folder_to_save_in, branch_commit_tag)
+        except CalledProcessError:
+            print('=' * 88)
+            raise customexceptions.InvalidValueError(318)
+        finally:
+            # Delete the '.git' folder
+            custom_io.remove_dir(os.path.join(folder_to_save_in, '.git'))
+        print('=' * 88)
+    elif user_specified_template.startswith('http://') or user_specified_template.startswith('https://'):
+        response = requests.get(user_specified_template, stream=True)
+        if response.ok:
+            content_type = response.headers.get('Content-Type', None)
+            if not content_type or content_type not in constants.ZIP_CONTENT_TYPES:
+                raise customexceptions.CorruptedFileError(320)
+
+            filename = response.headers.get('Content-Disposition', 'usertemplate.zip')
+            fullpath = os.path.join(folder_to_save_in, filename)
+
+            with open(fullpath, 'wb') as f:
+                f.write(response.content)
+
+            listing = custom_io.get_zip_listing(fullpath)
+            if not listing or not constants.VALID_USER_EXTENSION_TEMPLATE_FILES.issubset(set(listing)):
+                # must be an invalid zip file
+                raise customexceptions.CorruptedFileError(320)
+            
+            custom_io.extract_zip(fullpath, folder_to_save_in)
+            custom_io.remove_file(fullpath)
+        else:
+            raise customexceptions.InvalidValueError(319, response.status_code,
+                response.reason)
+    elif user_specified_template.endswith('.zip'):
+        if not os.path.exists(user_specified_template):
+            raise customexceptions.FileNotFoundError(313, user_specified_template)
+
+        listing = custom_io.get_zip_listing(user_specified_template)
+        if not listing or not constants.VALID_USER_EXTENSION_TEMPLATE_FILES.issubset(set(listing)):
+            # must be an invalid zip file
+            raise customexceptions.CorruptedFileError(311, user_specified_template)
+
+        # zip file contains all the expected files.
+        # Extract to a temporary folder
+        custom_io.extract_zip(user_specified_template, folder_to_save_in)
+    else:
+        success = False
+
+    return success
+
+
+def save_user_specified_template(template_path, template_details=None):
+    if not template_path:
+        return
+
+    user_templates_dir = os.path.join(package_dir, constants.USER_TEMPLATES_PATH)
+    custom_io.make_dir(user_templates_dir) # creates '_usertemplates_' folder
+
+    if template_details is None:
+        template_config_yml = os.path.join(template_path, constants.TEMPLATE_CONFIG_YAML)
+        template_details = custom_io.read_yaml(template_config_yml)
+
+    template_version = formatting.replace_nonalphanum_chars(
+        template_details['version'].lower())
+
+    template_to_save_dir = os.path.join(user_templates_dir,
+        '%s_%s' % (template_details['name'], template_version))
+
+    updating_template = os.path.exists(template_to_save_dir)
+
+    custom_io.remove_dir(template_to_save_dir) # if the template already exists, delete it
+    custom_io.make_dir(template_to_save_dir)
+    template.copy_template(template_path, template_to_save_dir,
+        keep_template_config=True)
+
+    return (template_details['name'], template_details['version'], updating_template)
+
+
+def initialize_uip(starter_template_name, variables, dir, save):
     if starter_template_name is None:
         # attempt to initialize an empty repository
         if is_valid_extension_template_dir(dir, require_setup_files=False):
             if not is_valid_dot_uip_dir(dir):
                 create_dot_uip_dir(dir)
                 for setup_file in constants.SETUP_SCRIPTS_RESOURCES:
                     setup_file_name = os.path.basename(setup_file)
                     if not os.path.exists(os.path.join(dir, setup_file_name)):
-                        template.copy_resources(constants.SETUP_SCRIPTS_RESOURCES, dir)
+                        template.copy_setup_scripts(dir)
                         break
                 return 'Successfully created %s folder in "%s"' % (constants.DOT_UIP_FOLDER_NAME, dir)
             else:
                 raise customexceptions.InitError(303, constants.DOT_UIP_FOLDER_NAME, dir)
         else:
             raise customexceptions.InvalidFolderError(308, dir)
     else:
-        extension_template = template.get_extension_templates([starter_template_name])
-        if not extension_template:
-            raise customexceptions.InvalidValueError(311, starter_template_name)
-
-        if is_valid_dot_uip_and_extension_template_dir(dir):
-            raise customexceptions.InitError(307, dir)
-
-        user_defined_variables = variables
-
-        template_path = extension_template[0].get('template_path')
-        template_details = template.get_extension_template_details(template_path)
-        files_to_template = template_details.get('files_to_template')
-        variable_dict = {}
-        for variable in template_details.get('user_defined_variables'):
-            variable_name = list(variable.keys())[0]
-            variable_default = variable[variable_name]['default']
-            variable_dict[variable_name] = variable_default
-
-        if user_defined_variables:
-            variable_dict.update(user_defined_variables)
-
-        internal_variables = template_details.get('internal_variables', None)
-        parsed_internal_variables = handle_internal_variables(internal_variables)
-        if parsed_internal_variables:
-            variable_dict.update(parsed_internal_variables)
-
-        create_dot_uip_dir(dir, overwrite=True)
-
-        if is_valid_dot_uip_dir(dir):
-            template.copy_template(template_path, dir)
-
-            resources_to_copy = template_details.get('resources_to_include', None)
-            template.copy_resources(resources_to_copy, dir)
-
-            env = Environment(loader=FileSystemLoader(template_path),
-                    keep_trailing_newline=True)
-            for file_to_template in files_to_template:
-                curr_template = env.get_template(file_to_template)
-                rendered_template = curr_template.render(variable_dict)
-                custom_io.write_to_file(os.path.join(dir, file_to_template), rendered_template)
-
-            return 'Successfully initialized "%s" template in "%s"' % (starter_template_name, dir)
+        try:
+            template_path = None
+            temp_folder = custom_io.get_temp_dir(prefix=constants.TEMP_DIRECTORY_PREFIX)
+            is_user_template = True
+
+            success = process_user_specified_template(starter_template_name, temp_folder)
+            
+            if success:
+                template_path = temp_folder
+            else:    
+                extension_template = template.get_extension_templates(starter_template_name)
+                if not extension_template:
+                    raise customexceptions.InvalidValueError(311, starter_template_name)
+                elif len(extension_template) > 1:
+                    # Found multiple templates. Need version to differentiate
+                    raise customexceptions.InitError(316, formatting.join_list_of_strings(
+                        list(map(lambda t: t['template_version'], extension_template)), 'or'))
+                template_path = extension_template[0].get('template_path')
+                is_user_template = False
+
+            if is_valid_dot_uip_and_extension_template_dir(dir):
+                raise customexceptions.InitError(307, dir)
+
+            template_details = template.get_extension_template_details(template_path)
+
+            if template_details is None:
+                # 'template_config.yml' must not exist
+                raise customexceptions.FileNotFoundError(313, constants.TEMPLATE_CONFIG_YAML)
+
+            # validate 'template_config.yml'
+            error = template.validate_template_config(template_details)
+            if error:
+                raise customexceptions.CorruptedFileError(314,
+                            constants.TEMPLATE_CONFIG_YAML, error)
+
+            template_name = template_details['name']
+            if is_user_template and template_name in constants.BUILT_IN_TEMPLATES:
+                raise customexceptions.InvalidValueError(315,
+                    formatting.join_list_of_strings(constants.BUILT_IN_TEMPLATES,
+                        'or'))        
+
+            files_to_template = template_details.get('files_to_template', [])
+
+            # ensure 'files_to_template' have correct jinja2 syntax
+            template.validate_jinja2_syntax(template_path, files_to_template)
+
+            variable_dict = {}
+            for var_name, var_details in template_details.get('variables', {}).items():
+                variable_dict[var_name] = var_details['default']
+
+            if variables:
+                variable_dict.update(variables)
+
+            create_dot_uip_dir(dir, overwrite=True)
+
+            if is_valid_dot_uip_dir(dir):
+                template.copy_setup_scripts(dir)
+
+                # Copying the template last will ensure user's '.uip', 
+                # 'setup.py', and 'setup.cfg' will overwrite the default ones.
+                template.copy_template(template_path, dir)
+
+                for file_to_template in files_to_template:
+                    if not os.path.exists(os.path.join(template_path, file_to_template)):
+                        continue
+                    rendered_template = formatting.jinja_render_file(
+                        template_path, file_to_template, variable_dict,
+                        **{'keep_trailing_newline': True, 'lstrip_blocks': True,
+                        'trim_blocks': True})
+                    custom_io.write_to_file(os.path.join(dir, file_to_template), rendered_template)
+
+                # Generate UUIDs for all 'sysId' fields in template.json
+                template_json_path = os.path.join(dir, constants.TEMPLATE_JSON_PATH)
+                template_json = custom_io.read_json(template_json_path)
+                if template_json is None:
+                    raise customexceptions.FileNotFoundError(313, template_json_path)
+                generic.update_key(template_json, constants.TEMPLATE_JSON_UUID_KEY,
+                    generic.generate_uuid)
+                custom_io.write_to_file(template_json_path, json.dumps(template_json, indent=2))
+
+                # Save the 'template' for future use if the user specified
+                if save and is_user_template:
+                    save_user_specified_template(template_path, template_details)
+
+                return 'Successfully initialized "%s (%s)" template in "%s"' % (
+                    template_name, template_details['version'], dir)
+        finally:
+            if temp_folder:
+                custom_io.remove_dir(temp_folder)
 
 
 def get_built_extension_zip_path():
     dir = os.getcwd()
     if is_valid_dot_uip_and_extension_template_dir(dir):
         search_dir = os.path.join(dir, constants.EXTENSION_BUILD_DIR)
         zip_files = custom_io.get_files_of_specific_type(search_dir, '*.zip')
@@ -289,54 +425,147 @@
     template_name = get_template_json_property('name')
     if template_name:
         return template_name
     else:
         raise customexceptions.CorruptedFileError(312)
 
 
-def build_extension(build_dir='extension_build', zip_filename=''):
+def is_setup_py_script_compatible():
     dot_uip_dir = os.getcwd()
-    if is_valid_dot_uip_and_extension_template_dir(dot_uip_dir):
 
-        requirements_txt_path = os.path.join(dot_uip_dir, 'requirements.txt')
-        if os.path.exists(requirements_txt_path):
-            threepp_path = os.path.join(dot_uip_dir, '3pp')
-            custom_io.make_dir(threepp_path)
+    # Make sure the setup.py in the extension template is compatible.
+    # If not, we will error out for now. Ideally, we should offer some
+    # way for user to "upgrade" their extension environment using a
+    # 'uip upgrade' command
+    is_compatible = True
+
+    setup_py_version = template.get_setup_py_script_version(
+        os.path.join(dot_uip_dir, constants.SETUP_PY))
 
-            generic.pip_install(requirements_txt_path, threepp_path)
+    if setup_py_version is None:
+        # Must be an older setup.py or a newer one without version
+        # information (which should never be the case)
+        is_compatible = False
+    else:
+        if setup_py_version.major <= 1 and setup_py_version.minor < 4:
+            # incompatible version
+            is_compatible = False
 
+    return is_compatible
+
+
+def build_extension(build_dir='extension_build', zip_filename='',
+                    dep_whl_only=False):
+    dot_uip_dir = os.getcwd()
+    if is_valid_dot_uip_and_extension_template_dir(dot_uip_dir):
+        if not is_setup_py_script_compatible():
+            # Raise an exception letting the user know the setup.py script is
+            # outdated and needs to be upgraded using 'uip upgrade'
+            raise customexceptions.CorruptedFileError(325)
+
+        extension_yml = custom_io.read_yaml(os.path.join(dot_uip_dir,
+                                            constants.EXTENSION_YML_PATH))
+
+        error = formatting.validate_using_jsonschema(
+                                extension_yml,
+                                constants.VALID_EXTENSION_YML_SCHEMA)
+        if error:
+            raise customexceptions.CorruptedFileError(314,
+                                        constants.EXTENSION_YML_PATH, error)
+
+        if not formatting.validate_regex_input(
+            constants.SEMVER_REGEX,
+            extension_yml['extension']['version']
+        ):
+            raise customexceptions.InvalidValueError(321)
+
+        # Assume extension is zip_safe, if 'zip_safe' is not in extension.yml
+        zip_safe = extension_yml['extension'].get('zip_safe', True)
+
+        # Make sure the 'dep_whl_only' flag is specified only if 'zip_safe' is False
+        if dep_whl_only and zip_safe:
+            raise customexceptions.InvalidValueError(324)
+
+        dep_wheel_temp_dir = custom_io.get_temp_dir()
+        extension_zip_temp_dir = custom_io.get_temp_dir()
+
+        dep_wheel_path = None
+        extension_zip_path = None
         try:
-            sandbox.run_setup('setup.py', ['clean', 'bdist_egg'])
+            # Install any third-party dependencies
+            sandbox.run_setup(constants.SETUP_PY,
+                              ['clean', '--all', 'install_deps'])
+            if zip_safe == False:
+                # Create the dependency wheel file in a temporary directory
+                # so we can be sure whether it actually got generated or not.
+                sandbox.run_setup(constants.SETUP_PY, ['clean', '--all',
+                                'bdist_dep_whl', '--dist-dir', dep_wheel_temp_dir])
+                temp_dep_wheel = custom_io.get_most_recent_file(
+                                        dep_wheel_temp_dir, filetype='*.whl')
+                if temp_dep_wheel is not None:
+                    # Copy dependency wheel to the appropriate folder
+                    dep_wheel_path = os.path.join(dot_uip_dir, 'dist', 'dep',
+                                                os.path.basename(temp_dep_wheel))
+                    custom_io.make_dir(os.path.dirname(dep_wheel_path))
+                    custom_io.remove_file(dep_wheel_path)
+                    custom_io.copy_file(temp_dep_wheel, dep_wheel_path)
+            if not dep_whl_only:
+                sandbox.run_setup(constants.SETUP_PY, ['clean', '--all',
+                            'bdist_egg', '--dist-dir', extension_zip_temp_dir])
+
+            print(('=' * 88))
+
+            temp_extension_zip = custom_io.get_most_recent_file(
+                                    extension_zip_temp_dir, filetype='*.zip')
+
+            if dep_whl_only:
+                return [dep_wheel_path]
+
+            if temp_extension_zip:
+                # Copy extension zip to the appropriate folder
+                extension_zip_build_dir = os.path.join(dot_uip_dir, 'dist', build_dir)
+                custom_io.make_dir(extension_zip_build_dir)
+                if len(zip_filename) == 0:
+                    zip_filename = os.path.basename(temp_extension_zip)
+                extension_zip_path = os.path.join(extension_zip_build_dir, zip_filename)
+                custom_io.remove_file(extension_zip_path)
+                custom_io.copy_file(temp_extension_zip, extension_zip_path)
+
+                if dep_wheel_path:
+                    return [extension_zip_path, dep_wheel_path]
+                else:
+                    return [extension_zip_path]
+            else:
+                raise customexceptions.BuildError(304)
         except SystemExit:
             pass
-        
-        print(('=' * 88))
-        most_recent_file = custom_io.get_most_recent_file(os.path.join(dot_uip_dir, 'dist'), filetype='*.zip')
-
-        extension_zip_build_dir = os.path.join(dot_uip_dir, 'dist', build_dir)
-        custom_io.make_dir(extension_zip_build_dir)
-
-        if most_recent_file:
-            if not zip_filename:
-                zip_filename = os.path.basename(most_recent_file)
-            zip_filename = os.path.join(extension_zip_build_dir, zip_filename)
-            custom_io.remove_file(zip_filename)
-            os.rename(most_recent_file, zip_filename)
-            return zip_filename
-        else:
-            raise customexceptions.BuildError(304)
+        except ValueError as ve:
+            # Expected if 'zip_safe' is specified for API level < 1.4.0 or
+            # if the user provided non-pep compliant extension version
+            raise customexceptions.InvalidValueError(602, str(ve))
+        finally:
+            custom_io.remove_dir(dep_wheel_temp_dir)
+            custom_io.remove_dir(extension_zip_temp_dir)
     else:
         raise customexceptions.InvalidFolderError(309, dot_uip_dir)
 
 
 def build_full_package():
     dot_uip_dir = os.getcwd()
     if is_valid_dot_uip_and_extension_template_dir(dot_uip_dir):
         full_package_build_dir = os.path.join(dot_uip_dir, 'dist', 'package_build')
-        extension_zip_path = build_extension(build_dir=full_package_build_dir, zip_filename='extension_archive.zip')
+        build_artifacts = build_extension(build_dir=full_package_build_dir,
+                                        zip_filename='extension_archive.zip')
+        # With the introduction of the new dependency wheel file, build_extension
+        # can return a list. In such case, filter out everything but 'extension_archive.zip'
+        build_artifacts = list(filter(lambda ezp: 'extension_archive.zip' in ezp,
+                                            build_artifacts))
+        if len(build_artifacts) != 1:
+            raise customexceptions.BuildError(305)
+        extension_zip_path = build_artifacts[0]
 
         template_json_path = os.path.join(dot_uip_dir, 'src', 'templates', 'template.json')
         template_json_data = custom_io.read_json(template_json_path)
         
         template_name = template_json_data.get('name', '').strip()
         if len(template_name) == 0:
             raise customexceptions.CorruptedFileError(306, "'name' must be defined.")
@@ -345,15 +574,15 @@
 
         template_icon_path = os.path.join(dot_uip_dir, 'src', 'templates', 'template_icon.png')
 
         extension_yml_path = os.path.join(dot_uip_dir, 'src', 'extension.yml')
         extension_yml_data = custom_io.read_yaml(extension_yml_path)
         extension_version = extension_yml_data['extension']['version']
         if not formatting.validate_regex_input(constants.SEMVER_REGEX, extension_version):
-            raise customexceptions.InvalidValueError(314)
+            raise customexceptions.InvalidValueError(321)
 
         template_dist_name = constants.UNIVERSAL_TEMPLATE_DIST_NAME % (
             template_name,
             extension_version
         )
 
         template_dist_zip = os.path.join(full_package_build_dir, template_dist_name)
@@ -368,42 +597,91 @@
         # delete extension_archive.zip
         custom_io.remove_file(extension_zip_path)
 
         most_recent_file = custom_io.get_most_recent_file(full_package_build_dir, '*.zip')
         if os.path.basename(most_recent_file) != template_dist_name:
             raise customexceptions.BuildError(305)
         else:
-            return template_dist_zip
+            return [template_dist_zip]
     else:
         raise customexceptions.InvalidFolderError(309, dot_uip_dir)
 
 
-def generate_build(build_all=False):
+def generate_build(build_all=False, dep_whl_only=False):
     if build_all:
         return build_full_package()
     else:
-        return build_extension()
+        return build_extension(dep_whl_only=dep_whl_only)
 
 
-def purge_build_artifacts():
+def purge_build_artifacts(clean_all=False):
     dot_uip_dir = os.getcwd()
     if is_valid_dot_uip_and_extension_template_dir(dot_uip_dir):
         purged_files = []
 
         for build_artifact_dir in constants.BUILD_ARTIFACT_DIRS:
             build_artifact_dir = os.path.join(dot_uip_dir, build_artifact_dir)
             if os.path.exists(build_artifact_dir):
                 purged_files.extend(custom_io.get_dir_listing(build_artifact_dir))
                 purged_files.append(build_artifact_dir)
                 custom_io.remove_dir(build_artifact_dir)
 
+        if clean_all and os.path.exists(constants.THREEPP_DIR):
+            # Purge the '3pp' folder, if it exists
+            purged_files.append(constants.THREEPP_DIR)
+            custom_io.remove_dir(constants.THREEPP_DIR)
+
         purged_files = [os.path.relpath(purged_file) for purged_file in purged_files]
 
         return purged_files
     else:
         raise customexceptions.InvalidFolderError(309, dot_uip_dir)
 
 
 def get_dot_uip_config_file_path(relative_to=os.getcwd()):
     config_file_path = os.path.join(relative_to, constants.DOT_UIP_FOLDER_NAME, constants.CONFIG_FILE_DIR_NAME,
                                     constants.CONFIG_FILE_NAME)
     return config_file_path if os.path.exists(config_file_path) else None
+
+
+def upgrade_extension_repo(repo_dir):
+    dot_uip_dir = repo_dir
+
+    if not is_valid_dot_uip_and_extension_template_dir(dot_uip_dir,
+                                                   require_setup_files=False):
+        raise customexceptions.InvalidFolderError(309, dot_uip_dir)
+
+    # For now, the upgrade process involves replacing the setup.py and 
+    # setup.cfg scripts with the newer versions and making a backup of the
+    # original ones. If they do not exist, then they will be added.
+
+    backup_folder = os.path.join(dot_uip_dir, constants.BACKUP_FOLDER_NAME)
+
+    setup_cfg_path = os.path.join(dot_uip_dir, constants.SETUP_CFG)
+    setup_py_path = os.path.join(dot_uip_dir, constants.SETUP_PY)
+
+    scripts_backed_up = []
+
+    if os.path.exists(setup_cfg_path):
+        custom_io.make_dir(backup_folder)
+        custom_io.copy_file(setup_cfg_path, os.path.join(backup_folder,
+                                        constants.SETUP_CFG))
+        scripts_backed_up.append(constants.SETUP_CFG)
+
+    if os.path.exists(setup_py_path):
+        custom_io.make_dir(backup_folder)
+        custom_io.copy_file(setup_py_path, os.path.join(backup_folder,
+                                        constants.SETUP_PY))
+        scripts_backed_up.append(constants.SETUP_PY)
+
+    template.copy_setup_scripts(dot_uip_dir)
+
+    msg = '{0} and {1} have been '.format(constants.SETUP_CFG,
+                                                    constants.SETUP_PY)
+    if len(scripts_backed_up) > 0:
+        msg += 'upgraded (original files were backed up in {} folder)'.format(
+            os.path.relpath(backup_folder)
+        )
+    else:
+        msg += 'added'
+
+    return msg
```

### Comparing `uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/extension.py` & `uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/extension.py`

 * *Files identical despite different names*

### Comparing `uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/src/templates/template.json` & `uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/src/templates/template.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904829641671747%*

 * *Differences: {"'events'": "{0: {'sysId': ''}}", "'fields'": "{0: {'sysId': ''}}", "'sysId'": "''"}*

```diff
@@ -23,15 +23,15 @@
     "events": [
         {
             "attributes": [],
             "attributesPolicy": "Prohibit Universal Event",
             "description": null,
             "label": "{{ event_name | replace('_', ' ') | title }}",
             "name": "{{ event_name }}",
-            "sysId": "{{ event_template_uuid }}",
+            "sysId": "",
             "ttl": 5
         }
     ],
     "exitCodeOutput": null,
     "exitCodeProcessing": "Success Exitcode Range",
     "exitCodeProcessingFieldsRestriction": "No Restriction",
     "exitCodeText": null,
@@ -71,15 +71,15 @@
             "requireIfField": null,
             "requireIfFieldValue": null,
             "requireIfVisible": false,
             "required": false,
             "sequence": 0,
             "showIfField": null,
             "showIfFieldValue": null,
-            "sysId": "{{ sleep_field_uuid }}",
+            "sysId": "",
             "textType": "Plain"
         }
     ],
     "logLevel": "Inherited",
     "minReleaseLevel": "7.0.0.0",
     "name": "{{ universal_template_name }}",
     "outputConditionOperator": "=",
@@ -97,13 +97,13 @@
     "retainSysIds": true,
     "runtimeDir": null,
     "script": null,
     "scriptTypeWindows": null,
     "scriptUnix": null,
     "scriptWindows": null,
     "sendVariables": "None",
-    "sysId": "{{ universal_template_uuid }}",
+    "sysId": "",
     "templateType": "Extension",
     "useCommonScript": false,
     "variablePrefix": "ext",
     "waitForOutput": false
 }
```

### Comparing `uip-cli-1.3.0/uip/uiptemplates/eventtemplates/ue-publisher/template_config.yml` & `uip-cli-2.0.0/uip/uiptemplates/eventtemplates/ue-publisher/template_config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-template_description: starter Extension with a local Universal Event template
+name: ue-publisher
 
-files_to_template:
-  - src/extension.py
-  - src/extension.yml
-  - src/templates/template.json
+version: 1.0.0
 
-resources_to_include:
-  - setupscripts/setup.cfg
-  - setupscripts/setup.py
+description: starter Extension with a local Universal Event template
 
-user_defined_variables:
-  - extension_name:
-      default: ue-publisher
-      description: Extension name
-  - extension_version:
-      default: "1.0.0"
-      description: Extension version
-  - extension_api_level:
-      default: "1.2.0"
-      description: Extension API level
-  - extension_requires_python:
-      default: ">=2.6"
-      description: Extension Python requirement
-  - owner_name:
-      default: Stonebranch
-      description: Extension owner's name
-  - owner_organization:
-      default: Stonebranch Inc.
-      description: Extension owner's organization
-  - universal_template_name:
-      default: UE Publisher
-      description: Universal Template name
-  - event_name:
-      default: publisher_event
-      description: Local Universal Event name
+files_to_template:
+    - src/extension.py
+    - src/extension.yml
+    - src/templates/template.json
 
-internal_variables:
-  - uuid_variables:
-      - sleep_field_uuid
-      - universal_template_uuid
-      - event_template_uuid
+variables:
+    extension_name:
+        default: ue-publisher
+        description: Extension name
+    extension_version:
+        default: "1.0.0"
+        description: Extension version
+    extension_api_level:
+        default: "1.4.0"
+        description: Maximum supported extension API level
+    extension_requires_python:
+        default: ">=2.6"
+        description: Extension Python requirement
+    zip_safe:
+        default: true
+        description: Describes whether the extension will be run from the zip archive or extracted to a folder (true = zip, false = extract)
+    owner_name:
+        default: Stonebranch
+        description: Extension owner's name
+    owner_organization:
+        default: Stonebranch Inc.
+        description: Extension owner's organization
+    universal_template_name:
+        default: UE Publisher
+        description: Universal Template name
+    event_name:
+        default: publisher_event
+        description: Local Universal Event name
```

### Comparing `uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/extension.py` & `uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/extension.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,15 +29,20 @@
         ExtensionResult
             once the work is done, an instance of ExtensionResult must be
             returned. See the documentation for a full list of parameters that
             can be passed to the ExtensionResult class constructor
         """
 
         # Get the value of the 'action' field
-        action = fields.get('action', [""])[0]
+        action_field = fields.get('action', [])
+        if len(action_field) != 1:
+            # 'action' field was not specified or is invalid
+            action = ''
+        else:
+            action = action_field[0]
 
         if action.lower() == 'print':
             # Print to standard output...
             print("Hello STDOUT!")
         else:
             # Log to standard error...
             logger.info('Hello STDERR!')
```

### Comparing `uip-cli-1.3.0/uip/uiptemplates/tasktemplates/ue-task/src/templates/template.json` & `uip-cli-2.0.0/uip/uiptemplates/tasktemplates/ue-task/src/templates/template.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907739557739558%*

 * *Differences: {"'fields'": "{0: {'choices': {0: {'sysId': ''}, 1: {'sysId': ''}}, 'sysId': ''}}", "'sysId'": "''"}*

```diff
@@ -40,22 +40,22 @@
             "choiceFields": [],
             "choiceSortOption": "Sequence",
             "choices": [
                 {
                     "fieldValue": "print",
                     "fieldValueLabel": "Print to STDOUT",
                     "sequence": 0,
-                    "sysId": "{{ print_choice_field_uuid }}",
+                    "sysId": "",
                     "useFieldValueForLabel": false
                 },
                 {
                     "fieldValue": "log",
                     "fieldValueLabel": "Log to STDERR",
                     "sequence": 1,
-                    "sysId": "{{ log_choice_field_uuid }}",
+                    "sysId": "",
                     "useFieldValueForLabel": false
                 }
             ],
             "defaultListView": false,
             "fieldLength": null,
             "fieldMapping": "Choice Field 1",
             "fieldRestriction": "No Restriction",
@@ -75,15 +75,15 @@
             "requireIfField": null,
             "requireIfFieldValue": null,
             "requireIfVisible": false,
             "required": false,
             "sequence": 1,
             "showIfField": null,
             "showIfFieldValue": null,
-            "sysId": "{{ action_field_uuid }}",
+            "sysId": "",
             "textType": "Plain"
         }
     ],
     "logLevel": "Inherited",
     "minReleaseLevel": "7.0.0.0",
     "name": "{{ universal_template_name }}",
     "outputConditionOperator": "=",
@@ -100,13 +100,13 @@
     "outputType": "STDOUT",
     "retainSysIds": true,
     "runtimeDir": null,
     "script": null,
     "scriptTypeWindows": null,
     "scriptUnix": null,
     "scriptWindows": null,
-    "sysId": "{{ universal_template_uuid }}",
+    "sysId": "",
     "templateType": "Extension",
     "useCommonScript": false,
     "variablePrefix": "ext",
     "waitForOutput": false
 }
```

### Comparing `uip-cli-1.3.0/uip/utils/custom_io.py` & `uip-cli-2.0.0/uip/utils/custom_io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import glob
 import hashlib
 import json
 import os
 import shutil
+import tempfile
 import io
 import zipfile
+import stat
 from distutils import dir_util
 
 import yaml
 
 
 def read_yaml(filepath):
     if os.path.exists(filepath):
@@ -42,15 +44,16 @@
     print(message)
     for index, value in enumerate(choice_list):
         print(('  (%d) %s' % ((index + 1), value)))
     print('')
 
     user_choice = -1
     while user_choice < 1 or user_choice > len(choice_list):
-        user_choice = read_user_input('Please type the number of one of the choices presented above: ')
+        user_choice = read_user_input(
+            'Please type the number of one of the choices presented above: ')
         try:
             user_choice = int(user_choice)
         except ValueError:
             user_choice = -1
             pass
 
     return choice_list[user_choice - 1]
@@ -100,42 +103,89 @@
 def extract_zip(zip_filepath, extract_dir):
     with zipfile.ZipFile(zip_filepath, 'r') as zf:
         zf.extractall(extract_dir)
 
 
 def remove_dir(dir):
     if os.path.exists(dir):
-        shutil.rmtree(dir)
+        def handle_error(func, path, exec_info):
+            os.chmod(path, stat.S_IWUSR)
+
+            try:
+                func(path)
+            except Exception as ex:
+                raise
+
+        shutil.rmtree(dir, False, handle_error)
 
 
 def remove_file(file):
     if os.path.exists(file):
         os.remove(file)
 
 
 def copy_tree(src, dst):
     if os.path.exists(src):
+        dir_util._path_created = {}
         dir_util.copy_tree(src, dst)
 
 
 def copy_file(src, dst):
     if os.path.exists(src) and os.path.isfile(src):
         shutil.copy(src, dst)
 
+
 def write_to_file(dst_file, contents):
     with io.open(dst_file, 'wb+') as f:
         f.write(contents.encode('utf-8'))
 
+
 def make_dir(dirpath):
     if not os.path.exists(dirpath):
         os.makedirs(dirpath)
 
+
 def get_dir_listing(dirpath):
     if os.path.exists(dirpath):
         dir_listing = []
         for path, _, files in os.walk(dirpath):
             for name in files:
                 dir_listing.append(os.path.join(path, name))
 
         return dir_listing
     else:
-        return []
+        return []
+
+
+def get_zip_listing(zip_filepath):
+    if not os.path.exists(zip_filepath):
+        return []
+
+    try:
+        with zipfile.ZipFile(zip_filepath, 'r') as z:
+            return z.namelist()
+    except zipfile.error:
+        return []
+
+
+def get_temp_dir(prefix=None):
+    return tempfile.mkdtemp(prefix=prefix)
+
+
+def zip_directory(filename, dirpath, include_parent=False):
+    if not os.path.exists(dirpath) or len(os.listdir(dirpath)) == 0:
+        return False
+
+    def zipdir(path, zip_handle):
+        for root, _, files in os.walk(path):
+            for f in files:
+                zip_handle.write(os.path.join(root, f),
+                        os.path.relpath(os.path.join(root, f),
+                        os.path.join(path, '..') if include_parent else path))
+
+    if not filename.endswith('.zip'):
+        filename += '.zip'
+
+    with zipfile.ZipFile(filename, 'w', zipfile.ZIP_DEFLATED) as zipf:
+        zipdir(dirpath, zipf)
+
+    return True
```

### Comparing `uip-cli-1.3.0/uip_cli.egg-info/PKG-INFO` & `uip-cli-2.0.0/uip_cli.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uip-cli
-Version: 1.3.0
+Version: 2.0.0
 Summary: Universal Extension CLI for interfacing with Controller Web Services
 Home-page: UNKNOWN
 Author: Stonebranch
 License: GNU General Public License
 Description: Universal Integration Platform Command Line Utility
         ===================================================
         
@@ -14,33 +14,35 @@
         to interface with the Universal Extension Web Service APIs. The goal of
         the CLI is to make the process of creating, editing, and deploying
         Extensions convenient and fast.
         
         Features
         --------
         
-        -  Quickly prototype Extensions using starter Extension Templates
+        -  Quickly prototype Extensions using starter (or custom) Extension Templates
         -  Build and upload Extensions and/or Universal Templates
         -  Pull the latest Universal Template source files from the Controller
         -  Download the full Universal Template package 
         
         Getting Started
         ===============
         Requirements
         ------------
         
-        ``uip-cli`` works with Python 2.7 and greater on Windows, Linux, and
+        ``uip-cli`` works with Python 3.6 and greater on Windows, Linux, and
         MacOS, and uses the following third party libraries:
         
+        - ``jsonschema`` (3.2.0)
         - ``colorama`` (0.4.4)
         - ``requests`` (2.26.0) 
         - ``jinja2`` (2.11.3) 
         - ``prettytable`` (1.0.1)
         - ``pyyaml`` (5.4.1)
         - ``setuptools`` (44.1.1)
+        - ``wheel`` (0.37.1)
         
         All the required libraries listed above are automatically installed
         during the installation process
         
         Installation
         ------------
         
@@ -77,71 +79,80 @@
             usage: uip [-h] <command> ...
         
             optional arguments:
             -h --help
                             show this help message and exit
         
             commands:
-            <command>
+              <command>
                 init         initialize a new project with starter Extension templates
-                template-list
-                             list of available Extension templates
+                template     used to perform actions on built-in (and external) templates
                 build        used to build Extension or full package
                 upload       upload Extension (or full package) to the Controller
                 push         build and upload Extension (or full package) to the Controller
                 pull         pulls the latest template.json (and template_icon.png, if
-                             present)
+                            present)
                 download     downloads the full Universal Template package
                 clean        used to purge build artifacts
                 task         used to perform actions on Universal Extension tasks
+                template-list
+                            list of available Extension templates. Note: this command will
+                            be deprecated in two releases
         
             examples:
             uip <command>
             uip init
             uip download
         
         Basic Usage 
         ===========
         ``uip-cli`` currently supports the following commands:
         
         - init 
-        - template-list
+        - template
+        
+          - list
+          - add
+          - delete
+          - export
         - build 
         - upload 
         - push 
         - pull 
         - download
         - clean
         - task
         
           - launch
           - status   
           - output
+        - template-list (will be deprecated in two releases. replaced by the ``template list`` command)
+        
         
         A brief overview of each of the commands is provided below along with 
-        some examples. For a more detailed demonstration of the commands, 
-        refer to the 'How-To/Getting Started' Document. 
+        some examples. It is highly recommended to go through the `Extension Development <https://docs.stonebranch.com/confluence/display/UC73/Extension+Development>`_
+        document for a more detailed demonstration.
         
         ``init`` 
         --------
-        This command is used to initialize a new project using one of the provided 
-        starter Extension templates. It can also be used to initialize an existing,
-        *partially valid* Extension project.
+        This command is used to initialize a new project using a custom, user-specified
+        template or one of the provided starter Extension templates. It can also be used
+        to initialize an existing, *partially valid* Extension project.
         
         **To initialize a brand new project using a starter Extension template, issue the 
         following command**:
         :: 
         
             $ uip init -t ue-task -e 'extension_name=my_sample_extension'
         
         
         - The ``-t`` option accepts the name of the starter Extension template. For a full 
-          list of the available Extension templates, see the ``template-list`` command below. 
+          list of the available Extension templates, see the ``template list`` command below. 
         - The ``-e`` option is used to configure the starter Extension template with user-defined 
-          variables. See the ``template-list`` command for instructions on obtaining 
+          variables. See the ``template list`` command for instructions on obtaining 
           a full list of configurable variables. 
         
         Once the CLI executes the command, a project will be initialized in the current 
         working directory with the following structure:
         ::
         
             |   setup.cfg
@@ -173,44 +184,229 @@
         
         :: 
         
             $ uip init 
         
         The CLI will first check to make sure ``extension.py``, ``extension.yml``, and ``template.json``
         exist in their respective directories shown above. If so, the CLI will create the ``.uip`` folder.
-        Additionally, if ``setup.py`` and ``setup.cfg`` are not present, they will be created along with the
-        ``.uip`` folder.
+        Additionally, if ``setup.py`` and ``setup.cfg`` are not present, they will be
+        created along with the ``.uip`` folder.
+        
+        **How to create a custom/configurable Extension template**:
+        
+        The CLI is equipped with two built-in, configurable Extension templates:
+        ``ue-task`` and ``ue-publisher``. These two templates may not be enough for some
+        users. To get around this, the CLI supports initializing from external, user-built
+        Extension templates. 
+        
+        This section will outline the basic requirements for creating a custom, configurable
+        Extension template.
+        
+        Assuming a folder named ``my_template`` exists, it must contain (at minimum) the following
+        files/folders to be considered a valid Extension template:
+        
+        ::
+        
+            my_template
+            â”œâ”€â”€ template_config.yml
+            â””â”€â”€ src/
+                â”œâ”€â”€ extension.py
+                â”œâ”€â”€ extension.yml
+                â””â”€â”€ templates/
+                    â””â”€â”€ template.json 
+        
+        Aside from the usual Extension related files, ``template_config.yml`` is also needed to make
+        the template configurable. 
+        
+        The file must contain:
+        
+        - ``name``: a string that identifies the name of the template (this is NOT referring to the Universal Template name).
+        - ``version``: a string that identifies the template version. Not restricted to ``x.y.z`` (SemVer); it could be anything (e.g. ``v1``). 
+        - ``description``: a string describing the template.
+        
+        and can optionally contain:
+        
+        - ``files_to_template``: an array containing paths to files that will be "templated" using ``Jinja2``. All files must be specified relative to ``template_config.yml``.
+        - ``variables``: a mapping/dictionary of variables that will be substituted in the relevant files specified by ``files_to_template``. The value of each key/variable is another mapping/dictionary that must contain ``default`` and ``description``.
+        
+        Shown below is a sample ``template_config.yml``:
+        
+        ::
+        
+            name: my_template
+        
+            version: 1.0.0
+        
+            description: this is the description for my_template
+        
+            files_to_template: 
+              - src/extension.py
+              - src/templates/template.json
+        
+            variables:
+              msg:
+                default: test_message
+                description: message to print to STDOUT and STDERR
+              log_level:
+                default: Info
+                description: Universal Template Log Level 
+        
+        As mentioned, the CLI uses the ``Jinja2`` module to substitute the variables in each file from ``files_to_template``. For instance,
+        if ``src/extension.py`` or ``src/templates/template.json`` mention ``{{ msg }}`` or ``{{ log_level }}``, the entirety of
+        ``{{ msg }}``/``{ log_level }}`` will be replaced with the user-specified value (or the default, if nothing is specified).
+        
+        Once the custom Extension template is created, it can be zipped up or pushed out to a Git repository. The CLI supports initializing from both
+        of these ways, which makes the custom template easy to distribute. The next section will outline the details regarding this functionality.
+        
+        **Packaging custom-built Extension Templates**:
+        
+        Once a custom template has been created, it must be packaged into either a
+        zip file or a Git repository.
+        
+        Shown below is the structure of a valid, custom template zip called ``my_template.zip``:
+        
+        ::
+        
+            my_template.zip
+            â”œâ”€â”€ template_config.yml
+            â””â”€â”€ src/
+                â”œâ”€â”€ extension.py
+                â”œâ”€â”€ extension.yml
+                â””â”€â”€ templates/
+                    â””â”€â”€ template.json 
+        
+        The custom template can also be pushed out to a Git repository. In this case, the zip file
+        won't be part of the repository. In other words, the top-level file and folder should be ``template_config.yml``
+        and ``src/``, respectively.
+        
+        **Initializing a custom-built Extension Template**:
+        
+        Assuming a custom template has been packaged based on the guidelines from the previous
+        section, it is ready to be used!
+        
+        The CLI supports initializing custom-built templates from:
+        
+        - a zip file
+        - a http(s) link to a zip file
+        - a Git repository
+        
+        **Initializing from a zip file**:
+        
+        To initialize the template zip without saving it:
+        ::
+        
+            $ uip init -t <path to zip file>
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t <path to zip file> --save
+        
+        Once saved, the template will be available in the ``template list`` command. At this point, the template can be
+        initialized similarly to ``ue-task`` and ``ue-publisher``.
         
+        **Initializing from a http(s) link**:
         
-        ``template-list`` 
+        The CLI supports initializing from both HTTP and HTTPS links that point to a zip file (link normally ends in .zip).
+        
+        It also supports basic authentication. The syntax is ``http://<username>:<password>@<actual url>`` (applies to HTTPS as well). For instance, if the url is ``http://mytestserver/test/my_template.zip``, the username is ``testuser``, and password is ``testpwd``, the formatted URL would be ``http://testuser:testpwd@mytestserver/test/my_template.zip``.
+        
+        To initialize the template without saving it:
+        ::
+        
+            $ uip init -t <link to http(s) url>
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t <link to http(s) url> --save
+        
+        **Initializing from a Git repository**:
+        
+        The CLI also supports initializing directly from a Git repository (similar to how pip installs work from a Git repo). The repo should not contain the zip file, just the raw files/folders that make up the template.
+        
+        The CLI relies on Git being installed on the system. If it is not, the CLI will issue an error.
+        
+        Both SSH and HTTPS protocols are supported.
+        
+        For HTTPS protocol, the url must start with ``git+`` followed by the HTTPS clone url. For instance, if the HTTPS Clone URL is ``https://gitlab-tst.com/test/templates/my_template.git``, then the syntax:
+        
+        To initialize the template without saving it:
+        ::
+        
+            $ uip init -t git+https://gitlab-tst.com/test/templates/my_template.git
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t git+https://gitlab-tst.com/test/templates/my_template.git --save
+        
+        If the repository is private and requires a username and access token to clone it, the URL should be specified as: ``git+https://<USERNAME>:<ACCESS TOKEN>@gitlab-tst.com/test/templates/my_template.git``.
+        
+        
+        For the SSH protocol, the url must start with ``git+`` followed by the SSH clone url. For instance, if the SSH Clone URL is ``git@gitlab-tst.com:test/templates/my_template.git``, then the syntax:
+        
+        To initialize the template without saving it:
+        ::
+        
+            $ uip init -t git+git@gitlab-tst.com:test/templates/my_template.git
+        
+        To initialize and save the template zip:
+        ::
+        
+            $ uip init -t git+git@gitlab-tst.com:test/templates/my_template.git --save
+        
+        The CLI also supports cloning a specific branch/commit/tag. This can be done by appending the branch/commit SHA/tag at the end of the URL using ``@branch``, ``@commit``, or ``@tag``. For instance, to clone
+        
+        a branch named ``test1``
+        ::
+        
+            HTTPS URL: git+https://gitlab-tst.com/test/templates/my_template.git@branch:test1
+            SSH URL: git+git@gitlab-tst.com:test/templates/my_template.git@branch:test1
+        
+        a commit with SHA ``9ab454ef``:
+        ::
+        
+            HTTPS URL: git+https://gitlab-tst.com/test/templates/my_template.git@commit:9ab454ef
+            SSH URL: git+git@gitlab-tst.com:test/templates/my_template.git@commit:9ab454ef
+        
+        a tag named ``v1``:
+        ::
+        
+            HTTPS URL: git+https://gitlab-tst.com/test/templates/my_template.git@tag:v1
+            SSH URL: git+git@gitlab-tst.com:test/templates/my_template.git@tag:v1
+        
+        
+        ``template`` 
         -----------------
-        This command is used to list all the available starter Extension templates as well as 
-        the variables used to configure the templates. 
+        This command is used to perform actions on all the available, custom-built and 
+        starter Extension templates. As of now, four actions/subcommands are supported: 
+        ``list``, ``add``, ``delete``, and ``export``.
         
         To see the list of available templates, type the following:
         ::
         
-            $ uip template-list 
+            $ uip template list
         
         Something similar to the output below should be shown:
         :: 
         
-            +--------------------+---------------------------------------------------------+
-            | Extension Template | Description                                             |
-            +--------------------+---------------------------------------------------------+
-            | ue-publisher       | starter Extension with a local Universal Event template |
-            +--------------------+---------------------------------------------------------+
-            | ue-task            | starter Extension with minimal code                     |
-            +--------------------+---------------------------------------------------------+
+            +--------------------+---------+---------------------------------------------------------+
+            | Extension Template | Version | Description                                             |
+            +--------------------+---------+---------------------------------------------------------+
+            | ue-task            | 1.0.0   | starter Extension with minimal code                     |
+            +--------------------+---------+---------------------------------------------------------+
+            | ue-publisher       | 1.0.0   | starter Extension with a local Universal Event template |
+            +--------------------+---------+---------------------------------------------------------+
         
         To see the list of configurable variables for one of the templates shown above, 
         type the following (same process applies to ``ue-publisher``): 
         :: 
         
-            $ uip template-list ue-task 
+            $ uip template list ue-task 
         
         and a table of variables will be shown: 
         :: 
         
             +---------------------------+------------------+--------------------------------+
             | Variable Name             | Default          | Description                    |
             +---------------------------+------------------+--------------------------------+
@@ -220,31 +416,71 @@
             | extension_requires_python | >=2.6            | Extension Python requirement   |
             | owner_name                | Stonebranch      | Extension owner's name         |
             | owner_organization        | Stonebranch Inc. | Extension owner's organization |
             | universal_template_name   | UE Task          | Universal Template name        |
             +---------------------------+------------------+--------------------------------+
         
         
+        To add a custom-built Extension template:
+        :: 
+        
+            $ uip template add <path to zip / link to zip / link to Git repository>
+        
+        Similar to the ``init`` command, the ``template add`` command also supports
+        adding/saving custom-built templates from:
+        
+        - a zip file
+        - a http(s) link to a zip file
+        - a Git repository
+        
+        In fact, it does so in the same exact manner. See the ``init`` section for details.
+        
+        Once the template is added, it will be available for use just like ``ue-task``
+        and ``ue-publisher``.
+        
+        
+        To delete a custom-built Extension template:
+        :: 
+        
+            $ uip template delete <template name>
+        
+        
+        To export an Extension template:
+        :: 
+        
+            $ uip template export <template name>
+        
+        
         ``build`` 
         ---------
-        This command is used to build an Extension or the full package.
-        
+        This command is used to build an Extension or the full package. 
         A full package build consists of the Universal Template and the Extension. 
         
+        The command also supports building extensions with third-party Python packages.
+        To do so, create a file called ``requirements.txt`` in the Extension folder.
+        Running ``uip build`` will then create a ``3pp`` folder, install all PyPi packages
+        specified in ``requirements.txt`` to ``3pp``, and package it in the extension zip
+        (or the full package).
+        
         
         To build the Extension only:
         :: 
         
             $ uip build 
         
         To build the full package:
         :: 
         
             $ uip build -a 
         
+        To build the dependency wheel file only:
+        :: 
+        
+            $ uip build -d
+        
         
         ``upload`` 
         ----------
         This command is used to upload an Extension or the full package to the 
         Controller. 
         
         To upload the Extension only:
@@ -329,14 +565,19 @@
         (including the folders themselves).
         
         To purge the build artifacts:
         :: 
         
             $ uip clean
         
+        Optionally, it is also possible to purge the 3pp folder (if it exists) using:
+        :: 
+        
+            $ uip clean --all
+        
         
         ``task``
         ------------
         This command is used to perform actions on Universal Extension tasks. 
         As of now, three actions/subcommands are supported: ``launch``, ``status``, 
         and ``output`` which allow the CLI to launch, get status, and get output of
         Universal Extension tasks. 
@@ -485,14 +726,28 @@
            * - Variables 
              - ``-e``
              - ``--variables``
              - UIP_TEMPLATE_VARIABLES 
              - variables 
              - NO 
              - None 
+           * - Save
+             - ``-s``
+             - ``--save``
+             - None
+             - None
+             - NO 
+             - False 
+           * - Upgrade
+             - ``-u``
+             - ``--upgrade``
+             - None
+             - None
+             - NO
+             - False
         
         
         Values for the **variables** option can be specified in three different ways:
         
         - Using the ``-e`` option multiple times:
           ::
         
@@ -529,30 +784,94 @@
              - NO 
              - Current Working Directory 
              - Where to initialize the Extension template. For example, in the following command:
                ``uip init -t ue-task -e '@vars.yml' my_extension_dir``, ``my_extension_dir`` is 
                where the ``ue-task`` Extension template will be initialized.
         
         
-        ``template-list`` command options  
+        ``template list`` command options  
         ---------------------------------
         .. list-table:: Positional Arguments 
            :header-rows: 1
         
            * - Option Name 
              - Required 
              - Default
              - Description
            * - <extension template name> 
              - NO 
              - None 
              - The name of the Extension template to get more details of. For example, in the 
-               following command: ``uip template-list ue-task``, ``ue-task`` is the value of 
+               following command: ``uip template list ue-task``, ``ue-task`` is the value of 
                ``<extension template name>``. 
         
+        .. list-table:: Optional Arguments 
+           :header-rows: 1
+        
+           * - Option Name
+             - Short Arg
+             - Long Arg
+             - Environment Variable
+             - Configuration File Arg
+             - Required
+             - Default
+           * - JSON
+             - ``-j``
+             - ``--json``
+             - None
+             - None
+             - NO
+             - False
+        
+        
+        ``template add`` command options  
+        --------------------------------
+        .. list-table:: Positional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Required 
+             - Default
+             - Description
+           * - <extension template> 
+             - YES 
+             - None 
+             - The name of the Extension template to add. Valid values include path to a zip
+               file, HTTP(S) url pointing to a zip file, or a Git repository clone url.
+        
+        
+        ``template delete`` command options  
+        -----------------------------------
+        .. list-table:: Positional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Required 
+             - Default
+             - Description
+           * - <extension template> 
+             - YES 
+             - None 
+             - The name of the Extension template to delete
+        
+        
+        ``template export`` command options  
+        -----------------------------------
+        .. list-table:: Positional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Required 
+             - Default
+             - Description
+           * - <extension template> 
+             - YES 
+             - None 
+             - The name of the Extension template to export
+        
         
         ``build`` command options  
         -------------------------
         .. list-table:: Optional Arguments 
            :header-rows: 1
         
            * - Option Name 
@@ -565,14 +884,21 @@
            * - Build All  
              - ``-a``
              - ``--all``
              - UIP_BUILD_ALL 
              - build-all 
              - NO 
              - False
+           * - Build Dependency Wheel Only 
+             - ``-d``
+             - ``--dep-whl-only``
+             - UIP_BUILD_DEPENDENCY_WHEEL_ONLY 
+             - dep-whl-only 
+             - NO 
+             - False
         
         
         ``upload`` command options  
         --------------------------
         .. list-table:: Optional Arguments 
            :header-rows: 1
         
@@ -630,14 +956,35 @@
              - ``--template-name``
              - UIP_TEMPLATE_NAME 
              - template-name 
              - NO 
              - Name from ``template.json``
         
         
+        ``clean`` command options  
+        -------------------------
+        .. list-table:: Optional Arguments 
+           :header-rows: 1
+        
+           * - Option Name 
+             - Short Arg 
+             - Long Arg
+             - Environment Variable
+             - Configuration File Arg 
+             - Required 
+             - Default
+           * - Clean All  
+             - ``-a``
+             - ``--all``
+             - UIP_CLEAN_ALL 
+             - clean-all 
+             - NO 
+             - False
+        
+        
         ``task launch`` command options  
         -------------------------------
         .. list-table:: Positional Arguments 
            :header-rows: 1
           
            * - Option Name 
              - Required 
@@ -739,23 +1086,23 @@
         Acknowledgements
         ================
         ``uip-cli`` acknowledges the use of the following open source Python modules:
         
         - `colorama <https://pypi.org/project/colorama/>`_ (BSD License)
         - `Jinja2 <https://pypi.org/project/Jinja2/>`_ (BSD-3-Clause License)
         - `prettytable <https://pypi.org/project/prettytable/>`_ (BSD-3-Clause License)
+        - `jsonschema <https://pypi.org/project/jsonschema/>`_ (MIT)
         - `PyYAML <https://pypi.org/project/PyYAML/>`_ (MIT)
         - `requests <https://pypi.org/project/requests/>`_ (Apache 2.0)
         - `setuptools <https://pypi.org/project/setuptools/>`_ (MIT)
         
         Copyright
         =========
-        Copyright (c) 2022. Stonebranch, Inc. All rights reserved.
+        Copyright (c) 2023. Stonebranch, Inc. All rights reserved.
         
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uip-cli-1.3.0/uip_cli.egg-info/SOURCES.txt` & `uip-cli-2.0.0/uip_cli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 uip/uipproject/__init__.py
 uip/uipproject/uipproject.py
 uip/uiptemplates/__init__.py
 uip/uiptemplates/template.py
 uip/uiptemplates/__pycache__/__init__.cpython-36.pyc
 uip/uiptemplates/__pycache__/template.cpython-36.pyc
 uip/uiptemplates/eventtemplates/ue-publisher/__init__.py
+uip/uiptemplates/eventtemplates/ue-publisher/requirements.txt
 uip/uiptemplates/eventtemplates/ue-publisher/template_config.yml
 uip/uiptemplates/eventtemplates/ue-publisher/src/__init__.py
 uip/uiptemplates/eventtemplates/ue-publisher/src/extension.py
 uip/uiptemplates/eventtemplates/ue-publisher/src/extension.yml
 uip/uiptemplates/eventtemplates/ue-publisher/src/templates/template.json
 uip/uiptemplates/resources/setupscripts/__init__.py
 uip/uiptemplates/resources/setupscripts/setup.cfg
 uip/uiptemplates/resources/setupscripts/setup.py
 uip/uiptemplates/tasktemplates/ue-task/__init__.py
+uip/uiptemplates/tasktemplates/ue-task/requirements.txt
 uip/uiptemplates/tasktemplates/ue-task/template_config.yml
 uip/uiptemplates/tasktemplates/ue-task/src/__init__.py
 uip/uiptemplates/tasktemplates/ue-task/src/extension.py
 uip/uiptemplates/tasktemplates/ue-task/src/extension.yml
 uip/uiptemplates/tasktemplates/ue-task/src/templates/template.json
 uip/utils/__init__.py
 uip/utils/custom_io.py
```

