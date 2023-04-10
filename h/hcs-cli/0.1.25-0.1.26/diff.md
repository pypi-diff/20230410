# Comparing `tmp/hcs-cli-0.1.25.tar.gz` & `tmp/hcs-cli-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.25.tar", last modified: Sat Apr  8 01:22:38 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.26.tar", last modified: Mon Apr 10 19:18:24 2023, max compression
```

## Comparing `hcs-cli-0.1.25.tar` & `hcs-cli-0.1.26.tar`

### file list

```diff
@@ -1,112 +1,124 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.727365 hcs-cli-0.1.25/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.25/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.25/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)      701 2023-04-08 01:22:34.000000 hcs-cli-0.1.25/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)     1963 2023-04-08 01:22:38.726840 hcs-cli-0.1.25/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1194 2023-04-06 16:09:03.000000 hcs-cli-0.1.25/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.659927 hcs-cli-0.1.25/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     1963 2023-04-08 01:22:38.000000 hcs-cli-0.1.25/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2444 2023-04-08 01:22:38.000000 hcs-cli-0.1.25/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-08 01:22:38.000000 hcs-cli-0.1.25/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-08 01:22:38.000000 hcs-cli-0.1.25/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:22:38.000000 hcs-cli-0.1.25/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-08 01:22:38.000000 hcs-cli-0.1.25/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.25/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:21:33.000000 hcs-cli-0.1.25/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-08 01:22:38.727485 hcs-cli-0.1.25/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      526 2023-04-08 01:21:49.000000 hcs-cli-0.1.25/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.662408 hcs-cli-0.1.25/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.25/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.25/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.25/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.663742 hcs-cli-0.1.25/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.25/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.664509 hcs-cli-0.1.25/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.25/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.667535 hcs-cli-0.1.25/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.25/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.669384 hcs-cli-0.1.25/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.25/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.25/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.25/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.25/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.25/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.670063 hcs-cli-0.1.25/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.25/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.671345 hcs-cli-0.1.25/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.674070 hcs-cli-0.1.25/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/cli/cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.25/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.675853 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.679335 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      129 2023-04-07 18:26:44.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.684406 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      504 2023-04-08 00:00:05.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      352 2023-04-07 18:24:18.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:57:03.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      380 2023-04-07 21:03:52.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1260 2023-04-07 18:57:03.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.25/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.689436 hcs-cli-0.1.25/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.25/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.25/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.25/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.25/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.25/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.25/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.690819 hcs-cli-0.1.25/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-04-08 01:06:36.000000 hcs-cli-0.1.25/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.25/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.694121 hcs-cli-0.1.25/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.25/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.25/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.25/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.25/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2109 2023-04-07 19:12:05.000000 hcs-cli-0.1.25/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.695701 hcs-cli-0.1.25/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.707724 hcs-cli-0.1.25/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      115 2023-04-07 23:27:53.000000 hcs-cli-0.1.25/vhcs/common/ctxp/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.710839 hcs-cli-0.1.25/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.25/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1817 2023-04-08 01:12:13.000000 hcs-cli-0.1.25/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4097 2023-04-08 01:06:36.000000 hcs-cli-0.1.25/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/common/ctxp/cli_state.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.25/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.25/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.25/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.25/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3695 2023-04-08 01:06:36.000000 hcs-cli-0.1.25/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1260 2023-04-08 01:02:30.000000 hcs-cli-0.1.25/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.25/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.25/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.716709 hcs-cli-0.1.25/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.25/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.25/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3811 2023-04-07 19:16:27.000000 hcs-cli-0.1.25/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.25/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-07 00:40:33.000000 hcs-cli-0.1.25/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.718894 hcs-cli-0.1.25/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.25/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.722953 hcs-cli-0.1.25/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-07 21:33:14.000000 hcs-cli-0.1.25/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2538 2023-04-07 21:33:14.000000 hcs-cli-0.1.25/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.25/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.25/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-08 01:22:38.725760 hcs-cli-0.1.25/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.25/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.25/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.707967 hcs-cli-0.1.26/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.26/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.26/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)      701 2023-04-08 01:22:34.000000 hcs-cli-0.1.26/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)     1957 2023-04-10 19:18:24.707583 hcs-cli-0.1.26/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1188 2023-04-08 01:25:45.000000 hcs-cli-0.1.26/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.597969 hcs-cli-0.1.26/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     1957 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2738 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-10 19:18:24.000000 hcs-cli-0.1.26/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.26/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:21:33.000000 hcs-cli-0.1.26/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-10 19:18:24.708530 hcs-cli-0.1.26/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      544 2023-04-10 17:59:22.000000 hcs-cli-0.1.26/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.601120 hcs-cli-0.1.26/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.26/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.26/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.603270 hcs-cli-0.1.26/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.26/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.604548 hcs-cli-0.1.26/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.26/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.614493 hcs-cli-0.1.26/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.617700 hcs-cli-0.1.26/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.618803 hcs-cli-0.1.26/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.26/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.620694 hcs-cli-0.1.26/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.624157 hcs-cli-0.1.26/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.625572 hcs-cli-0.1.26/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.628937 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      343 2023-04-10 19:16:01.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.631383 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      351 2023-04-10 19:13:27.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1393 2023-04-10 17:45:24.000000 hcs-cli-0.1.26/vhcs/cli/cmds/admin/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.26/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.633484 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.637570 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      129 2023-04-07 18:26:44.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.644247 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      644 2023-04-10 18:54:41.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      352 2023-04-07 18:24:18.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-10 19:14:17.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      962 2023-04-10 19:04:36.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1260 2023-04-07 18:57:03.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.26/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.653177 hcs-cli-0.1.26/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.26/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.656115 hcs-cli-0.1.26/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.26/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.661446 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     1960 2023-04-10 18:54:37.000000 hcs-cli-0.1.26/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.664761 hcs-cli-0.1.26/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.678871 hcs-cli-0.1.26/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.26/vhcs/common/ctxp/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.682829 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1817 2023-04-08 01:12:13.000000 hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4097 2023-04-10 19:00:11.000000 hcs-cli-0.1.26/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/cli_state.py
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.26/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.26/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.26/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.26/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3695 2023-04-08 01:06:36.000000 hcs-cli-0.1.26/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-10 19:10:32.000000 hcs-cli-0.1.26/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.26/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.26/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.690491 hcs-cli-0.1.26/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.26/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.26/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3879 2023-04-10 18:18:13.000000 hcs-cli-0.1.26/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.26/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.26/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.694245 hcs-cli-0.1.26/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.26/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.702797 hcs-cli-0.1.26/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-10 16:58:33.000000 hcs-cli-0.1.26/vhcs/service/_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      822 2023-04-10 19:16:10.000000 hcs-cli-0.1.26/vhcs/service/admin.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2777 2023-04-10 18:36:25.000000 hcs-cli-0.1.26/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.26/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.26/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-10 19:18:24.705710 hcs-cli-0.1.26/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/util/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.26/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.26/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.26/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.25/.gitignore` & `hcs-cli-0.1.26/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/Makefile` & `hcs-cli-0.1.26/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/PKG-INFO` & `hcs-cli-0.1.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.25
+Version: 0.1.26
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
@@ -72,9 +72,9 @@
 hcs auth --details
 ```
 
 ### Examples
 
 Each service has its own sub-command. Take PKI service as example, to request a resource certificate:
 ```
-./bin/hcs pki sign-resource-cert my-res1
+hcs pki sign-resource-cert my-res1
 ```
```

### Comparing `hcs-cli-0.1.25/README.md` & `hcs-cli-0.1.26/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,9 +54,9 @@
 hcs auth --details
 ```
 
 ### Examples
 
 Each service has its own sub-command. Take PKI service as example, to request a resource certificate:
 ```
-./bin/hcs pki sign-resource-cert my-res1
+hcs pki sign-resource-cert my-res1
 ```
```

### Comparing `hcs-cli-0.1.25/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.26/hcs_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.25
+Version: 0.1.26
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
@@ -72,9 +72,9 @@
 hcs auth --details
 ```
 
 ### Examples
 
 Each service has its own sub-command. Take PKI service as example, to request a resource certificate:
 ```
-./bin/hcs pki sign-resource-cert my-res1
+hcs pki sign-resource-cert my-res1
 ```
```

### Comparing `hcs-cli-0.1.25/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.26/hcs_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 tests/vhcs/cli/cmds/pki/get_root_ca.py
 vhcs/__init__.py
 vhcs/cli/__init__.py
 vhcs/cli/main.py
 vhcs/cli/cmds/__init__.py
 vhcs/cli/cmds/auth.py
 vhcs/cli/cmds/upgrade.py
+vhcs/cli/cmds/admin/__init__.py
+vhcs/cli/cmds/admin/edge/__init__.py
+vhcs/cli/cmds/admin/edge/get.py
+vhcs/cli/cmds/admin/edge/list.py
+vhcs/cli/cmds/admin/template/__init__.py
+vhcs/cli/cmds/admin/template/get.py
+vhcs/cli/cmds/admin/template/list.py
 vhcs/cli/cmds/lcm/__init__.py
 vhcs/cli/cmds/lcm/test.py
 vhcs/cli/cmds/lcm/provider/__init__.py
 vhcs/cli/cmds/lcm/provider/delete.py
 vhcs/cli/cmds/lcm/provider/get.py
 vhcs/cli/cmds/lcm/provider/list.py
 vhcs/cli/cmds/lcm/template/__init__.py
@@ -75,13 +82,15 @@
 vhcs/common/sglib/ez_client.py
 vhcs/common/sglib/hcs_client.py
 vhcs/common/sglib/util.py
 vhcs/config/__init__.py
 vhcs/config/hcs-deployments.yaml
 vhcs/service/__init__.py
 vhcs/service/_util.py
+vhcs/service/admin.py
 vhcs/service/lcm.py
 vhcs/service/pki.py
 vhcs/service/vmhub.py
 vhcs/util/__init__.py
 vhcs/util/pki_util.py
+vhcs/util/query_util.py
 vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.25/pyproject.toml` & `hcs-cli-0.1.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/setup.py` & `hcs-cli-0.1.26/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
+VERSION = "0.1.26"
 
 def get_version():
-    version = "0.1.25"
+    version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
     return version
 
 
 setup(
```

### Comparing `hcs-cli-0.1.25/tests/test_utils.py` & `hcs-cli-0.1.26/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.26/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.26/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.26/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.26/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.26/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/redeem-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.26/vhcs/cli/cmds/vmhub/request-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/cli/main.py` & `hcs-cli-0.1.26/vhcs/cli/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 _script_dir = path.abspath(path.join(path.dirname(path.realpath(__file__)), "."))
 _module_dir = path.dirname(_script_dir)
 if __name__ == "__main__":
     _cli_dir = path.dirname(_module_dir)
     sys.path.append(_cli_dir)
 
 import vhcs.common.ctxp as ctxp
+from vhcs.common.ctxp.util import option_output, option_verbose
 
 # -----------------------------------------------------------
 import vhcs.common.logger as logger
 
 logger.setup()
 logging.getLogger("charset_normalizer").setLevel(logging.WARN)
 logging.getLogger("csp").setLevel(logging.INFO)
@@ -23,22 +24,16 @@
 logging.getLogger("init").setLevel(logging.WARN)
 logging.getLogger("profile").setLevel(logging.WARN)
 # -----------------------------------------------------------
 
 
 @click.group()
 @click.version_option(package_name="hcs-cli")
-@click.option("--verbose", "-v", count=True, default=False, help="Print details")
-@click.option(
-    "--output",
-    "-o",
-    type=click.Choice(["json", "json-compact", "yaml", "text"]),
-    default="json",
-    help="Specify output format",
-)
+@option_verbose
+@option_output
 @click.option("--profile", "-p", type=str, required=False, help="Specify the profile to use. Optional.")
 @click.option("--upgrade-check/--no-upgrade-check", default=True, help="Check new version of HCS CLI.")
 @click.option("--telemetry/--no-telemetry", default=True, help="Send telemetry")
 def cli(verbose: bool, output: str, profile: str, upgrade_check: bool, telemetry: bool):
 
     if upgrade_check:
         from vhcs.util.versions import check_upgrade
```

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.26/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 import json
+import yaml
 import sys
 import click
-import typing
 
 
 class CtxpException(Exception):
     pass
 
 
 def print_output(data: any, output: str = "json"):
     if type(data) is str:
         text = data
+    elif output == "json":
+        text = json.dumps(data, indent=4)
     elif output == "json-compact":
         text = json.dumps(data)
     elif output == "yaml":
-        import yaml
         import vhcs.common.ctxp as ctxp
-
         text = yaml.dump(ctxp.jsondot.plain(data))
     elif output == "text":
-        text = json.dumps(data, indent=4)
+        if isinstance(data, list):
+            text = ""
+            for i in data:
+                line = i if type(i) is str else json.dumps(i)
+                text += line + "\n"
+        elif isinstance(data, dict):
+            text = json.dumps(data, indent=4)
+        else:
+            text = json.dumps(data, indent=4)
     else:
-        text = json.dumps(data, indent=4)
+        raise Exception(f"Unexpected output format: {output}")
+    
     print(text, end="")
 
 
 def panic(reason: any = None, code: int = 1):
     print(reason, file=sys.stderr)
     sys.exit(code)
 
 
-F = typing.TypeVar("F", bound=typing.Callable[..., typing.Any])
-
-
-def command(
-    name: typing.Optional[str] = None,
-    cls: typing.Optional[typing.Type[click.Command]] = None,
-    **attrs: typing.Any,
-) -> typing.Callable[[F], click.Command]:
-    print("wrapping")
-    return click.command(name, cls, **attrs)
-
-
 option_verbose = click.option(
     "-v",
     "--verbose",
     count=True,
     default=0,
     help="Print debug logs",
 )
@@ -53,7 +50,15 @@
 option_output = click.option(
     "-o",
     "--output",
     type=click.Choice(["json", "json-compact", "yaml", "text"]),
     default="json",
     help="Specify output format",
 )
+
+option_id_only = click.option(
+    "--id-only/--full-object",
+    type=bool,
+    default=False,
+    required=False,
+    help="Output only the object, instead of the full data object"
+)
```

### Comparing `hcs-cli-0.1.25/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.26/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/logger.py` & `hcs-cli-0.1.26/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.26/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.26/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.26/vhcs/common/sglib/ez_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from http.client import HTTPResponse
 import httpx
+import sys
 import logging
 import json
 from vhcs.common.ctxp import jsondot
 
 log = logging.getLogger(__name__)
 
 log_http_details = False
 
 
 def _raise_on_4xx_5xx(response: httpx.Response):
-    response.read()  # read the content so the response can be dumped later
+    
+    if not response.is_success:
+        response.read()
+        if len(response.text) > 0:
+            text = _try_formatting_json(response.text)
+            print(text, file=sys.stderr)
+
     response.raise_for_status()
 
 
 def _try_formatting_json(text: str):
     try:
         return json.dumps(json.loads(text), indent=4)
     except:
@@ -69,15 +76,14 @@
         resp = func()
         return _parse_resp(resp)
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 404:
             return None
         raise
 
-
 class EzClient:
     def __init__(self, base_url: str, get_auth: callable = None) -> None:
         event_hooks = {"response": [_raise_on_4xx_5xx]}
         event_hooks["request"] = [_log_request]
         event_hooks["response"].insert(0, _log_response)
 
         self._client = httpx.Client(base_url=base_url, timeout=30, event_hooks=event_hooks)
@@ -97,36 +103,35 @@
 
     def get(self, url: str, raise_on_404: bool = False):
         self.login()
         try:
             resp = self._client.get(url)
             return _parse_resp(resp)
         except httpx.HTTPStatusError as e:
-            print(e)
-            if not raise_on_404 and e.response.status_code == 404:
-                return None
-            raise e
+            if e.response.status_code == 404 and raise_on_404:
+                raise e
 
     def patch(self, url: str, json: dict):
         self.login()
         resp = self._client.patch(url, json=json)
         return _parse_resp(resp)
+        
 
     def delete(self, url: str, raise_on_404: bool = False):
         self.login()
         try:
             return self._client.delete(url)
         except httpx.HTTPStatusError as e:
             if not raise_on_404 and e.response.status_code == 404:
                 return None
-            raise e
 
     def put(self, url: str, json: dict):
         self.login()
         resp = self._client.put(url, json=json)
         return _parse_resp(resp)
 
     def close(self):
         self._client.close()
 
     def dump_response(self, response: HTTPResponse):
         log.info("response text: " + response.text())
+
```

### Comparing `hcs-cli-0.1.25/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.26/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.26/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/service/_util.py` & `hcs-cli-0.1.26/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/service/lcm.py` & `hcs-cli-0.1.26/vhcs/service/lcm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 import time
 from ._util import hdc_service_client
+from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("lcm")
 
 
 class template:
     @staticmethod
-    def get(id: str):
-        return _client.get(f"/v1/templates/{id}")
+    def get(id: str, **kwargs: any):
+        url = with_query(f"/v1/templates/{id}", **kwargs)
+        return _client.get(url)
 
     @staticmethod
-    def list(type: str = None, name: str = None):
-        base = "/v1/templates?size=200"
-        if type:
-            base += "&type=" + type
-        pageIndex = 0
-        ret = []
-
-        def filter_fn(t):
-            if name:
+    def list(limit: int = 20, name: str = None, **kwargs):
+        def _get_page(query_string):
+            url = "/v1/templates?" + query_string
+            return _client.get(url)
+
+        ret = PageRequest(_get_page, limit, **kwargs).get()
+        if name:
+            #filter_fn = lambda t : t.name.find(name) >= 0
+            def filter_fn(t):
                 return t.name.find(name) >= 0
-            return True
-
-        while True:
-            url = base + "&page=" + str(pageIndex)
-            page = _client.get(url)
-            if not page.content:
-                break
-            ret.append(list(filter(filter_fn, page.content)))
-            pageIndex += 1
+            ret = list(filter(filter_fn, ret))
         return ret
 
     @staticmethod
-    def delete(force: bool):
+    def delete(id: str, force: bool):
         return _client.delete(f"/v1/templates/{id}?force={force}")
 
     @staticmethod
     def create(payload: str, type: str):
         url = "/v1/templates"
         if type:
             url += "/" + type
@@ -78,21 +72,26 @@
             time.sleep(delay)
 
             print(f"Waiting for template {id}. Expected={exclude_status}, current={status}...")
 
 
 class provider:
     @staticmethod
-    def get(id: str):
-        return _client.get(f"/v1/providers/{id}")
+    def get(id: str, **kwargs: any):
+        url = with_query(f"/v1/providers/{id}", **kwargs)
+        return _client.get(url)
 
     @staticmethod
-    def list():
-        return _client.get("/v1/providers")
+    def list(limit: int = 20, **kwargs):
+        def _get_page(query_string):
+            url = "/v1/providers?" + query_string
+            return _client.get(url)
+
+        return PageRequest(_get_page, limit, **kwargs).get()
 
     @staticmethod
-    def delete():
+    def delete(id: str):
         return _client.delete(f"/v1/providers/{id}")
 
 
 def test():
     print("test")
```

### Comparing `hcs-cli-0.1.25/vhcs/service/pki.py` & `hcs-cli-0.1.26/vhcs/service/pki.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/service/vmhub.py` & `hcs-cli-0.1.26/vhcs/service/vmhub.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/util/pki_util.py` & `hcs-cli-0.1.26/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.25/vhcs/util/versions.py` & `hcs-cli-0.1.26/vhcs/util/versions.py`

 * *Files identical despite different names*

