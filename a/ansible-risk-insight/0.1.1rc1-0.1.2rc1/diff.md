# Comparing `tmp/ansible-risk-insight-0.1.1rc1.tar.gz` & `tmp/ansible-risk-insight-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.1rc1.tar", last modified: Mon Apr  3 07:09:13 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.2rc1.tar", last modified: Mon Apr 10 02:38:49 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.1rc1.tar` & `ansible-risk-insight-0.1.2rc1.tar`

### file list

```diff
@@ -1,215 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.978188 ansible-risk-insight-0.1.1rc1/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.922389 ansible-risk-insight-0.1.1rc1/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.928377 ansible-risk-insight-0.1.1rc1/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.1rc1/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.1rc1/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.1rc1/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.1rc1/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-03 07:09:13.977963 ansible-risk-insight-0.1.1rc1/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.1rc1/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.939472 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-03-24 05:43:40.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-03 07:08:49.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3378 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.942225 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.946661 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9100 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   828053 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.946880 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     6600 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.948923 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     2863 2023-03-31 00:25:16.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31412 2023-02-07 04:27:38.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    41806 2023-03-30 03:55:16.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    10101 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8733 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    58114 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    73355 2023-04-03 02:24:40.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5239 2023-03-31 00:25:16.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    40464 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)    10820 2023-04-03 02:53:03.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.964821 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4041 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     4088 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     4543 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    44858 2023-03-31 00:25:16.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    38347 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.940405 ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-03 07:09:13.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8051 2023-04-03 07:09:13.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-03 07:09:13.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-03 07:09:13.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       85 2023-04-03 07:09:13.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-03 07:09:13.000000 ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.1rc1/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.923122 ansible-risk-insight-0.1.1rc1/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.967609 ansible-risk-insight-0.1.1rc1/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.1rc1/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.1rc1/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.1rc1/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.1rc1/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.969542 ansible-risk-insight-0.1.1rc1/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.1rc1/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.1rc1/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.1rc1/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.1rc1/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.973338 ansible-risk-insight-0.1.1rc1/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.1rc1/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.973900 ansible-risk-insight-0.1.1rc1/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.974282 ansible-risk-insight-0.1.1rc1/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.1rc1/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.1rc1/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.974590 ansible-risk-insight-0.1.1rc1/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.1rc1/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.1rc1/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.1rc1/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      980 2023-03-24 05:44:37.000000 ansible-risk-insight-0.1.1rc1/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-03 07:09:13.978702 ansible-risk-insight-0.1.1rc1/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.1rc1/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.974877 ansible-risk-insight-0.1.1rc1/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.1rc1/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.924288 ansible-risk-insight-0.1.1rc1/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.923825 ansible-risk-insight-0.1.1rc1/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.975627 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.923968 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.924197 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.975905 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.976208 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.976517 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.924341 ansible-risk-insight-0.1.1rc1/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.924556 ansible-risk-insight-0.1.1rc1/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.976761 ansible-risk-insight-0.1.1rc1/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.977372 ansible-risk-insight-0.1.1rc1/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-03 07:09:13.977624 ansible-risk-insight-0.1.1rc1/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.1rc1/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.1rc1/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.711360 ansible-risk-insight-0.1.2rc1/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.640038 ansible-risk-insight-0.1.2rc1/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.650149 ansible-risk-insight-0.1.2rc1/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.2rc1/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-10 02:38:49.711165 ansible-risk-insight-0.1.2rc1/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.662224 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-10 02:37:44.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.666080 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.673412 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9100 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   828053 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.673765 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7085 2023-04-04 15:35:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.676236 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31556 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-10 01:04:18.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    10390 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    59635 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    73975 2023-04-10 01:06:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5452 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    40173 2023-04-10 02:35:50.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8059 2023-04-04 15:35:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.695936 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4041 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4088 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4543 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-03 07:57:55.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46105 2023-04-04 16:17:13.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    38570 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.663637 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.641546 ansible-risk-insight-0.1.2rc1/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.698915 ansible-risk-insight-0.1.2rc1/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.701207 ansible-risk-insight-0.1.2rc1/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.2rc1/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.2rc1/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.706182 ansible-risk-insight-0.1.2rc1/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.706828 ansible-risk-insight-0.1.2rc1/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707275 ansible-risk-insight-0.1.2rc1/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707614 ansible-risk-insight-0.1.2rc1/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.2rc1/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2rc1/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-10 02:38:49.711431 ansible-risk-insight-0.1.2rc1/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707948 ansible-risk-insight-0.1.2rc1/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643942 ansible-risk-insight-0.1.2rc1/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643004 ansible-risk-insight-0.1.2rc1/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.708757 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643287 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643774 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709171 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709470 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709826 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.644092 ansible-risk-insight-0.1.2rc1/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.644604 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710133 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710436 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710765 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.2rc1/tox.ini
```

### Comparing `ansible-risk-insight-0.1.1rc1/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.2rc1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/.github/workflows/test.yml` & `ansible-risk-insight-0.1.2rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/.gitignore` & `ansible-risk-insight-0.1.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/CONTRIBUTING.md` & `ansible-risk-insight-0.1.2rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/LICENSE` & `ansible-risk-insight-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/README.md` & `ansible-risk-insight-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.1-rc1"
+__version__ = "0.1.2-rc1"
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,32 @@
 from typing import List
 from ansible_risk_insight.annotators.risk_annotator_base import RiskAnnotator
 import ansible_risk_insight.logger as logger
 from .models import TaskCallsInTree, AnsibleRunContext
 from .utils import load_classes_in_dir
 
 
+annotator_cache = []
+
+
 def load_annotators(ctx: AnsibleRunContext = None):
+    global annotator_cache
+
+    if annotator_cache:
+        return annotator_cache
+
     _annotator_classes, _ = load_classes_in_dir("annotators", RiskAnnotator, __file__)
     _annotators = []
     for a in _annotator_classes:
         try:
             _annotator = a(context=ctx)
             _annotators.append(_annotator)
         except Exception:
             raise ValueError(f"failed to load an annotator: {a}")
+    annotator_cache = _annotators
     return _annotators
 
 
 def load_taskcalls_in_trees(path: str) -> List[TaskCallsInTree]:
     taskcalls_in_trees = []
     try:
         with open(path, "r") as file:
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,16 +43,18 @@
         parser.add_argument("--taskfile-only", action="store_true", help="if true, don't load playbooks/roles arround the specified taskfile")
         parser.add_argument("--skip-install", action="store_true", help="if true, skip install for the specified target")
         parser.add_argument("--dependency-dir", nargs="?", help="path to a directory that have dependencies for the target")
         parser.add_argument("--collection-name", nargs="?", help="if provided, use it as a collection name")
         parser.add_argument("--role-name", nargs="?", help="if provided, use it as a role name")
         parser.add_argument("--source", help="source server name in ansible config file (if empty, use public ansible galaxy)")
         parser.add_argument("--without-ram", action="store_true", help="if true, RAM data is not used and not even updated")
+        parser.add_argument("--read-ram-for-dependency", action="store_true", help="if true, RAM data is used only for dependency")
         parser.add_argument("--update-ram", action="store_true", help="if true, RAM data is not used for scan but updated with the scan result")
         parser.add_argument("--include-tests", action="store_true", help='if true, load test contents in "tests/integration/targets"')
+        parser.add_argument("--silent", action="store_true", help='if true, do not print anything"')
         parser.add_argument("--objects", action="store_true", help="if true, output objects.json to the output directory")
         parser.add_argument("--show-all", action="store_true", help="if true, show findings even if missing dependencies are found")
         parser.add_argument("--json", help="if specified, show findings in json format")
         parser.add_argument("--yaml", help="if specified, show findings in yaml format")
         parser.add_argument("-o", "--out-dir", help="output directory for the rule evaluation result")
         parser.add_argument(
             "-r", "--rules-dir", help=f"specify custom rule directories. use `-R` instead to ignore default rules in {config.rules_dir}"
@@ -95,40 +97,46 @@
 
         rules_dir = config.rules_dir
         if args.rules_dir_without_default:
             rules_dir = args.rules_dir_without_default
         elif args.rules_dir:
             rules_dir = args.rules_dir + ":" + config.rules_dir
 
-        silent = False
+        silent = args.silent
         pretty = False
         output_format = ""
         if args.json or args.yaml:
             silent = True
             pretty = True
             if args.json:
                 output_format = "json"
             elif args.yaml:
                 output_format = "yaml"
 
         read_ram = True
         write_ram = True
+        read_ram_for_dependency = False
         if args.without_ram:
             read_ram = False
             write_ram = False
         elif args.update_ram:
             read_ram = False
             write_ram = True
+        elif args.read_ram_for_dependency:
+            read_ram_for_dependency = True
+            read_ram = False
+            write_ram = False
 
         c = ARIScanner(
             root_dir=config.data_dir,
             rules_dir=rules_dir,
             do_save=args.save,
             read_ram=read_ram,
             write_ram=write_ram,
+            read_ram_for_dependency=read_ram_for_dependency,
             show_all=args.show_all,
             silent=silent,
             pretty=pretty,
             output_format=output_format,
         )
         if not silent and not pretty:
             print("Start preparing dependencies")
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/generate.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     def __init__(self):
         parser = argparse.ArgumentParser(description="TODO")
         parser.add_argument("target_type", help="content type", choices={"ram"})
         parser.add_argument("action", help="action for RAM command or target_name of search action")
         parser.add_argument("-f", "--file", help='target list like "collection community.general"')
         parser.add_argument("-r", "--resume", help="line number to resume scanning")
+        parser.add_argument("--serial", action="store_true", help="if True, do not parallelize ram generation")
         parser.add_argument("--no-module-spec", action="store_true", help="if True, ansible-doc is not used")
         parser.add_argument("--download-only", action="store_true", help="if True, just download the content")
         parser.add_argument("--include-tests", action="store_true", help='if true, load test contents in "tests/integration/targets"')
         parser.add_argument("--no-retry", action="store_true", help="if True, not retry failed items.")
         parser.add_argument("-o", "--out-dir", help="output directory for the rule evaluation result")
         args = parser.parse_args()
         self.args = args
@@ -49,17 +50,23 @@
                 if len(parts) != 2:
                     raise ValueError('target list file must be lines of "<type> <name>" such as "collection community.general"')
                 target_list.append((parts[0], parts[1]))
 
         resume = -1
         if args.resume:
             resume = int(args.resume)
+
+        parallel = True
+        if args.serial:
+            parallel = False
+
         ram_generator = RAMGenerator(
             target_list=target_list,
             resume=resume,
+            parallel=parallel,
             download_only=args.download_only,
             include_test_contents=args.include_tests,
             out_dir=args.out_dir,
             no_module_spec=args.no_module_spec,
             no_retry=args.no_retry,
         )
         ram_generator.run()
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,14 +686,16 @@
     for b in found_var_blocks:
         parts = b.split("|")
         var_name = ""
         default_var_name = ""
         for i, p in enumerate(parts):
             if i == 0:
                 var_name = p.replace("{{", "").replace("}}", "").replace(" ", "")
+                if "lookup(" in var_name and "first_found" in var_name:
+                    var_name = var_name.split(",")[-1].replace(")", "")
             else:
                 if "default(" in p and ")" in p:
                     default_var = p.replace("}}", "").replace("default(", "").replace(")", "").replace(" ", "")
                     if not default_var.startswith('"') and not default_var.startswith("'") and not re.compile(r"[0-9].*").match(default_var):
                         default_var_name = default_var
         tmp_b = {
             "original": b,
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,18 +113,27 @@
     dependency_dirs: list = field(default_factory=list)
 
     def prepare_dir(self, root_install=True, is_src_installed=False, cache_enabled=False, cache_dir=""):
         logger.debug("setup base dirs")
         self.setup_dirs(cache_enabled, cache_dir)
         logger.debug("prepare target dir")
         self.prepare_root_dir(root_install, is_src_installed, cache_enabled, cache_dir)
-        logger.debug("search dependencies")
-        dependencies = find_dependency(self.target_type, self.target_path, self.target_dependency_dir)
-        logger.debug("prepare dir for dependencies")
-        self.prepare_dependency_dir(dependencies, cache_enabled, cache_dir)
+
+        prepare_dependency = False
+        # if a project target is a local path, check dependency
+        if self.target_type in [LoadType.PROJECT, LoadType.PLAYBOOK, LoadType.TASKFILE] and not is_url(self.target_name):
+            prepare_dependency = True
+        # if a collection/role is a local path, check dependency
+        if self.target_type in [LoadType.COLLECTION, LoadType.ROLE] and is_local_path(self.target_name):
+            prepare_dependency = True
+        if prepare_dependency:
+            logger.debug("search dependencies")
+            dependencies = find_dependency(self.target_type, self.target_path, self.target_dependency_dir)
+            logger.debug("prepare dir for dependencies")
+            self.prepare_dependency_dir(dependencies, cache_enabled, cache_dir)
         return self.dependency_dirs
 
     def setup_dirs(self, cache_enabled=False, cache_dir=""):
         self.download_location = os.path.join(self.root_dir, "archives")
         self.dependency_dir_path = self.root_dir
         # check download_location
         if not os.path.exists(self.download_location):
@@ -185,184 +194,190 @@
 
         col_dependency_dirs = dependencies.get("paths", {}).get("collections", {})
         role_dependency_dirs = dependencies.get("paths", {}).get("roles", {})
 
         col_dependency_metadata = dependencies.get("metadata", {}).get("collections", {})
         # role_dependency_metadata = dependencies.get("metadata", {}).get("roles", {})
 
-        # TODO: if requirements.yml is provided, download dependencies using it.
-
-        for cdep in col_dependencies:
-            col_name = cdep
-            col_version = ""
-            if type(cdep) is dict:
-                col_name = cdep.get("name", "")
-                col_version = cdep.get("version", "")
-                if col_name == "":
-                    col_name = cdep.get("source", "")
-
-            logger.debug("prepare dir for {}:{}".format(col_name, col_version))
-            downloaded_dep = Dependency(
-                name=col_name,
-            )
-            downloaded_dep.metadata.type = LoadType.COLLECTION
-            downloaded_dep.metadata.name = col_name
-            downloaded_dep.metadata.cache_enabled = cache_enabled
-            sub_dependency_dir_path = os.path.join(
-                self.dependency_dir_path,
-                "collections",
-                "src",
-            )
-
-            if not os.path.exists(sub_dependency_dir_path):
-                os.makedirs(sub_dependency_dir_path)
+        if col_dependencies:
+            for cdep in col_dependencies:
+                col_name = cdep
+                col_version = ""
+                if type(cdep) is dict:
+                    col_name = cdep.get("name", "")
+                    col_version = cdep.get("version", "")
+                    if col_name == "":
+                        col_name = cdep.get("source", "")
+
+                logger.debug("prepare dir for {}:{}".format(col_name, col_version))
+                downloaded_dep = Dependency(
+                    name=col_name,
+                )
+                downloaded_dep.metadata.type = LoadType.COLLECTION
+                downloaded_dep.metadata.name = col_name
+                downloaded_dep.metadata.cache_enabled = cache_enabled
+                sub_dependency_dir_path = os.path.join(
+                    self.dependency_dir_path,
+                    "collections",
+                    "src",
+                )
 
-            if cache_enabled:
-                logger.debug("cache enabled")
-                # TODO: handle version
-                is_exist, targz_file = self.is_download_file_exist(LoadType.COLLECTION, col_name, cache_dir)
-                # check cache data
-                if is_exist:
-                    logger.debug("found cache data {}".format(targz_file))
-                    metadata_file = os.path.join(targz_file.rsplit("/", 1)[0], download_metadata_file)
-                    md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
-                    downloaded_dep.metadata = md
+                if not os.path.exists(sub_dependency_dir_path):
+                    os.makedirs(sub_dependency_dir_path)
+                if cache_enabled:
+                    logger.debug("cache enabled")
+                    # TODO: handle version
+                    is_exist, targz_file = self.is_download_file_exist(LoadType.COLLECTION, col_name, cache_dir)
+                    # check cache data
+                    if is_exist:
+                        logger.debug("found cache data {}".format(targz_file))
+                        metadata_file = os.path.join(targz_file.rsplit("/", 1)[0], download_metadata_file)
+                        md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
+                        downloaded_dep.metadata = md
+                    else:
+                        # if no cache data, download
+                        logger.debug("cache data not found")
+                        cache_location = os.path.join(cache_dir, "collection", col_name)
+                        install_msg = self.download_galaxy_collection(col_name, cache_location, col_version, self.source_repository)
+                        metadata = self.extract_collections_metadata(install_msg, cache_location)
+                        metadata_file = self.export_data(metadata, cache_location, download_metadata_file)
+                        md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
+                        downloaded_dep.metadata = md
+                        if md:
+                            targz_file = md.download_src_path
+                    # install collection from tar.gz
+                    self.install_galaxy_collection_from_targz(targz_file, sub_dependency_dir_path)
+                    downloaded_dep.metadata.cache_dir = targz_file
+                    parts = col_name.split(".")
+                    full_path = os.path.join(sub_dependency_dir_path, "ansible_collections", parts[0], parts[1])
+                    downloaded_dep.dir = full_path.replace(f"{self.root_dir}/", "")
+                elif col_name in col_dependency_dirs:
+                    logger.debug("use the specified dependency dirs")
+                    sub_dependency_dir_path = col_dependency_dirs[col_name]
+                    col_galaxy_data = col_dependency_metadata.get(col_name, {})
+                    if isinstance(col_galaxy_data, dict):
+                        download_url = col_galaxy_data.get("download_url", "")
+                        hash = ""
+                        if download_url:
+                            hash = get_hash_of_url(download_url)
+                        version = col_galaxy_data.get("version", "")
+                        downloaded_dep.metadata.source_repository = self.source_repository
+                        downloaded_dep.metadata.download_url = download_url
+                        downloaded_dep.metadata.hash = hash
+                        downloaded_dep.metadata.version = version
+                        downloaded_dep.dir = sub_dependency_dir_path
                 else:
-                    # if no cache data, download
-                    logger.debug("cache data not found")
-                    cache_location = os.path.join(cache_dir, "collection", col_name)
-                    install_msg = self.download_galaxy_collection(col_name, cache_location, col_version, self.source_repository)
-                    metadata = self.extract_collections_metadata(install_msg, cache_location)
-                    metadata_file = self.export_data(metadata, cache_location, download_metadata_file)
-                    md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
-                    downloaded_dep.metadata = md
-                    if md:
-                        targz_file = md.download_src_path
-                # install collection from tar.gz
-                self.install_galaxy_collection_from_targz(targz_file, sub_dependency_dir_path)
-                downloaded_dep.metadata.cache_dir = targz_file
-                parts = col_name.split(".")
-                downloaded_dep.dir = os.path.join(sub_dependency_dir_path, "ansible_collections", parts[0], parts[1])
-            elif col_name in col_dependency_dirs:
-                logger.debug("use the specified dependency dirs")
-                sub_dependency_dir_path = col_dependency_dirs[col_name]
-                col_galaxy_data = col_dependency_metadata.get(col_name, {})
-                if isinstance(col_galaxy_data, dict):
-                    download_url = col_galaxy_data.get("download_url", "")
-                    hash = ""
-                    if download_url:
-                        hash = get_hash_of_url(download_url)
-                    version = col_galaxy_data.get("version", "")
+                    logger.debug("download dependency {}".format(col_name))
+                    is_exist, targz = self.is_download_file_exist(
+                        LoadType.COLLECTION, col_name, os.path.join(self.download_location, "collection", col_name)
+                    )
+                    if is_exist:
+                        metadata_file = os.path.join(self.download_location, "collection", col_name, download_metadata_file)
+                        self.install_galaxy_collection_from_targz(targz, sub_dependency_dir_path)
+                        md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
+                    else:
+                        # check download_location
+                        sub_download_location = os.path.join(self.download_location, "collection", col_name)
+                        if not os.path.exists(sub_download_location):
+                            os.makedirs(sub_download_location)
+                        install_msg = self.download_galaxy_collection(col_name, sub_download_location, col_version, self.source_repository)
+                        metadata = self.extract_collections_metadata(install_msg, sub_download_location)
+                        metadata_file = self.export_data(metadata, sub_download_location, download_metadata_file)
+                        md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
+                        if md:
+                            self.install_galaxy_collection_from_reqfile(md.requirements_file, sub_dependency_dir_path)
+                        # self.install_galaxy_collection_from_targz(md.download_src_path, sub_dependency_dir_path)
+                    if md is not None:
+                        downloaded_dep.metadata = md
                     downloaded_dep.metadata.source_repository = self.source_repository
-                    downloaded_dep.metadata.download_url = download_url
-                    downloaded_dep.metadata.hash = hash
-                    downloaded_dep.metadata.version = version
-                    downloaded_dep.dir = sub_dependency_dir_path
-            else:
-                logger.debug("download dependency {}".format(col_name))
-                is_exist, targz = self.is_download_file_exist(
-                    LoadType.COLLECTION, col_name, os.path.join(self.download_location, "collection", col_name)
+                    parts = col_name.split(".")
+                    fullpath = os.path.join(sub_dependency_dir_path, "ansible_collections", parts[0], parts[1])
+                    downloaded_dep.dir = fullpath.replace(f"{self.root_dir}/", "")
+                self.dependency_dirs.append(asdict(downloaded_dep))
+
+        if role_dependencies:
+            for rdep in role_dependencies:
+                target_version = None
+                if isinstance(rdep, dict):
+                    rdep_name = rdep.get("name", None)
+                    target_version = rdep.get("version", None)
+                    if not rdep_name:
+                        rdep_name = rdep.get("role", None)
+                    rdep = rdep_name
+                name = rdep
+                if type(rdep) is dict:
+                    name = rdep.get("name", "")
+                    if name == "":
+                        name = rdep.get("src", "")
+                logger.debug("prepare dir for {}".format(name))
+                downloaded_dep = Dependency(
+                    name=name,
                 )
-                if is_exist:
-                    metadata_file = os.path.join(self.download_location, "collection", col_name, download_metadata_file)
-                    self.install_galaxy_collection_from_targz(targz, sub_dependency_dir_path)
-                    md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
-                else:
-                    # check download_location
-                    sub_download_location = os.path.join(self.download_location, "collection", col_name)
-                    if not os.path.exists(sub_download_location):
-                        os.makedirs(sub_download_location)
-                    install_msg = self.download_galaxy_collection(col_name, sub_download_location, col_version, self.source_repository)
-                    metadata = self.extract_collections_metadata(install_msg, sub_download_location)
-                    metadata_file = self.export_data(metadata, sub_download_location, download_metadata_file)
-                    md = self.find_target_metadata(LoadType.COLLECTION, metadata_file, col_name)
-                    if md:
-                        self.install_galaxy_collection_from_reqfile(md.requirements_file, sub_dependency_dir_path)
-                    # self.install_galaxy_collection_from_targz(md.download_src_path, sub_dependency_dir_path)
-                if md is not None:
-                    downloaded_dep.metadata = md
-                downloaded_dep.metadata.source_repository = self.source_repository
-                parts = col_name.split(".")
-                downloaded_dep.dir = os.path.join(sub_dependency_dir_path, "ansible_collections", parts[0], parts[1])
-            self.dependency_dirs.append(asdict(downloaded_dep))
-
-        for rdep in role_dependencies:
-            target_version = None
-            if isinstance(rdep, dict):
-                rdep_name = rdep.get("name", None)
-                target_version = rdep.get("version", None)
-                if not rdep_name:
-                    rdep_name = rdep.get("role", None)
-                rdep = rdep_name
-            name = rdep
-            if type(rdep) is dict:
-                name = rdep.get("name", "")
-                if name == "":
-                    name = rdep.get("src", "")
-            logger.debug("prepare dir for {}".format(name))
-            downloaded_dep = Dependency(
-                name=name,
-            )
-            downloaded_dep.metadata.type = LoadType.ROLE
-            downloaded_dep.metadata.name = name
-            downloaded_dep.metadata.cache_enabled = cache_enabled
-            # sub_dependency_dir_path = "{}/{}".format(dependency_dir_path, rdep)
-
-            sub_dependency_dir_path = os.path.join(
-                self.dependency_dir_path,
-                "roles",
-                "src",
-                name,
-            )
+                downloaded_dep.metadata.type = LoadType.ROLE
+                downloaded_dep.metadata.name = name
+                downloaded_dep.metadata.cache_enabled = cache_enabled
+                # sub_dependency_dir_path = "{}/{}".format(dependency_dir_path, rdep)
 
-            if not os.path.exists(sub_dependency_dir_path):
-                os.makedirs(sub_dependency_dir_path)
-            if cache_enabled:
-                logger.debug("cache enabled")
-                cache_dir_path = os.path.join(
-                    cache_dir,
+                sub_dependency_dir_path = os.path.join(
+                    self.dependency_dir_path,
                     "roles",
                     "src",
                     name,
                 )
-                if os.path.exists(cache_dir_path) and len(os.listdir(cache_dir_path)) != 0:
-                    logger.debug("cache data found")
-                    metadata_file = os.path.join(cache_dir_path, download_metadata_file)
-                    md = self.find_target_metadata(LoadType.ROLE, metadata_file, self.target_name)
-                else:
-                    logger.debug("cache data not found")
-                    install_msg = install_galaxy_target(name, LoadType.ROLE, cache_dir_path, self.source_repository, target_version)
-                    logger.debug("role install msg: {}".format(install_msg))
-                    metadata = self.extract_roles_metadata(install_msg)
-                    metadata_file = self.export_data(metadata, cache_dir_path, download_metadata_file)
-                    md = self.find_target_metadata(LoadType.ROLE, metadata_file, self.target_name)
-                self.move_src(sub_dependency_dir_path, cache_dir_path)
-                if md is not None:
-                    downloaded_dep.metadata = md
-            elif name in role_dependency_dirs:
-                logger.debug("use the specified dependency dirs")
-                sub_dependency_dir_path = role_dependency_dirs[name]
-            else:
-                is_exist, _ = self.is_download_file_exist(LoadType.ROLE, name, os.path.join(self.download_location, "role", name))
-                if is_exist:
-                    metadata_file = os.path.join(self.download_location, "role", name, download_metadata_file)
-                    md = self.find_target_metadata(LoadType.ROLE, metadata_file, name)
-                    self.move_src(md.download_src_path, sub_dependency_dir_path)
+
+                if not os.path.exists(sub_dependency_dir_path):
+                    os.makedirs(sub_dependency_dir_path)
+                if cache_enabled:
+                    logger.debug("cache enabled")
+                    cache_dir_path = os.path.join(
+                        cache_dir,
+                        "roles",
+                        name,
+                    )
+                    download_meta_dir_path = os.path.join(
+                        cache_dir,
+                        "roles_download_meta",
+                        name,
+                    )
+                    if os.path.exists(cache_dir_path) and len(os.listdir(cache_dir_path)) != 0:
+                        logger.debug("dependency cache data found")
+                        metadata_file = os.path.join(download_meta_dir_path, download_metadata_file)
+                        md = self.find_target_metadata(LoadType.ROLE, metadata_file, name)
+                        self.move_src(cache_dir_path, sub_dependency_dir_path)
+                    else:
+                        logger.debug("dependency cache data not found")
+                        install_msg = install_galaxy_target(name, LoadType.ROLE, sub_dependency_dir_path, self.source_repository, target_version)
+                        logger.debug("role install msg: {}".format(install_msg))
+                        metadata = self.extract_roles_metadata(install_msg)
+                        if not metadata:
+                            raise ValueError("failed to install {} {}".format(LoadType.ROLE, name))
+                        metadata_file = self.export_data(metadata, download_meta_dir_path, download_metadata_file)
+                        md = self.find_target_metadata(LoadType.ROLE, metadata_file, name)
+                        # save cache
+                        if not os.path.exists(cache_dir_path):
+                            os.makedirs(cache_dir_path)
+                        self.move_src(sub_dependency_dir_path, cache_dir_path)
+                    if md:
+                        downloaded_dep.metadata = md
+                elif name in role_dependency_dirs:
+                    logger.debug("use the specified dependency dirs")
+                    sub_dependency_dir_path = role_dependency_dirs[name]
                 else:
                     install_msg = install_galaxy_target(name, LoadType.ROLE, sub_dependency_dir_path, self.source_repository)
                     logger.debug("role install msg: {}".format(install_msg))
                     metadata = self.extract_roles_metadata(install_msg)
+                    if not metadata:
+                        raise ValueError("failed to install {} {}".format(LoadType.ROLE, name))
                     sub_download_location = os.path.join(self.download_location, "role", name)
                     metadata_file = self.export_data(metadata, sub_download_location, download_metadata_file)
                     md = self.find_target_metadata(LoadType.ROLE, metadata_file, name)
-                if md is not None:
-                    downloaded_dep.metadata = md
-            downloaded_dep.metadata.source_repository = self.source_repository
-            downloaded_dep.dir = sub_dependency_dir_path
-            self.dependency_dirs.append(asdict(downloaded_dep))
+                    if md is not None:
+                        downloaded_dep.metadata = md
+                downloaded_dep.metadata.source_repository = self.source_repository
+                self.dependency_dirs.append(asdict(downloaded_dep))
         return
 
     def src_install(self):
         try:
             self.setup_tmp_dir()
             self.root_install(self.tmp_install_dir)
         finally:
@@ -403,28 +418,38 @@
             if md:
                 self.install_galaxy_collection_from_reqfile(md.requirements_file, tmp_src_dir)
             dst_src_dir = self.target_path_mappings["src"]
             dependency_dir = tmp_src_dir
             self.metadata = md
         elif self.target_type == LoadType.ROLE:
             install_msg = ""
-            sub_download_location = os.path.join(self.download_location, "role", self.target_name)
+            sub_download_location = os.path.join(self.download_location, "roles", self.target_name)
+            metafile_location = os.path.join(self.download_location, "roles_download_meta", self.target_name)
             if os.path.exists(sub_download_location) and len(os.listdir(sub_download_location)) != 0:
                 logger.debug("found cache data {}".format(sub_download_location))
-                metadata_file = os.path.join(sub_download_location, download_metadata_file)
+                metadata_file = os.path.join(metafile_location, download_metadata_file)
                 md = self.find_target_metadata(LoadType.ROLE, metadata_file, self.target_name)
-                self.move_src(sub_download_location, tmp_src_dir)
+                tmp_target_dir = os.path.join(tmp_src_dir, self.target_name)
+                if not os.path.exists(tmp_target_dir):
+                    os.makedirs(tmp_target_dir)
+                self.move_src(sub_download_location, tmp_target_dir)
             else:
                 install_msg = install_galaxy_target(
                     self.target_name, self.target_type, tmp_src_dir, self.source_repository, target_version=self.target_version
                 )
                 logger.debug("role install msg: {}".format(install_msg))
                 metadata = self.extract_roles_metadata(install_msg)
-                metadata_file = self.export_data(metadata, sub_download_location, download_metadata_file)
+                if not metadata:
+                    raise ValueError("failed to install {} {}".format(self.target_type, self.target_name))
+                metadata_file = self.export_data(metadata, metafile_location, download_metadata_file)
                 md = self.find_target_metadata(LoadType.ROLE, metadata_file, self.target_name)
+                # save cache
+                if not os.path.exists(sub_download_location):
+                    os.makedirs(sub_download_location)
+                self.move_src(tmp_src_dir, sub_download_location)
             if not md:
                 raise ValueError("failed to install {} {}".format(self.target_type, self.target_name))
             dependency_dir = tmp_src_dir
             dst_src_dir = self.target_path_mappings["src"]
             self.metadata.download_src_path = "{}.{}".format(dst_src_dir, self.target_name)
             self.metadata = md
         else:
@@ -453,14 +478,17 @@
 
         if self.target_type == LoadType.PROJECT and self.target_dependency_dir:
             dst_dependency_dir = self.target_path_mappings["dependencies"]
             if not os.path.exists(dst_dependency_dir):
                 os.makedirs(dst_dependency_dir)
             self.move_src(dependency_dir, dst_dependency_dir)
             logger.debug("root metadata: {}".format(json.dumps(asdict(self.metadata))))
+
+        # prepare dependency data
+        self.dependency_dirs = self.dependnecy_dirs(metadata_file, self.target_type, self.target_name)
         return
 
     def set_index(self, path):
         if not self.silent:
             print("crawl content")
         dep_type = LoadType.UNKNOWN
         target_path_list = []
@@ -548,35 +576,39 @@
         logger.debug("STDOUT: {}".format(install_msg))
         # return proc.stdout
 
     def install_galaxy_collection_from_reqfile(self, requirements, output_dir):
         if not os.path.isfile(requirements):
             # get requirements file from archives dir under current root_dir
             child_dir_path = requirements.split("archives")[-1]
-            requirements = f'{self.download_location}{child_dir_path}'
+            requirements = f"{self.download_location}{child_dir_path}"
             if not os.path.isfile(requirements):
                 logger.warning("requirements file not found: {}".format(requirements))
                 return
         logger.debug("install collection from {}".format(requirements))
         src_dir = requirements.replace(requirements_yml, "")
         proc = subprocess.run(
             "cd {} && ansible-galaxy collection install -r {} -p {}".format(src_dir, requirements, output_dir),
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
         )
+        try:
+            proc.check_returncode()
+        except Exception as exc:
+            raise ValueError("failed to install collection: " + proc.stderr) from exc
         install_msg = proc.stdout
         logger.debug("STDOUT: {}".format(install_msg))
         # return proc.stdout
 
     def is_download_file_exist(self, type, target, dir):
         is_exist = False
         filename = ""
-        download_metadata_files = glob.glob(f'{dir}/{type}/{target}/**/{download_metadata_file}', recursive=True)
+        download_metadata_files = glob.glob(f"{dir}/{type}/{target}/**/{download_metadata_file}", recursive=True)
         # check if tar.gz file already exists
         if len(download_metadata_files) != 0:
             for metafile in download_metadata_files:
                 md = self.find_target_metadata(type, metafile, target)
                 if md is not None:
                     is_exist = True
                     filename = md.download_src_path
@@ -605,15 +637,15 @@
         # Downloading collection 'community.rabbitmq:1.2.3' to
         # Downloading https://galaxy.ansible.com/download/ansible-posix-1.4.0.tar.gz to ...
         download_url_pattern = r"Downloading (.*) to"
         url = ""
         version = ""
         hash = ""
         match_messages = re.findall(download_url_pattern, log_message)
-        download_path_from_root_dir = download_location.replace(f'{self.root_dir}/', "")
+        download_path_from_root_dir = download_location.replace(f"{self.root_dir}/", "")
         metadata_list = []
         for m in match_messages:
             metadata = DownloadMetadata()
             metadata.type = LoadType.COLLECTION
             if m.endswith("tar.gz"):
                 logger.debug("extracted url from download log message: {}".format(m))
                 url = m
@@ -657,36 +689,40 @@
         for i, line in enumerate(messages):
             if line.startswith("- downloading role from "):
                 metadata = DownloadMetadata()
                 metadata.type = LoadType.ROLE
                 url = line.split(" ")[-1]
                 logger.debug("extracted url from download log message: {}".format(url))
                 version = url.split("/")[-1].replace(".tar.gz", "")
-                name = messages[i + 1].split("/")[-1]
-                metadata.download_url = url
-                metadata.version = version
-                metadata.name = name
-                role_dir = messages[i + 1].split(" ")[-1]
-                m_time = os.path.getmtime(role_dir)
-                dt_m = datetime.datetime.utcfromtimestamp(m_time).isoformat()
-                metadata.download_timestamp = dt_m
-                metadata.download_src_path = role_dir.replace(f'{self.root_dir}/', "")
-                if url != "":
-                    hash = get_hash_of_url(url)
-                    metadata.hash = hash
-                logger.debug("metadata: {}".format(json.dumps(asdict(metadata))))
-                metadata_list.append(asdict(metadata))
+                if len(messages) > i:
+                    name = messages[i + 1].split("/")[-1]
+                    metadata.download_url = url
+                    metadata.version = version
+                    metadata.name = name
+                    role_dir = messages[i + 1].split(" ")[-1]
+                    m_time = os.path.getmtime(role_dir)
+                    dt_m = datetime.datetime.utcfromtimestamp(m_time).isoformat()
+                    metadata.download_timestamp = dt_m
+                    metadata.download_src_path = role_dir.replace(f"{self.root_dir}/", "")
+                    if url != "":
+                        hash = get_hash_of_url(url)
+                        metadata.hash = hash
+                    logger.debug("metadata: {}".format(json.dumps(asdict(metadata))))
+                    metadata_list.append(asdict(metadata))
+        if len(metadata_list) == 0:
+            logger.warning(f"failed to extract download metadata from install log: {log_message}")
+            return None
         result = {"roles": metadata_list}
         return result
 
     def find_target_metadata(self, type, metadata_file, target):
         if not os.path.isfile(metadata_file):
             # get metadata file from archives dir under current root_dir
             child_dir_path = metadata_file.split("archives")[-1]
-            metadata_file = f'{self.download_location}{child_dir_path}'
+            metadata_file = f"{self.download_location}{child_dir_path}"
             if not os.path.isfile(metadata_file):
                 logger.warning("metadata file not found: {}".format(target))
                 return None
         with open(metadata_file, "r") as f:
             metadata = json.load(f)
         if type == LoadType.COLLECTION:
             metadata_list = metadata.get("collections", [])
@@ -742,15 +778,27 @@
         if src == "" or not os.path.exists(src) or not os.path.isdir(src):
             raise ValueError("src {} is not directory".format(src))
         if dst == "" or ".." in dst:
             raise ValueError("dst {} is invalid".format(dst))
         # we use cp command here because shutil module is slow,
         # but the behavior of cp command is slightly different between Mac and Linux
         # we use a command like `cp -r <src>/* <dst>/` so the behavior will be the same
-        os.system("cp -r {}/* {}/".format(src, dst))
+        dirs = os.listdir(src)
+        proc = subprocess.run(
+            f"cp -r {src}/* {dst}/",
+            shell=True,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            text=True,
+        )
+        # raise if copy failed
+        try:
+            proc.check_returncode()
+        except Exception as exc:
+            raise ValueError(proc.stderr + "\ndirs: " + ", ".join(dirs)) from exc
         return
 
     def setup_tmp_dir(self):
         if self.tmp_install_dir is None or not os.path.exists(self.tmp_install_dir.name):
             self.tmp_install_dir = tempfile.TemporaryDirectory()
             if self.periodical_cleanup:
                 self.cleanup_queue.append(deepcopy(self.tmp_install_dir))
@@ -836,45 +884,83 @@
     def update_role_download_src(self, metadata_file, dst_src_dir):
         with open(metadata_file, "r") as f:
             metadata = json.load(f)
         metadata_list = metadata.get("roles", [])
         for i, data in enumerate(metadata_list):
             dm = DownloadMetadata(**data)
             full_path = "{}/{}".format(dst_src_dir, dm.name)
-            path_from_root = full_path.replace(f'{self.root_dir}/', "")
+            path_from_root = full_path.replace(f"{self.root_dir}/", "")
             key = "download_src_path"
             if hasattr(dm, key):
                 setattr(dm, key, path_from_root)
             metafile_path, _ = self.get_metafile_in_target(LoadType.ROLE, full_path)
-            dm.metafile_path = metafile_path.replace(f'{self.root_dir}/', "")
+            dm.metafile_path = metafile_path.replace(f"{self.root_dir}/", "")
             dm.author = self.get_author(LoadType.ROLE, metafile_path)
             metadata_list[i] = asdict(dm)
             logger.debug("update {} in metadata: {}".format(key, dm))
         metadata["roles"] = metadata_list
         with open(metadata_file, "w") as f:
             json.dump(metadata, f)
         return
 
     def get_author(self, type, metafile_path):
         if not os.path.exists(metafile_path):
-            metafile_path = f'{self.root_dir}/{metafile_path}'
+            metafile_path = f"{self.root_dir}/{metafile_path}"
             if not os.path.exists(metafile_path):
                 logger.warning("invalid file path: {}".format(metafile_path))
                 return ""
         if type == LoadType.COLLECTION:
             with open(metafile_path, "r") as f:
                 metadata = json.load(f)
             authors = metadata.get("collection_info", {}).get("authors", [])
             return ",".join(authors)
         elif type == LoadType.ROLE:
             with open(metafile_path, "r") as f:
                 metadata = yaml.safe_load(f)
             author = metadata.get("galaxy_info", {}).get("author", "")
             return author
 
+    def dependnecy_dirs(self, metadata_file, target_type, target_name):
+        dependency_dirs = []
+        if not os.path.isfile(metadata_file):
+            # get metadata file from archives dir under current root_dir
+            child_dir_path = metadata_file.split("archives")[-1]
+            metadata_file = f"{self.download_location}{child_dir_path}"
+            if not os.path.isfile(metadata_file):
+                logger.warning("metadata file not found: {}".format(target_name))
+                return dependency_dirs
+        with open(metadata_file, "r") as f:
+            metadata = json.load(f)
+        metadata_list = metadata.get("roles", [])
+        for _, data in enumerate(metadata_list):
+            dm = DownloadMetadata(**data)
+            downloaded_dep = Dependency(
+                name=dm.name,
+                metadata=dm,
+            )
+            downloaded_dep.dir = os.path.join(dm.download_src_path)
+            if target_type == LoadType.ROLE and target_name == dm.name:
+                continue
+            dependency_dirs.append(asdict(downloaded_dep))
+
+        metadata_list = metadata.get("collections", [])
+        for _, data in enumerate(metadata_list):
+            dm = DownloadMetadata(**data)
+            downloaded_dep = Dependency(
+                name=dm.name,
+                metadata=dm,
+            )
+            parts = dm.name.split(".")
+            full_path = os.path.join(self.target_path_mappings["src"], "ansible_collections", parts[0], parts[1])
+            downloaded_dep.dir = full_path.replace(f"{self.root_dir}/", "")
+            if target_type == LoadType.COLLECTION and target_name == dm.name:
+                continue
+            dependency_dirs.append(asdict(downloaded_dep))
+        return dependency_dirs
+
 
 def find_ext_dependencies(path):
     collection_meta_files = safe_glob(os.path.join(path, "**", collection_manifest_json), recursive=True)
     if len(collection_meta_files) > 0:
         collection_path_list = [trim_suffix(f, ["/" + collection_manifest_json]) for f in collection_meta_files]
         collection_path_list = remove_subdirectories(collection_path_list)
         return LoadType.COLLECTION, collection_path_list
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 # limitations under the License.
 
 from dataclasses import dataclass
 from pathlib import Path
 import re
 import os
 import yaml
+
+try:
+    # if `libyaml` is available, use C based loader for performance
+    import _yaml  # noqa: F401
+    from yaml import CSafeLoader as Loader
+except Exception:
+    # otherwise, use Python based loader
+    from yaml import SafeLoader as Loader
 import ansible_risk_insight.logger as logger
 from .safe_glob import safe_glob
 from .awx_utils import could_be_playbook, search_playbooks
 
 
 module_name_re = re.compile(r"^[a-z0-9_]+\.[a-z0-9_]+\.[a-z0-9_]+$")
 
@@ -84,26 +92,26 @@
 
 
 def get_task_blocks(fpath="", yaml_str="", task_dict_list=None):
     d = None
     yaml_lines = ""
     if yaml_str:
         try:
-            d = yaml.safe_load(yaml_str)
+            d = yaml.load(yaml_str, Loader=Loader)
             yaml_lines = yaml_str
         except Exception as e:
             logger.debug("failed to load this yaml string to get task blocks; {}".format(e.args[0]))
             return None, None
     elif fpath:
         if not os.path.exists(fpath):
             return None, None
         with open(fpath, "r") as file:
             try:
                 yaml_lines = file.read()
-                d = yaml.safe_load(yaml_lines)
+                d = yaml.load(yaml_lines, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load this yaml file to get task blocks; {}".format(e.args[0]))
                 return None, None
     elif task_dict_list is not None:
         d = task_dict_list
     else:
         return None, None
@@ -217,15 +225,15 @@
                 continue
             # if it is a playbook, skip it
             if could_be_playbook(f):
                 continue
             d = None
             with open(f, "r") as file:
                 try:
-                    d = yaml.safe_load(file)
+                    d = yaml.load(file, Loader=Loader)
                 except Exception as e:
                     logger.debug("failed to load this yaml file to search task" " files; {}".format(e.args[0]))
             # if d cannot be loaded as tasks yaml file, skip it
             if d is None or not isinstance(d, list):
                 continue
             candidates.append(f)
     return candidates
@@ -281,15 +289,15 @@
     found_galaxy_ymls = safe_glob(pattern, recursive=True)
     my_collection_name = ""
     if len(found_galaxy_ymls) > 0:
         galaxy_yml = found_galaxy_ymls[0]
         my_collection_info = None
         with open(galaxy_yml, "r") as file:
             try:
-                my_collection_info = yaml.safe_load(file)
+                my_collection_info = yaml.load(file, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load this yaml file to read galaxy.yml; {}".format(e.args[0]))
         if my_collection_info is None:
             return ""
         namespace = my_collection_info.get("namespace", "")
         name = my_collection_info.get("name", "")
         my_collection_name = "{}.{}".format(namespace, name)
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import pathlib
 import json
-import git
+import pygit2
 import pkg_resources
 from .models import LoadType
 
 collection_manifest_json = "MANIFEST.json"
 role_meta_main_yml = "meta/main.yml"
 role_meta_main_yaml = "meta/main.yaml"
 
@@ -56,17 +56,16 @@
     except Exception:
         pass
     if version != "":
         return version
     # try to get version from commit ID in source code repository
     try:
         script_dir = pathlib.Path(__file__).parent.resolve()
-        repo = git.Repo(path=script_dir, search_parent_directories=True)
-        sha = repo.head.object.hexsha
-        version = sha
+        repo = pygit2.Repository(script_dir)
+        version = repo.head.target
     except Exception:
         pass
     return version
 
 
 def get_target_name(target_type, target_path):
     target_name = ""
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/model_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 # limitations under the License.
 
 import datetime
 import json
 import os
 import re
 import yaml
+
+try:
+    # if `libyaml` is available, use C based loader for performance
+    import _yaml  # noqa: F401
+    from yaml import CSafeLoader as Loader
+except Exception:
+    # otherwise, use Python based loader
+    from yaml import SafeLoader as Loader
 from ansible.module_utils.parsing.convert_bool import boolean
 
 import ansible_risk_insight.logger as logger
 from .safe_glob import safe_glob
 from .models import (
     ExecutableType,
     Inventory,
@@ -233,15 +241,15 @@
     data = {}
     if file_ext == "":
         # TODO: parse it as INI file
         pass
     elif file_ext == ".yml" or file_ext == ".yaml":
         with open(fullpath, "r") as file:
             try:
-                data = yaml.safe_load(file)
+                data = yaml.load(file, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load this yaml file (inventory); {}".format(e.args[0]))
     elif file_ext == ".json":
         with open(fullpath, "r") as file:
             try:
                 data = json.load(file)
             except Exception as e:
@@ -296,30 +304,36 @@
     pre_tasks = []
     post_tasks = []
     tasks = []
     roles = []
     play_options = {}
     import_module = ""
     import_playbook = ""
-    __pre_task_blocks, _ = get_task_blocks(task_dict_list=data_block.get("pre_tasks", []))
-    __task_blocks, _ = get_task_blocks(task_dict_list=data_block.get("tasks", []))
-    pre_task_num = len(__pre_task_blocks) if __pre_task_blocks else 0
-    task_num = len(__task_blocks) if __task_blocks else 0
-    for k, v in data_block.items():
+
+    tasks_keys = ["pre_tasks", "tasks", "post_tasks"]
+    keys = [k for k in data_block if k not in tasks_keys]
+    keys.extend(tasks_keys)
+    task_count = 0
+
+    for k in keys:
+        if k not in data_block:
+            continue
+        v = data_block[k]
         if k == "name":
             pass
         elif k == "collections":
             pass
         elif k == "pre_tasks":
             if not isinstance(v, list):
                 continue
             task_blocks, _ = get_task_blocks(task_dict_list=v)
             if task_blocks is None:
                 continue
-            for i, task_dict in enumerate(task_blocks):
+            for task_dict in task_blocks:
+                i = task_count
                 try:
                     t = load_task(
                         path=path,
                         index=i,
                         task_block_dict=task_dict,
                         role_name=role_name,
                         collection_name=collection_name,
@@ -330,81 +344,84 @@
                         yaml_lines=yaml_lines,
                         basedir=basedir,
                     )
                     pre_tasks.append(t)
                 except TaskFormatError:
                     if skip_task_format_error:
                         logger.debug("this task is wrong format; skip the task in {}," " index: {}; skip this".format(path, i))
-                        continue
                     else:
                         raise TaskFormatError(f"this task is wrong format; skip the task in {path}," " index: {i}")
                 except Exception:
                     logger.exception("error while loading the task at {} (index={})".format(path, i))
+                finally:
+                    task_count += 1
         elif k == "tasks":
             if not isinstance(v, list):
                 continue
             task_blocks, _ = get_task_blocks(task_dict_list=v)
             if task_blocks is None:
                 continue
-            for i, task_dict in enumerate(task_blocks):
-                _i = i + pre_task_num
+            for task_dict in task_blocks:
+                i = task_count
                 try:
                     t = load_task(
                         path=path,
-                        index=_i,
+                        index=i,
                         task_block_dict=task_dict,
                         role_name=role_name,
                         collection_name=collection_name,
                         collections_in_play=collections_in_play,
                         play_index=index,
                         parent_key=pbObj.key,
                         parent_local_key=pbObj.local_key,
                         yaml_lines=yaml_lines,
                         basedir=basedir,
                     )
                     tasks.append(t)
                 except TaskFormatError:
                     if skip_task_format_error:
                         logger.debug("this task is wrong format; skip the task in {}," " index: {}; skip this".format(path, i))
-                        continue
                     else:
                         raise TaskFormatError(f"this task is wrong format; skip the task in {path}," " index: {i}")
                 except Exception:
                     logger.exception("error while loading the task at {} (index={})".format(path, i))
+                finally:
+                    task_count += 1
         elif k == "post_tasks":
             if not isinstance(v, list):
                 continue
             task_blocks, _ = get_task_blocks(task_dict_list=v)
             if task_blocks is None:
                 continue
-            for i, task_dict in enumerate(task_blocks):
-                _i = i + pre_task_num + task_num
+            for task_dict in task_blocks:
+                i = task_count
                 try:
                     t = load_task(
                         path=path,
-                        index=_i,
+                        index=i,
                         task_block_dict=task_dict,
                         role_name=role_name,
                         collection_name=collection_name,
                         collections_in_play=collections_in_play,
                         play_index=index,
                         parent_key=pbObj.key,
                         parent_local_key=pbObj.local_key,
                         yaml_lines=yaml_lines,
                         basedir=basedir,
                     )
                     post_tasks.append(t)
                 except TaskFormatError:
                     if skip_task_format_error:
                         logger.debug("this task is wrong format; skip the task in {}," " index: {}; skip this".format(path, i))
-                        continue
                     else:
                         raise TaskFormatError(f"this task is wrong format; skip the task in {path}," " index: {i}")
                 except Exception:
                     logger.exception("error while loading the task at {} (index={})".format(path, i))
+                finally:
+                    task_count += 1
         elif k == "roles":
             if not isinstance(v, list):
                 continue
             for i, r_block in enumerate(v):
                 r_name = ""
                 role_options = {}
                 if isinstance(r_block, dict):
@@ -515,25 +532,25 @@
     pbObj.collection = collection_name
     pbObj.set_key()
     yaml_lines = ""
     data = None
     if yaml_str:
         try:
             yaml_lines = yaml_str
-            data = yaml.safe_load(yaml_lines)
+            data = yaml.load(yaml_lines, Loader=Loader)
         except Exception as e:
             if skip_playbook_format_error:
                 logger.debug(f"failed to load this yaml string to load playbook, skip this yaml; {e}")
             else:
                 raise PlaybookFormatError(f"failed to load this yaml string to load playbook; {e}")
     elif fullpath != "":
         with open(fullpath, "r") as file:
             try:
                 yaml_lines = file.read()
-                data = yaml.safe_load(yaml_lines)
+                data = yaml.load(yaml_lines, Loader=Loader)
             except Exception as e:
                 if skip_playbook_format_error:
                     logger.debug(f"failed to load this yaml file to load playbook, skip this yaml; {e}")
                 else:
                     raise PlaybookFormatError(f"failed to load this yaml file to load playbook; {e}")
     if data is None:
         return pbObj
@@ -647,27 +664,27 @@
         vars_dir_path = os.path.join(fullpath, "vars")
         tasks_dir_path = os.path.join(fullpath, "tasks")
         handlers_dir_path = os.path.join(fullpath, "handlers")
         includes_dir_path = os.path.join(fullpath, "includes")
     if os.path.exists(meta_file_path):
         with open(meta_file_path, "r") as file:
             try:
-                roleObj.metadata = yaml.safe_load(file)
+                roleObj.metadata = yaml.load(file, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load this yaml file to raed metadata; {}".format(e.args[0]))
 
             if roleObj.metadata is not None and isinstance(roleObj.metadata, dict):
                 roleObj.dependency["roles"] = roleObj.metadata.get("dependencies", [])
                 roleObj.dependency["collections"] = roleObj.metadata.get("collections", [])
 
     requirements_yml_path = os.path.join(fullpath, "requirements.yml")
     if os.path.exists(requirements_yml_path):
         with open(requirements_yml_path, "r") as file:
             try:
-                roleObj.requirements = yaml.safe_load(file)
+                roleObj.requirements = yaml.load(file, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load requirements.yml; {}".format(e.args[0]))
 
     parts = tasks_dir_path.split("/")
     if len(parts) < 2:
         raise ValueError("role path is wrong")
     role_name = parts[-2] if name == "" else name
@@ -725,15 +742,15 @@
             defaults_dir_path + "/**/*.ya?ml",
         ]
         defaults_yaml_files = safe_glob(patterns, recursive=True)
         default_variables = {}
         for fpath in defaults_yaml_files:
             with open(fpath, "r") as file:
                 try:
-                    vars_in_yaml = yaml.safe_load(file)
+                    vars_in_yaml = yaml.load(file, Loader=Loader)
                     if vars_in_yaml is None:
                         continue
                     if not isinstance(vars_in_yaml, dict):
                         continue
                     default_variables.update(vars_in_yaml)
                 except Exception as e:
                     logger.debug("failed to load this yaml file to read default" " variables; {}".format(e.args[0]))
@@ -742,15 +759,15 @@
     if os.path.exists(vars_dir_path):
         patterns = [vars_dir_path + "/**/*.ya?ml"]
         vars_yaml_files = safe_glob(patterns, recursive=True)
         variables = {}
         for fpath in vars_yaml_files:
             with open(fpath, "r") as file:
                 try:
-                    vars_in_yaml = yaml.safe_load(file)
+                    vars_in_yaml = yaml.load(file, Loader=Loader)
                     if vars_in_yaml is None:
                         continue
                     if not isinstance(vars_in_yaml, dict):
                         continue
                     variables.update(vars_in_yaml)
                 except Exception as e:
                     logger.debug("failed to load this yaml file to read variables; {}".format(e.args[0]))
@@ -791,16 +808,14 @@
         modules = sorted(modules)
     roleObj.modules = modules
 
     patterns = [tasks_dir_path + "/**/*.ya?ml"]
     # ansible.network collection has this type of another taskfile directory
     if os.path.exists(includes_dir_path):
         patterns.extend([includes_dir_path + "/**/*.ya?ml"])
-    if os.path.exists(handlers_dir_path):
-        patterns.extend([handlers_dir_path + "/**/*.ya?ml"])
     task_yaml_files = safe_glob(patterns, recursive=True)
 
     taskfiles = []
     for task_yaml_path in task_yaml_files:
         tf = None
         try:
             tf = load_taskfile(
@@ -823,14 +838,46 @@
             taskfiles.append(tf)
         else:
             taskfiles.append(tf.defined_in)
     if not load_children:
         taskfiles = sorted(taskfiles)
     roleObj.taskfiles = taskfiles
 
+    if os.path.exists(handlers_dir_path):
+        handler_patterns = [handlers_dir_path + "/**/*.ya?ml"]
+        handler_files = safe_glob(handler_patterns, recursive=True)
+
+        handlers = []
+        for handler_yaml_path in handler_files:
+            tf = None
+            try:
+                tf = load_taskfile(
+                    handler_yaml_path,
+                    role_name=fqcn,
+                    collection_name=collection_name,
+                    basedir=basedir,
+                    skip_task_format_error=skip_task_format_error,
+                )
+            except TaskFormatError as e:
+                if skip_task_format_error:
+                    logger.debug(f"Task format error found; skip this taskfile {task_yaml_path}")
+                else:
+                    raise TaskFormatError(f"Task format error found: {e.args[0]}")
+            except Exception:
+                logger.exception("error while loading the task file at {}".format(task_yaml_path))
+            if not tf:
+                continue
+            if load_children:
+                handlers.append(tf)
+            else:
+                handlers.append(tf.defined_in)
+        if not load_children:
+            handlers = sorted(handlers)
+        roleObj.handlers = handlers
+
     return roleObj
 
 
 def load_roles(
     path,
     basedir="",
     use_ansible_doc=True,
@@ -897,15 +944,15 @@
 
 def load_requirements(path):
     requirements = {}
     requirements_yml_path = os.path.join(path, "requirements.yml")
     if os.path.exists(requirements_yml_path):
         with open(requirements_yml_path, "r") as file:
             try:
-                requirements = yaml.safe_load(file)
+                requirements = yaml.load(file, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load requirements.yml; {}".format(e.args[0]))
     return requirements
 
 
 def load_installed_roles(installed_roles_path):
     search_path = installed_roles_path
@@ -991,15 +1038,15 @@
             examples = module_specs.get(moduleObj.fqcn, {}).get("examples", "")
     else:
         # parse the script file for a quick scan (this does not contain doc from `doc_fragments`)
         doc_yaml = get_documentation_in_module_file(fullpath)
     if doc_yaml:
         doc_dict = {}
         try:
-            doc_dict = yaml.safe_load(doc_yaml)
+            doc_dict = yaml.load(doc_yaml, Loader=Loader)
         except Exception:
             logger.debug(f"failed to load the arguments documentation of the module: {module_name}")
         if not doc_dict:
             doc_dict = {}
         arg_specs = doc_dict.get("options", {})
         if isinstance(arg_specs, dict):
             for arg_name in arg_specs:
@@ -1359,34 +1406,34 @@
 
     manifest_file_path = os.path.join(fullpath, "MANIFEST.json")
     if os.path.exists(manifest_file_path):
         with open(manifest_file_path, "r") as file:
             colObj.metadata = json.load(file)
 
         if colObj.metadata is not None and isinstance(colObj.metadata, dict):
-            colObj.dependency["collections"] = colObj.metadata.get("dependencies", {})
+            colObj.dependency["collections"] = colObj.metadata.get("collection_info", {}).get("dependencies", {})
 
     files_file_path = os.path.join(fullpath, "FILES.json")
     if os.path.exists(files_file_path):
         with open(files_file_path, "r") as file:
             colObj.files = json.load(file)
 
     meta_runtime_file_path = os.path.join(fullpath, "meta", "runtime.yml")
     if os.path.exists(meta_runtime_file_path):
         with open(meta_runtime_file_path, "r") as file:
             try:
-                colObj.meta_runtime = yaml.safe_load(file)
+                colObj.meta_runtime = yaml.load(file, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load meta/runtime.yml; {}".format(e.args[0]))
 
     requirements_yml_path = os.path.join(fullpath, "requirements.yml")
     if os.path.exists(requirements_yml_path):
         with open(requirements_yml_path, "r") as file:
             try:
-                colObj.requirements = yaml.safe_load(file)
+                colObj.requirements = yaml.load(file, Loader=Loader)
             except Exception as e:
                 logger.debug("failed to load requirements.yml; {}".format(e.args[0]))
 
     if isinstance(colObj.metadata, dict):
         license_filename = colObj.metadata.get("collection_info", {}).get("license_file", None)
         if license_filename:
             license_filepath = os.path.join(fullpath, license_filename)
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1529,22 +1529,25 @@
     @property
     def action_type(self):
         return self.spec.executable_type
 
 
 @dataclass
 class AnsibleRunContext(object):
-    sequence: RunTargetList = None
+    sequence: RunTargetList = field(default_factory=RunTargetList)
     root_key: str = ""
     parent: Object = None
 
     # used by rule check
     current: RunTarget = None
     _i: int = 0
 
+    # used if ram generate / other data generation by loop
+    last_item: bool = False
+
     # TODO: implement the following attributes
     vars: any = None
     host_info: any = None
 
     def __len__(self):
         return len(self.sequence)
 
@@ -1561,67 +1564,75 @@
         self._i += 1
         return t
 
     def __getitem__(self, i):
         return self.sequence[i]
 
     @staticmethod
-    def from_tree(tree: ObjectList, parent: Object = None):
+    def from_tree(tree: ObjectList, parent: Object = None, last_item: bool = False):
         if not tree:
-            return AnsibleRunContext(parent=parent)
+            return AnsibleRunContext(parent=parent, last_item=last_item)
         if len(tree.items) == 0:
-            return AnsibleRunContext(parent=parent)
+            return AnsibleRunContext(parent=parent, last_item=last_item)
 
         root_key = tree.items[0].spec.key
         sequence_items = []
         for item in tree.items:
             if not isinstance(item, RunTarget):
                 continue
             sequence_items.append(item)
         tl = RunTargetList(items=sequence_items)
-        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent)
+        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item)
 
     @staticmethod
-    def from_targets(targets: List[RunTarget], root_key: str = "", parent: Object = None):
+    def from_targets(targets: List[RunTarget], root_key: str = "", parent: Object = None, last_item: bool = False):
         if not root_key:
             if len(targets) > 0:
                 root_key = targets[0].spec.key
         tl = RunTargetList(items=targets)
-        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent)
+        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item)
 
     def find(self, target: RunTarget):
         for t in self.sequence:
             if t.key == target.key:
                 return t
         return None
 
     def before(self, target: RunTarget):
         targets = []
         for rt in self.sequence:
             if rt.key == target.key:
                 break
             targets.append(rt)
-        return AnsibleRunContext.from_targets(targets, root_key=self.root_key, parent=self.parent)
+        return AnsibleRunContext.from_targets(targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item)
 
     def search(self, cond: AnnotationCondition):
         targets = [t for t in self.sequence if t.type == RunTargetType.Task and t.has_annotation_by_condition(cond)]
-        return AnsibleRunContext.from_targets(targets, root_key=self.root_key, parent=self.parent)
+        return AnsibleRunContext.from_targets(targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item)
 
     def is_end(self, target: RunTarget):
         if len(self) == 0:
             return False
         return target.key == self.sequence[-1].key
 
+    def is_last_task(self, target: RunTarget):
+        if len(self) == 0:
+            return False
+        taskcalls = self.taskcalls
+        if len(taskcalls) == 0:
+            return False
+        return target.key == taskcalls[-1].key
+
     def is_begin(self, target: RunTarget):
         if len(self) == 0:
             return False
         return target.key == self.sequence[0].key
 
     def copy(self):
-        return AnsibleRunContext.from_targets(targets=self.sequence.items, root_key=self.root_key, parent=self.parent)
+        return AnsibleRunContext.from_targets(targets=self.sequence.items, root_key=self.root_key, parent=self.parent, last_item=self.last_item)
 
     @property
     def info(self):
         if not self.root_key:
             return {}
         return get_obj_info_by_key(self.root_key)
 
@@ -1690,14 +1701,15 @@
     local_key: str = ""
     fqcn: str = ""
     metadata: dict = field(default_factory=dict)
     collection: str = ""
     playbooks: list = field(default_factory=list)
     # 1 role can have multiple task yamls
     taskfiles: list = field(default_factory=list)
+    handlers: list = field(default_factory=list)
     # roles/xxxx/library/zzzz.py can be called as module zzzz
     modules: list = field(default_factory=list)
     dependency: dict = field(default_factory=dict)
     requirements: dict = field(default_factory=dict)
 
     source: str = ""  # collection/scm repo/galaxy
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ram_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,19 +50,27 @@
         self._no_module_spec = no_module_spec
         self._no_retry = no_retry
 
         use_ansible_doc = True
         if self._no_module_spec:
             use_ansible_doc = False
 
+        read_ram = True
+        write_ram = True
+        if self._include_test_contents:
+            read_ram = False
+            write_ram = False
+
         self._scanner = ARIScanner(
             root_dir=config.data_dir,
             silent=True,
             use_ansible_doc=use_ansible_doc,
             persist_dependency_cache=True,
+            read_ram=read_ram,
+            write_ram=write_ram,
         )
 
     def run(self):
         num = len(self._queue)
         resume_str = f"(resume from {self._resume})" if self._resume > 0 else ""
         print(f"Start scanning {num} targets {resume_str}")
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_assessment_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 @dataclass
 class RAMClient(object):
     root_dir: str = ""
 
     findings_json_list_cache: list = field(default_factory=list)
 
     findings_cache: dict = field(default_factory=dict)
+    findings_search_cache: dict = field(default_factory=dict)
 
     module_search_cache: dict = field(default_factory=dict)
     role_search_cache: dict = field(default_factory=dict)
     taskfile_search_cache: dict = field(default_factory=dict)
     task_search_cache: dict = field(default_factory=dict)
 
     builtin_modules_cache: dict = field(default_factory=dict)
@@ -84,18 +85,20 @@
                 self.role_index = json.load(file)
 
         taskfile_index_path = os.path.join(self.root_dir, "indices", taskfile_index_name)
         if os.path.exists(taskfile_index_path):
             with open(taskfile_index_path, "r") as file:
                 self.taskfile_index = json.load(file)
 
+        self.init_findings_json_list_cache()
+
     def clear_old_cache(self):
         size = self.max_cache_size
-        self._remove_old_item(self.findings_json_list_cache, size)
         self._remove_old_item(self.findings_cache, size)
+        self._remove_old_item(self.findings_search_cache, size)
         self._remove_old_item(self.module_search_cache, size)
         self._remove_old_item(self.role_search_cache, size)
         self._remove_old_item(self.taskfile_search_cache, size)
         self._remove_old_item(self.task_search_cache, size)
         return
 
     def _remove_old_item(self, data: dict, size: int):
@@ -757,27 +760,26 @@
                         "name": parts[-5],
                         "version": parts[-4],
                         "hash": parts[-3],
                     },
                 }
         return matched_obj
 
+    def init_findings_json_list_cache(self):
+        search_patterns = os.path.join(self.root_dir, "collections", "findings", "*", "*", "*", "findings.json")
+        findings_json_list_coll = safe_glob(search_patterns)
+        findings_json_list_coll = sort_by_version(findings_json_list_coll)
+        search_patterns = os.path.join(self.root_dir, "roles", "findings", "*", "*", "*", "findings.json")
+        findings_json_list_role = safe_glob(search_patterns)
+        findings_json_list_role = sort_by_version(findings_json_list_role)
+        findings_json_list = findings_json_list_coll + findings_json_list_role
+        self.findings_json_list_cache = findings_json_list
+
     def list_all_ram_metadata(self):
-        findings_json_list = []
-        if self.findings_json_list_cache:
-            findings_json_list = self.findings_json_list_cache
-        else:
-            search_patterns = os.path.join(self.root_dir, "collections", "findings", "*", "*", "*", "findings.json")
-            findings_json_list_coll = safe_glob(search_patterns)
-            findings_json_list_coll = sort_by_version(findings_json_list_coll)
-            search_patterns = os.path.join(self.root_dir, "roles", "findings", "*", "*", "*", "findings.json")
-            findings_json_list_role = safe_glob(search_patterns)
-            findings_json_list_role = sort_by_version(findings_json_list_role)
-            findings_json_list = findings_json_list_coll + findings_json_list_role
-            self.findings_json_list_cache = findings_json_list
+        findings_json_list = self.findings_json_list_cache
 
         metadata_list = []
         for findings_path in findings_json_list:
             parts = findings_path.split("/")
 
             metadata_list.append(
                 {
@@ -786,47 +788,55 @@
                     "version": parts[-3],
                     "hash": parts[-2],
                 }
             )
         return metadata_list
 
     def search_findings(self, target_name, target_version, target_type=None):
+        args_str = json.dumps([target_name, target_version, target_type])
+        if args_str in self.findings_search_cache:
+            return self.findings_search_cache[args_str]
+
         if not target_name:
             raise ValueError("target name must be specified for searching RAM data")
         if not target_version:
             target_version = "*"
-        search_patterns = []
-        if not target_type or target_type == "collection":
-            search_patterns.append(os.path.join(self.root_dir, "collections", "findings", target_name, target_version, "*", "findings.json"))
-        if not target_type or target_type == "role":
-            search_patterns.append(os.path.join(self.root_dir, "roles", "findings", target_name, target_version, "*", "findings.json"))
-        if not target_type or target_type == "project":
-            e_target_name = escape_url(target_name)
-            search_patterns.append(os.path.join(self.root_dir, "projects", "findings", e_target_name, target_version, "*", "findings.json"))
-        if not target_type or target_type == "playbook":
-            e_target_name = escape_url(target_name)
-            search_patterns.append(os.path.join(self.root_dir, "playbooks", "findings", e_target_name, target_version, "*", "findings.json"))
-        if not target_type or target_type == "taskfile":
-            e_target_name = escape_url(target_name)
-            search_patterns.append(os.path.join(self.root_dir, "taskfiles", "findings", e_target_name, target_version, "*", "findings.json"))
-        found_path_list = safe_glob(search_patterns)
+        findings_json_list = self.findings_json_list_cache
+        found_path_list = []
+        for findings_path in findings_json_list:
+            parts = findings_path.split("/")
+            _type = parts[-5][:-1]  # collection or role
+            _name = parts[-4]
+            _version = parts[-3]
+            if _name != target_name:
+                continue
+            if target_version and target_version != "*":
+                if _version != target_name:
+                    continue
+            if target_type and target_type != "*":
+                if _type != target_type:
+                    continue
+            found_path_list.append(findings_path)
+
         latest_findings_path = ""
         if len(found_path_list) == 1:
             latest_findings_path = found_path_list[0]
         elif len(found_path_list) > 1:
             latest_findings_path = found_path_list[0]
             mtime = os.path.getmtime(latest_findings_path)
             for fpath in found_path_list:
                 tmp_mtime = os.path.getmtime(fpath)
                 if tmp_mtime > mtime:
                     latest_findings_path = fpath
                     mtime = tmp_mtime
         findings = None
         if os.path.exists(latest_findings_path):
             findings = self.load_findings(latest_findings_path)
+
+        self.findings_search_cache[args_str] = findings
         return findings
 
     def load_findings(self, path: str):
 
         basename = os.path.basename(path)
         dir_path = path
         if basename == "findings.json":
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -585,16 +585,17 @@
                     logger.info("  tree file saved")
         return
 
     def resolve_variables(self):
         taskcalls_in_trees = resolve(self.trees, self.additional)
         self.taskcalls_in_trees = taskcalls_in_trees
 
-        for tree in self.trees:
-            ctx = AnsibleRunContext.from_tree(tree=tree, parent=self.target_object)
+        for i, tree in enumerate(self.trees):
+            last_item = i + 1 == len(self.trees)
+            ctx = AnsibleRunContext.from_tree(tree=tree, parent=self.target_object, last_item=last_item)
             self.contexts.append(ctx)
 
         if self.do_save:
             root_def_dir = self.__path_mappings["root_definitions"]
             tasks_in_t_path = os.path.join(root_def_dir, "tasks_in_trees.json")
             tasks_in_t_lines = []
             for d in taskcalls_in_trees:
@@ -721,14 +722,15 @@
 
     root_dir: str = ""
     rules_dir: str = ""
     rules: list = field(default_factory=list)
 
     ram_client: RAMClient = None
     read_ram: bool = True
+    read_ram_for_dependency: bool = True
     write_ram: bool = True
 
     persist_dependency_cache: bool = False
 
     skip_playbook_format_error: bool = (True,)
     skip_task_format_error: bool = (True,)
 
@@ -774,14 +776,16 @@
         role_name: str = "",
         install_dependencies: bool = True,
         version: str = "",
         hash: str = "",
         target_path: str = "",
         dependency_dir: str = "",
         download_only: bool = False,
+        load_only: bool = False,
+        skip_dependency: bool = False,
         use_src_cache: bool = False,
         source_repository: str = "",
         playbook_yaml: str = "",
         playbook_only: bool = False,
         taskfile_yaml: str = "",
         taskfile_only: bool = False,
         raw_yaml: str = "",
@@ -846,102 +850,110 @@
             if loaded:
                 scandata.set_metadata(metadata, dependencies)
                 metdata_loaded = True
                 if not self.silent:
                     logger.debug(f'Use metadata for "{scandata.name}" in RAM DB')
 
         if scandata.install_dependencies and not metdata_loaded:
-            print(f"start preparing {scandata.type} {scandata.name}")
+            logger.debug(f"start preparing {scandata.type} {scandata.name}")
             scandata._prepare_dependencies()
-            print(f"finished preparing {scandata.type} {scandata.name}")
+            logger.debug(f"finished preparing {scandata.type} {scandata.name}")
 
         if download_only:
             scandata.set_metadata_findings()
             self.register_findings_to_ram(scandata.findings)
             return None
         self.record_end(time_records, "metadata_load")
 
-        ext_list = []
-        ext_list.extend(
-            [
-                (
-                    d.get("metadata", {}).get("type", ""),
-                    d.get("metadata", {}).get("name", ""),
-                    d.get("metadata", {}).get("version", ""),
-                    d.get("metadata", {}).get("hash", ""),
-                    d.get("dir"),
-                )
-                for d in scandata.loaded_dependency_dirs
-            ]
-        )
-        ext_count = len(ext_list)
+        if not skip_dependency:
+            ext_list = []
+            ext_list.extend(
+                [
+                    (
+                        d.get("metadata", {}).get("type", ""),
+                        d.get("metadata", {}).get("name", ""),
+                        d.get("metadata", {}).get("version", ""),
+                        d.get("metadata", {}).get("hash", ""),
+                        d.get("dir"),
+                    )
+                    for d in scandata.loaded_dependency_dirs
+                ]
+            )
+            ext_count = len(ext_list)
+
+            # Start ARI Scanner main flow
+            self.record_begin(time_records, "dependency_load")
+            for i, (ext_type, ext_name, ext_ver, ext_hash, ext_path) in enumerate(ext_list):
+                if not self.silent:
+                    if i == 0:
+                        logger.info("start loading {} {}(s)".format(ext_count, ext_type))
+                    logger.info("[{}/{}] {} {}".format(i + 1, ext_count, ext_type, ext_name))
+
+                # avoid infinite loop
+                is_root = False
+                if scandata.type == ext_type and scandata.name == ext_name:
+                    is_root = True
+
+                if not is_root:
+                    key = "{}-{}".format(ext_type, ext_name)
+                    read_ram_for_dependency = self.read_ram or self.read_ram_for_dependency
+
+                    dep_loaded = False
+                    if read_ram_for_dependency:
+                        # searching findings from ARI RAM and use them if found
+                        dep_loaded, ext_defs = self.load_definitions_from_ram(ext_type, ext_name, ext_ver, ext_hash)
+                        if dep_loaded:
+                            scandata.ext_definitions[key] = ext_defs
+                            if not self.silent:
+                                logger.debug(f'Use spec data for "{ext_name}" in RAM DB')
+
+                    if not dep_loaded:
+                        # scan dependencies and save findings to ARI RAM
+                        dep_scanner = ARIScanner(
+                            root_dir=self.root_dir,
+                            rules_dir="",
+                            rules=[],
+                            ram_client=self.ram_client,
+                            read_ram=read_ram_for_dependency,
+                            read_ram_for_dependency=self.read_ram_for_dependency,
+                            write_ram=self.write_ram,
+                            use_ansible_doc=self.use_ansible_doc,
+                            do_save=self.do_save,
+                            silent=True,
+                        )
+                        # use prepared dep dirs
+                        dep_scanner.evaluate(
+                            type=ext_type,
+                            name=ext_name,
+                            version=ext_ver,
+                            hash=ext_hash,
+                            target_path=ext_path,
+                            dependency_dir=scandata.dependency_dir,
+                            skip_dependency=True,
+                            source_repository=scandata.source_repository,
+                            include_test_contents=include_test_contents,
+                            load_only=True,
+                        )
+                        dep_scandata = dep_scanner.get_last_scandata()
+                        scandata.ext_definitions[key] = dep_scandata.root_definitions
+                        dep_loaded = True
+
+            self.record_end(time_records, "dependency_load")
+
+            if not self.silent:
+                logger.debug("load_definition_ext() done")
 
         # PRM Finder
         self.record_begin(time_records, "prm_load")
         # playbooks, roles, modules = find_playbook_role_module(scandata.target_path, self.use_ansible_doc)
         # scandata.prm["playbooks"] = playbooks
         # scandata.prm["roles"] = roles
         # scandata.prm["modules"] = modules
         self.record_end(time_records, "prm_load")
 
-        # Start ARI Scanner main flow
-        self.record_begin(time_records, "dependency_load")
-        for i, (ext_type, ext_name, ext_ver, ext_hash, ext_path) in enumerate(ext_list):
-            if not self.silent:
-                if i == 0:
-                    logger.info("start loading {} {}(s)".format(ext_count, ext_type))
-                logger.info("[{}/{}] {} {}".format(i + 1, ext_count, ext_type, ext_name))
-
-            # avoid infinite loop
-            is_root = False
-            if scandata.type == ext_type and scandata.name == ext_name:
-                is_root = True
-
-            if not is_root:
-                # scan dependencies and save findings to ARI RAM
-                dep_scanner = ARIScanner(
-                    root_dir=self.root_dir,
-                    rules_dir=self.rules_dir,
-                    rules=self.rules,
-                    ram_client=self.ram_client,
-                    read_ram=self.read_ram,
-                    write_ram=self.write_ram,
-                    use_ansible_doc=self.use_ansible_doc,
-                    do_save=self.do_save,
-                    silent=True,
-                )
-                # use prepared dep dirs
-                dep_scanner.evaluate(
-                    type=ext_type,
-                    name=ext_name,
-                    version=ext_ver,
-                    hash=ext_hash,
-                    target_path=ext_path,
-                    dependency_dir=scandata.dependency_dir,
-                    source_repository=scandata.source_repository,
-                    include_test_contents=include_test_contents,
-                )
-
-                if self.read_ram:
-                    # searching findings from ARI RAM and use them if found
-                    loaded, ext_defs = self.load_definitions_from_ram(ext_type, ext_name, ext_ver, ext_hash)
-                    if loaded:
-                        key = "{}-{}".format(ext_type, ext_name)
-                        scandata.ext_definitions[key] = ext_defs
-                        if not self.silent:
-                            logger.debug(f'Use spec data for "{ext_name}" in RAM DB')
-                        continue
-
-                # load the src directory
-                scandata.load_definition_ext(ext_type, ext_name, ext_path)
-        self.record_end(time_records, "dependency_load")
-
-        if not self.silent:
-            logger.debug("load_definition_ext() done")
-
         loaded = False
         self.record_begin(time_records, "target_load")
         if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE]:
             loaded, root_defs = self.load_definitions_from_ram(scandata.type, scandata.name, scandata.version, scandata.hash, allow_unresolved=True)
             logger.debug(f"spec data loaded: {loaded}")
             if loaded:
                 scandata.root_definitions = root_defs
@@ -965,14 +977,19 @@
 
         self.record_begin(time_records, "apply_spec_rules")
         scandata.apply_spec_mutations()
         self.record_end(time_records, "apply_spec_rules")
         if not self.silent:
             logger.debug("apply_spec_rules() done")
 
+        # load_only is True when this scanner is scanning dependency
+        # otherwise, move on tree construction / rule evaluation
+        if load_only:
+            return None
+
         _ram_client = None
         if self.read_ram:
             _ram_client = self.ram_client
 
         self.record_begin(time_records, "tree_construction")
         scandata.construct_trees(_ram_client)
         self.record_end(time_records, "tree_construction")
@@ -1053,14 +1070,16 @@
                     role_name=role_name,
                     install_dependencies=install_dependencies,
                     version=version,
                     hash=hash,
                     target_path=target_path,
                     dependency_dir=dependency_dir,
                     download_only=download_only,
+                    load_only=load_only,
+                    skip_dependency=skip_dependency,
                     use_src_cache=use_src_cache,
                     source_repository=source_repository,
                     playbook_yaml=playbook_yaml,
                     playbook_only=playbook_only,
                     taskfile_yaml=taskfile_yaml,
                     taskfile_only=taskfile_only,
                     include_test_contents=include_test_contents,
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -481,29 +481,34 @@
         for i, mapping in enumerate(self.taskfile_mappings):
             logger.debug("[{}/{}] {}".format(i + 1, len(self.taskfile_mappings), mapping[1]))
             taskfile_key = mapping[1]
             tree_objects = self._recursive_get_calls(taskfile_key)
             self.trees.append(tree_objects)
         return self.trees, additional_objects
 
-    def _recursive_get_calls(self, key, caller=None, handover={}, index=0):
+    def _recursive_get_calls(self, key, caller=None, handover={}, index=0, history=[]):
         obj_list = ObjectList()
         obj = self.get_object(key)
         if obj is None:
             return obj_list
+        if key in history:
+            return obj_list
+        _history = deepcopy(history)
         call_obj = call_obj_from_spec(spec=obj, caller=caller, index=index)
         if call_obj is not None:
             obj_list.add(call_obj, update_dict=False)
+            history.append(key)
         children_keys, from_ram, handover = self._get_children_keys(obj, handover_from_upper_node=handover)
         for i, c_key in enumerate(children_keys):
             child_objects = self._recursive_get_calls(
                 c_key,
                 call_obj,
                 handover,
                 i,
+                _history,
             )
             if isinstance(call_obj, TaskCall):
                 taskcall = call_obj
                 if len(child_objects.items) > 0:
                     c_obj = child_objects.items[0]
                     if taskcall.spec.executable_type == ExecutableType.MODULE_TYPE:
                         taskcall.module = c_obj.spec
@@ -662,16 +667,18 @@
             children_keys.extend(obj.post_tasks)
         elif isinstance(obj, Role):
             target_taskfiles = ["main.yml", "main.yaml"]
             if isinstance(handover_from_upper_node, dict) and "tasks_from" in handover_from_upper_node:
                 tasks_from = handover_from_upper_node.get("tasks_from")
                 if tasks_from:
                     target_taskfiles = [tasks_from]
-            main_taskfile_key = [tf for tf in obj.taskfiles if tf.split(key_delimiter)[-1].split("/")[-1] in target_taskfiles]
-            children_keys.extend(main_taskfile_key)
+            target_taskfile_key = [
+                tf for tf in obj.taskfiles if tf.split(key_delimiter)[-1].split("/")[-1] in target_taskfiles and "/handlers/" not in tf
+            ]
+            children_keys.extend(target_taskfile_key)
         elif isinstance(obj, TaskFile):
             children_keys = obj.tasks
         elif isinstance(obj, Task):
             executable_type = obj.executable_type
             resolved_key = ""
             if obj.executable == "":
                 return [], {}, {}
```

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 ansible_risk_insight/rules/R305_unresolved_role.py
 ansible_risk_insight/rules/R306_undefined_variable.py
 ansible_risk_insight/rules/R401_list_all_inbound_src.py
 ansible_risk_insight/rules/R402_list_all_used_variables.py
 ansible_risk_insight/rules/R404_show_variables.py
 ansible_risk_insight/rules/R501_dependency_suggestion.py
 ansible_risk_insight/rules/__init__.py
+ansible_risk_insight/rules/rule_versions.json
 ansible_risk_insight/rules/sample_rule.py
 doc/images/ari-apply-rules.png
 doc/images/ari-arch.png
 doc/images/ari-overview.png
 doc/images/ari-ram-list.png
 docs/annotation.md
 docs/customize_rules.md
```

### Comparing `ansible-risk-insight-0.1.1rc1/data-struct.txt` & `ansible-risk-insight-0.1.2rc1/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.2rc1/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/docs/annotation.md` & `ansible-risk-insight-0.1.2rc1/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/docs/customize_rules.md` & `ansible-risk-insight-0.1.2rc1/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.2rc1/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/example/readme.md` & `ansible-risk-insight-0.1.2rc1/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.2rc1/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/example/sample.py` & `ansible-risk-insight-0.1.2rc1/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/mkdocs.yml` & `ansible-risk-insight-0.1.2rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/pyproject.toml` & `ansible-risk-insight-0.1.2rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 keywords = ["one", "two"]
 license = {text = "Apache License 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "gitdb",
-    "GitPython",
+    "pygit2",
     "joblib",
     "jsonpickle",
     "PyYAML",
     "smmap",
     "tabulate",
     "requests",
     "ansible",
```

### Comparing `ansible-risk-insight-0.1.1rc1/test/test_scanner.py` & `ansible-risk-insight-0.1.2rc1/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.1rc1/tox.ini` & `ansible-risk-insight-0.1.2rc1/tox.ini`

 * *Files identical despite different names*

