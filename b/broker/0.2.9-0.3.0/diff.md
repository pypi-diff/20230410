# Comparing `tmp/broker-0.2.9.tar.gz` & `tmp/broker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broker-0.2.9.tar", last modified: Tue Nov  1 17:54:04 2022, max compression
+gzip compressed data, was "broker-0.3.0.tar", last modified: Mon Apr 10 19:38:44 2023, max compression
```

## Comparing `broker-0.2.9.tar` & `broker-0.3.0.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.297927 broker-0.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.301927 broker-0.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-01 17:53:54.000000 broker-0.2.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-11-01 17:53:54.000000 broker-0.2.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-11-01 17:53:54.000000 broker-0.2.9/.github/workflows/update_broker_image.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-11-01 17:53:54.000000 broker-0.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-11-01 17:53:54.000000 broker-0.2.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     7038 2022-11-01 17:53:54.000000 broker-0.2.9/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)    35121 2022-11-01 17:53:54.000000 broker-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-01 17:53:54.000000 broker-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    24979 2022-11-01 17:54:04.305927 broker-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12559 2022-11-01 17:53:54.000000 broker-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.301927 broker-0.2.9/broker/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-01 17:53:54.000000 broker-0.2.9/broker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.301927 broker-0.2.9/broker/binds/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 17:53:54.000000 broker-0.2.9/broker/binds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4058 2022-11-01 17:53:54.000000 broker-0.2.9/broker/binds/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14343 2022-11-01 17:53:54.000000 broker-0.2.9/broker/broker.py
--rw-r--r--   0 runner    (1001) docker     (121)    13611 2022-11-01 17:53:54.000000 broker-0.2.9/broker/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-11-01 17:53:54.000000 broker-0.2.9/broker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    19134 2022-11-01 17:53:54.000000 broker-0.2.9/broker/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-11-01 17:53:54.000000 broker-0.2.9/broker/hosts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-11-01 17:53:54.000000 broker-0.2.9/broker/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.301927 broker-0.2.9/broker/providers/
--rw-r--r--   0 runner    (1001) docker     (121)     4605 2022-11-01 17:53:54.000000 broker-0.2.9/broker/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26158 2022-11-01 17:53:54.000000 broker-0.2.9/broker/providers/ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (121)    10347 2022-11-01 17:53:54.000000 broker-0.2.9/broker/providers/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-11-01 17:53:54.000000 broker-0.2.9/broker/providers/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     9173 2022-11-01 17:53:54.000000 broker-0.2.9/broker/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-11-01 17:53:54.000000 broker-0.2.9/broker/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.301927 broker-0.2.9/broker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24979 2022-11-01 17:54:04.000000 broker-0.2.9/broker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-11-01 17:54:04.000000 broker-0.2.9/broker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 17:54:04.000000 broker-0.2.9/broker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 17:54:04.000000 broker-0.2.9/broker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 17:54:03.000000 broker-0.2.9/broker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-11-01 17:54:04.000000 broker-0.2.9/broker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-01 17:54:04.000000 broker-0.2.9/broker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-11-01 17:53:54.000000 broker-0.2.9/broker_settings.yaml.example
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.301927 broker-0.2.9/logs/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-01 17:53:54.000000 broker-0.2.9/logs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-01 17:53:54.000000 broker-0.2.9/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-11-01 17:54:04.305927 broker-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-01 17:53:54.000000 broker-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-11-01 17:53:54.000000 broker-0.2.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/data/ansible_tower/
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/ansible_tower/fake_children.json
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/ansible_tower/fake_jobs.json
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/ansible_tower/fake_workflows.json
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/args_file.json
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/args_file.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/broker_args.json
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/broker_args.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.301927 broker-0.2.9/tests/data/cli_scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/data/cli_scenarios/containers/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/data/cli_scenarios/satlab/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/data/container/
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/container/fake_containers.json
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-11-01 17:53:54.000000 broker-0.2.9/tests/data/container/fake_images.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-11-01 17:53:54.000000 broker-0.2.9/tests/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-11-01 17:53:54.000000 broker-0.2.9/tests/functional/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-11-01 17:53:54.000000 broker-0.2.9/tests/functional/test_satlab.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:54:04.305927 broker-0.2.9/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (121)     3616 2022-11-01 17:53:54.000000 broker-0.2.9/tests/providers/test_ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-11-01 17:53:54.000000 broker-0.2.9/tests/providers/test_container.py
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-11-01 17:53:54.000000 broker-0.2.9/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-11-01 17:53:54.000000 broker-0.2.9/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-11-01 17:53:54.000000 broker-0.2.9/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.150156 broker-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:38:30.000000 broker-0.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 19:38:30.000000 broker-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 19:38:30.000000 broker-0.3.0/.github/workflows/update_broker_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-10 19:38:30.000000 broker-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-10 19:38:30.000000 broker-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-10 19:38:30.000000 broker-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 19:38:30.000000 broker-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-10 19:38:44.162156 broker-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-10 19:38:30.000000 broker-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:38:30.000000 broker-0.3.0/broker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/broker/binds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:30.000000 broker-0.3.0/broker/binds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-04-10 19:38:30.000000 broker-0.3.0/broker/binds/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-10 19:38:30.000000 broker-0.3.0/broker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-10 19:38:30.000000 broker-0.3.0/broker/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-10 19:38:30.000000 broker-0.3.0/broker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-04-10 19:38:30.000000 broker-0.3.0/broker/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-10 19:38:30.000000 broker-0.3.0/broker/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-10 19:38:30.000000 broker-0.3.0/broker/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/broker/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-04-10 19:38:30.000000 broker-0.3.0/broker/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 19:38:30.000000 broker-0.3.0/broker/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/broker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:38:43.000000 broker-0.3.0/broker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-10 19:38:30.000000 broker-0.3.0/broker_settings.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-10 19:38:30.000000 broker-0.3.0/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 19:38:30.000000 broker-0.3.0/logs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 19:38:30.000000 broker-0.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-10 19:38:44.162156 broker-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:38:30.000000 broker-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-10 19:38:30.000000 broker-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/ansible_tower/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/ansible_tower/fake_children.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/ansible_tower/fake_jobs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/ansible_tower/fake_workflows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/args_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/args_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/broker_args.json
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/broker_args.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.150156 broker-0.3.0/tests/data/cli_scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/cli_scenarios/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/cli_scenarios/satlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/tests/data/container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/container/fake_containers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/container/fake_images.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/fake_inventory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 19:38:30.000000 broker-0.3.0/tests/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-10 19:38:30.000000 broker-0.3.0/tests/functional/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-04-10 19:38:30.000000 broker-0.3.0/tests/functional/test_satlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-10 19:38:30.000000 broker-0.3.0/tests/providers/test_ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-10 19:38:30.000000 broker-0.3.0/tests/providers/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-10 19:38:30.000000 broker-0.3.0/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-10 19:38:30.000000 broker-0.3.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-10 19:38:30.000000 broker-0.3.0/tests/test_settings.py
```

### Comparing `broker-0.2.9/.github/workflows/python-publish.yml` & `broker-0.3.0/.github/workflows/python-publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 jobs:
   publish:
     name: Build and Deploy to PyPi
     runs-on: ubuntu-latest
     strategy:
       matrix:
         # build/push in lowest support python version
-        python-version: [ 3.8 ]
+        python-version: [ 3.9 ]
 
     steps:
     - uses: actions/checkout@v2
 
     - uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `broker-0.2.9/.github/workflows/update_broker_image.yml` & `broker-0.3.0/.github/workflows/update_broker_image.yml`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/.gitignore` & `broker-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/LICENSE` & `broker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/broker/binds/containers.py` & `broker-0.3.0/broker/binds/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 class ContainerBind:
+    _sensitive_attrs = ["password", "host_password"]
+
     def __init__(self, host=None, username=None, password=None, port=22, timeout=None):
         self.host = host
         self.username = username
         self.password = password
         self.port = port
         self.timeout = timeout
         self._client = None
@@ -64,15 +66,15 @@
             "container_config": cont.attrs.get("Config", {}),
             "host_config": cont.attrs.get("HostConfig", {}),
             "ports": cont.ports or cont.attrs.get("Ports"),
         }
 
     def __repr__(self):
         inner = ", ".join(
-            f"{k}={v}"
+            f"{k}={'******' if k in self._sensitive_attrs and v else v}"
             for k, v in self.__dict__.items()
             if not k.startswith("_") and not callable(v)
         )
         return f"{self.__class__.__name__}({inner})"
 
 
 class PodmanBind(ContainerBind):
```

### Comparing `broker-0.2.9/broker/broker.py` & `broker-0.3.0/broker/broker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 from logzero import logger
-from broker.providers.ansible_tower import AnsibleTower
-from broker.providers.container import Container
-from broker.providers.test_provider import TestProvider
+from broker.providers import PROVIDERS, PROVIDER_ACTIONS, _provider_imports
 from broker.hosts import Host
 from broker import exceptions, helpers
-from concurrent.futures import ProcessPoolExecutor, as_completed
+from concurrent.futures import ThreadPoolExecutor, as_completed
 
-
-PROVIDERS = {
-    "AnsibleTower": AnsibleTower,
-    "Container": Container,
-    "TestProvider": TestProvider,
-}
-
-PROVIDER_ACTIONS = {
-    # action: (InterfaceClass, "method_name")
-    "workflow": (AnsibleTower, "execute"),
-    "job_template": (AnsibleTower, "execute"),
-    "template": (AnsibleTower, None),  # needed for list-templates
-    "inventory": (AnsibleTower, None),
-    "container_host": (Container, "run_container"),
-    "container_app": (Container, "execute"),
-    "test_action": (TestProvider, "test_action"),
-}
+# load all the provider class so they are registered
+for _import in _provider_imports:
+    __import__(f"broker.providers.{_import}", globals(), locals(), [], 0)
 
 
 def _try_teardown(host_obj):
     """Try a host's teardown method and return an exception message if needed"""
     try:
         host_obj.teardown()
     except Exception as err:
@@ -34,34 +18,19 @@
 
 
 class mp_decorator:
     """This decorator wraps Broker methods to enable multiprocessing
 
     The decorated method is expected to return an itearable.
     """
-
-    # Note that this is a descriptor as the other option -- using nested function
-    # like this:
-    #
-    # def mp_decorator(func)
-    #   @wraps(func)
-    #   def wrapper(func)
-    #       return
-    #
-    #   return wrapper
-    #
-    # is not working with pickling that is necessary for the ProcessPoolExecutor of
-    # concurrent.futures. I got errors like:
-    # _pickle.PicklingError: Can't pickle ... it's not the same object as ...
-
     MAX_WORKERS = None
     """ If set to integer, the count of workers will be limited to that amount.
      If set to None, the max workers count of the EXECUTOR will match the count of items."""
 
-    EXECUTOR = ProcessPoolExecutor
+    EXECUTOR = ThreadPoolExecutor
 
     def __init__(self, func=None):
         self.func = func
 
     def __get__(self, instance, owner):
         if not instance:
             return self.func
@@ -107,88 +76,93 @@
         # Allow users to more simply pass a host class instead of a dict
         if "host_class" in kwargs:
             self.host_classes["host"] = kwargs.pop("host_class")
         elif "host_classes" in kwargs:
             self.host_classes.update(kwargs.pop("host_classes"))
         # determine the provider actions based on kwarg parameters
         self._provider_actions = {}
-        for key, action in PROVIDER_ACTIONS.items():
-            if key in kwargs:
-                self._provider_actions[key] = action
+        self._update_provider_actions(kwargs)
         self._kwargs = kwargs
 
     def _act(self, provider, method, checkout=False):
         """Perform a general action against a provider's method"""
+        logger.debug(f"Resolving action {method} on provider {provider}.")
         provider_inst = provider(**self._kwargs)
         helpers.emit(
             {
                 "provider": provider_inst.__class__.__name__,
                 "action": method,
                 "arguments": self._kwargs,
             }
         )
-        result = getattr(provider_inst, method)(**self._kwargs)
-        logger.debug(result)
+        method_obj = getattr(provider_inst, method)
+        logger.debug(
+            f"On {provider_inst=} executing {method_obj=} with params {self._kwargs=}."
+        )
+        result = method_obj(**self._kwargs)
+        logger.debug(f"Action {result=}")
         if result and checkout:
             return provider_inst.construct_host(
                 provider_params=result, host_classes=self.host_classes, **self._kwargs
             )
         else:
             return result
 
+    def _update_provider_actions(self, kwargs):
+        if not self._provider_actions:
+            for key, action in PROVIDER_ACTIONS.items():
+                if key in kwargs:
+                    self._provider_actions[key] = action
+
     @mp_decorator
     def _checkout(self):
         """checkout one or more VMs
 
         :return: List of Host objects
         """
         hosts = []
+        logger.debug(f"Doing _checkout(): {self._provider_actions=}")
         if not self._provider_actions:
             raise self.BrokerError("Could not determine an appropriate provider")
         for action in self._provider_actions.keys():
             provider, method = PROVIDER_ACTIONS[action]
             logger.info(f"Using provider {provider.__name__} to checkout")
             try:
                 host = self._act(provider, method, checkout=True)
             except exceptions.ProviderError as err:
                 host = err
+            hosts.append(host)
             if host and not isinstance(host, exceptions.ProviderError):
-                hosts.append(host)
                 logger.info(f"{host.__class__.__name__}: {host.hostname}")
         return hosts
 
     def checkout(self):
         """checkout one or more VMs
 
         :return: Host obj or list of Host objects
         """
         hosts = self._checkout()
-        err, to_emit = None, []
-        for host in hosts:
-            if not isinstance(host, exceptions.ProviderError):
-                to_emit.append(host.to_dict())
-            else:
+        err = None
+        for host in hosts[:]:
+            if isinstance(host, exceptions.ProviderError):
                 err = host
                 hosts.remove(host)
         helpers.emit(hosts=[host.to_dict() for host in hosts])
         self._hosts.extend(hosts)
         helpers.update_inventory([host.to_dict() for host in hosts])
         if err:
             raise err
         return hosts if not len(hosts) == 1 else hosts[0]
 
     def execute(self, **kwargs):
         """execute a provider action
 
-        :return: Any The results given back by the provider
+        :return: Any results given back by the provider
         """
-        if not self._provider_actions:
-            for key, action in PROVIDER_ACTIONS.items():
-                if key in kwargs:
-                    self._provider_actions[key] = action
+        self._update_provider_actions(kwargs)
         self._kwargs.update(kwargs)
         if not self._provider_actions:
             raise self.BrokerError("Could not determine an appropriate provider")
         for action, arg in self._provider_actions.items():
             provider, method = PROVIDER_ACTIONS[action]
         logger.info(f"Using provider {provider.__name__} for execution")
         return self._act(provider, method)
@@ -207,43 +181,46 @@
             host.release()
         except Exception as err:
             logger.warning(f"Encountered exception during checkin: {err}")
             raise
             # pass
         return host
 
-    def checkin(self, sequential=False, host=None):
+    def checkin(self, sequential=False, host=None, in_context=False):
         """checkin one or more VMs
 
         :param host: can be one of:
             None - Will use the contents of self._hosts
             A single host object
             A list of host objects
             A dictionary mapping host types to one or more host objects
 
         :param sequential: boolean whether to run checkins sequentially
+        :param in_context: Whether checkin is part of context manager
         """
         # default to hosts listed on the instance
         hosts = host or self._hosts
         logger.debug(
             f"Checkin called with: {hosts}, "
             f'running {"sequential" if sequential else "concurrent"}'
         )
         # normalize the type since the function accepts multiple types
         if isinstance(hosts, dict):
             # flatten the lists of hosts from the values of the dict
             hosts = [host for host_list in hosts.values() for host in host_list]
-        if not isinstance(hosts, list):
-            hosts = [hosts]
-
+        else:
+            if not isinstance(hosts, list):
+                hosts = [hosts]
+            if in_context:
+                hosts = [host for host in hosts if not getattr(host, '_skip_context_checkin', False)]
         if not hosts:
             logger.debug("Checkin called with no hosts, taking no action")
             return
 
-        with ProcessPoolExecutor(max_workers=1 if sequential else None) as workers:
+        with ThreadPoolExecutor(max_workers=1 if sequential else None) as workers:
             completed_checkins = as_completed(
                 # reversing over a copy of the list to avoid skipping
                 workers.submit(self._checkin, _host)
                 for _host in hosts[::-1]
             )
             for completed in completed_checkins:
                 _host = completed.result()
@@ -256,15 +233,15 @@
         helpers.update_inventory(remove=[h.hostname for h in hosts])
 
     def _extend(self, host):
         """extend a single VM"""
         logger.info(f"Extending host {host.hostname}")
         provider = PROVIDERS[host._broker_provider]
         self._kwargs["target_vm"] = host
-        self._act(provider, "extend_vm", checkout=False)
+        self._act(provider, "extend", checkout=False)
         return host
 
     def extend(self, sequential=False, host=None):
         """extend one or more VMs
 
         :param host: can be one of:
             None - Will use the contents of self._hosts
@@ -287,15 +264,15 @@
         if not isinstance(hosts, list):
             hosts = [hosts]
 
         if not hosts:
             logger.debug("Extend called with no hosts, taking no action")
             return
 
-        with ProcessPoolExecutor(
+        with ThreadPoolExecutor(
             max_workers=1 if sequential else len(hosts)
         ) as workers:
             completed_extends = as_completed(
                 workers.submit(self._extend, _host) for _host in hosts
             )
             for completed in completed_extends:
                 _host = completed.result()
@@ -312,17 +289,16 @@
         logger.info(
             f"Pulling remote inventory from {f'{instance } ' if instance else ''}{provider}"
         )
         if instance:
             instance = {provider: instance}
         prov_inventory = PROVIDERS[provider](**instance).get_inventory(additional_arg)
         curr_inventory = [
-            host.get("hostname", host.get("name"))
-            for host in helpers.load_inventory()
-            if host["_broker_provider"] == provider
+            hostname if (hostname := host.get("hostname")) else host.get("name")
+            for host in helpers.load_inventory(filter=f"_broker_provider={provider}")
         ]
         helpers.update_inventory(add=prov_inventory, remove=curr_inventory)
 
     def reconstruct_host(self, host_export_data):
         """reconstruct a host from export data"""
         logger.debug(f"reconstructing host with export: {host_export_data}")
         provider = PROVIDERS.get(host_export_data.get("_broker_provider"))
@@ -371,10 +347,10 @@
             self.checkin()
             raise err
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         last_exception = None
         for host in self._hosts:
             last_exception = _try_teardown(host)
-        self.checkin()
+        self.checkin(in_context=True)
         if last_exception:
             raise last_exception
```

### Comparing `broker-0.2.9/broker/commands.py` & `broker-0.3.0/broker/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,43 @@
+from functools import wraps
 import signal
 import sys
 import click
 from logzero import logger
+from broker import exceptions, helpers, settings
 from broker.broker import PROVIDERS, PROVIDER_ACTIONS, Broker
-from broker.providers import Provider
+from broker.logger import LOG_LEVEL
 from broker import exceptions, helpers, settings
 
 
 signal.signal(signal.SIGINT, helpers.handle_keyboardinterrupt)
 
 
+def loggedcli(group=None, *cli_args, **cli_kwargs):
+    """Updates the group command wrapper function in order to add logging"""
+    if not group:
+        group = cli  # default to the main cli group
+
+    def decorator(func):
+        @group.command(*cli_args, **cli_kwargs)
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            logger.log(LOG_LEVEL.TRACE.value, f"Calling {func=}(*{args=} **{kwargs=}")
+            retval = func(*args, **kwargs)
+            logger.log(
+                LOG_LEVEL.TRACE.value,
+                f"Finished {func=}(*{args=} **{kwargs=}) {retval=}",
+            )
+            return retval
+
+        return wrapper
+
+    return decorator
+
+
 class ExceptionHandler(click.Group):
     """Wraps click group to catch and handle raised exceptions"""
 
     def __call__(self, *args, **kwargs):
         try:
             return self.main(*args, **kwargs)
         except Exception as err:
@@ -22,15 +46,15 @@
             helpers.emit(return_code=err.error_code, error_message=str(err.message))
             sys.exit(err.error_code)
         helpers.emit(return_code=0)
 
 
 def provider_options(command):
     """Applies provider-specific decorators to each command this decorates"""
-    for prov in Provider.__subclasses__():
+    for prov in PROVIDERS.values():
         if prov.hidden:
             continue
         for option in getattr(prov, f"_{command.__name__}_options"):
             command = option(command)
     return command
 
 
@@ -46,17 +70,31 @@
         --workflow TEXT  Get information about a workflow
         --help           Show this message and exit.
 
     Note: This currently only works for the default instance for each provider
     """
     for prov, prov_class in (pairs for pairs in PROVIDERS.items()):
 
-        @click_group.command(name=prov, hidden=prov_class.hidden)
-        def provider_cmd(*args, **kwargs):  # the actual subcommand
+        @loggedcli(
+            group=click_group,
+            name=prov,
+            hidden=prov_class.hidden,
+            context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
+        )
+        @click.pass_context
+        def provider_cmd(ctx, *args, **kwargs):  # the actual subcommand
             """Get information about a provider's actions"""
+            # if additional arguments were passed, include them in the broker args
+            # strip leading -- characters
+            kwargs.update(
+                {
+                    (key[2:] if key.startswith("--") else key): val
+                    for key, val in zip(ctx.args[::2], ctx.args[1::2])
+                }
+            )
             broker_inst = Broker(**kwargs)
             broker_inst.nick_help()
 
         # iterate through available actions and populate options from them
         for action in (
             action
             for action, prov_info in PROVIDER_ACTIONS.items()
@@ -83,16 +121,16 @@
             help="Apply a broker filter to returned results",
         )(provider_cmd)
 
 
 @click.group(cls=ExceptionHandler, invoke_without_command=True)
 @click.option(
     "--log-level",
-    type=click.Choice(["info", "warning", "error", "critical", "debug", "silent"]),
-    default="debug" if settings.settings.debug else "info",
+    type=click.Choice(["info", "warning", "error", "debug", "trace", "silent"]),
+    default=settings.settings.logging.console_level,
     callback=helpers.update_log_level,
     is_eager=True,
     expose_value=False,
 )
 @click.option(
     "--output-file",
     type=click.Path(dir_okay=False),
@@ -107,34 +145,49 @@
     help="Get broker system-level information",
 )
 def cli(version):
     if version:
         import pkg_resources
 
         broker_version = pkg_resources.get_distribution("broker").version
+        # check the latest version publish to PyPi
+        try:
+            import requests
+            from packaging.version import Version
+
+            latest_version = Version(
+                requests.get("https://pypi.org/pypi/broker/json").json()["info"][
+                    "version"
+                ]
+            )
+            if latest_version > Version(broker_version):
+                click.secho(
+                    f"A newer version of broker is available: {latest_version}",
+                    fg="yellow",
+                )
+        except:
+            pass
         click.echo(f"Version: {broker_version}")
         broker_directory = settings.BROKER_DIRECTORY.absolute()
         click.echo(f"Broker Directory: {broker_directory}")
         click.echo(f"Settings File: {settings.settings_path.absolute()}")
         click.echo(f"Inventory File: {broker_directory}/inventory.yaml")
         click.echo(f"Log File: {broker_directory}/logs/broker.log")
 
 
-@cli.command(
-    context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
-)
+@loggedcli(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
 @click.option("-b", "--background", is_flag=True, help="Run checkout in the background")
 @click.option("-n", "--nick", type=str, help="Use a nickname defined in your settings")
 @click.option(
     "-c", "--count", type=int, help="Number of times broker repeats the checkout"
 )
 @click.option(
     "--args-file",
     type=click.Path(exists=True),
-    help="A json or yaml file mappng arguments to values",
+    help="A json or yaml file mapping arguments to values",
 )
 @provider_options
 @click.pass_context
 def checkout(ctx, background, nick, count, args_file, **kwargs):
     """Checkout or "create" a Virtual Machine broker instance
     COMMAND: broker checkout --workflow "workflow-name" --workflow-arg1 something
     or
@@ -142,15 +195,15 @@
 
     :param ctx: clicks context object
 
     :param background: run a new broker subprocess to carry out command
 
     :param nick: shortcut for arguments saved in settings.yaml, passed in as a string
 
-    :param args_file: this broker argument wil be replaced with the contents of the file passed in
+    :param args_file: this broker argument will be replaced with the contents of the file passed in
     """
     broker_args = helpers.clean_dict(kwargs)
     if nick:
         broker_args["nick"] = nick
     if count:
         broker_args["_count"] = count
     if args_file:
@@ -174,15 +227,15 @@
     """Get information about a provider and its actions"""
     pass
 
 
 populate_providers(providers)
 
 
-@cli.command()
+@loggedcli()
 @click.argument("vm", type=str, nargs=-1)
 @click.option("-b", "--background", is_flag=True, help="Run checkin in the background")
 @click.option("--all", "all_", is_flag=True, help="Select all VMs")
 @click.option("--sequential", is_flag=True, help="Run checkins sequentially")
 @click.option(
     "--filter", type=str, help="Checkin only what matches the specified filter"
 )
@@ -213,15 +266,15 @@
             or all_
         ):
             to_remove.append(Broker().reconstruct_host(host))
     broker_inst = Broker(hosts=to_remove)
     broker_inst.checkin(sequential=sequential)
 
 
-@cli.command()
+@loggedcli()
 @click.option("--details", is_flag=True, help="Display all host details")
 @click.option(
     "--sync",
     type=str,
     help="Class-style name of a supported broker provider. (AnsibleTower)",
 )
 @click.option(
@@ -243,15 +296,15 @@
         if details:
             logger.info(f"{num}: {display_name}, Details: {helpers.yaml_format(host)}")
         else:
             logger.info(f"{num}: {display_name}")
     helpers.emit({"inventory": emit_data})
 
 
-@cli.command()
+@loggedcli()
 @click.argument("vm", type=str, nargs=-1)
 @click.option("-b", "--background", is_flag=True, help="Run extend in the background")
 @click.option("--all", "all_", is_flag=True, help="Select all VMs")
 @click.option("--sequential", is_flag=True, help="Run extends sequentially")
 @click.option(
     "--filter", type=str, help="Extend only what matches the specified filter"
 )
@@ -279,15 +332,15 @@
     for num, host in enumerate(inventory):
         if str(num) in vm or host["hostname"] in vm or host["name"] in vm or all_:
             to_extend.append(Broker().reconstruct_host(host))
     broker_inst = Broker(hosts=to_extend, **broker_args)
     broker_inst.extend(sequential=sequential)
 
 
-@cli.command()
+@loggedcli()
 @click.argument("vm", type=str, nargs=-1)
 @click.option(
     "-b", "--background", is_flag=True, help="Run duplicate in the background"
 )
 @click.option(
     "-c", "--count", type=int, help="Number of times broker repeats the duplicate"
 )
@@ -322,31 +375,29 @@
                 broker_inst.checkout()
             else:
                 logger.warning(
                     f"Unable to duplicate {host['hostname']}, no _broker_args found"
                 )
 
 
-@cli.command(
-    context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
-)
+@loggedcli(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
 @click.option("-b", "--background", is_flag=True, help="Run execute in the background")
 @click.option("--nick", type=str, help="Use a nickname defined in your settings")
 @click.option(
     "--output-format", "-o", type=click.Choice(["log", "raw", "yaml"]), default="log"
 )
 @click.option(
     "--artifacts",
     type=click.Choice(["merge", "last"]),
     help="AnsibleTower: return artifacts associated with the execution.",
 )
 @click.option(
     "--args-file",
     type=click.Path(exists=True),
-    help="A json or yaml file mappng arguments to values",
+    help="A json or yaml file mapping arguments to values",
 )
 @provider_options
 @click.pass_context
 def execute(ctx, background, nick, output_format, artifacts, args_file, **kwargs):
     """Execute an arbitrary provider action
     COMMAND: broker execute --workflow "workflow-name" --workflow-arg1 something
     or
@@ -358,15 +409,15 @@
 
     :param nick: shortcut for arguments saved in settings.yaml, passed in as a string
 
     :param output_format: change the format of the output to one of the choice options
 
     :param artifacts: AnsibleTower provider specific option for choosing what to return
 
-    :param args_file: this broker argument wil be replaced with the contents of the file passed in
+    :param args_file: this broker argument will be replaced with the contents of the file passed in
     """
     broker_args = helpers.clean_dict(kwargs)
     if nick:
         broker_args["nick"] = nick
     if artifacts:
         broker_args["artifacts"] = artifacts
     if args_file:
```

### Comparing `broker-0.2.9/broker/exceptions.py` & `broker-0.3.0/broker/exceptions.py`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/broker/helpers.py` & `broker-0.3.0/broker/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Miscellaneous helpers live here"""
+import collections
 from contextlib import contextmanager
 import getpass
 import inspect
 import json
-import logging
 import os
-import pickle
 import sys
 import tarfile
 import time
 from collections import UserDict, namedtuple
 from collections.abc import MutableMapping
 from copy import deepcopy
 from pathlib import Path
@@ -86,66 +85,37 @@
                 del value[index]
             flattened.append((new_key, value))
         else:
             flattened.append((new_key, value))
     return dict(flattened)
 
 
-def classify_filter(filter_string):
-    """Given a filter string, determine the filter action and components"""
-    tests = {
-        "!<": "'{needle}' not in '{haystack}'",
-        "<": "'{needle}' in '{haystack}'",
-        "!=": "'{haystack}' != '{needle}'",
-        "=": "'{haystack}' == '{needle}'",
-        "!{": "not '{haystack}'.startswith('{needle}')",
-        "{": "'{haystack}'.startswith('{needle}')",
-        "!}": "not '{haystack}'.endswith('{needle}')",
-        "}": "'{haystack}'.endswith('{needle}')",
-    }
-    if "," in filter_string:
-        return [classify_filter(f) for f in filter_string.split(",")]
-    for cond, test in tests.items():
-        if cond in filter_string:
-            k, v = filter_string.split(cond)
-            return FilterTest(haystack=k, needle=v, test=test)
-
-
-def inventory_filter(inventory, raw_filter):
-    """Filter out inventory items depending on the filter provided"""
-    resolved_filter = classify_filter(raw_filter)
-    if not isinstance(resolved_filter, list):
-        resolved_filter = [resolved_filter]
-    matching = []
-    for host in inventory:
-        flattened_host = flatten_dict(host, separator=".")
-        eval_list = [
-            eval(rf.test.format(haystack=flattened_host[rf.haystack], needle=rf.needle))
-            for rf in resolved_filter
-            if rf.haystack in flattened_host
-        ]
-        if eval_list and all(eval_list):
-            matching.append(host)
-    return matching
-
-
-def results_filter(results, raw_filter):
-    """Filter out a list of results depending on the filter provided"""
-    resolved_filter = classify_filter(raw_filter)
-    if not isinstance(resolved_filter, list):
-        resolved_filter = [resolved_filter]
-    matching = []
-    for res in results:
-        eval_list = [
-            eval(rf.test.format(haystack=res, needle=rf.needle))
-            for rf in resolved_filter
-        ]
-        if eval_list and all(eval_list):
-            matching.append(res)
-    return matching
+def eval_filter(filter_list, raw_filter, filter_key="inv"):
+    """Run each filter through an eval to get the results"""
+    filter_list = [
+        MockStub(item) if isinstance(item, dict) else item for item in filter_list
+    ]
+    for raw_f in raw_filter.split("|"):
+        if f"@{filter_key}[" in raw_f:
+            # perform a list filter on the inventory
+            filter_list = eval(
+                raw_f.replace(f"@{filter_key}", filter_key), {filter_key: filter_list}
+            )
+            filter_list = filter_list if isinstance(filter_list, list) else [filter_list]
+        elif f"@{filter_key}" in raw_f:
+            # perform an attribute filter on each host
+            filter_list = list(
+                filter(
+                    lambda item: eval(
+                        raw_f.replace(f"@{filter_key}", filter_key), {filter_key: item}
+                    ),
+                    filter_list,
+                )
+            )
+    return [dict(item) if isinstance(item, MockStub) else item for item in filter_list]
 
 
 def resolve_nick(nick):
     """Checks if the nickname exists. Used to define broker arguments
 
     :param nick: String representing the name of a nick
 
@@ -175,78 +145,87 @@
 
 
 def resolve_file_args(broker_args):
     """Check for files being passed in as values to arguments,
     then attempt to resolve them. If not resolved, keep arg/value pair intact.
     """
     final_args = {}
-    for key, val in broker_args.items():
+    # parse the eventual args_file first
+    if val := broker_args.pop("args_file", None):
         if isinstance(val, Path) or (
             isinstance(val, str) and val[-4:] in ("json", "yaml", ".yml")
         ):
             if data := load_file(val):
-                if key == "args_file":
-                    if isinstance(data, dict):
-                        final_args.update(data)
-                    elif isinstance(data, list):
-                        for d in data:
-                            final_args.update(d)
-                else:
-                    final_args[key] = data
-            elif key == "args_file":
+                if isinstance(data, dict):
+                    final_args.update(data)
+                elif isinstance(data, list):
+                    for d in data:
+                        final_args.update(d)
+            else:
                 raise exceptions.BrokerError(f"No data loaded from {val}")
+
+    for key, val in broker_args.items():
+        if isinstance(val, Path) or (
+            isinstance(val, str) and val[-4:] in ("json", "yaml", ".yml")
+        ):
+            if data := load_file(val):
+                final_args.update({key: data})
             else:
-                final_args[key] = val
+                final_args.update({key: val})
         else:
-            final_args[key] = val
+            final_args.update({key: val})
     return final_args
 
 
 def load_inventory(filter=None):
     """Loads all local hosts in inventory
 
     :return: list of dictionaries
     """
-    inventory_file = settings.BROKER_DIRECTORY.joinpath(
-        settings.settings.INVENTORY_FILE
-    )
-    inv_data = load_file(inventory_file, warn=False)
-    return inv_data if not filter else inventory_filter(inv_data, filter)
+    inv_data = load_file(settings.inventory_path, warn=False)
+    return inv_data if not filter else eval_filter(inv_data, filter)
 
 
 def update_inventory(add=None, remove=None):
     """Updates list of local hosts in the checkout interface
 
     :param add: list of dictionaries representing new hosts
 
     :param remove: list of strings representing hostnames or names to be removed
 
     :return: no return value
     """
-    inventory_file = settings.BROKER_DIRECTORY.joinpath(
-        settings.settings.INVENTORY_FILE
-    )
     if add and not isinstance(add, list):
         add = [add]
+    elif not add:
+        add = []
     if remove and not isinstance(remove, list):
         remove = [remove]
-    with FileLock(inventory_file):
+    with FileLock(settings.inventory_path):
         inv_data = load_inventory()
         if inv_data:
-            inventory_file.unlink()
+            settings.inventory_path.unlink()
 
         if remove:
             for host in inv_data[::-1]:
                 if host["hostname"] in remove or host["name"] in remove:
+                    # iterate through new hosts and update with old host data if it would nullify
+                    for new_host in add:
+                        if (
+                            host["hostname"] == new_host["hostname"]
+                            or host["name"] == new_host["name"]
+                        ):
+                            # update missing data in the new_host with the old_host data
+                            new_host.update(merge_dicts(new_host, host))
                     inv_data.remove(host)
         if add:
             inv_data.extend(add)
 
-        inventory_file.touch()
-        with inventory_file.open("w") as inv_file:
+        settings.inventory_path.touch()
+        with settings.inventory_path.open("w") as inv_file:
             yaml.dump(inv_data, inv_file)
 
 
 def yaml_format(in_struct):
     """Convert a yaml-compatible structure to a yaml dumped string
 
     :param in_struct: yaml-compatible structure or string containing structure
@@ -335,24 +314,29 @@
         except KeyError:
             item = self
         return item
 
     def __call__(self, *args, **kwargs):
         return self
 
+    def __hash__(self):
+        return hash(
+            tuple(
+                (
+                    kp
+                    for kp in self.__dict__.items()
+                    if isinstance(kp[1], collections.abc.Hashable)
+                )
+            )
+        )
+
 
 def update_log_level(ctx, param, value):
-    silent = False
-    if value == "silent":
-        silent = True
-        value = "info"
-    if getattr(logging, value.upper()) is not logger.getEffectiveLevel() or silent:
-        b_log.setup_logzero(level=value, silent=silent)
-        if not silent:
-            print(f"Log level changed to [{value}]")
+    b_log.set_log_level(value)
+    b_log.set_file_logging(value)
 
 
 def set_emit_file(ctx, param, value):
     global emit
     emit.set_file(value)
 
 
@@ -545,50 +529,7 @@
     temp_tar = Path(f"{uuid4().hex[-10]}.tar")
     with tarfile.open(temp_tar, mode="w") as tar:
         for path in paths:
             logger.debug(f"Adding {path.absolute()} to {temp_tar.absolute()}")
             tar.add(path, arcname=path.name)
     yield temp_tar.absolute()
     temp_tar.unlink()
-
-
-class PickleSafe:
-    """A class that helps with pickling and unpickling complex objects"""
-
-    def _pre_pickle(self):
-        """This method is called before pickling an object"""
-        pass
-
-    def _post_pickle(self, purified):
-        """This method is called after pickling an object
-
-        purified will be a list of names of attributes that were removed
-        """
-        pass
-
-    def _purify(self):
-        """Strip all unpickleable attributes from a Host before pickling"""
-        self.purified = getattr(self, "purified", [])
-        for name in list(self.__dict__):
-            self._purify_target = name
-            try:
-                pickle.dumps(self.__dict__[name])
-            except (pickle.PicklingError, AttributeError):
-                self.__dict__[name] = None
-                self.purified.append(name)
-
-    def __getstate__(self):
-        """If a session is active, remove it for pickle compatability"""
-        self._pre_pickle()
-        try:
-            self._purify()
-        except RecursionError:
-                logger.warning(f"Recursion limit reached on {self._purify_target}")
-                self.__dict__[self._purify_target] = None
-                self.__getstate__()
-        self.__dict__.pop("_purify_target", None)
-        return self.__dict__
-
-    def __setstate__(self, state):
-        """Sometimes pickle strips things that we need. This should be used to restore them"""
-        self.__dict__.update(state)
-        self._post_pickle(purified=getattr(self, "purified", []))
```

### Comparing `broker-0.2.9/broker/hosts.py` & `broker-0.3.0/broker/hosts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # from functools import cached_property
 from logzero import logger
-from broker.exceptions import NotImplementedError
-from broker.helpers import PickleSafe
+from broker.exceptions import NotImplementedError, HostError
 from broker.session import ContainerSession, Session
 from broker.settings import settings
 
 
-class Host(PickleSafe):
+class Host:
 
     default_timeout = 0  # timeout in ms, 0 is infinite
 
-    def __init__(self, hostname, name=None, from_dict=False, **kwargs):
+    def __init__(self, hostname=None, name=None, from_dict=False, **kwargs):
         # Allow the class to construct itself from kwargs
         if from_dict:
             self.__dict__.update(kwargs)
         else:
-            self.hostname = hostname
+            self.hostname = hostname or kwargs.get("ip", None)
+            if not self.hostname:
+                raise HostError("Host must be constructed with a hostname or ip")
             self.name = name
         self.username = kwargs.get("username", settings.HOST_USERNAME)
         self.password = kwargs.get("password", settings.HOST_PASSWORD)
         self.timeout = kwargs.get(
             "connection_timeout", settings.HOST_CONNECTION_TIMEOUT
         )
         self.port = kwargs.get("port", settings.HOST_SSH_PORT)
@@ -39,21 +40,14 @@
             # Check to see if we're a non-ssh-enabled Container Host
             if hasattr(self, "_cont_inst") and not self._cont_inst.ports.get(22):
                 self._session = ContainerSession(self)
             else:
                 self.connect()
         return self._session
 
-    def _pre_pickle(self):
-        self.close()
-
-    def _post_pickle(self, purified):
-        if "_cont_inst" in purified and not getattr(self, "_checked_in", False):
-            self._cont_inst = self._prov_inst._cont_inst_by_name(self.name)
-
     def connect(
         self, username=None, password=None, timeout=None, port=22, key_filename=None
     ):
         username = username or self.username
         password = password or self.password
         timeout = timeout or self.timeout
         _hostname = self.hostname
@@ -91,22 +85,25 @@
         timeout = timeout or self.default_timeout
         logger.debug(f"{self.hostname} executing command: {command}")
         res = self.session.run(command, timeout=timeout)
         logger.debug(f"{self.hostname} command result:\n{res}")
         return res
 
     def to_dict(self):
-        return {
+        ret_dict = {
             "hostname": self.hostname,
             "name": getattr(self, "name", None),
             "_broker_provider": self._broker_provider,
             "_broker_provider_instance": self._prov_inst.instance,
             "type": "host",
             "_broker_args": self._broker_args,
         }
+        if hasattr(self, "tower_inventory"):
+            ret_dict["tower_inventory"] = self.tower_inventory
+        return ret_dict
 
     def setup(self):
         """Automatically ran when entering a Broker context manager"""
         pass
 
     def teardown(self):
         """Automatically ran when exiting a Broker context manager"""
```

### Comparing `broker-0.2.9/broker/providers/__init__.py` & `broker-0.3.0/broker/providers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,148 @@
-import pickle
+from abc import ABCMeta, abstractmethod
 import dynaconf
+from pathlib import Path
 
 from broker import exceptions
-from broker.helpers import PickleSafe
 from broker.settings import settings
 from logzero import logger
 
 
-class Provider(PickleSafe):
+# populate a list of all provider module names
+_provider_imports = [
+    f.stem
+    for f in Path(__file__).parent.glob("*.py")
+    if f.is_file() and f.stem != "__init__"
+]
+
+# ProviderName: ProviderClassObject
+PROVIDERS = {}
+# action: (InterfaceClass, "method_name")
+PROVIDER_ACTIONS = {}
+
+
+class ProviderMeta(ABCMeta):
+    """Metaclass that registers provider classes and actions"""
+
+    def __new__(cls, name, bases, attrs):
+        """Register provider classes and actions"""
+        new_cls = super().__new__(cls, name, bases, attrs)
+        if name != "Provider":
+            PROVIDERS[name] = new_cls
+            logger.debug(f"Registered provider {name}")
+            for attr in attrs.values():
+                if hasattr(attr, "_as_action"):
+                    for action in attr._as_action:
+                        PROVIDER_ACTIONS[action] = (new_cls, attr.__name__)
+                        logger.debug(f"Registered action {action} for provider {name}")
+        return new_cls
+
+
+class Provider(metaclass=ProviderMeta):
     # Populate with a list of Dynaconf Validators specific to your provider
     _validators = []
     # Set to true if you don't want your provider shown in the CLI
     hidden = False
     # Populate these to add your checkout and execute options to each command
     # _checkout_options = [click.option("--workflow", type=str, help="Help text")]
     _checkout_options = []
     _execute_options = []
+    _fresh_settings = settings.dynaconf_clone()
+    _sensitive_attrs = []
 
     def __init__(self, **kwargs):
         self._construct_params = []
         cls_name = self.__class__.__name__
         logger.debug(f"{cls_name} provider instantiated with {kwargs=}")
-        instance_name = kwargs.pop(f"{cls_name}", None)
-        self._validate_settings(instance_name)
+        self.instance = kwargs.pop(f"{cls_name}", None)
+        self._validate_settings(self.instance)
 
     def _validate_settings(self, instance_name=None):
         """Load and validate provider settings
 
-        Each provider's settings must include an instances list with specific instance
+        Each provider's settings can include an instances list with specific instance
         details.
+        One instance should have a "default" key set to True, if instances are defined.
         General provider settings should live on the top level for that provider.
-        One instance should have a "default" key set to True
 
         :param instance_name: A string matching an instance name
         """
-        instance_name = instance_name or getattr(self, "instance", None)
         section_name = self.__class__.__name__.upper()
-        # make sure each instance isn't loading values from another
-        fresh_settings = settings.get_fresh(section_name)
-        instance, default = None, False
-        for candidate in fresh_settings.instances:
-            logger.debug(f"Checking {instance_name} against {candidate}")
-            if instance_name in candidate:
-                instance = candidate
-                default = False
-                break
-            elif (
-                candidate.values()[0].get("default")
-                or len(fresh_settings.instances) == 1
-            ):
-                instance = candidate
-                default = True
-        self.instance, *_ = instance  # store the instance name on the provider
-        fresh_settings.update(instance.values()[0])
-        settings[section_name] = fresh_settings
-        if default:
-            # if a default provider is selected, defer to loaded environment variables
-            settings.execute_loaders(loaders=[dynaconf.loaders.env_loader])
+        # if the provider has instances, load the instance settings
+        if self._fresh_settings.get(section_name).get("instances"):
+            fresh_settings = self._fresh_settings.get(section_name).copy()
+            instance_name = instance_name or getattr(self, "instance", None)
+            # iterate through the instances and find the one that matches the instance_name
+            # if no instance matches, use the default instance
+            for candidate in fresh_settings.instances:
+                logger.debug("Checking %s against %s", instance_name, candidate)
+                if instance_name in candidate:
+                    instance = candidate
+                    break
+                elif (
+                    candidate.values()[0].get("default")
+                    or len(fresh_settings.instances) == 1
+                ):
+                    instance = candidate
+            self.instance, *_ = instance  # store the instance name on the provider
+            fresh_settings.update((inst_vals := instance.values()[0]))
+            settings[section_name] = fresh_settings
+            if not inst_vals.get("override_envars"):
+                # if a provider instance doesn't want to override envars, load them
+                settings.execute_loaders(loaders=[dynaconf.loaders.env_loader])
 
-        settings.validators.extend(self._validators)
+        settings.validators.extend([v for v in self._validators if v not in settings.validators])
         # use selective validation to only validate the instance settings
         try:
             settings.validators.validate(only=section_name)
         except dynaconf.ValidationError as err:
             raise exceptions.ConfigurationError(err)
 
-    def _host_release(self):
-        raise exceptions.NotImplementedError("_host_release has not been implemented")
-
     def _set_attributes(self, obj, attrs):
         obj.__dict__.update(attrs)
 
     def _get_params(arg_list, kwargs):
         return {k: v for k, v in kwargs.items() if k in arg_list}
 
     def construct_host(self, host_cls, provider_params, **kwargs):
         host_inst = host_cls(**provider_params, **kwargs)
         host_attrs = self._get_params(self._construct_params)
         host_attrs["release"] = self._host_release
         self._set_attributes(host_inst, host_attrs)
         return host_inst
 
+    @abstractmethod
     def nick_help(self):
-        raise exceptions.NotImplementedError("nick_help has not been implemented")
+        pass
 
+    @abstractmethod
     def get_inventory(self, **kwargs):
-        raise exceptions.NotImplementedError("get_inventory has not been implemented")
+        pass
 
+    @abstractmethod
     def extend(self):
-        raise exceptions.NotImplementedError("extend has not been implemented")
+        pass
 
+    @abstractmethod
     def release(self, host_obj):
-        raise exceptions.NotImplementedError("release has not been implemented")
+        pass
 
     def __repr__(self):
         inner = ", ".join(
-            f"{k}={v}"
+            f"{k}={'******' if k in self._sensitive_attrs and v else v}"
             for k, v in self.__dict__.items()
             if not k.startswith("_") and not callable(v)
         )
         return f"{self.__class__.__name__}({inner})"
 
-    def __getstate__(self):
-        """If a session is active, remove it for pickle compatability"""
-        self._purify()
-        return self.__dict__
-
-    def _purify(self):
-        """Strip all unpickleable attributes from a Host before pickling"""
-        for key, obj in self.__dict__.items():
-            try:
-                pickle.dumps(obj)
-            except (pickle.PicklingError, AttributeError):
-                self.__dict__[key] = None
-            except RecursionError:
-                logger.warning(f"Recursion limit reached on {obj=}")
+    @staticmethod
+    def register_action(*as_names):
+        """Decorator to register a provider action
+
+        :param as_names: One or more action names to register the decorated function as
+        """
+
+        def decorator(func):
+            func._as_action = as_names or [func.__name__]
+            return func
+
+        return decorator
```

### Comparing `broker-0.2.9/broker/providers/ansible_tower.py` & `broker-0.3.0/broker/providers/ansible_tower.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,86 @@
 import click
 import inspect
 import json
 import yaml
 from urllib import parse as url_parser
-from functools import cached_property
+from functools import cache, cached_property
 from dynaconf import Validator
 from broker import exceptions
-from broker.helpers import find_origin, results_filter
+from broker.helpers import find_origin, eval_filter
 from broker.settings import settings
 from logzero import logger
 from datetime import datetime
 
 try:
     import awxkit
-except:
+except ImportError:
     raise exceptions.ProviderError(
         provider="AnsibleTower", message="Unable to import awxkit. Is it installed?"
     )
 
 from broker.providers import Provider
 from broker import helpers
 
 
+@cache
+def get_awxkit_and_uname(
+    config=None, root=None, url=None, token=None, uname=None, pword=None
+):
+    """Return an awxkit api object and resolved username"""
+    # Prefer token if its set, otherwise use username/password
+    # auth paths for the API taken from:
+    # https://github.com/ansible/awx/blob/ddb6c5d0cce60779be279b702a15a2fddfcd0724/awxkit/awxkit/cli/client.py#L85-L94
+    # unit test mock structure means the root API instance can't be loaded on the same line
+    config = config or awxkit.config
+    config.base_url = url
+    if root is None:
+        root = awxkit.api.Api()  # support mock stub for unit tests
+    if token:
+        helpers.emit(auth_type="token")
+        logger.info("Using token authentication")
+        config.token = token
+        try:
+            root.connection.login(
+                username=None, password=None, token=token, auth_type="Bearer"
+            )
+        except awxkit.exceptions.Unauthorized as err:
+            raise exceptions.AuthenticationError(err.args[0])
+        versions = root.get().available_versions
+        try:
+            # lookup the user that authenticated with the token
+            # If a username was specified in config, use that instead
+            my_username = uname or versions.v2.get().me.get().results[0].username
+        except (IndexError, AttributeError):
+            # lookup failed for whatever reason
+            raise exceptions.ProviderError(
+                provider="AnsibleTower",
+                message="Failed to lookup a username for the given token, please check credentials",
+            )
+    else:  # dynaconf validators should have checked that either token or password was provided
+        helpers.emit(auth_type="password")
+        if datetime.now() < datetime(2023, 2, 6):
+            time_based_modifier = " and will be unavailable soon"
+        else:
+            time_based_modifier = ""
+        logger.warning(
+            f"Password-based authentication is deprecated{time_based_modifier}. "
+            "Please use a token instead.\n"
+            "See https://docs.ansible.com/automation-controller/latest/html/userguide/"
+            "applications_auth.html#applications-tokens for more information"
+        )
+
+        config.credentials = {"default": {"username": uname, "password": pword}}
+        config.use_sessions = True
+        root.load_session().get()
+        versions = root.available_versions
+        my_username = uname
+    return versions.v2.get(), my_username
+
+
 class AnsibleTower(Provider):
 
     _validators = [
         Validator("ANSIBLETOWER.release_workflow", default="remove-vm"),
         Validator("ANSIBLETOWER.extend_workflow", default="extend-vm"),
         Validator("ANSIBLETOWER.new_expire_time", default="+172800"),
         Validator("ANSIBLETOWER.workflow_timeout", is_type_of=int, default=3600),
@@ -68,71 +123,39 @@
         click.option(
             "--new-expire-time",
             type=str,
             help="Time host should expire or time added to host reservation.",
         ),
     ]
 
+    _sensitive_attrs = ["pword", "password", "token"]
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         # get our instance settings
         self.url = settings.ANSIBLETOWER.base_url
         self.uname = settings.ANSIBLETOWER.get("username")
         self.pword = settings.ANSIBLETOWER.get("password")
         self.token = settings.ANSIBLETOWER.get("token")
         self._inventory = (
             kwargs.get("tower_inventory") or settings.ANSIBLETOWER.inventory
         )
         # Init the class itself
-        config = kwargs.get("config", awxkit.config)
-        config.base_url = self.url
+        config = kwargs.get("config")
         root = kwargs.get("root")
-        if root is None:
-            root = awxkit.api.Api()  # support mock stub for unit tests
-        # Prefer token if its set, otherwise use username/password
-        # auth paths for the API taken from:
-        # https://github.com/ansible/awx/blob/ddb6c5d0cce60779be279b702a15a2fddfcd0724/awxkit/awxkit/cli/client.py#L85-L94
-        # unit test mock structure means the root API instance can't be loaded on the same line
-        if self.token:
-            helpers.emit(auth_type="token")
-            logger.info("Using token authentication")
-            config.token = self.token
-            try:
-                root.connection.login(
-                    username=None, password=None, token=self.token, auth_type="Bearer"
-                )
-            except awxkit.exceptions.Unauthorized as err:
-                raise exceptions.AuthenticationError(err.args[0])
-            versions = root.get().available_versions
-            try:
-                # lookup the user that authenticated with the token
-                # If a username was specified in config, use that instead
-                my_username = (
-                    self.uname or versions.v2.get().me.get().results[0].username
-                )
-            except (IndexError, AttributeError):
-                # lookup failed for whatever reason
-                raise exceptions.ProviderError(
-                    provider="AnsibleTower",
-                    message="Failed to lookup a username for the given token, please check credentials",
-                )
-        else:  # dynaconf validators should have checked that either token or password was provided
-            helpers.emit(auth_type="password")
-            logger.info("Using username and password authentication")
-            config.credentials = {
-                "default": {"username": self.uname, "password": self.pword}
-            }
-            config.use_sessions = True
-            root.load_session().get()
-            versions = root.available_versions
-            my_username = self.uname
-        self.v2 = versions.v2.get()
+        self.v2, self.username = get_awxkit_and_uname(
+            config=config,
+            root=root,
+            url=self.url,
+            token=self.token,
+            uname=self.uname,
+            pword=self.pword,
+        )
         # Check to see if we're running AAP (ver 4.0+)
         self._is_aap = False if self.v2.ping.get().version[0] == "3" else True
-        self.username = my_username
 
     @staticmethod
     def _pull_params(kwargs):
         """Given a kwarg dict, separate AT-specific parameters from other kwargs
         AT-specific params must stat with double underscores.
         Example: __page_size
         """
@@ -157,23 +180,25 @@
         if prov_inv:
             logger.debug(f"prov_inv: {prov_inv}")
             broker_args["inventory"] = prov_inv
         caller_host._prov_inst.release(
             broker_args.get("source_vm", caller_host.name), broker_args
         )
 
-    def _set_attributes(self, host_inst, broker_args=None):
+    def _set_attributes(self, host_inst, broker_args=None, misc_attrs=None):
         host_inst.__dict__.update(
             {
                 "release": self._host_release,
                 "_prov_inst": self,
                 "_broker_provider": "AnsibleTower",
                 "_broker_args": broker_args,
             }
         )
+        if isinstance(misc_attrs, dict):
+            host_inst.__dict__.update(misc_attrs)
 
     def _translate_inventory(self, inventory):
         if isinstance(inventory, int):  # already an id, silly
             if inventory_info := self.v2.inventory.get(id=inventory):
                 return inventory_info.results[0].name
             else:
                 raise exceptions.ProviderError(
@@ -317,22 +342,27 @@
             time_stamp = (
                 self.v2.hosts.get(id=host_id)
                 .results[0]
                 .related.ansible_facts.get()
                 .expire_date
             )
             return str(datetime.fromtimestamp(int(time_stamp)))
-        except:
+        except Exception:
             return None
 
     def _compile_host_info(self, host):
+        # attempt to get the hostname from the host variables and then facts
+        if not (hostname := host.variables.get("fqdn")):
+            if hasattr(host_facts := host.related.ansible_facts.get(), "results"):
+                hostname = host_facts.results[0].ansible_facts.get("ansible_fqdn")
         host_info = {
             "name": host.name,
             "type": host.type,
-            "hostname": host.variables.get("fqdn"),
+            "hostname": hostname,
+            "ip": host.variables.get("ansible_host"),
             "tower_inventory": self._translate_inventory(host.inventory),
             "_broker_provider": "AnsibleTower",
             "_broker_provider_instance": self.instance,
             "_broker_args": getattr(host, "_broker_args", {}),
         }
         expire_time = self._get_expire_date(host.id)
         if expire_time:
@@ -347,28 +377,31 @@
             if "last_job" in host.related:
                 # potentially not create job, but easier processing below
                 create_job = host.get_related("last_job")
                 try:
                     host_info["_broker_args"]["workflow"] = host.get_related(
                         "last_job"
                     ).summary_fields.source_workflow_job.name
-                except:
+                except Exception:
                     logger.warning(
                         f"Unable to determine workflow for {host_info['hostname']}"
                     )
             else:
                 return host_info
         create_vars = json.loads(create_job.extra_vars)
         host_info["_broker_args"].update(
             {
                 arg: val
                 for arg, val in create_vars.items()
                 if val and isinstance(val, str)
             }
         )
+        # temporary workaround for OSP hosts that have lost their hostname
+        if not host_info["hostname"] and host.variables.get("openstack"):
+            host_info["hostname"] = host.variables["openstack"]["metadata"].get("fqdn")
         return host_info
 
     @cached_property
     def inventory(self):
         if not self._inventory:
             return
         elif isinstance(self._inventory, int):
@@ -383,28 +416,32 @@
         :param provider_params: dictionary of what the provider returns when initially
         creating the vm
 
         :param host_classes: host object
 
         :return: broker object of constructed host instance
         """
+        misc_attrs = {}  # used later to add misc attributes to host object
         if provider_params:
             job = provider_params
             job_attrs = self._merge_artifacts(
                 job, strategy=kwargs.get("strategy", "last")
             )
             # pull information about the job arguments
             job_extra_vars = json.loads(job.extra_vars)
             # and update them if they have resolved values
             for key in job_extra_vars.keys():
                 job_extra_vars[key] = job_attrs.get(key)
             kwargs.update({key: val for key, val in job_extra_vars.items() if val})
             kwargs.update({key: val for key, val in job_attrs.items() if val})
-            if "tower_inventory" in job_attrs:
-                kwargs["tower_inventory"] = job_attrs["tower_inventory"]
+            misc_attrs = {
+                "tower_inventory": job_attrs["tower_inventory"]
+                if "tower_inventory" in job_attrs
+                else self._translate_inventory(job.summary_fields.inventory)
+            }
             job_attrs = helpers.flatten_dict(job_attrs)
             logger.debug(job_attrs)
             hostname, name, host_type = None, None, "host"
             for key, value in job_attrs.items():
                 if key.endswith("fqdn") and not hostname:
                     hostname = value if not isinstance(value, list) else value[0]
                 if key in ("name", "vm_provisioned") and not name:
@@ -415,17 +452,18 @@
                 logger.warning(f"No hostname found in job attributes:\n{job_attrs}")
             logger.debug(f"hostname: {hostname}, name: {name}, host type: {host_type}")
             host_inst = host_classes[host_type](
                 **{**kwargs, "hostname": hostname, "name": name}
             )
         else:
             host_inst = host_classes[kwargs.get("type")](**kwargs)
-        self._set_attributes(host_inst, broker_args=kwargs)
+        self._set_attributes(host_inst, broker_args=kwargs, misc_attrs=misc_attrs)
         return host_inst
 
+    @Provider.register_action("workflow", "job_template")
     def execute(self, **kwargs):
         """Execute workflow or job template in Ansible Tower
 
         :param kwargs: workflow or job template name passed in a string
 
         :return: dictionary containing all information about executed workflow/job template
         """
@@ -453,16 +491,22 @@
             raise exceptions.ProviderError(
                 provider="AnsibleTower",
                 message=f"{subject.capitalize()} not found by name: {name}",
             )
         payload = {}
         if inventory := kwargs.pop("inventory", None):
             payload["inventory"] = inventory
+            logger.info(
+                f"Using tower inventory: {self._translate_inventory(inventory)}"
+            )
         elif self.inventory:
             payload["inventory"] = self.inventory
+            logger.info(
+                f"Using tower inventory: {self._translate_inventory(self.inventory)}"
+            )
         else:
             logger.info("No inventory specified, Ansible Tower will use a default.")
         payload["extra_vars"] = str(kwargs)
         logger.debug(
             f"Launching {subject}: {url_parser.urljoin(self.url, str(target.url))}\n"
             f"{payload=}"
         )
@@ -503,113 +547,117 @@
         ]
         hosts = []
         for inv in invs:
             inv_hosts = inv.get_related("hosts", page_size=200).results
             hosts.extend(inv_hosts)
         return [self._compile_host_info(host) for host in hosts]
 
-    def extend_vm(self, target_vm, new_expire_time=None):
+    def extend(self, target_vm, new_expire_time=None):
         """Run the extend workflow with defaults args
 
         :param target_vm: This should be a host object
         """
         # check if an inventory was specified. if so overwrite the current inventory
         if new_inv := target_vm._broker_args.get("tower_inventory"):
             if new_inv != self._inventory:
                 self._inventory = new_inv
-                del self.inventory  # clear the cached value
+                if hasattr(self.__dict__, 'inventory'):
+                    del self.inventory  # clear the cached value
         return self.execute(
             workflow=settings.ANSIBLETOWER.extend_workflow,
             target_vm=target_vm.name,
             new_expire_time=new_expire_time
             or settings.ANSIBLETOWER.get("new_expire_time"),
         )
 
+    @Provider.register_action("template", "inventory")
     def nick_help(self, **kwargs):
         """Get a list of extra vars and their defaults from a workflow"""
         results_limit = kwargs.get("results_limit", settings.ANSIBLETOWER.results_limit)
         if workflow := kwargs.get("workflow"):
             wfjt = self.v2.workflow_job_templates.get(name=workflow).results.pop()
+            default_inv = self.v2.inventory.get(id=wfjt.inventory).results.pop()
             logger.info(
+                f"\nDescription:\n{wfjt.description}\n\n"
                 f"Accepted additional nick fields:\n{helpers.yaml_format(wfjt.extra_vars)}"
+                f"tower_inventory: {default_inv['name']}"
             )
         elif kwargs.get("workflows"):
             workflows = [
                 workflow.name
                 for workflow in self.v2.workflow_job_templates.get(
                     page_size=1000
                 ).results
                 if workflow.summary_fields.user_capabilities.get("start")
             ]
             if res_filter := kwargs.get("results_filter"):
-                workflows = results_filter(workflows, res_filter)
+                workflows = eval_filter(workflows, res_filter, "res")
+                workflows = workflows if isinstance(workflows, list) else [workflows]
             workflows = "\n".join(workflows[:results_limit])
             logger.info(f"Available workflows:\n{workflows}")
         elif inventory := kwargs.get("inventory"):
             inv = self.v2.inventory.get(name=inventory, kind="").results.pop()
             inv = {"Name": inv.name, "ID": inv.id, "Description": inv.description}
             logger.info(f"Accepted additional nick fields:\n{helpers.yaml_format(inv)}")
         elif kwargs.get("inventories"):
             inv = [
                 inv.name
                 for inv in self.v2.inventory.get(kind="", page_size=1000).results
             ]
             if res_filter := kwargs.get("results_filter"):
-                inv = results_filter(inv, res_filter)
+                inv = eval_filter(inv, res_filter, "res")
+                inv = inv if isinstance(inv, list) else [inv]
             inv = "\n".join(inv[:results_limit])
             logger.info(f"Available Inventories:\n{inv}")
         elif job_template := kwargs.get("job_template"):
             jt = self.v2.job_templates.get(name=job_template).results.pop()
+            default_inv = self.v2.inventory.get(id=jt.inventory).results.pop()
             logger.info(
+                f"\nDescription:\n{jt.description}\n\n"
                 f"Accepted additional nick fields:\n{helpers.yaml_format(jt.extra_vars)}"
+                f"tower_inventory: {default_inv['name']}"
             )
         elif kwargs.get("job_templates"):
             job_templates = [
                 job_template.name
                 for job_template in self.v2.job_templates.get(page_size=1000).results
                 if job_template.summary_fields.user_capabilities.get("start")
             ]
             if res_filter := kwargs.get("results_filter"):
-                job_templates = results_filter(job_templates, res_filter)
+                job_templates = eval_filter(job_templates, res_filter, "res")
+                job_templates = job_templates if isinstance(job_templates, list) else [job_templates]
             job_templates = "\n".join(job_templates[:results_limit])
             logger.info(f"Available job templates:\n{job_templates}")
         elif kwargs.get("templates"):
             templates = list(
                 {
                     tmpl
                     for tmpl in self.execute(
                         workflow="list-templates", artifacts="last"
                     )["data_out"]["list_templates"]
                 }
             )
             templates.sort(reverse=True)
             if res_filter := kwargs.get("results_filter"):
-                templates = results_filter(templates, res_filter)
+                templates = eval_filter(templates, res_filter, "res")
+                templates = templates if isinstance(templates, list) else [templates]
             templates = "\n".join(templates[:results_limit])
             logger.info(f"Available templates:\n{templates}")
         else:
             logger.warning("That action is not yet implemented.")
 
     def release(self, name, broker_args=None):
-        if broker_args == None:
+        if broker_args is None:
             broker_args = {}
         return self.execute(
             workflow=settings.ANSIBLETOWER.release_workflow,
             source_vm=name,
             **broker_args,
         )
 
-    def __repr__(self):
-        inner = ", ".join(
-            f"{k}={v}"
-            for k, v in self.__dict__.items()
-            if not k.startswith("_") and not callable(v)
-        )
-        return f"{self.__class__.__name__}({inner})"
-
 
 def awxkit_representer(dumper, data):
     """In order to resolve awxkit objects, a custom representer is needed"""
     return dumper.represent_dict(dict(data))
 
 
 yaml.add_representer(awxkit.utils.PseudoNamespace, awxkit_representer)
```

### Comparing `broker-0.2.9/broker/providers/container.py` & `broker-0.3.0/broker/providers/container.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import cache
 import getpass
 import inspect
 from uuid import uuid4
 import click
 from logzero import logger
 from dynaconf import Validator
 from broker import exceptions
@@ -28,14 +29,27 @@
         caller_host._cont_inst = caller_host._prov_inst._cont_inst_by_name(
             caller_host.name
         )
     caller_host._cont_inst.remove(v=True, force=True)
     caller_host._checked_in = True
 
 
+@cache
+def get_runtime(
+    runtime_cls=None, host=None, username=None, password=None, port=None, timeout=None
+):
+    return runtime_cls(
+        host=host,
+        username=username,
+        password=password,
+        port=port,
+        timeout=timeout,
+    )
+
+
 class Container(Provider):
     _validators = [
         Validator("CONTAINER.runtime", default="podman"),
         Validator("CONTAINER.host", default="localhost"),
         Validator("CONTAINER.host_username", default="root"),
         Validator(
             "CONTAINER.host_password",
@@ -56,47 +70,39 @@
             "--container-app",
             type=str,
             help="Name of a container application image",
         ),
     ]
     _extend_options = []
 
+    _sensitive_attrs = ["password", "host_password"]
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if kwargs.get("bind") is not None:
             self._runtime_cls = kwargs.pop("bind")
         elif settings.container.runtime.lower() == "podman":
             self._runtime_cls = containers.PodmanBind
         elif settings.container.runtime.lower() == "docker":
             self._runtime_cls = containers.DockerBind
         else:
             raise exceptions.ProviderError(
                 "Container",
                 f"Broker has no bind for {settings.container.runtime} containers",
             )
-        self.runtime = self._runtime_cls(
+        self.runtime = get_runtime(
+            runtime_cls=self._runtime_cls,
             host=settings.container.host,
             username=settings.container.host_username,
             password=settings.container.host_password,
             port=settings.container.host_port,
             timeout=settings.container.timeout,
         )
         self._name_prefix = settings.container.get("name_prefix", getpass.getuser())
 
-
-    def _post_pickle(self, purified):
-        self._validate_settings()
-        self.runtime = self._runtime_cls(
-            host=settings.container.host,
-            username=settings.container.host_username,
-            password=settings.container.host_password,
-            port=settings.container.host_port,
-            timeout=settings.container.timeout,
-        )
-
     def _ensure_image(self, name):
         """Check if an image exists on the provider, attempt a pull if not"""
         for image in self.runtime.images:
             if name in image.tags:
                 return
             elif ("localhost/" in name) and (name[10:] in image.tags):
                 return
@@ -215,21 +221,23 @@
         elif kwargs.get("container_hosts"):
             images = [
                 img.tags[0]
                 for img in self.runtime.images
                 if img.labels.get("broker_compatible") and img.tags
             ]
             if res_filter := kwargs.get("results_filter"):
-                images = helpers.results_filter(images, res_filter)
+                images = helpers.eval_filter(images, res_filter, "res")
+                images = images if isinstance(images, list) else [images]
             images = "\n".join(images[:results_limit])
             logger.info(f"Available host images:\n{images}")
         elif kwargs.get("container_apps"):
             images = [img.tags[0] for img in self.runtime.images if img.tags]
             if res_filter := kwargs.get("results_filter"):
-                images = helpers.results_filter(images, res_filter)
+                images = helpers.eval_filter(images, res_filter, "res")
+                images = images if isinstance(images, list) else [images]
             images = "\n".join(images[:results_limit])
             logger.info(f"Available app images:\n{images}")
 
     def get_inventory(self, name_prefix):
         """Get all containers that have a matching name prefix"""
         name_prefix = name_prefix or self._name_prefix
         return [
@@ -240,33 +248,40 @@
 
     def extend(self):
         pass
 
     def release(self, host_obj):
         host_obj._cont_inst.remove(force=True)
 
+    @Provider.register_action("container_host")
     def run_container(self, container_host, **kwargs):
         """Start a container based on an image name (container_host)"""
         self._ensure_image(container_host)
         if not kwargs.get("name"):
             kwargs["name"] = self._gen_name()
         kwargs["ports"] = self._port_mapping(container_host, **kwargs)
+
+        envars = kwargs.get('environment', {})
+        if isinstance(envars, str):
+            envars = {var.split('=')[0]: var.split('=')[1] for var in envars.split(',')}
         # add some context information about the container's requester
-        envars, origin = {}, helpers.find_origin()
+        origin = helpers.find_origin()
+
         if "for" in origin:
             origin = origin.split()[-1]
         envars["BROKER_ORIGIN"] = origin[0]
         if origin[1]:
             envars["JENKINS_URL"] = origin[1]
         kwargs["environment"] = envars
         kwargs["labels"] = envars
         container_inst = self.runtime.create_container(container_host, **kwargs)
         container_inst.start()
         return container_inst
 
+    @Provider.register_action("container_app")
     def execute(self, container_app, **kwargs):
         """Run a container and return the raw results"""
         return self.runtime.execute(container_app, **kwargs)
 
     def run_wait_container(self, image_name, **kwargs):
         cont_inst = self.run_container(image_name, **kwargs)
         cont_inst.wait(condition="excited")
```

### Comparing `broker-0.2.9/broker/providers/test_provider.py` & `broker-0.3.0/broker/providers/test_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,27 @@
     def construct_host(self, provider_params, host_classes, **kwargs):
         host_params = provider_params.copy()
         host_params.update(kwargs)
         host_inst = host_classes[host_params["host_type"]](**host_params)
         self._set_attributes(host_inst, broker_args=kwargs)
         return host_inst
 
+    @Provider.register_action()
     def test_action(self, **kwargs):
         action = kwargs.get("test_action")
         if action == "release":
             return "released", kwargs
         if action in HOST_PROPERTIES:
             return HOST_PROPERTIES
         return HOST_PROPERTIES["basic"]
 
     def release(self, host_obj):
         return self.test_action(test_action="release", **host_obj.to_dict())
+
+    def extend(self):
+        pass
+
+    def get_inventory(self, **kwargs):
+        pass
+
+    def nick_help(self):
+        pass
```

### Comparing `broker-0.2.9/broker/session.py` & `broker-0.3.0/broker/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import socket
+import tempfile
 from pathlib import Path
 from logzero import logger
 from ssh2.session import Session as ssh2_Session
 from ssh2 import sftp as ssh2_sftp
 from broker import helpers
 
 SESSIONS = {}
@@ -72,63 +73,78 @@
         return results
 
     def shell(self, pty=False):
         """Create and return an interactive shell instance"""
         channel = self.session.open_session()
         return InteractiveShell(channel, pty)
 
-    def sftp_read(self, source, destination=None):
-        """read a remote file into a local destination"""
-        if not destination:
-            destination = source
-        # create the destination path if it doesn't exist
-        destination = Path(destination)
-        destination.parent.mkdir(parents=True, exist_ok=True)
-        destination.touch()
+    def sftp_read(self, source, destination=None, return_data=False):
+        """read a remote file into a local destination or return a bytes object if return_data is True"""
+        if not return_data:
+            if not destination:
+                destination = source
+            elif destination.endswith("/"):
+                destination = destination + Path(source).name
+            # create the destination path if it doesn't exist
+            destination = Path(destination)
+            destination.parent.mkdir(parents=True, exist_ok=True)
         # initiate the sftp session, read data, write it to a local destination
         sftp = self.session.sftp_init()
         with sftp.open(
             source, ssh2_sftp.LIBSSH2_FXF_READ, ssh2_sftp.LIBSSH2_SFTP_S_IRUSR
         ) as remote:
-            with destination.open("wb") as local:
-                for size, data in remote:
-                    local.write(data)
+            captured_data = bytes()
+            for rc, data in remote:
+                captured_data += data
+            if return_data:
+                return captured_data
+            destination.write_bytes(data)
 
-    def sftp_write(self, source, destination=None):
+    def sftp_write(self, source, destination=None, ensure_dir=True):
         """sftp write a local file to a remote destination"""
         if not destination:
             destination = source
+        elif destination.endswith("/"):
+            destination = destination + Path(source).name
         data = Path(source).read_bytes()
+        if ensure_dir:
+            self.run(f"mkdir -p {Path(destination).absolute().parent}")
         sftp = self.session.sftp_init()
         with sftp.open(destination, FILE_FLAGS, SFTP_MODE) as remote:
             remote.write(data)
 
-    def remote_copy(self, source, dest_host):
+    def remote_copy(self, source, dest_host, ensure_dir=True):
         """Copy a file from this host to another"""
         sftp_down = self.session.sftp_init()
         sftp_up = dest_host.session.session.sftp_init()
+        if ensure_dir:
+            dest_host.run(f"mkdir -p {Path(source).absolute().parent}")
         with sftp_down.open(
             source, ssh2_sftp.LIBSSH2_FXF_READ, ssh2_sftp.LIBSSH2_SFTP_S_IRUSR
         ) as download:
             with sftp_up.open(source, FILE_FLAGS, SFTP_MODE) as upload:
                 for size, data in download:
                     upload.write(data)
 
-    def scp_write(self, source, destination=None):
+    def scp_write(self, source, destination=None, ensure_dir=True):
         """scp write a local file to a remote destination"""
         if not destination:
             destination = source
+        elif destination.endswith("/"):
+            destination = destination + Path(source).name
         fileinfo = os.stat(source)
         chan = self.session.scp_send64(
             destination,
             fileinfo.st_mode & 0o777,
             fileinfo.st_size,
             fileinfo.st_mtime,
             fileinfo.st_atime,
         )
+        if ensure_dir:
+            self.run(f"mkdir -p {Path(destination).absolute().parent}")
         with open(source, "rb") as local:
             for data in local:
                 chan.write(data)
 
     def __enter__(self):
         return self
 
@@ -196,61 +212,83 @@
     def __init__(self, cont_inst):
         self._cont_inst = cont_inst
 
     def run(self, command, demux=True, **kwargs):
         """This is the container approximation of Session.run"""
         kwargs.pop("timeout", None)  # Timeouts are set at the client level
         kwargs["demux"] = demux
+        if "'" in command:
+            with tempfile.NamedTemporaryFile(mode="w", suffix=".sh") as tmp:
+                tmp.write(command)
+                tmp.seek(0)
+                command = f"/bin/bash {tmp.name}"
+                self.sftp_write(tmp.name)
         if any([s in command for s in "|&><"]):
             # Containers don't handle pipes, redirects, etc well in a bare exec_run
             command = f"/bin/bash -c '{command}'"
         result = self._cont_inst._cont_inst.exec_run(command, **kwargs)
         if demux:
             result = helpers.Result.from_duplexed_exec(result)
         else:
             result = helpers.Result.from_nonduplexed_exec(result)
         return result
 
     def disconnect(self):
         """Needed for simple compatability with Session"""
         pass
 
-    def sftp_write(self, source, destination=None):
+    def sftp_write(self, source, destination=None, ensure_dir=True):
         """Add one of more files to the container"""
         # ensure source is a list of Path objects
         if not isinstance(source, list):
             source = [Path(source)]
         else:
             source = [Path(src) for src in source]
         # validate each source's existenence
         for src in source:
             if not Path(src).exists():
                 raise FileNotFoundError(src)
-        destination = destination or source[0].parent
+        destination = destination or f"{source[0].parent}/"
         # Files need to be added to a tarfile
         with helpers.temporary_tar(source) as tar:
             logger.debug(
                 f"{self._cont_inst.hostname} adding file(s) {source} to {destination}"
             )
+            if ensure_dir:
+                if destination.endswith("/"):
+                    self.run(f"mkdir -m 666 -p {destination}")
+                else:
+                    self.run(f"mkdir -m 666 -p {Path(destination).parent}")
             self._cont_inst._cont_inst.put_archive(str(destination), tar.read_bytes())
 
-    def sftp_read(self, source, destination=None):
+    def sftp_read(self, source, destination=None, return_data=False):
         """Get a file or directory from the container"""
         destination = Path(destination or source)
-        logger.debug(
-            f"{self._cont_inst.hostname} getting file {source} from {destination}"
-        )
+        logger.debug(f"{self._cont_inst.hostname} getting file {source}")
         data, status = self._cont_inst._cont_inst.get_archive(source)
         logger.debug(f"{self._cont_inst.hostname}: {status}")
-        all_data = b"".join(d for d in data)
+        data = b"".join(d for d in data)
         if destination.name == "_raw":
-            return all_data
-        with helpers.data_to_tempfile(all_data, as_tar=True) as tar:
-            logger.debug(f"Extracting {source} to {destination}")
-            tar.extractall(destination.parent if destination.is_file() else destination)
+            return data
+        with helpers.data_to_tempfile(data, as_tar=True) as tar:
+            del data
+            if len(tar.getmembers()) == 1:
+                f = tar.extractfile(tar.getmember(Path(source).name))
+                if return_data:
+                    logger.debug(f"Extracting {source}")
+                    return f.read()
+                else:
+                    logger.debug(f"Extracting {source} to {destination}")
+                    destination.parent.mkdir(parents=True, exist_ok=True)
+                    destination.write_bytes(f.read())
+            else:
+                logger.warning("More than one member was found in the tar file.")
+                tar.extractall(
+                    destination.parent if destination.is_file() else destination
+                )
 
     def shell(self, pty=False):
         """Create and return an interactive shell instance"""
         raise NotImplementedError("ContainerSession.shell has not been implemented")
 
     def __enter__(self):
         return self
```

### Comparing `broker-0.2.9/broker.egg-info/SOURCES.txt` & `broker-0.3.0/broker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .gitignore
 Dockerfile
-HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
 broker_settings.yaml.example
+catalog-info.yaml
 pytest.ini
 setup.cfg
 setup.py
 .github/workflows/codeql-analysis.yml
 .github/workflows/python-publish.yml
 .github/workflows/update_broker_image.yml
 broker/__init__.py
@@ -38,14 +38,15 @@
 tests/test_broker.py
 tests/test_helpers.py
 tests/test_settings.py
 tests/data/args_file.json
 tests/data/args_file.yaml
 tests/data/broker_args.json
 tests/data/broker_args.yaml
+tests/data/fake_inventory.yaml
 tests/data/ansible_tower/fake_children.json
 tests/data/ansible_tower/fake_jobs.json
 tests/data/ansible_tower/fake_workflows.json
 tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
 tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
 tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
 tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
```

### Comparing `broker-0.2.9/broker_settings.yaml.example` & `broker-0.3.0/broker_settings.yaml.example`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Broker settings
-debug: False
-inventory_file: "inventory.yaml"
+# different log levels for file and stdout
+logging:
+    console_level: info
+    file_level: debug
 # Host Settings
+# These can be left alone if you're not using Broker as a library
 host_username: "root"
 host_password: "<password>"
 host_ssh_port: "<port>"
 host_ssh_key_filename: "</path/to/the/ssh-key>"
 # Provider settings
 AnsibleTower:
     instances:
@@ -49,14 +52,15 @@
 TestProvider:
     instances:
         - test1:
             foo: "bar"
             default: True
         - test2:
             foo: "baz"
+            override_envars: True
         - bad:
             nothing: False
     config_value: "something"
 # You can set a nickname as a shortcut for arguments
 nicks:
     rhel7:
         workflow: "deploy-base-rhel"
```

### Comparing `broker-0.2.9/setup.cfg` & `broker-0.3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [metadata]
 name = broker
 description = The infrastructure middleman.
-long_description = file: README.md, HISTORY.md
+long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jacob J Callahan
 author_email = jacob.callahan05@gmail.com
 url = https://github.com/SatelliteQE/broker
 license = GNU General Public License v3
 keywords = broker, AnsibleTower
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Natural Language :: English
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 install_requires = 
 	awxkit
 	click
 	dynaconf>=3.1.0
 	logzero
@@ -42,11 +42,14 @@
 	paramiko
 podman = podman-py
 
 [options.entry_points]
 console_scripts = 
 	broker = broker.commands:cli
 
+[flake8]
+max-line-length = 110
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `broker-0.2.9/tests/data/ansible_tower/fake_children.json` & `broker-0.3.0/tests/data/ansible_tower/fake_children.json`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/tests/data/ansible_tower/fake_jobs.json` & `broker-0.3.0/tests/data/ansible_tower/fake_jobs.json`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/tests/data/container/fake_containers.json` & `broker-0.3.0/tests/data/container/fake_containers.json`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/tests/data/container/fake_images.json` & `broker-0.3.0/tests/data/container/fake_images.json`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/tests/functional/README.md` & `broker-0.3.0/tests/functional/README.md`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/tests/providers/test_ansible_tower.py` & `broker-0.3.0/tests/providers/test_ansible_tower.py`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/tests/providers/test_container.py` & `broker-0.3.0/tests/providers/test_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from asyncio import QueueEmpty
 import json
 import pytest
 from broker.broker import Broker
 from broker.providers.container import Container
 from broker.helpers import MockStub
```

### Comparing `broker-0.2.9/tests/test_broker.py` & `broker-0.3.0/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `broker-0.2.9/tests/test_settings.py` & `broker-0.3.0/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 @pytest.mark.parametrize(
     "set_envars", [("BROKER_TESTPROVIDER__foo", "override me")], indirect=True
 )
 def test_nondefault_envar(set_envars):
     """Set a top-level instance value via environment variable
     then verify that the value has been overriden when the provider is specified.
     """
-    test_provider = TestProvider(TestProvider="test1")
-    assert test_provider.instance == "test1"
-    assert test_provider.foo == "bar"
+    test_provider = TestProvider(TestProvider="test2")
+    assert test_provider.instance == "test2"
+    assert test_provider.foo == "baz"
 
 
 @pytest.mark.parametrize(
     "set_envars", [("VAULT_ENABLED_FOR_DYNACONF", "1")], indirect=True
 )
 def test_purge_vault_envars(set_envars):
     """Set dynaconf vault envars and verify that they have no effect"""
```

