# Comparing `tmp/seven_studio-1.1.9.tar.gz` & `tmp/seven_studio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seven_studio-1.1.9.tar", last modified: Thu Dec  8 05:04:54 2022, max compression
+gzip compressed data, was "dist/seven_studio-1.2.0.tar", last modified: Mon Apr 10 07:25:52 2023, max compression
```

## Comparing `seven_studio-1.1.9.tar` & `seven_studio-1.2.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.265902 seven_studio-1.1.9/
--rw-r--r--   0 root         (0) root         (0)     2781 2022-12-08 05:04:54.264902 seven_studio-1.1.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1386 2022-12-08 05:03:49.000000 seven_studio-1.1.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-08 05:04:54.265902 seven_studio-1.1.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1265 2022-12-08 05:03:49.000000 seven_studio-1.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.210903 seven_studio-1.1.9/seven_studio/
--rwxrwxrwx   0 root         (0) root         (0)      156 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.217903 seven_studio-1.1.9/seven_studio/handlers/
--rwxrwxrwx   0 root         (0) root         (0)      132 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1626 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/monitor.py
--rwxrwxrwx   0 root         (0) root         (0)    25666 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/studio_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.222903 seven_studio-1.1.9/seven_studio/handlers/system/
--rwxrwxrwx   0 root         (0) root         (0)      224 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8699 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/system/core.py
--rwxrwxrwx   0 root         (0) root         (0)    20920 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/system/file.py
--rwxrwxrwx   0 root         (0) root         (0)    16654 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/system/menu.py
--rwxrwxrwx   0 root         (0) root         (0)    30112 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/system/power.py
--rwxrwxrwx   0 root         (0) root         (0)     6155 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/system/product.py
--rwxrwxrwx   0 root         (0) root         (0)     2448 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/handlers/system/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.223903 seven_studio-1.1.9/seven_studio/libs/
--rwxrwxrwx   0 root         (0) root         (0)      156 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.228903 seven_studio-1.1.9/seven_studio/libs/file/
--rwxrwxrwx   0 root         (0) root         (0)      156 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8612 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/file/bos.py
--rwxrwxrwx   0 root         (0) root         (0)     8613 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/file/cos.py
--rwxrwxrwx   0 root         (0) root         (0)    19074 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/file/ks3.py
--rwxrwxrwx   0 root         (0) root         (0)     9588 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/file/oss2.py
--rwxrwxrwx   0 root         (0) root         (0)     8593 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/file/s3.py
--rwxrwxrwx   0 root         (0) root         (0)    14037 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/file/upload.py
--rwxrwxrwx   0 root         (0) root         (0)     6306 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/libs/geetest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.233903 seven_studio-1.1.9/seven_studio/models/
--rwxrwxrwx   0 root         (0) root         (0)      180 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.234902 seven_studio-1.1.9/seven_studio/models/db_models/
--rwxrwxrwx   0 root         (0) root         (0)      156 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.241902 seven_studio-1.1.9/seven_studio/models/db_models/file/
--rwxrwxrwx   0 root         (0) root         (0)      308 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1492 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/file/file_history_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1131 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/file/file_resource_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2433 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/file/file_restrict_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1578 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/file/file_restrict_pic_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1451 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/file/file_storage_path_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/file/file_water_image_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.242902 seven_studio-1.1.9/seven_studio/models/db_models/log/
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/log/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1298 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/log/log_action_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.247902 seven_studio-1.1.9/seven_studio/models/db_models/menu/
--rwxrwxrwx   0 root         (0) root         (0)       67 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/menu/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1583 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/menu/menu_cote_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2174 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/menu/menu_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)    19071 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/menu/menu_info_model_ex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.250902 seven_studio-1.1.9/seven_studio/models/db_models/product/
--rwxrwxrwx   0 root         (0) root         (0)       52 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/product/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1689 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/product/product_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)      983 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/product/product_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.255902 seven_studio-1.1.9/seven_studio/models/db_models/role/
--rwxrwxrwx   0 root         (0) root         (0)       87 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/role/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1148 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/role/role_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1014 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/role/role_power_model.py
--rwxrwxrwx   0 root         (0) root         (0)      952 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/role/role_power_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1036 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/role/role_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.256902 seven_studio-1.1.9/seven_studio/models/db_models/settings/
--rwxrwxrwx   0 root         (0) root         (0)       32 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/settings/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1152 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/settings/settings_base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.261902 seven_studio-1.1.9/seven_studio/models/db_models/user/
--rwxrwxrwx   0 root         (0) root         (0)       68 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/user/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2025 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/user/user_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1125 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/user/user_info_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1035 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/db_models/user/user_login_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/dto_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2419 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/enum.py
--rwxrwxrwx   0 root         (0) root         (0)    34400 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/power_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2689 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/models/seven_model.py
--rwxrwxrwx   0 root         (0) root         (0)     4398 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.263902 seven_studio-1.1.9/seven_studio/utils/
--rwxrwxrwx   0 root         (0) root         (0)      156 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1959 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/utils/dict.py
--rwxrwxrwx   0 root         (0) root         (0)      637 2022-12-08 05:03:49.000000 seven_studio-1.1.9/seven_studio/utils/random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 05:04:54.216903 seven_studio-1.1.9/seven_studio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2781 2022-12-08 05:04:53.000000 seven_studio-1.1.9/seven_studio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2669 2022-12-08 05:04:54.000000 seven_studio-1.1.9/seven_studio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-08 05:04:53.000000 seven_studio-1.1.9/seven_studio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-12-08 05:04:53.000000 seven_studio-1.1.9/seven_studio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-12-08 05:04:53.000000 seven_studio-1.1.9/seven_studio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.657166 seven_studio-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-04-10 07:25:52.657166 seven_studio-1.2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1449 2023-04-10 07:25:27.000000 seven_studio-1.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 07:25:52.657166 seven_studio-1.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1265 2023-04-10 07:25:27.000000 seven_studio-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.629154 seven_studio-1.2.0/seven_studio/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.632155 seven_studio-1.2.0/seven_studio/handlers/
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1626 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/monitor.py
+-rwxrwxrwx   0 root         (0) root         (0)    24916 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/studio_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.635156 seven_studio-1.2.0/seven_studio/handlers/system/
+-rwxrwxrwx   0 root         (0) root         (0)      224 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8880 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    22072 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/file.py
+-rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/menu.py
+-rwxrwxrwx   0 root         (0) root         (0)    31748 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/power.py
+-rwxrwxrwx   0 root         (0) root         (0)     6606 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/product.py
+-rwxrwxrwx   0 root         (0) root         (0)     2582 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.636157 seven_studio-1.2.0/seven_studio/libs/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.639158 seven_studio-1.2.0/seven_studio/libs/file/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8612 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/bos.py
+-rwxrwxrwx   0 root         (0) root         (0)     8613 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/cos.py
+-rwxrwxrwx   0 root         (0) root         (0)    19074 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/ks3.py
+-rwxrwxrwx   0 root         (0) root         (0)     9588 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/oss2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8593 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/s3.py
+-rwxrwxrwx   0 root         (0) root         (0)    14037 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/upload.py
+-rwxrwxrwx   0 root         (0) root         (0)     6306 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/geetest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.641159 seven_studio-1.2.0/seven_studio/models/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.641159 seven_studio-1.2.0/seven_studio/models/db_models/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.645161 seven_studio-1.2.0/seven_studio/models/db_models/file/
+-rwxrwxrwx   0 root         (0) root         (0)      308 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1492 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_history_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_resource_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2433 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1578 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_pic_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1451 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_storage_path_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_water_image_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.645161 seven_studio-1.2.0/seven_studio/models/db_models/log/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/log/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1298 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/log/log_action_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.647162 seven_studio-1.2.0/seven_studio/models/db_models/menu/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1583 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_cote_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2174 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    19404 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model_ex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.649163 seven_studio-1.2.0/seven_studio/models/db_models/product/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/product/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/product/product_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      983 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/product/product_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.651164 seven_studio-1.2.0/seven_studio/models/db_models/role/
+-rwxrwxrwx   0 root         (0) root         (0)       87 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1014 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      952 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.652164 seven_studio-1.2.0/seven_studio/models/db_models/settings/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/settings/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/settings/settings_base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.654165 seven_studio-1.2.0/seven_studio/models/db_models/user/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2025 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1125 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1035 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/user_login_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/dto_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2419 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/enum.py
+-rwxrwxrwx   0 root         (0) root         (0)    37518 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2689 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/seven_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     4391 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.656166 seven_studio-1.2.0/seven_studio/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1959 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/utils/dict.py
+-rwxrwxrwx   0 root         (0) root         (0)      637 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/utils/random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.631154 seven_studio-1.2.0/seven_studio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2669 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/top_level.txt
```

### Comparing `seven_studio-1.1.9/PKG-INFO` & `seven_studio-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven_studio
-Version: 1.1.9
+Version: 1.2.0
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         
@@ -15,14 +15,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.2.0 更新内容
+        * GetUserInfoHandler增加字段返回
+        
         ### 1.1.9 更新内容
         * 基础配置更新
         * 用户登录过期处理
         
         ### 1.1.8 更新内容
         * 用户登录过期
```

### Comparing `seven_studio-1.1.9/README.md` & `seven_studio-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
  * @LastEditors: ChenXiaolei
  * @Description: 
 -->
 # seven_studio
 
 ## 天志互联Python公共基础后台管理平台
 
+### 1.2.0 更新内容
+* GetUserInfoHandler增加字段返回
+
 ### 1.1.9 更新内容
 * 基础配置更新
 * 用户登录过期处理
 
 ### 1.1.8 更新内容
 * 用户登录过期
```

### Comparing `seven_studio-1.1.9/setup.py` & `seven_studio-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_studio",
-    version="1.1.9",
+    version="1.2.0",
     author="seven",
     author_email="tech@gao7.com",
     description="seven studio",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/python/seven_studio",
```

### Comparing `seven_studio-1.1.9/seven_studio/handlers/monitor.py` & `seven_studio-1.2.0/seven_studio/handlers/monitor.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/handlers/studio_base.py` & `seven_studio-1.2.0/seven_studio/handlers/studio_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: ChenXiaolei
 :Date: 2020-03-24 10:42:34
-:LastEditTime: 2022-12-08 10:48:47
+:LastEditTime: 2023-02-07 09:17:25
 :LastEditors: HuangJingCan
 :Description: StudioBaseHandler
 """
 
 from seven_framework.web_tornado.base_handler.base_cookie_handler import *
 from seven_framework.redis import *
 
@@ -101,19 +101,19 @@
         :param result_message: 字符串，服务端返回的错误信息
         :param data: 返回结果对象，即为数组，字典
         :return: 将dumps后的数据字符串返回给客户端
         :last_editors: HuangJingCan
         """
         if hasattr(data, '__dict__'):
             data = data.__dict__
-        rep_dic = {}
-        rep_dic['ResultCode'] = result_code
-        rep_dic['ResultMessage'] = result_message
-        rep_dic['Data'] = data
-
+        rep_dic = {
+            'ResultCode': result_code,
+            'ResultMessage': result_message,
+            'Data': data,
+        }
         self.http_reponse(self.json_dumps(rep_dic))
 
     def response_json_success(self, data=None, desc='调用成功'):
         """
         :description: 通用成功返回json结构
         :param data: 返回结果对象，即为数组，字典
         :param desc: 字符串，服务端返回的错误信息
@@ -142,16 +142,15 @@
 
     def redis_init(self, db=None):
         """
         :description: redis初始化
         :return: redis_cli
         :last_editors: HuangJingCan
         """
-        redis_cli = RedisHelper.redis_init(config_dict=config.get_value("redis"))
-        return redis_cli
+        return RedisHelper.redis_init(config_dict=config.get_value("redis"))
 
     def set_default_headers(self):
         allow_origin_list = config.get_value("allow_origin_list")
         origin = self.request.headers.get("Origin")
         if origin in allow_origin_list:
             self.set_header("Access-Control-Allow-Origin", origin)
 
@@ -166,71 +165,51 @@
             for info in reqInfoList:
                 kv = str.split(info, "=")
                 header_token[kv[0]] = kv[1]
         return header_token
 
     def request_user_id(self):
         header_token = self.request_header_token()
-        if not header_token.__contains__("UserID"):
-            return ""
-        return header_token["UserID"]
+        return header_token["UserID"] if header_token.__contains__("UserID") else ""
 
     def request_user_id_md5(self):
         header_token = self.request_header_token()
-        if not header_token.__contains__("UserIDMD5"):
-            return ""
-        return header_token["UserIDMD5"]
+        return (header_token["UserIDMD5"] if header_token.__contains__("UserIDMD5") else "")
 
     def request_user_token(self):
         header_token = self.request_header_token()
-        if not header_token.__contains__("UserToken"):
-            return ""
-        return header_token["UserToken"]
+        return (header_token["UserToken"] if header_token.__contains__("UserToken") else "")
 
     def request_product_id(self):
         header_product_id = ""
         if self.request.headers.__contains__("Manage-Productid"):
             header_product_id = self.request.headers["Manage-Productid"]
         product_id = int(header_product_id) if header_product_id.strip() != "" else 0
         if product_id == 0:
             product_id = int(self.get_param("manage-productid", "0"))
         return product_id
 
     def request_manage_page_id(self):
-        if not self.request.headers.__contains__("Manage-PageID"):
-            return ""
-        return self.request.headers["Manage-PageID"]
+        return (self.request.headers["Manage-PageID"] if self.request.headers.__contains__("Manage-PageID") else "")
 
     def get_product_info(self):
-        product_info = None
         product_id = self.request_product_id()
-        if product_id > 0:
-            product_info = ProductInfoModel(config.get_value("base_manage_context_key")).get_entity_by_id(product_id)
-        return product_info
+        return (ProductInfoModel(config.get_value("base_manage_context_key")).get_entity_by_id(product_id) if product_id > 0 else None)
 
     def get_curr_user_info(self):
-        user_info = None
         user_id = self.request_user_id()
-        if user_id:
-            user_info = UserInfoModel(self.get_manage_context_key()).get_entity_by_id(user_id)
-        return user_info
+        return (UserInfoModel(self.get_manage_context_key()).get_entity_by_id(user_id) if user_id else None)
 
     def get_base_user_info(self):
-        user_info = None
         user_id = self.request_user_id()
-        if user_id:
-            user_info = UserInfoModel(config.get_value("base_manage_context_key")).get_entity_by_id(user_id)
-        return user_info
+        return (UserInfoModel(config.get_value("base_manage_context_key")).get_entity_by_id(user_id) if user_id else None)
 
     def get_is_super(self):
         base_user_info = self.get_base_user_info()
-        is_super = False
-        if base_user_info:
-            is_super = True if base_user_info.IsSuper == 1 else False
-        return is_super
+        return base_user_info.IsSuper == 1 if base_user_info else False
 
     def get_manage_context_key(self):
         manage_context_key = config.get_value("manage_context_key")
         product_info = self.get_product_info()
         if product_info:
             manage_context_key = product_info.ManageContextKey
         return manage_context_key
@@ -248,35 +227,35 @@
         if product_info:
             log_context_key = product_info.LogContextKey
         return log_context_key
 
     def get_page_index(self):
         page_index = 0
         r_page_index = self.get_param("PageIndex", "")
-        if not r_page_index == "":
+        if r_page_index != "":
             dict_page_index = json.loads(r_page_index)
             if dict_page_index and dict_page_index.__contains__("Value"):
                 page_index = dict_page_index["Value"]
         return page_index
 
     def get_page_size(self):
         page_size = 10
         r_page_size = self.get_param("PageSize", "")
-        if not r_page_size == "":
+        if r_page_size != "":
             dict_page_size = json.loads(r_page_size)
             if dict_page_size and dict_page_size.__contains__("Value"):
                 page_size = dict_page_size["Value"]
         return page_size
 
     def get_page_cote_id(self):
-        page_cote_id = ""
         page_id = self.request_manage_page_id()
-        if not page_id == "":
-            page_cote_id = page_id.split("$")[1] if page_id.__contains__("$") else ""
-        return page_cote_id
+        if page_id != "":
+            return page_id.split("$")[1] if page_id.__contains__("$") else ""
+        else:
+            return ""
 
     def get_dict_page_info_list(self, page_index, page_size, p_dict, total=0):
         """
         :description: 获取分页信息
         :param page_index：页索引
         :param page_size：页大小
         :param p_dict：字典列表
@@ -297,20 +276,16 @@
         :param source_dict
         :param keys
         :return: 值
         :last_editors: HuangJingCan
         """
         if isinstance(source_dict, str):
             source_dict = json.loads(source_dict)
-        result = {}
         key_list = list(keys.split(","))
-        for i in key_list:
-            if i in source_dict:
-                result[i] = source_dict[i]
-        return result
+        return {i: source_dict[i] for i in key_list if i in source_dict}
 
     def get_condition_by_body(self):
         """
         :description: 获取页面查询条件
         :param {type} 
         :return: condition, order
         :last_editors: HuangJingCan
@@ -354,16 +329,15 @@
     def get_system_user_table(self):
         """
         :description: 获取系统用户
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        user_dict = UserInfoModel(self.get_manage_context_key()).get_dict_list()
-        return user_dict
+        return UserInfoModel(self.get_manage_context_key()).get_dict_list()
 
     def logout(self, user_id):
         """
         :description: 用户退出
         :param user_id：用户id
         :return: 
         :last_editors: HuangJingCan
@@ -416,23 +390,21 @@
         :return: True or False
         :last_editors: HuangJingCan
         """
         manage_context_key = self.get_manage_context_key()
         menu_info_list = MenuInfoModel(manage_context_key).get_list(f"ApiPath LIKE '%{api_path}%'")
         if not menu_info_list:
             return False
-        if len([i for i in menu_info_list if i.IsPower == 0]) > 0:
+        if [i for i in menu_info_list if i.IsPower == 0]:
             return True
         role_user_list = RoleUserModel(manage_context_key).get_list("UserID=%s", params=self.request_user_id())
         role_power_list = RolePowerModelEx(manage_context_key).get_role_power_list([i.RoleID for i in role_user_list])
         cote_list = [i for i in role_power_list if i.CoteID == cote_id]
         menu_list = [i.MenuID for i in menu_info_list]
-        if len([i for i in cote_list if menu_list.__contains__(i.MenuID)]) > 0:
-            return True
-        return False
+        return bool([i for i in cote_list if menu_list.__contains__(i.MenuID)])
 
     def auto_mapper(self, s_model, map_dict=None):
         """
         :description: 对象映射（把map_dict值赋值到实体s_model中）
         :param s_model：需要映射的实体对象
         :param map_dict：被映射的实体字典
         :return: 映射后的实体s_model
@@ -441,45 +413,41 @@
             field_list = s_model.get_field_list()
             for filed in field_list:
                 if filed in map_dict:
                     setattr(s_model, filed, map_dict[filed])
         return s_model
 
     def login_filter(self, is_need_login, optional_params):
+        # sourcery skip: class-extract-method
         """
         :description: 登录过滤器
         :param is_need_login: 是否需要登录（true需要false不需要）
         :param optional_params: 其他参数
         :return: InvokeResult
         """
         invoke_result = InvokeResult()
         base_manage_context_key = config.get_value("base_manage_context_key")
         # 获取头部信息
         header_token = self.request_header_token()
         user_id = header_token["UserID"] if header_token.__contains__("UserID") else ""
         user_token = header_token["UserToken"] if header_token.__contains__("UserToken") else ""
         user_id_md5 = header_token["UserIDMD5"] if header_token.__contains__("UserIDMD5") else ""
         if user_id.strip() == "" or user_token.strip() == "" or user_id_md5.strip() == "":
-            # return self.response_common("NoLogin", "操作失败，用户未登录")
             invoke_result.ResultCode = "error"
             invoke_result.ResultMessage = "操作失败，用户未登录"
             return invoke_result
         if is_need_login and CryptoHelper.md5_encrypt(user_id, config.get_value("login_encrypt_key")) != user_id_md5:
-            # return self.response_common("NoLogin", "操作失败，用户未登录")
             invoke_result.ResultCode = "error"
             invoke_result.ResultMessage = "操作失败，用户未登录"
             return invoke_result
 
         # 登陆日志判断，Redis还是MySQL
         if config.get_value("login_type") == "redis":
             redis_user_login = self.redis_init().hget(config.get_value("redis_provider_name_user_login"), user_id)
-            user_login = {}
-            if redis_user_login:
-                user_login = json.loads(redis_user_login)
-
+            user_login = json.loads(redis_user_login) if redis_user_login else {}
             if not user_login or TimeHelper.format_time_to_datetime(user_login["ExpireTime"]) < TimeHelper.get_now_datetime():
                 if not is_need_login:
                     return invoke_result
                 self.clear_user_cookie()
                 invoke_result.ResultCode = "login_expire"
                 invoke_result.ResultMessage = "用户已过期，请重新登录"
                 return invoke_result
```

### Comparing `seven_studio-1.1.9/seven_studio/handlers/system/core.py` & `seven_studio-1.2.0/seven_studio/handlers/system/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: HuangJingCan
 :Date: 2020-03-24 19:48:05
-:LastEditTime: 2022-12-08 10:42:51
+:LastEditTime: 2023-02-06 16:29:03
 :LastEditors: HuangJingCan
 :Description: 
 """
 from seven_studio.handlers.studio_base import *
 from seven_studio.libs.geetest import *
 
 from seven_studio.models.db_models.user.user_info_model_ex import *
@@ -38,18 +38,23 @@
 
 
 class LoginPlatformHandler(StudioBaseHandler):
     """
     :description: 登陆
     """
     def get_async(self):
+        # 账号
         account = self.get_param("account")
+        # 密码
         password = self.get_param("password")
+        # 极验证参数challenge
         challenge = self.get_param("challenge")
+        # 极验证参数validate
         validate = self.get_param("validate")
+        # 极验证参数seccode
         seccode = self.get_param("seccode")
 
         if account == "":
             return self.response_common("EmptyAccount", "对不起，请你输入账号")
 
         if password == "":
             return self.response_common("EmptyPassword", "对不起，请您输入密码")
@@ -63,17 +68,17 @@
                 return self.response_common("CaptchaError", "对不起，验证码验证失败")
 
         return self.response_custom(self.login(account, password, True))
 
     def check_code(self, challenge="", validate="", seccode=""):
         """
         :description: 验证码校验
-        :param challenge：challenge
-        :param validate：validate
-        :param seccode：seccode
+        :param challenge：极验证参数challenge
+        :param validate：极验证参数validate
+        :param seccode：极验证参数seccode
         :return: true or false
         :last_editors: HuangJingCan
         """
         gt = GeetestLib(config.get_value("pc_geetest_id"), config.get_value("pc_geetest_key"))
         result = gt.success_validate(challenge, validate, seccode, JSON_FORMAT=0)
         return result == 1
```

### Comparing `seven_studio-1.1.9/seven_studio/handlers/system/file.py` & `seven_studio-1.2.0/seven_studio/handlers/system/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: HuangJingCan
 :Date: 2020-03-17 16:12:54
-:LastEditTime: 2022-12-06 09:48:49
+:LastEditTime: 2023-02-07 17:17:49
 :LastEditors: HuangJingCan
 :Description: 文件操作相关接口
 """
 from seven_studio.handlers.studio_base import *
 
 from seven_studio.models.db_models.file.file_storage_path_model import *
 from seven_studio.models.db_models.file.file_resource_model import *
@@ -25,17 +25,21 @@
     def post_async(self):
         """
         :description: 获取存储配置列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 数据库连接串
         file_storage_path_model = FileStoragePathModel(self.get_file_context_key())
+        # 页索引
         page_index = self.get_page_index()
+        # 页大小
         page_size = self.get_page_size()
+        # 查询条件,排序字段
         condition, order = self.get_condition_by_body()
 
         p_dict, total = file_storage_path_model.get_dict_page_list("*", page_index, page_size, condition, "", order)
 
         return self.response_json_success(self.get_dict_page_info_list(page_index, page_size, p_dict, total))
 
 
@@ -70,24 +74,33 @@
     def post_async(self):
         """
         :description: 保存存储配置
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 存储标识
         file_storage_path_id = self.get_param("FileStoragePathID")
+        # 存储名称
         storage_path_name = self.get_param("StoragePathName")
+        # 存储类型1本地存储2FTP3文件系统
         storage_type_id = int(self.get_param("StorageTypeID", "0"))
+        # 虚目录
         virtual_name = self.get_param("VirtualName")
+        # 存储地址
         storage_path = self.get_param("StoragePath")
+        # IP
         ip_address = self.get_param("IPAddress")
+        # 帐号
         account = self.get_param("Account")
+        # 密码
         password = self.get_param("Password")
+        # 端口
         port = self.get_param("Port")
+        # 配置文件
         storage_config = self.get_param("StorageConfig")
 
         # 验证数据
         if storage_path_name == "":
             return self.response_common("StoragePathNameEmpty", "存储名称参数为空")
 
         file_storage_path_model = FileStoragePathModel(self.get_file_context_key())
@@ -148,17 +161,21 @@
     def post_async(self):
         """
         :description: 获取文件配置列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 文件上下文配置
         file_resource_model = FileResourceModel(self.get_file_context_key())
+        # 页索引
         page_index = self.get_page_index()
+        # 页大小
         page_size = self.get_page_size()
+        # 查询条件,排序字段
         condition, order = self.get_condition_by_body()
 
         p_dict, total = file_resource_model.get_dict_page_list("*", page_index, page_size, condition, "", order)
 
         return self.response_json_success(self.get_dict_page_info_list(page_index, page_size, p_dict, total))
 
 
@@ -190,17 +207,19 @@
     def post_async(self):
         """
         :description: 保存文件配置
         :param id：id
         :return: 
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 文件资源标识
         file_resource_id = self.get_param("FileResourceID")
+        # 文件资源名称
         file_resource_name = self.get_param("FileResourceName")
+        # 文件资源代码
         file_resource_code = self.get_param("FileResourceCode")
 
         # 验证数据
         if file_resource_name == "":
             return self.response_common("FileResourceNameEmpty", "FileResourceName参数为空")
         if file_resource_code == "":
             return self.response_common("FileResourceCodeEmpty", "FileResourceCode参数为空")
@@ -292,36 +311,57 @@
     def post_async(self):
         """
         :description: SaveRestrict
         :param id：id
         :return: response_json_success
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 文件限制标识
         file_restrict_id = self.get_param("FileRestrictID")
+        # 存储路经标识
         file_storage_path_id = self.get_param("FileStoragePathID")
+        # 文件资源标识
         access_mode_code_type = int(self.get_param("AccessModeCodeType", "0"))
+        # 文件访问方式
         path_format_code_type = int(self.get_param("PathFormatCodeType", "0"))
+        # 限制名称
         restrict_name = self.get_param("RestrictName")
+        # 资源代码
         restrict_code = self.get_param("RestrictCode")
+        # 1文件2图片3flash4mid
         file_type = int(self.get_param("FileType", "0"))
+        # 文件扩展名
         file_extension = self.get_param("FileExtension")
+        # 大小限制单位(K)0不限制
         file_max_size = int(self.get_param("FileMaxSize", "0"))
+        # 是否返回尺寸
         is_return_size = int(self.get_param("IsReturnSize", "0"))
+        # 是否Md5
         is_md5 = int(self.get_param("IsMd5", "0"))
+        # 是否记录文件记录
         is_history = int(self.get_param("IsHistory", "0"))
+        # 是否创建水印
         is_water_mark = int(self.get_param("IsWaterMark", "0"))
+        # 是否格式化成Jpeg
         is_format_jpeg = int(self.get_param("IsFormatJpeg", "0"))
+        # 水印文字
         water_mark_text = self.get_param("WatermarkText")
+        # 水平位置
         horizontal_align = int(self.get_param("HorizontalAlign", "0"))
+        # 垂直位置
         vertical_align = int(self.get_param("VerticalAlign", "0"))
+        # 图片宽度
         image_width = int(self.get_param("ImageWidth", "0"))
+        # 图片高度
         image_height = int(self.get_param("ImageHeight", "0"))
+        # 质量压缩
         quality_value = int(self.get_param("QualityValue", "0"))
+        # 水印类型
         water_mark_type = int(self.get_param("WatermarkType", "0"))
+        # 水印标识
         water_image_id = self.get_param("WaterImageID")
 
         # 验证数据
         if restrict_name == "":
             return self.response_common("RestrictNameEmpty", "RestrictName参数为空")
         if restrict_code == "":
             return self.response_common("RestrictCodeEmpty", "RestrictCode参数为空")
@@ -446,17 +486,19 @@
         :description: 保存图片水印
         :param WaterImageID：水印图片id 
         :param WaterImagePath：水印图片路径
         :param WaterName：水印图片名称
         :return: response_json_success
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 水印id
         water_image_id = self.get_param("WaterImageID")
+        # 水印地址
         water_image_path = self.get_param("WaterImagePath")
+        # 水印名称
         water_name = self.get_param("WaterName")
 
         # 验证数据
         if water_name == "":
             return self.response_common("WaterNameEmpty", "水印名称为空")
 
         file_water_image_model = FileWaterImageModel(self.get_file_context_key())
@@ -488,15 +530,17 @@
     def get_async(self):
         """
         :description: 删除
         :param WaterImageID：主键id
         :return: 
         :last_editors: HuangJingCan
         """
+        # 水印图id
         water_image_id = self.get_param("WaterImageID")
+
         if water_image_id == "":
             return self.response_common("WaterImageIDEmpty", "WaterImageID为空")
 
         FileWaterImageModel(self.get_file_context_key()).del_entity("WaterImageID=%s", water_image_id)
 
         return self.response_json_success()
 
@@ -533,15 +577,17 @@
     def get_async(self):
         """
         :description: 删除文件历史记录
         :param FileHistoryID：主键id
         :return: 
         :last_editors: HuangJingCan
         """
+        # 文件历史记录id
         file_history_id = self.get_param("FileHistoryID")
+
         if file_history_id == "":
             return self.response_common("FileHistoryIDEmpty", "FileHistoryID为空")
 
         result = 0
         file_context_key = self.get_file_context_key()
         file_history_model = FileHistoryModel(file_context_key)
         file_history = file_history_model.get_entity_by_id(file_history_id)
```

### Comparing `seven_studio-1.1.9/seven_studio/handlers/system/menu.py` & `seven_studio-1.2.0/seven_studio/handlers/system/menu.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: dongyu
 :Date: 2020-04-11 18:44:08
-:LastEditTime: 2022-12-06 17:07:54
+:LastEditTime: 2023-02-08 16:50:13
 :LastEditors: HuangJingCan
 :Description: 菜单相关类
 """
 from seven_studio.handlers.studio_base import *
 from seven_studio.models.db_models.menu.menu_cote_model import *
 from seven_studio.models.db_models.menu.menu_info_model_ex import *
 from seven_studio.models.power_model import *
@@ -20,17 +20,21 @@
     def get_async(self):
         """
         :description: 根据登陆用户获取用户有权限的栏目菜单
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 数据库连接串
         manage_context_key = self.get_manage_context_key()
+        # 是否超管
         is_super = self.get_is_super()
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 产品id
         product_id = self.request_product_id()
 
         power_model = PowerModel(manage_context_key, is_super, curr_user_id, product_id)
         result = power_model.get_platform_power_menu_list()
 
         return self.response_json_success(result)
 
@@ -151,32 +155,49 @@
     def post_async(self):
         """
         :description: 保存菜单
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        # 获取参数
-        parent_id = self.get_param("parentID")
+        # 菜单标识
         menu_id = self.get_param("id")
+        # 父标识
+        parent_id = self.get_param("parentID")
+        # 菜单类型
         menu_type = self.get_param("menuType")
+        # 图标地址
         menu_icon = self.get_param("menuIcon")
+        # 菜单名称
         menu_name = self.get_param("menuName")
+        # 是否显示0不显示1显示
         is_show = int(self.get_param("isShow", "0"))
+        # 是否授权0不1是
         is_power = int(self.get_param("isPower", "0"))
+        # 接口地址
         api_path = self.get_param("apiPath")
+        # 视图地址
         view_path = self.get_param("viewPath")
+        # 跳转地址
         target_url = self.get_param("targetUrl")
+        # 菜单命令
         command_name = self.get_param("commandName")
+        # 菜单参数
         command_parms = self.get_param("commandParms")
+        # 1顶部2列表3底部
         button_place = self.get_param("buttonPlace")
+        # 按钮颜色
         button_color = self.get_param("buttonColor")
+        # 菜单显示条件
         show_condition_str = self.get_param("showConditionStr")
+        # 栏目数据ID
         menu_cote_id = int(self.get_param("menuCoteID", "0"))
+        # 栏目标识
         menu_cote_key = self.get_param("menuCoteKey")
+        # 排序号
         sort_index = int(self.get_param("sortIndex", "0"))
         old_menu_name = ""
 
         # 验证数据
         if menu_name == "":
             return self.response_common("MenuNameEmpty", "菜单名为空")
         if [1, 2, 3].__contains__(menu_type):
@@ -223,22 +244,22 @@
 class AddFastMenuHandler(StudioBaseHandler):
     """
     :description: 快速添加菜单
     """
     def get_async(self):
         """
         :description: 快速添加菜单-保存
-        :param parent_id
-        :param button_type_str
-        :param suffix_name
         :return: 菜单id
         :last_editors: HuangJingCan
         """
+        # 父栏目id
         parent_id = self.get_param("parentID")
+        # 按钮类型
         button_type_str = self.get_param("buttonTypeStr")
+        # 按钮名称后缀
         suffix_name = self.get_param("suffixName")
 
         if parent_id == "":
             return self.response_common("ParentIDEmpty", "父节点为空")
         if button_type_str == "":
             return self.response_common("ButtonTypeEmpty", "菜单类型为空")
 
@@ -275,15 +296,17 @@
         """
         :description: 复制粘贴菜单
         :param copyMenuID：复制的菜单id
         :param stickMenuID：粘贴的菜单id
         :return: 
         :last_editors: HuangJingCan
         """
+        # 复制的菜单id
         copy_menu_id = self.get_param("copyMenuID")
+        # 粘贴的菜单id
         stick_menu_id = self.get_param("stickMenuID")
         if copy_menu_id == "":
             return self.response_common("SaveCopyMenuHandler", "操作失败，复制节点为空")
         if stick_menu_id == "":
             return self.response_common("SaveCopyMenuHandler", "操作失败，粘贴节点为空")
         if copy_menu_id == stick_menu_id:
             return self.response_common("SaveCopyMenuHandler", "操作失败，无法粘贴到自身节点下")
@@ -304,40 +327,41 @@
         :description: 移动菜单
         :param id：被移动的菜单id
         :param targetId：目的地菜单id
         :param moveType：移动类型
         :return: 
         :last_editors: HuangJingCan
         """
+        # 目的地菜单id
+        target_id = self.get_param("targetId")
+        # 移动类型
+        move_type = self.get_param("moveType")
+        # 被移动的菜单id
         menu_id = self.get_param("id")
         if menu_id == "":
             return self.response_common("MenuIDEmpty", "菜单ID为空")
 
         menu_info_model_ex = MenuInfoModelEx(self.get_manage_context_key())
         menu_info = menu_info_model_ex.get_entity_by_id(menu_id)
 
         if not menu_info:
             return self.response_common("NoExit", "菜单不存在")
 
-        target_id = self.get_param("targetId")
-        move_type = self.get_param("moveType")
-
         menu_info = menu_info_model_ex.get_entity_by_id(target_id)
         if menu_info and menu_info.MenuType == 1:
             return self.response_common("MoveMenuHandler", "移动失败，请勿移动到最外层")
         if menu_info and menu_info.MenuType == 3:
             return self.response_common("MoveMenuHandler", "移动失败，请勿移动到操作菜单下")
 
         if move_type == "inner":
             menu_info_model_ex.update_move(menu_id, target_id)
+        elif move_type == "after":
+            menu_info_model_ex.update_after_before_move(menu_id, target_id, "SortIndex", f"ParentID='{menu_info.ParentID}'")
         else:
-            if move_type == "after":
-                menu_info_model_ex.update_after_before_move(menu_id, target_id, "SortIndex", f"ParentID='{menu_info.ParentID}'")
-            else:
-                menu_info_model_ex.update_after_before_move(menu_id, target_id, "SortIndex", f"ParentID='{menu_info.ParentID}'", False)
+            menu_info_model_ex.update_after_before_move(menu_id, target_id, "SortIndex", f"ParentID='{menu_info.ParentID}'", False)
 
         return self.response_json_success()
 
 
 class SaveMenuCoteHandler(StudioBaseHandler):
     """
     :description: 修改栏目数据
@@ -345,27 +369,39 @@
     def post_async(self):
         """
         :description: 保存栏目数据
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 栏目数据id
         menu_cote_id = int(self.get_param("MenuCoteID", "0"))
+        # 栏目名称
         cote_title = self.get_param("CoteTitle")
+        # 栏目表名
         cote_table_name = self.get_param("CoteTableName")
+        # 主键名
         id_name = self.get_param("IDName")
+        # 显示名称
         name = self.get_param("Name")
+        # 父节点标识
         parent_id_name = self.get_param("ParentIDName")
+        # ID路经名称
         id_path_name = self.get_param("IDPathName")
+        # 链接字符串
         connection_string_name = self.get_param("ConnectionStringName")
+        # 根节点ID值
         root_id_value = self.get_param("RootIDValue")
+        # ID类型1整型2字符串
         id_data_type = int(self.get_param("IDDataType", "0"))
+        # 排序
         sort_Expression = self.get_param("SortExpression")
+        # 条件
         condtion = self.get_param("Condtion")
+        # 是否父节点链接
         is_paren_url = int(self.get_param("IsParentUrl", "0"))
 
         menu_cote_model = MenuCoteModel(self.get_manage_context_key())
         menu_cote = MenuCote()
         if menu_cote_id > 0:
             menu_cote = menu_cote_model.get_entity_by_id(menu_cote_id)
             if not menu_cote:
@@ -419,14 +455,15 @@
     def get_async(self):
         """
         :description: 
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 栏目ID
         menu_id = self.get_param("menuID")
         if menu_id == "":
             return self.response_common("MenuIDEmpty", "栏目ID为空")
 
         sql = PowerModel().export_sql(menu_id)
 
         sql_file_name = config.get_value("export_sql_folder") + "SyncSql" + TimeHelper.get_now_format_time("%Y-%m-%d") + ".sql"
```

### Comparing `seven_studio-1.1.9/seven_studio/handlers/system/power.py` & `seven_studio-1.2.0/seven_studio/handlers/system/power.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: wang kui
 :Date: 2020-03-24 16:32:52
-:LastEditTime: 2022-12-06 09:52:36
+:LastEditTime: 2023-04-10 15:18:57
 :LastEditors: HuangJingCan
 :Description: power 用户权限相关接口
 """
 from seven_studio.handlers.studio_base import *
 from seven_studio.utils.dict import *
 
 from seven_studio.models.db_models.product.product_info_model import *
@@ -32,15 +32,17 @@
         :last_editors: HuangJingCan
         """
         user_info = self.get_curr_user_info()
         curr_info = {}
         if user_info:
             curr_info["Account"] = user_info.Account
             curr_info["IsSuper"] = user_info.IsSuper
+            curr_info["UserName"] = user_info.UserName
             curr_info["NickName"] = user_info.NickName
+            curr_info["JobNo"] = user_info.JobNo
             curr_info["Avatar"] = user_info.Avatar
             curr_info["Phone"] = user_info.Phone
             curr_info["Email"] = user_info.Email
             curr_info["PersonalitySignature"] = user_info.PersonalitySignature
 
         return self.response_json_success(curr_info)
 
@@ -65,17 +67,16 @@
         product_data = []
         product_infos = []
         home_info = {"Title": "平台管理", "ImageUrl": "", "ManageUrl": "", "WebUrl": "", "ProductID": 0}
         is_super = self.get_is_super()
 
         if is_super:
             product_infos = product_info_model.get_list("IsRelease=1")
-            if product_id > 0:
-                if self.__has_home_platform_power(self.get_curr_user_info()).ResultCode == "0":
-                    product_data.append(home_info)
+            if product_id > 0 and self.__has_home_platform_power(self.get_curr_user_info()).ResultCode == "0":
+                product_data.append(home_info)
         else:
             if self.__has_home_platform_power(self.get_curr_user_info()).ResultCode == "0":
                 product_data.append(home_info)
 
             product_user_list = product_user_model.get_list("UserID=%s", params=user_id)
 
             if product_user_list:
@@ -89,15 +90,17 @@
             product_data.append(self.__to_user_product_data(user_id, product_info, is_super))
 
         return self.response_json_success(product_data)
 
     def __to_user_product_data(self, user_id, product_info, is_super):
         """
         :description: 判断该用户是否有用户管理和角色管理权限
-        :param {type} 
+        :param user_id: 用户id
+        :param product_info: 产品信息
+        :param is_super: 是否超管
         :return: 
         :last_editors: HuangJingCan
         """
         has_user_manage = False
         has_role_manage = False
         if is_super:
             has_user_manage = True
@@ -106,31 +109,30 @@
             role_user_list = RoleUserModel(product_info.ManageContextKey).get_list("UserID=%s", params=user_id)
             role_power_list = RolePowerModelEx(product_info.ManageContextKey).get_role_power_list([i.RoleID for i in role_user_list])
             if [i for i in role_power_list if i.MenuID == config.get_value("menu_id_user")]:
                 has_user_manage = True
             if [i for i in role_power_list if i.MenuID == config.get_value("menu_id_role")]:
                 has_role_manage = True
 
-        result_dict = {}
-        result_dict["Title"] = product_info.ProductName
-        result_dict["SubTitle"] = product_info.ProductSubName
-        result_dict["ImageUrl"] = product_info.ImageUrl
-        result_dict["ManageUrl"] = product_info.ManageUrl
-        result_dict["PowerUrl"] = product_info.PowerUrl
-        result_dict["ProductID"] = product_info.ProductID
-        result_dict["HasUserManage"] = has_user_manage
-        result_dict["HasRoleManage"] = has_role_manage
-        result_dict["IsBrank"] = product_info.IsBrank
-
-        return result_dict
+        return {
+            "Title": product_info.ProductName,
+            "SubTitle": product_info.ProductSubName,
+            "ImageUrl": product_info.ImageUrl,
+            "ManageUrl": product_info.ManageUrl,
+            "PowerUrl": product_info.PowerUrl,
+            "ProductID": product_info.ProductID,
+            "HasUserManage": has_user_manage,
+            "HasRoleManage": has_role_manage,
+            "IsBrank": product_info.IsBrank,
+        }
 
     def __has_home_platform_power(self, user_info):
         """
         :description: 获取该账号是否有平台管理权限
-        :param {type} 
+        :param user_info：用户信息
         :return: 
         :last_editors: HuangJingCan
         """
         invoke_result = InvokeResult()
         invoke_result.ResultCode = "AccountLock"
         invoke_result.ResultMessage = "对不起该账号没有平台管理权限"
         context_key = config.get_value("base_manage_context_key")
@@ -141,18 +143,16 @@
         if base_user_info.IsSuper == 1:
             return InvokeResult()
         role_user_list = RoleUserModel(context_key).get_list("UserID=%s", params=self.request_user_id())
         if not role_user_list:
             return invoke_result
         role_power_list = RolePowerModelEx(context_key).get_role_power_list([i.RoleID for i in role_user_list])
         role_power_info = [i for i in role_power_list if i.MenuID == config.get_value("menu_id_platform")]
-        if not role_power_info:
-            return invoke_result
 
-        return InvokeResult()
+        return InvokeResult() if role_power_info else invoke_result
 
 
 class FocusPasswordHandler(StudioBaseHandler):
     """
     :description: 强制修改密码弹窗
     """
     @login_filter(True)
@@ -180,28 +180,29 @@
     def post_async(self):
         """
         :description: 强制修改密码
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        invoke_result = InvokeResult()
+        # 密码
         password = self.get_param("password")
+
+        invoke_result = InvokeResult()
         user_info_model_ex = UserInfoModel(config.get_value("base_manage_context_key"))
         user_info_ex = UserInfoModelEx()
         base_user_info = self.get_base_user_info()
-        user_id = ""
-        if base_user_info:
-            user_id = base_user_info.UserID
 
+        user_id = base_user_info.UserID if base_user_info else ""
         is_force_password = user_info_ex.is_force_password(base_user_info)
         if not is_force_password:
             return self.response_common("Error", "无需强制更改密码")
+
         sign_password = user_info_ex.sign_password(password, user_id)
-        user_info_model_ex.update_table(f"Password=%s", "UserID=%s", [sign_password, user_id])
+        user_info_model_ex.update_table("Password=%s", "UserID=%s", [sign_password, user_id])
 
         self.logout(user_id)
 
         return self.response_custom(invoke_result)
 
 
 class ChangeCurrUserPwHandler(StudioBaseHandler):
@@ -212,27 +213,29 @@
     def post_async(self):
         """
         :description: 修改密码
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        invoke_result = InvokeResult()
+        # 旧密码
         password = self.get_param("Password")
+        # 新密码
         new_password = self.get_param("NewPassword")
+
+        invoke_result = InvokeResult()
         user_info_model_ex = UserInfoModelEx(config.get_value("base_manage_context_key"))
         base_user_info = self.get_base_user_info()
-        user_id = ""
-        if base_user_info:
-            user_id = base_user_info.UserID
 
+        user_id = base_user_info.UserID if base_user_info else ""
         if not user_info_model_ex.verify_password(password, base_user_info.Password, user_id):
             return self.response_common("ErrorPassword", "旧密码错误，请重新输入")
+
         sign_password = user_info_model_ex.sign_password(new_password, user_id)
-        user_info_model_ex.update_table(f"Password=%s", "UserID=%s", [sign_password, user_id])
+        user_info_model_ex.update_table("Password=%s", "UserID=%s", [sign_password, user_id])
 
         self.logout(user_id)
 
         return self.response_custom(invoke_result)
 
 
 class GetRoleListHandler(StudioBaseHandler):
@@ -247,18 +250,15 @@
         :return: 
         :last_editors: HuangJingCan
         """
         manage_context_key = self.get_manage_context_key()
         user_id = self.request_user_id()
         is_super = self.get_is_super()
 
-        condition = ""
-        if not is_super:
-            condition = f"ChiefUserID='{user_id}'"
-
+        condition = "" if is_super else f"ChiefUserID='{user_id}'"
         role_dict_list = RoleInfoModel(manage_context_key).get_dict_list(condition, field="RoleID,RoleName")
 
         return self.response_json_success(role_dict_list)
 
 
 class GetRoleUserListHandler(StudioBaseHandler):
     """
@@ -269,19 +269,25 @@
     def post_async(self):
         """
         :description: 角色用户列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 数据库db
         manage_context_key = self.get_manage_context_key()
+        # 用户id
         user_id = self.request_user_id()
+        # 是否超管
         is_super = self.get_is_super()
+        # 页索引
         page_index = self.get_page_index()
+        # 页大小
         page_size = self.get_page_size()
+        # 查询条件、排序字段
         condition, order = self.get_condition_by_body()
 
         page_data = PageInfo()
         role_user_dto_list = []
         role_info_model = RoleInfoModel(manage_context_key)
 
         if not is_super:
@@ -330,21 +336,28 @@
     def post_async(self):
         """
         :description: 用户角色列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 数据库db
         manage_context_key = self.get_manage_context_key()
-        product_id = config.get_value("product_id")
+        # 用户id
         user_id = self.request_user_id()
+        # 是否超管
         is_super = self.get_is_super()
+        # 页索引
         page_index = self.get_page_index()
+        # 页大小
         page_size = self.get_page_size()
+        # 查询条件、排序字段
         condition, order = self.get_condition_by_body()
+        # 产品id
+        product_id = config.get_value("product_id")
 
         page_data = PageInfo()
         user_role_dto_list = []
         user_info_model = UserInfoModel(manage_context_key)
 
         if not is_super:
             if condition:
@@ -394,26 +407,37 @@
     def post_async(self):
         """
         :description: 保存用户
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 用户id（空为新增）
         user_id = self.get_param("UserID")
+        # 账号
         account = self.get_param("Account")
+        # 密码
         password = self.get_param("Password")
+        # 电子邮箱
         email = self.get_param("Email")
+        # 用户真实名称
         user_name = self.get_param("UserName")
+        # 用户昵称
         nick_name = self.get_param("NickName")
+        # 工号
         job_no = self.get_param("JobNo")
+        # 用户电话
         phone = self.get_param("Phone")
+        # 用户头像
         avatar = self.get_param("Avatar")
+        # 用户角色列表（多个角色逗号分隔）
         user_role_id_str = self.get_param("UserRoleIdStr")
+        # 用户产品列表（多个产品逗号分隔）
         user_product_id_str = self.get_param("UserProductIdStr")
+        # 是否修改密码
         change_pw = bool(self.get_param("ChangePw", False))
 
         manage_context_key = self.get_manage_context_key()
         is_super = self.get_is_super()
         curr_user_id = self.request_user_id()
         product_id = self.request_product_id()
 
@@ -424,20 +448,19 @@
         user_info_model = UserInfoModel(self.get_manage_context_key())
         user_info = UserInfo()
         if user_id != "":
             user_info = user_info_model.get_entity_by_id(user_id)
             if not user_info:
                 return self.response_common("NoExit", "用户不存在")
             user_info_c = user_info_model.get_entity("Account=%s AND UserID!=%s", params=[account, user_id])
-            if user_info_c:
-                return self.response_common("Exit", "账号已存在")
         else:
             user_info_c = user_info_model.get_entity("Account=%s", params=account)
-            if user_info_c:
-                return self.response_common("Exit", "账号已存在")
+
+        if user_info_c:
+            return self.response_common("Exit", "账号已存在")
 
         user_info.Account = account
         user_info.Email = email
         user_info.UserName = user_name
         user_info.NickName = nick_name
         user_info.JobNo = job_no
         user_info.Phone = phone
@@ -460,20 +483,25 @@
     def post_async(self):
         """
         :description: 保存用户
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 用户id
         user_id = self.request_user_id()
+        # 电子邮箱
         email = self.get_param("Email")
+        # 用户昵称
         nick_name = self.get_param("NickName")
+        # 用户电话
         phone = self.get_param("Phone")
+        # 用户头像
         avatar = self.get_param("Avatar")
+        # 个性签名
         personality_signature = self.get_param("PersonalitySignature")
 
         user_info_model = UserInfoModel(self.get_manage_context_key())
         user_info = user_info_model.get_entity_by_id(user_id)
         if user_id == "" or not user_info:
             return self.response_common("Exit", "账号不存在")
 
@@ -500,18 +528,15 @@
         :return: 
         :last_editors: HuangJingCan
         """
         manage_context_key = self.get_manage_context_key()
         user_id = self.request_user_id()
         is_super = self.get_is_super()
 
-        condition = ""
-        if not is_super:
-            condition = f"ChiefUserID='{user_id}'"
-
+        condition = "" if is_super else f"ChiefUserID='{user_id}'"
         user_dict_list = UserInfoModel(manage_context_key).get_dict_list(condition, field="UserID,Account,UserName")
 
         return self.response_json_success(user_dict_list)
 
 
 class SaveRoleHandler(StudioBaseHandler):
     """
@@ -522,24 +547,31 @@
     def post_async(self):
         """
         :description: 修改角色
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        # 获取参数
+        # 角色id
         role_id = self.get_param("RoleID")
+        # 角色名称
         role_name = self.get_param("RoleName")
+        # 备注
         summary = self.get_param("Summary")
+        # 角色用户id
         role_user_id_str = self.get_param("RoleUserIdStr")
+        # 角色栏目id
         role_menu_id_str = self.get_param("RoleMenuIdStr")
-
+        # 数据库连接串
         manage_context_key = self.get_manage_context_key()
+        # 是否超管
         is_super = self.get_is_super()
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 产品id
         product_id = self.request_product_id()
 
         # 验证数据
         if role_name == "":
             return self.response_common("RoleNameEmpty", "角色名为空")
 
         role_info_model = RoleInfoModel(self.get_manage_context_key())
@@ -582,21 +614,27 @@
     def get_async(self):
         """
         :description: 删除用户角色
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 数据库连接串
         manage_context_key = self.get_manage_context_key()
+        # 是否超管
         is_super = self.get_is_super()
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 产品id
         product_id = self.request_product_id()
-
+        # 角色id
         role_id = self.get_param("roleID")
+        # 用户id
         user_id = self.get_param("userID")
+
         if role_id == "":
             return self.response_common("EmptyRoleID", "角色ID为空")
         if user_id == "":
             return self.response_common("EmptyUserID", "用户ID为空")
 
         power_model = PowerModel(manage_context_key, is_super, curr_user_id, product_id)
         power_model.remove_role_user(role_id, user_id)
@@ -613,14 +651,15 @@
     def get_async(self):
         """
         :description: 删除用户角色
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 角色id
         role_id = self.get_param("RoleID")
 
         if role_id == "":
             return self.response_common("EmptyRoleID", "角色ID为空")
 
         manage_context_key = self.get_manage_context_key()
 
@@ -641,19 +680,23 @@
     def get_async(self):
         """
         :description: 删除用户
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 要删除的用户id
         user_id = self.get_param("UserID")
-
+        # 数据库连接串
         manage_context_key = self.get_manage_context_key()
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 产品id
         product_id = self.request_product_id()
+        # 是否超管
         is_super = self.get_is_super()
 
         if user_id == "":
             return self.response_common("EmptyUserID", "用户ID为空")
 
         if user_id == self.request_user_id():
             return self.response_common("RemoveLimit", "当前账号不能删除")
@@ -676,25 +719,29 @@
     def get_async(self):
         """
         :description: 更新用户状态
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 用户id
         user_id = self.get_param("UserID")
+        # 是否锁定
         is_lock = int(self.get_param("IsLock", -1))
-
+        # 数据库连接串
         manage_context_key = self.get_manage_context_key()
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 是否超管
         is_super = self.get_is_super()
 
         if user_id == "":
             return self.response_json_error_params()
 
-        if is_lock != 0 and is_lock != 1:
+        if is_lock not in [0, 1]:
             return self.response_json_error_params()
 
         user_info_model = UserInfoModel(manage_context_key)
         user_info = UserInfoModel(manage_context_key).get_entity_by_id(user_id)
         if not user_info:
             return self.response_common("NoExit", "用户不存在")
 
@@ -716,18 +763,22 @@
     def get_async(self):
         """
         :description: 重置密码
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 用户id
         user_id = self.get_param("UserID")
+        # 数据库连接串
+        base_manage_context_key = config.get_value("base_manage_context_key")
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 是否超管
         is_super = self.get_is_super()
-        base_manage_context_key = config.get_value("base_manage_context_key")
 
         user_info_model = UserInfoModel(base_manage_context_key)
         user_info = UserInfoModel(base_manage_context_key).get_entity_by_id(user_id)
         if not user_info:
             return self.response_common("NoExit", "用户不存在")
 
         if not is_super and user_info.ChiefUserID != curr_user_id:
@@ -753,17 +804,20 @@
         """
         :description: 登录失败重置
         :param {type}
         :return:
         :last_editors: HuangJingCan
         """
         user_id = self.get_param("UserID")
+        # 数据库连接串
+        base_manage_context_key = config.get_value("base_manage_context_key")
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 是否超管
         is_super = self.get_is_super()
-        base_manage_context_key = config.get_value("base_manage_context_key")
 
         user_info_model = UserInfoModel(base_manage_context_key)
         user_info = UserInfoModel(base_manage_context_key).get_entity_by_id(user_id)
         if not user_info:
             return self.response_common("NoExit", "用户不存在")
 
         if not is_super and user_info.ChiefUserID != curr_user_id:
@@ -784,18 +838,22 @@
     def get_async(self):
         """
         :description: 收回权限
         :param {type}
         :return:
         :last_editors: HuangJingCan
         """
+        # 被收回权限的用户id
         user_id = self.get_param("UserID")
+        # 数据库连接串
+        manage_context_key = self.get_manage_context_key()
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 是否超管
         is_super = self.get_is_super()
-        manage_context_key = self.get_manage_context_key()
 
         role_user_model = RoleUserModel(manage_context_key)
 
         if is_super:
             role_user_model.del_entity("UserID=%s", user_id)
         else:
             user_info = role_user_model.get_entity_by_id(user_id)
@@ -815,18 +873,24 @@
     def get_async(self):
         """
         :description: 复制权限
         :param {type}
         :return:
         :last_editors: HuangJingCan
         """
+        # 复制用户id
         copy_user_id = self.get_param("copyUserID")
+        # 用户id
         user_id = self.get_param("userID")
+        # 数据库连接串
+        manage_context_key = self.get_manage_context_key()
+        # 当前用户id
         curr_user_id = self.request_user_id()
+        # 产品id
         product_id = self.request_product_id()
+        # 是否超管
         is_super = self.get_is_super()
-        manage_context_key = self.get_manage_context_key()
 
         power_model = PowerModel(manage_context_key, is_super, curr_user_id, product_id)
         power_model.copy_user_role(copy_user_id, user_id)
 
         return self.response_json_success()
```

### Comparing `seven_studio-1.1.9/seven_studio/handlers/system/product.py` & `seven_studio-1.2.0/seven_studio/handlers/system/product.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 :Author: HuangJingCan
 :Date: 2020-04-22 14:32:40
-:LastEditTime: 2022-12-06 09:46:28
+:LastEditTime: 2023-02-07 14:59:25
 :LastEditors: HuangJingCan
 :Description: 产品相关Handler
 """
 
 from seven_studio.handlers.studio_base import *
 from seven_studio.models.db_models.product.product_info_model import *
 from seven_studio.models.db_models.product.product_user_model import *
@@ -21,17 +21,21 @@
     def post_async(self):
         """
         :description: 产品列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 数据库连接串
         product_info_model = ProductInfoModel(config.get_value("base_manage_context_key"))
+        # 页索引
         page_index = self.get_page_index()
+        # 页大小
         page_size = self.get_page_size()
+        # 查询条件,排序字段
         condition, order = self.get_condition_by_body()
 
         source_dict_list = product_info_model.get_dict_list(condition, "", order)
         if len(source_dict_list) > 0:
             merge_dict_list = UserInfoModel(self.get_manage_context_key()).get_dict_list(field="UserID,UserName")
             source_dict_list = DictUtil.merge_dict_list(source_dict_list, "SuperID", merge_dict_list, "UserID", "UserID,UserName")
         page_dict = self.get_dict_page_info_list(page_index, page_size, source_dict_list)
@@ -66,29 +70,43 @@
     def post_async(self):
         """
         :description: 保存产品
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
+        # 数据库连接串
         base_manage_context_key = config.get_value("base_manage_context_key")
-        # 获取参数
+        # 产品id
         product_id = int(self.get_param("ProductID", "0"))
+        # 产品名称
         product_name = self.get_param("ProductName")
+        # 产品子名称
         product_sub_name = self.get_param("ProductSubName")
+        # 业务地址
         manage_url = self.get_param("ManageUrl")
+        # 权限地址
         power_url = self.get_param("PowerUrl")
+        # 说明
         summary = self.get_param("Summary")
+        # 图片地址
         image_url = self.get_param("ImageUrl")
+        # 超管ID
         super_id = self.get_param("SuperID")
+        # 文件上下文配置
         file_context_key = self.get_param("FileContextKey")
+        # 权限上下文配置
         manage_context_key = self.get_param("ManageContextKey")
+        # 日志上下文配置
         log_context_key = self.get_param("LogContextKey")
+        # 作业上下文配置
         plug_work_context_key = self.get_param("PlugWorkContextKey")
+        # 是否发布
         is_release = int(self.get_param("IsRelease", "0"))
+        # 是否新页面打开
         is_brank = int(self.get_param("IsBrank", "0"))
 
         # 验证数据
         if product_name == "":
             return self.response_common("ProductNameEmpty", "产品名称为空")
 
         if not config.get_value(manage_context_key):
@@ -96,19 +114,19 @@
 
         product_info_model = ProductInfoModel(base_manage_context_key)
         product_info = ProductInfo()
         if product_id > 0:
             product_info = product_info_model.get_entity_by_id(product_id)
             if not product_info:
                 return self.response_common("NoExit", "产品不存在")
-            if not manage_url == "" or not power_url == "":
+            if manage_url != "" or power_url != "":
                 product_info_c = product_info_model.get_entity("(ManageUrl=%s OR PowerUrl=%s) AND ProductID<>%s", params=[manage_url, power_url, product_id])
                 if product_info_c:
                     return self.response_common("HasExit", "WebUrl或ApiUrl已存在")
-        elif not manage_url == "" or not power_url == "":
+        elif manage_url != "" or power_url != "":
             product_info_c = product_info_model.get_entity("ManageUrl=%s OR PowerUrl=%s", params=[manage_url, power_url])
             if product_info_c:
                 return self.response_common("HasExit", "WebUrl或ApiUrl已存在")
 
         # 赋值
         product_info.ProductName = product_name
         product_info.ProductSubName = product_sub_name
```

### Comparing `seven_studio-1.1.9/seven_studio/handlers/system/settings.py` & `seven_studio-1.2.0/seven_studio/handlers/system/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,23 @@
     @login_filter(True)
     def post_async(self):
         """
         :description: 设置站点基础信息
         :return 基础信息
         :last_editors: ChenXiaolei
         """
+        # 登录页背景图
         login_background = self.get_param("login_background")
+        # 登录页logo
         login_logo = self.get_param("login_logo")
+        # 首页顶部logo
         banner_logo = self.get_param("banner_logo")
+        # 标题
         title = self.get_param("title")
+        # 登录过期时间(小时)
         login_expire = int(self.get_param("login_expire", 2))
 
         settings_base_model = SettingsBaseModel(config.get_value("manage_context_key"))
 
         settings_base = settings_base_model.get_entity()
 
         if not settings_base:
```

### Comparing `seven_studio-1.1.9/seven_studio/libs/file/bos.py` & `seven_studio-1.2.0/seven_studio/libs/file/bos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/libs/file/cos.py` & `seven_studio-1.2.0/seven_studio/libs/file/cos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/libs/file/ks3.py` & `seven_studio-1.2.0/seven_studio/libs/file/ks3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/libs/file/oss2.py` & `seven_studio-1.2.0/seven_studio/libs/file/oss2.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/libs/file/s3.py` & `seven_studio-1.2.0/seven_studio/libs/file/s3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/libs/file/upload.py` & `seven_studio-1.2.0/seven_studio/libs/file/upload.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/libs/geetest.py` & `seven_studio-1.2.0/seven_studio/libs/geetest.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/file/file_history_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/file/file_history_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/file/file_resource_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/file/file_resource_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/file/file_restrict_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/file/file_restrict_pic_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_pic_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/file/file_storage_path_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/file/file_storage_path_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/file/file_water_image_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/file/file_water_image_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/log/log_action_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/log/log_action_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/menu/menu_cote_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_cote_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/menu/menu_info_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/menu/menu_info_model_ex.py` & `seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model_ex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 :Author: HuangJingCan
 :Date: 2020-04-22 14:32:40
-:LastEditTime: 2022-12-07 09:11:59
+:LastEditTime: 2023-02-08 14:48:56
 :LastEditors: HuangJingCan
 :Description: 栏目扩展类
 """
 
 from seven_framework.uuid import *
 from seven_studio.utils.dict import *
 
 from seven_studio.models.db_models.menu.menu_info_model import *
 from seven_studio.models.enum import ButtonType
 from seven_studio.models.enum import ButtonPlace
+from seven_studio.models.seven_model import InvokeResult
 
 
 class MenuInfoDto():
     """
     :description: 自定义实体(栏目)
     :param {type} 
     :return: 
@@ -59,15 +60,15 @@
 
     def get_entity_by_menu_info(self, menu_info):
         menu_info.MenuChildID = menu_info.MenuID + ":Child"
         menu_info.ApiPathValue = "/" + menu_info.MenuID + menu_info.ApiPath
 
         view_path_find_index = menu_info.ViewPath.find("/:")
         if view_path_find_index > 0:
-            menu_info.ViewPathValue = menu_info.ViewPath[0:view_path_find_index]
+            menu_info.ViewPathValue = menu_info.ViewPath[:view_path_find_index]
         else:
             menu_info.ViewPathValue = menu_info.ViewPath
 
         menu_cote_key = "$" + menu_info.MenuCoteKey if menu_info.MenuCoteKey.strip() != "" else ""
 
         menu_info.RedirctPathValue = f"/{menu_info.MenuID}{menu_cote_key}{menu_info.ViewPathValue.lower()}"
 
@@ -85,15 +86,17 @@
     :param {type} 
     :return: 
     :last_editors: HuangJingCan
     """
     def add_fast_menu(self, parent_id, suffix_name, button_type_str):
         """
         :description: 快速添加菜单
-        :param {type} 
+        :param parent_id: 父栏目id
+        :param suffix_name: 按钮名称后缀
+        :param button_type_str: 按钮类型
         :return: 
         :last_editors: HuangJingCan
         """
         button_type_list = button_type_str.split(",")
         for button_Type in button_type_list:
             curr_button_type_enum = int(button_Type)
             curr_menu_info = MenuInfo()
@@ -216,15 +219,16 @@
         """
         self.update(menu_info)
         return DictUtil.auto_mapper(MenuInfoDto(), menu_info.__dict__)
 
     def add_copy_menu(self, copy_menu_id, stick_menu_id):
         """
         :description: 粘贴菜单
-        :param {type} 
+        :param copy_menu_id: 复制的菜单id
+        :param stick_menu_id: 黏贴的菜单id
         :return: 
         :last_editors: HuangJingCan
         """
         invoke_result = InvokeResult()
 
         menu_info_list = self.get_list(f"IDPath LIKE '%{copy_menu_id}%'")
         if not menu_info_list:
@@ -265,15 +269,17 @@
         self.add_copy_child_menu(copy_menu_id, copy_menu_info.MenuID, sub_menu_list)
 
         return invoke_result
 
     def add_copy_child_menu(self, old_parent_id, curr_parent_id, menu_info_list):
         """
         :description: 粘贴子节点
-        :param {type} 
+        :param old_parent_id: 旧父id
+        :param curr_parent_id: 当前父id
+        :param menu_info_list: 栏目id列表
         :return: 
         :last_editors: HuangJingCan
         """
         curr_menu_info_list = [i for i in menu_info_list if i.ParentID == old_parent_id]
         for curr_menu_info in curr_menu_info_list:
             curr_menu_id = curr_menu_info.MenuID
             curr_menu_info.MenuID = UUIDHelper.get_uuid()
@@ -301,32 +307,30 @@
 
         old_parent_id = move_menu_info.ParentID
         id_path = move_menu_info.IDPath
         menu_name_path = move_menu_info.MenuNamePath
         depth = move_menu_info.Depth
         menu_info_list = self.get_list(f"IDPath LIKE '{id_path}%'")
         target_menu_info = self.get_entity_by_id(target_id)
-        update_id_path = target_id + "," + move_id if not target_menu_info else target_menu_info.IDPath + move_id + ","
-        update_name_path = "," + move_menu_info.MenuName if not target_menu_info else target_menu_info.MenuNamePath + move_menu_info.MenuName + ","
-        update_depth = 1 if not target_menu_info else target_menu_info.Depth
+        update_id_path = (target_menu_info.IDPath + move_id + "," if target_menu_info else target_id + "," + move_id)
+        update_name_path = (target_menu_info.MenuNamePath + move_menu_info.MenuName + "," if target_menu_info else "," + move_menu_info.MenuName)
+        update_depth = target_menu_info.Depth if target_menu_info else 1
 
         for power_menu in menu_info_list:
             power_menu.MenuNamePath = power_menu.MenuNamePath.replace(menu_name_path, update_name_path)
             power_menu.IDPath = power_menu.IDPath.replace(id_path, update_id_path)
             power_menu.Depth = power_menu.Depth - depth + 1 + update_depth
             if power_menu.MenuID == move_id:
                 power_menu.ParentID = target_id
             self.update_entity(power_menu)
 
         self.update_table("HaveChild=1", "MenuID=%s", target_id)
 
         dict_total = self.get_total("ParentID=%s", params=old_parent_id)
-        have_child = 0
-        if dict_total and int(dict_total) > 0:
-            have_child = 1
+        have_child = 1 if dict_total and int(dict_total) > 0 else 0
         self.update_table("HaveChild=%s", "MenuID=%s", [have_child, target_id])
 
     def update_after_before_move(self, move_id, target_id, top_field_name, condition="", is_after=True):
         """
         :description: 移动
         :param move_id：被移动的菜单id
         :param target_id：目的地菜单id
@@ -395,16 +399,16 @@
         sql_list = [i for i in sql.split(";") if i != ""]
 
         return self.transaction_execute(sql_list)
 
     def get_sort_list(self, dict_list, top_field_name):
         """
         :description: 列表加工后返回id和sort的列表
-        :param dict_list：
-        :param top_field_name：
+        :param dict_list：要加工的列表
+        :param top_field_name：字段名称
         :return: 字典列表
         :last_editors: HuangJingCan
         """
         obj_list = []
         top_field_name = top_field_name.replace("`", "")
         primary_key = MenuInfo().get_primary_key()
         for dr in dict_list:
```

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/product/product_info_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/product/product_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/product/product_user_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/product/product_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/role/role_info_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/role/role_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/role/role_power_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/role/role_power_model_ex.py` & `seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/role/role_user_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/role/role_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/settings/settings_base_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/settings/settings_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/user/user_info_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/user/user_info_model_ex.py` & `seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/db_models/user/user_login_model.py` & `seven_studio-1.2.0/seven_studio/models/db_models/user/user_login_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/dto_model.py` & `seven_studio-1.2.0/seven_studio/models/dto_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/enum.py` & `seven_studio-1.2.0/seven_studio/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/models/power_model.py` & `seven_studio-1.2.0/seven_studio/models/power_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: HuangJingCan
 :Date: 2020-04-15 09:56:24
-:LastEditTime: 2021-06-30 19:46:55
+:LastEditTime: 2023-02-08 17:30:15
 :LastEditors: HuangJingCan
 :Description: 权限角色栏目相关
 """
 from asq.initiators import query
 from seven_studio.utils.dict import *
 from seven_framework.time import *
 
@@ -86,14 +86,23 @@
                 # if len(menu_list) > 0:
                 if menu_list:
                     curr_menu_item_dto.MenuItemDtoList = menu_list
             menu_item_list.append(curr_menu_item_dto.__dict__)
         return menu_item_list
 
     def __get_menu_item_dto_list(self, menu_item, child_menu_infos, hidden_power_menu_list, depth=0):
+        """
+        :description: 获取菜单数据
+        :param menu_item: 当前菜单信息
+        :param child_menu_infos: 子菜单列表
+        :param hidden_power_menu_list: 隐藏权限菜单列表
+        :param depth: 深度
+        :return: 
+        :last_editors: HuangJingCan
+        """
         menu_info_list = [i for i in child_menu_infos if i.ParentID == menu_item.MenuID]
         for menu_info in menu_info_list:
             if menu_info.MenuType == 3 and menu_info.IsShow == 1:
                 curr_menu_button_dto = PowerButtonDto()
                 curr_menu_button_dto.ID = menu_info.MenuID
                 curr_menu_button_dto.Title = menu_info.MenuName
                 curr_menu_button_dto.Icon = menu_info.MenuIcon
@@ -136,25 +145,32 @@
                 if (menu_info.MenuCoteID > 0):
                     is_power = self.is_super or menu_info.IsPower == 0
                     self.__get_power_cote_menu_item(menu_info.MenuCoteID, curr_menu_item_dto, is_power)
 
                 menu_item.MenuItemDtoList.append(curr_menu_item_dto.__dict__)
 
     def __get_power_cote_menu_item(self, coteID, curr_menu_info, is_power):
+        """
+        :description: 获取栏目菜单数据
+        :param coteID: 栏目菜单码
+        :param curr_menu_info: 当前栏目信息
+        :param is_power: 是否超管
+        :return: 
+        :last_editors: HuangJingCan
+        """
         menu_item_list = curr_menu_info.MenuItemDtoList
         curr_menu_info.MenuItemDtoList = []
-        cote_menu_info_list = []
-        menu_item_dto_list = []
         if coteID > 0:
             menu_cote = MenuCoteModel(self.db_connect_key).get_entity_by_id(coteID)
             if not menu_cote:
-                return menu_item_dto_list
+                return []
             menu_cote_list = self.__get_cote_menu_data(menu_cote)
             menu_cote_id = curr_menu_info.MenuID + "$"
 
+            cote_menu_info_list = []
             for menu_cote_item in menu_cote_list:
                 if not self.__check_menu_power(is_power, curr_menu_info.MenuID, menu_cote_item[menu_cote.IDName]):
                     continue
                 cote_menu_info = MenuInfo()
                 cote_menu_info.MenuID = menu_cote_id + str(menu_cote_item[menu_cote.IDName])
                 cote_menu_info.MenuName = menu_cote_item[menu_cote.Name]
                 cote_menu_info.ParentID = menu_cote_id + str(menu_cote_item[menu_cote.ParentIDName]) if menu_cote.ParentIDName.strip() != "" else menu_cote_id + menu_cote.RootIDValue
@@ -192,38 +208,58 @@
                     curr_menu_item_dto.MenuButtonDtoList.extend(curr_menu_info.MenuButtonDtoList)
                     if len(menu_item_list) > 1:
                         curr_menu_item_dto.MenuItemDtoList.extend(self.__to_cote_menu_list(menu_item_list, menu_info["TargetUrl"], is_power))
 
                 curr_menu_info.MenuItemDtoList.append(curr_menu_item_dto.__dict__)
 
     def __get_cote_menu_data(self, menu_cote):
+        """
+        :description: 获取栏目菜单数据
+        :param menu_cote: 栏目菜单码
+        :return: 
+        :last_editors: HuangJingCan
+        """
         field_parms = f"{menu_cote.IDName},{menu_cote.Name}"
         if menu_cote.ParentIDName.strip() != "":
             field_parms += f",{menu_cote.ParentIDName}"
         if menu_cote.IDPathName.strip() != "":
             field_parms += f",{menu_cote.IDPathName}"
 
         condition = ""
         if menu_cote.Condtion.strip() == "":
             condition = f" ORDER BY {menu_cote.SortExpression}"
         else:
             condition = f"{menu_cote.Condtion} ORDER BY {menu_cote.SortExpression}"
 
         sql = f"SELECT {field_parms} FROM {menu_cote.CoteTableName}{condition}"
-        # list_row = MySQLHelper(config.get_value(self.db_connect_key)).fetch_all_rows(sql)
-        list_row = MySQLHelper(config.get_value(menu_cote.ConnectionStringName)).fetch_all_rows(sql)
-        return list_row
+        return MySQLHelper(config.get_value(menu_cote.ConnectionStringName)).fetch_all_rows(sql)
 
     def __check_menu_power(self, is_power, menu_id, cote_id):
+        """
+        :description: 菜单权限判断
+        :param is_power: 是否超管
+        :param menu_id: 菜单id
+        :param cote_id: 栏目id
+        :return: 
+        :last_editors: HuangJingCan
+        """
         is_contains = [i for i in self.ROLE_POWERS if f"{i.MenuID}${i.CoteID}".lower() == f"{menu_id}${cote_id}".lower()]
-        if is_power == 0 and not is_contains:
-            return False
-        return True
+        return bool(is_power != 0 or is_contains)
 
     def __get_child_cote_menu_list(self, root_power_menu_list, button_menu_dto_list, menu_item, menu_info_list, is_super):
+        """
+        :description: 获取栏目菜单列表
+        :param root_power_menu_list: 根目录菜单列表
+        :param button_menu_dto_list: 按钮菜单列表
+        :param menu_item: 当前菜单
+        :param menu_info_list: 菜单信息列表
+        :param is_super: 是否超管
+        :return: 
+        :last_editors: HuangJingCan
+        """
         for curr_menu_info in [i for i in menu_info_list if i["ParentID"] == menu_item.MenuID]:
             curr_menu_item_dto = PowerMenuInfoDto()
             curr_menu_item_dto.MenuID = curr_menu_info["MenuID"]
             curr_menu_item_dto.MenuName = curr_menu_info["MenuName"]
             curr_menu_item_dto.ViewPath = curr_menu_info["ViewPathValue"]
             curr_menu_item_dto.Path = curr_menu_info["RoutePathValue"]
 
@@ -243,14 +279,23 @@
                 childInfo.MenuName = curr_menu_info["MenuName"]
                 childInfo.ViewPath = curr_menu_info["ViewPathValue"]
                 childInfo.Path = curr_menu_info["RoutePathValue"]
                 childInfo.IsHidden = True
                 curr_menu_item_dto.MenuItemDtoList.append(childInfo.__dict__)
 
     def __to_cote_menu_list(self, menu_info_list, menu_cote_key, is_super, is_hidden=False):
+        """
+        :description: 获取栏目菜单
+        :param menu_info_list: 当前菜单信息
+        :param menu_cote_key: 跳转地址
+        :param is_super: 是否超管
+        :param is_hidden: 是否隐藏
+        :return: 
+        :last_editors: HuangJingCan
+        """
         menu_item_list = menu_info_list if is_super else query(menu_info_list).where(lambda x: query(self.ROLE_POWERS).select(lambda y: y["MenuCoteID"]).contains(str(x["MenuID"]) + "$" + menu_cote_key)).to_list()
         for curr_power_menu_info_dto in menu_item_list:
             curr_power_menu_info_dto['MenuID'] = curr_power_menu_info_dto['MenuID'] + "$" + menu_cote_key
             curr_power_menu_info_dto['Path'] = "/" + curr_power_menu_info_dto['MenuID'] + curr_power_menu_info_dto['ViewPath']
 
             if is_hidden:
                 curr_power_menu_info_dto['MenuID'] = curr_power_menu_info_dto['ViewPath'] + "hidden"
@@ -267,29 +312,37 @@
                 curr_power_menu_info_dto['MenuItemDtoList'] = self.__to_cote_menu_list(curr_power_menu_info_dto['MenuItemDtoList'], menu_cote_key, is_super, is_hidden)
 
         return menu_item_list
 
     def get_menu_item_tree(self, is_load_cote_menu=True):
         """
         :description: 获取栏目树
-        :param {type} 
+        :param is_load_cote_menu: 是否加载栏目菜单
         :return: 
         :last_editors: HuangJingCan
         """
         menu_info_list = self.get_power_menu_list()
         menu_item_list = []
         for menu_info in [i for i in menu_info_list if i.MenuType == 1 and i.ParentID == ""]:
             curr_menu_dto = DictUtil.auto_mapper(MenuInfoDto(), menu_info.__dict__)
             self.__get_child_menu_item_list(curr_menu_dto, menu_info_list, is_load_cote_menu)
             if is_load_cote_menu and menu_info.MenuCoteID > 0:
                 curr_menu_dto.ChildList = self.__get_cote_menu_item(menu_info, curr_menu_dto.ChildList)
             menu_item_list.append(curr_menu_dto.__dict__)
         return menu_item_list
 
     def __get_child_menu_item_list(self, menu_item, menu_infos, is_load_cote_menu):
+        """
+        :description: 获取子菜单
+        :param menu_item: 当前菜单信息
+        :param menu_infos: 子菜单列表
+        :param is_load_cote_menu: 是否加载栏目菜单
+        :return: 
+        :last_editors: HuangJingCan
+        """
         menu_item_list = []
         for curr_menu_info in [i for i in menu_infos if i.ParentID == menu_item.MenuID]:
             curr_menu_dto = DictUtil.auto_mapper(MenuInfoDto(), curr_menu_info.__dict__)
             id_path_list = [i for i in menu_infos if curr_menu_info.MenuID in i.IDPath]
             self.__get_child_menu_item_list(curr_menu_dto, id_path_list, is_load_cote_menu)
             if is_load_cote_menu and curr_menu_info.MenuCoteID > 0:
                 curr_menu_dto.ChildList = self.__get_cote_menu_item(curr_menu_info, curr_menu_dto.ChildList)
@@ -297,14 +350,21 @@
                 curr_menu_dto.MenuID = curr_menu_dto.MenuID + "$" + curr_menu_dto.MenuCoteKey
             menu_item.ChildList.append(curr_menu_dto.__dict__)
             menu_item_list.append(menu_item)
 
         return menu_item_list
 
     def __get_cote_menu_item(self, curr_menu_info, child_menu_info_list):
+        """
+        :description: 获取栏目菜单
+        :param curr_menu_info: 当前菜单信息
+        :param child_menu_info_list: 子菜单列表
+        :return: 
+        :last_editors: HuangJingCan
+        """
         menu_item_list = []
         cote_menu_info_list = []
         if curr_menu_info.MenuCoteID > 0:
             menu_cote = MenuCoteModel(self.db_connect_key).get_entity_by_id(curr_menu_info.MenuCoteID)
             if not menu_cote:
                 return menu_item_list
 
@@ -349,27 +409,42 @@
                     curr_menu_dto.ChildList.extend(curr_child_menu_info)
 
                 menu_item_list.append(curr_menu_dto.__dict__)
 
         return menu_item_list
 
     def __revise_child_cote_menu_list(self, menu_info_dto, cote_key):
+        """
+        :description: 更改子菜单中栏目数据的MenuID和ParentID
+        :param menu_info_dto: 需要修改的菜单信息
+        :param cote_key: cote_key
+        :return: 
+        :last_editors: HuangJingCan
+        """
         if menu_info_dto['ChildList']:
             for info in menu_info_dto['ChildList']:
                 info['MenuID'] = str(info['MenuID']) + "$" + str(cote_key)
                 info['ParentID'] = str(info['ParentID']) + "$" + str(cote_key)
                 self.__revise_child_cote_menu_list(info, cote_key)
 
     def __get_child_cote_menu_item_list(self, menu_item, menu_infos, child_menu_info_list):
+        """
+        :description: 获取子菜单中栏目数据
+        :param menu_item: 当前菜单信息
+        :param menu_infos: 子菜单信息
+        :param child_menu_info_list: 子菜单列表
+        :return: 
+        :last_editors: HuangJingCan
+        """
         menu_item_list = []
         for curr_menu_info in [i for i in menu_infos if i['ParentID'] == menu_item.MenuID]:
-            curr_child_menu_info = []
             curr_menu_dto = DictUtil.auto_mapper(MenuInfoDto(), curr_menu_info)
             child_menu_list = [i for i in menu_infos if i['ParentID'] == curr_menu_info['MenuID']]
             if not child_menu_list:
+                curr_child_menu_info = []
                 for c_menu_info_dto in child_menu_info_list:
                     new_c_menu_info_dto = MenuInfoDto()
                     new_c_menu_info_dto.MenuID = str(c_menu_info_dto['MenuID']) + "$" + str(curr_menu_info['TargetUrl'])
                     new_c_menu_info_dto.MenuIcon = c_menu_info_dto['MenuIcon']
                     new_c_menu_info_dto.MenuName = c_menu_info_dto['MenuName']
                     new_c_menu_info_dto.ParentID = str(curr_menu_info['MenuID']) + "$" + str(curr_menu_info['TargetUrl'])
                     new_c_menu_info_dto.IDPath = c_menu_info_dto['IDPath']
@@ -386,57 +461,60 @@
             menu_item.ChildList.append(curr_menu_dto.__dict__)
             menu_item_list.append(menu_item.__dict__)
 
         return menu_item_list
 
     def get_power_menu_role_list(self, menu_id):
         """
-        :description: 根据栏目id获取角色和用户
-        :param menu_id：栏目id
-        :return: 角色用户列表
+        :description: 根据菜单id获取角色和用户
+        :param menu_id：菜单id
+        :return: 
         :last_editors: HuangJingCan
         """
         menu_role_list = []
         rowle_power_list = RolePowerModelEx(self.db_connect_key).get_list("MenuID=%s", params=menu_id)
         if rowle_power_list:
             role_info_list = RoleInfoModel(self.db_connect_key).get_list("RoleID IN ("+','.join("'"+str(item.RoleID)+"'" for item in rowle_power_list)+")")
             role_user_list = RoleUserModel(self.db_connect_key).get_list("RoleID IN ("+','.join("'"+str(item.RoleID)+"'" for item in rowle_power_list)+")")
             user_info_list = UserInfoModel(self.db_connect_key).get_list("UserID IN ("+','.join("'"+str(item.UserID)+"'" for item in role_user_list)+")")
             for curr_role_info in role_info_list:
                 curr_user_info_list = [i for j in [i.UserID for i in role_user_list if i.RoleID == curr_role_info.RoleID] for i in user_info_list if j in i.UserID]
-                info = {}
-                info["RoleID"] = curr_role_info.RoleID
-                info["RoleName"] = curr_role_info.RoleName
-                info["Summary"] = curr_role_info.Summary
-                curr_user_dict = []
-                for user_info in curr_user_info_list:
-                    curr_user_dict.append(user_info.__dict__)
+                info = {
+                    "RoleID": curr_role_info.RoleID,
+                    "RoleName": curr_role_info.RoleName,
+                    "Summary": curr_role_info.Summary,
+                }
+                curr_user_dict = [user_info.__dict__ for user_info in curr_user_info_list]
                 info["UserInfoList"] = curr_user_dict
                 menu_role_list.append(info)
         return menu_role_list
 
     def remove_role_user(self, role_id, user_id):
         """
         :description: 删除用户角色
-        :param {type} 
+        :param role_id: 角色id
+        :param user_id: 用户id
         :return: 
         :last_editors: HuangJingCan
         """
         role_user_model = RoleUserModel(self.db_connect_key)
         if self.is_super:
             role_user_model.del_entity("RoleID=%s and UserID=%s", [role_id, user_id])
         else:
             user_info = UserInfoModel().get_entity_by_id(user_id)
             if user_info and user_info.ChiefUserID == user_id:
                 role_user_model.del_entity("RoleID=%s and UserID=%s", [role_id, user_id])
 
     def set_role(self, role_info, user_id_list, menu_id_list, is_add=False):
         """
         :description: 设置角色
-        :param {type} 
+        :param role_info: 角色信息
+        :param user_id_list: 用户id列表
+        :param menu_id_list: 菜单id列表
+        :param is_add:是否新增
         :return: 
         :last_editors: HuangJingCan
         """
         role_info_model = RoleInfoModel(self.db_connect_key)
         user_id_list = [i for i in user_id_list if i != ""]
         menu_id_list = [i for i in menu_id_list if i != ""]
 
@@ -454,28 +532,42 @@
         result = DictUtil.auto_mapper(RoleUserDto(), role_info.__dict__)
         result.RoleUserIds = user_id_list
         result.RoleMenuIds = menu_id_list
         result.IsAdd = is_add
         return result
 
     def add_role_user(self, role_id, user_id_list):
+        """
+        :description: 添加角色用户
+        :param role_id: 角色id
+        :param user_id_list: 用户id列表
+        :return: 
+        :last_editors: HuangJingCan
+        """
         role_user_mode = RoleUserModel(self.db_connect_key)
         role_user_mode.del_entity("RoleID=%s", role_id)
         if len(user_id_list) > 0:
             role_user_list = []
             for user_id in user_id_list:
                 role_user = RoleUser()
                 role_user.RoleUserID = CryptoHelper.md5_encrypt_int(role_id + user_id)
                 role_user.UserID = user_id
                 role_user.RoleID = role_id
                 role_user.CreateDate = TimeHelper.get_now_format_time()
                 role_user_list.append(role_user)
             role_user_mode.add_list(role_user_list, True, True)
 
     def add_role_menu(self, role_id, menu_id_list):
+        """
+        :description: 添加角色菜单
+        :param role_id: 角色id
+        :param menu_id_list: 菜单id列表
+        :return: 
+        :last_editors: HuangJingCan
+        """
         role_power_mode = RolePowerModel(self.db_connect_key)
         role_power_mode.del_entity("RoleID=%s", role_id)
         if len(menu_id_list) > 0:
             role_power_list = []
             for menu_id in menu_id_list:
                 role_power = RolePower()
                 role_power.RolePowerID = CryptoHelper.md5_encrypt_int(role_id + menu_id)
@@ -488,16 +580,21 @@
                 role_power.RoleID = role_id
                 role_power_list.append(role_power)
 
             role_power_mode.add_list(role_power_list, True)
 
     def set_user(self, user_info, role_id_list, product_id_list, password, change_pw=False, is_add=False):
         """
-        :description: 
-        :param {type} 
+        :description: 设置用户信息/角色/产品
+        :param user_info: 用户信息
+        :param role_id_list: 角色id列表
+        :param product_id_list: 产品id列表
+        :param password: 密码
+        :param change_pw: 修改密码
+        :param is_add: 是否添加
         :return: 
         :last_editors: HuangJingCan
         """
         user_info_model = UserInfoModel(self.db_connect_key)
         base_user_info_model = UserInfoModel(config.get_value("base_manage_context_key"))
         role_id_list = [i for i in role_id_list if i != ""]
         product_id_list = [i for i in product_id_list if i != ""]
@@ -505,67 +602,67 @@
 
         if change_pw:
             update_field.append("Password")
         if is_add:
             base_user_info = base_user_info_model.get_entity("Account=%s", params=user_info.Account)
             if base_user_info:
                 user_info.UserID = base_user_info.UserID
-                user_info_model.add_entity(user_info, True)
             else:
                 user_info.UserID = UUIDHelper.get_uuid()
                 base_user_info_model.add_entity(user_info)
-                user_info_model.add_entity(user_info, True)
+            user_info_model.add_entity(user_info, True)
+            
             if change_pw:
                 user_info.Password = UserInfoModelEx().sign_password(password, user_info.UserID)
             else:
                 user_info.Password = UserInfoModelEx().sign_password(config.get_value("default_password"))
-            user_info_model.update_entity(user_info, field_list=update_field)
-            base_user_info_model.update_table("Password=%s", "UserID=%s", params=[user_info.Password, user_info.UserID])
-        else:
-            if change_pw:
-                user_info.Password = UserInfoModelEx().sign_password(password, user_info.UserID)
-            user_info_model.update_entity(user_info, field_list=update_field)
-            base_user_info_model.update_table("Password=%s", "UserID=%s", params=[user_info.Password, user_info.UserID])
+        elif change_pw:
+            user_info.Password = UserInfoModelEx().sign_password(password, user_info.UserID)
 
-        if len(role_id_list) > 0:
+        user_info_model.update_entity(user_info, field_list=update_field)
+        base_user_info_model.update_table("Password=%s", "UserID=%s", params=[user_info.Password, user_info.UserID])
+
+        if role_id_list:
             self.add_user_role(user_info.UserID, role_id_list)
 
-        if len(product_id_list) > 0:
+        if product_id_list:
             self.add_product_user(user_info.UserID, product_id_list)
 
         self.set_base_user(user_info)
 
         result = DictUtil.auto_mapper(UserRoleDto(), user_info.__dict__)
         result.IsAdd = is_add
         return result
 
     def add_user_role(self, user_id, role_id_list):
         """
         :description: 添加用户角色
-        :param {type} 
+        :param user_id: 用户id
+        :param role_id_list: 角色id列表
         :return: 
         :last_editors: HuangJingCan
         """
         role_user_model = RoleUserModel(self.db_connect_key)
         role_user_model.del_entity("UserID=%s", user_id)
-        if len(role_id_list) > 0:
+        if role_id_list:
             role_user_list = []
             for role_id in role_id_list:
                 role_user = RoleUser()
                 role_user.RoleUserID = CryptoHelper.md5_encrypt_int(role_id + user_id)
                 role_user.UserID = user_id
                 role_user.RoleID = role_id
                 role_user.CreateDate = TimeHelper.get_now_format_time()
                 role_user_list.append(role_user)
             role_user_model.add_list(role_user_list, True, True)
 
     def add_product_user(self, user_id, product_id_list):
         """
         :description: 添加产品用户
-        :param {type} 
+        :param user_id: 用户id
+        :param role_id_list: 产品id列表
         :return: 
         :last_editors: HuangJingCan
         """
         product_user_model = ProductUserModel(config.get_value("base_manage_context_key"))
         product_user_model.del_entity("UserID=%s", user_id)
         if len(product_id_list) > 0:
             product_user_list = []
@@ -575,15 +672,15 @@
                 product_user.ProductID = product_id
                 product_user_list.append(product_user)
             product_user_model.add_list(product_user_list, True, True)
 
     def set_base_user(self, user_info):
         """
         :description: 子产品将用户同步回主库之中
-        :param {type} 
+        :param user_info: 用户信息
         :return: 
         :last_editors: HuangJingCan
         """
         if self.product_id > 0:
             base_user_info_model = UserInfoModel(config.get_value("base_manage_context_key"), "")
             base_product_user_model = ProductUserModel(config.get_value("base_manage_context_key"), "")
 
@@ -620,15 +717,16 @@
                 sql = menu_info_model.build_data_sql(model_list)
 
         return sql
 
     def remove_user(self, curr_user_id, user_id):
         """
         :description: 删除用户
-        :param {*}
+        :param curr_user_id: 当前用户id
+        :param user_id: 用户id
         :return {*}
         :last_editors: HuangJingCan
         """
         user_info_model = UserInfoModel(self.db_connect_key)
 
         if self.is_super:
             user_info_model.del_entity("UserID=%s", user_id)
@@ -636,15 +734,16 @@
             user_info = user_info_model.get_entity_by_id(user_id)
             if user_info and user_info.ChiefUserID == curr_user_id:
                 user_info_model.del_entity("UserID=%s", user_id)
 
     def copy_user_role(self, copy_user_id, user_id):
         """
         :description: 复制权限
-        :param {*}
+        :param copy_user_id: 复制用户id
+        :param user_id: 用户id
         :return {*}
         :last_editors: HuangJingCan
         """
         role_id_list = RoleUserModel(self.db_connect_key).get_list("UserID=%s", params=copy_user_id)
         role_id_list = [i.RoleID for i in role_id_list if i != ""]
-        if len(role_id_list) > 0:
+        if role_id_list:
             self.add_user_role(user_id, role_id_list)
```

### Comparing `seven_studio-1.1.9/seven_studio/models/seven_model.py` & `seven_studio-1.2.0/seven_studio/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/route.py` & `seven_studio-1.2.0/seven_studio/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 ﻿# -*- coding: utf-8 -*-
 """
 :Author: ChenXiaolei
 :Date: 2020-04-16 14:38:22
-:LastEditTime: 2022-03-07 14:05:19
-:LastEditors: ChenXiaolei
+:LastEditTime: 2023-02-07 14:26:24
+:LastEditors: HuangJingCan
 :Description: 内容管理平台基础路由
 """
 
 # 框架引用
 from .handlers.system import *
 from seven_framework.web_tornado.monitor import *
 
+
 def seven_studio_route():
     return [
         (r"/monitor", MonitorHandler),
         # 登陆、注销
         (r"/Core/GetGeetestCode", core.GeetestCodeHandler),
         (r"/power/loginPlatform", core.LoginPlatformHandler),
         (r"/power/logout", core.LogoutHandler),
@@ -35,16 +36,15 @@
         (r"/Power/RemoveRoleUser", power.RemoveRoleUserHandler),
         (r"/Power/DeleteRole", power.DeleteRoleHandler),
         (r"/Power/DeleteUser", power.DeleteUserHandler),
         (r"/Power/ModifyUserStatus", power.ModifyUserStatusHandler),
         (r"/Power/CopyUserRole", power.CopyUserRoleHandler),
         (r"/Power/RemoveUserAllRole", power.RemoveUserAllRoleHandler),
         (r"/Power/ResetUserPassword", power.ResetUserPasswordHandler),
-        (r"/Power/ResetUserFaildLoginCount",
-         power.ResetUserFaildLoginCountHandler),
+        (r"/Power/ResetUserFaildLoginCount", power.ResetUserFaildLoginCountHandler),
         # 产品管理
         (r"/Power/GetProductList", product.GetProductListHandler),
         (r"/Power/GetAllProductList", product.GetAllProductListHandler),
         (r"/Power/SaveProduct", product.SaveProductHandler),
         (r"/Power/DeleteProduct", product.DeleteProductHandler),
         # 文件管理
         (r"/File/GetStoragePathList", file.GetStoragePathListHandler),
```

### Comparing `seven_studio-1.1.9/seven_studio/utils/dict.py` & `seven_studio-1.2.0/seven_studio/utils/dict.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio/utils/random.py` & `seven_studio-1.2.0/seven_studio/utils/random.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.1.9/seven_studio.egg-info/PKG-INFO` & `seven_studio-1.2.0/seven_studio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven-studio
-Version: 1.1.9
+Version: 1.2.0
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         
@@ -15,14 +15,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.2.0 更新内容
+        * GetUserInfoHandler增加字段返回
+        
         ### 1.1.9 更新内容
         * 基础配置更新
         * 用户登录过期处理
         
         ### 1.1.8 更新内容
         * 用户登录过期
```

### Comparing `seven_studio-1.1.9/seven_studio.egg-info/SOURCES.txt` & `seven_studio-1.2.0/seven_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

