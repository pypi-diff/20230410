# Comparing `tmp/automation_rest_server-3.6.3.tar.gz` & `tmp/automation_rest_server-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automation_rest_server-3.6.3.tar", last modified: Mon Apr 10 08:49:44 2023, max compression
+gzip compressed data, was "dist\automation_rest_server-3.6.4.tar", last modified: Mon Apr 10 10:02:29 2023, max compression
```

## Comparing `automation_rest_server-3.6.3.tar` & `automation_rest_server-3.6.4.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/
--rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/configuration/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/configuration/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/configuration/config.yaml
--rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.3/automation_rest_server/configuration/firmware_build.yaml
--rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/configuration/pci.ids
--rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/configuration/version.yaml
--rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.3/automation_rest_server/configuration/web_server.yaml
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/
--rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/models/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/models/__init__.py
--rw-rw-rw-   0        0        0     4264 2022-08-12 01:44:10.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/models/helper.py
--rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/node_resource.py
--rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/test_resource.py
--rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/web_resource.py
--rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.3/automation_rest_server/rest_client/web_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/reset_server.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/__init__.py
--rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/benchmark_resource.py
--rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/build_firmware_resource.py
--rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/git_resource.py
--rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/models/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/models/__init__.py
--rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/models/ftp_server.py
--rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/models/helper.py
--rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/oakgate_resource.py
--rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/operation_resource.py
--rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/state_resource.py
--rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/stop_flag_resource.py
--rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/test_resource.py
--rw-rw-rw-   0        0        0     1244 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/upgrade_resource.py
--rw-rw-rw-   0        0        0     5980 2023-03-06 02:10:37.000000 automation_rest_server-3.6.3/automation_rest_server/run.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/__init__.py
--rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/database.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/
--rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/__init__.py
--rw-rw-rw-   0        0        0     3039 2022-09-15 07:43:45.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/slot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/
--rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/__init__.py
--rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
--rw-rw-rw-   0        0        0     3383 2022-12-14 01:26:41.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
--rw-rw-rw-   0        0        0      608 2023-02-28 09:02:51.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
--rw-rw-rw-   0        0        0     8892 2022-09-27 01:01:15.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/
--rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/__init__.py
--rw-rw-rw-   0        0        0     2067 2022-12-13 09:26:23.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/nose_engine.py
--rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/oakgate_engine.py
--rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/perses_engine.py
--rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
--rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/special_parameter.py
--rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/sse_engine.py
--rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_build.py
--rw-rw-rw-   0        0        0     2724 2022-12-14 00:39:53.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_download.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/__init__.py
--rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
--rw-rw-rw-   0        0        0     3914 2023-04-10 08:49:21.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
--rw-rw-rw-   0        0        0     1992 2023-04-10 08:33:59.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
--rw-rw-rw-   0        0        0     1581 2022-09-27 01:01:15.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
--rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
--rw-rw-rw-   0        0        0     5467 2022-08-12 02:31:49.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/node_database.py
--rw-rw-rw-   0        0        0    10711 2023-03-31 07:34:14.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/performance_database.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/reboot_engine/
--rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/reboot_engine/__init__.py
--rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
--rw-rw-rw-   0        0        0     2052 2023-04-04 09:26:41.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/state.py
--rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/status_file.py
--rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_base.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_benchmark.py
--rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_benchmark_group.py
--rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_case.py
--rw-rw-rw-   0        0        0    21722 2023-04-04 09:26:41.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_pool.py
--rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_reboot_handle.py
--rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_result.py
--rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_runner.py
--rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/test_framework/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/
--rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/
--rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/__init__.py
--rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/buf.dll
--rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/buf.so
--rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/build.py
--rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/linux_nvme.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/
--rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/__init__.py
--rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/buf.py
--rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/ctype.py
--rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/get_feature.py
--rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/ioctl.py
--rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/nvme.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/
--rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/__init__.py
--rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/command.py
--rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/features.py
--rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/hmb.py
--rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/identify.py
--rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/log_page.py
--rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/memory.py
--rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/pcie.py
--rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/registers.py
--rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/utility_vu.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/diskpart/
--rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/diskpart/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/diskpart/diskpart.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/fio/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/fio/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/fio/fio.py
--rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/fio/fio_linux.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/fio/tool/
--rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/fio/tool/fio
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/git/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/git/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.3/automation_rest_server/tool/git/git_operator.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/tool/iometer/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/tool/iometer/__init__.py
--rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.3/automation_rest_server/tool/iometer/iometer.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server/utils/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/utils/__init__.py
--rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/utils/buf.py
--rw-rw-rw-   0        0        0     5547 2023-04-07 03:23:26.000000 automation_rest_server-3.6.3/automation_rest_server/utils/firmware_path.py
--rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/utils/log.py
--rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.3/automation_rest_server/utils/message.py
--rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/utils/nose_xml.py
--rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.3/automation_rest_server/utils/pip_operation.py
--rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/utils/process.py
--rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.3/automation_rest_server/utils/ssh.py
--rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.3/automation_rest_server/utils/system.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/automation_rest_server.egg-info/
--rw-rw-rw-   0        0        0      551 2023-04-10 08:49:43.000000 automation_rest_server-3.6.3/automation_rest_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2023-04-10 08:49:43.000000 automation_rest_server-3.6.3/automation_rest_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 08:49:43.000000 automation_rest_server-3.6.3/automation_rest_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-10 08:49:43.000000 automation_rest_server-3.6.3/automation_rest_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-04-10 08:49:43.000000 automation_rest_server-3.6.3/automation_rest_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-10 08:49:43.000000 automation_rest_server-3.6.3/automation_rest_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-04-10 08:49:44.000000 automation_rest_server-3.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-04-10 08:49:33.000000 automation_rest_server-3.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/
+-rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/config.yaml
+-rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/firmware_build.yaml
+-rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/pci.ids
+-rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/version.yaml
+-rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.4/automation_rest_server/configuration/web_server.yaml
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/
+-rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     4264 2022-08-12 01:44:10.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/helper.py
+-rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/node_resource.py
+-rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/test_resource.py
+-rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/web_resource.py
+-rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.4/automation_rest_server/rest_client/web_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/reset_server.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/__init__.py
+-rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/benchmark_resource.py
+-rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/build_firmware_resource.py
+-rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/git_resource.py
+-rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/ftp_server.py
+-rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/helper.py
+-rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/oakgate_resource.py
+-rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/operation_resource.py
+-rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/state_resource.py
+-rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/stop_flag_resource.py
+-rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/test_resource.py
+-rw-rw-rw-   0        0        0     1244 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/upgrade_resource.py
+-rw-rw-rw-   0        0        0     5980 2023-03-06 02:10:37.000000 automation_rest_server-3.6.4/automation_rest_server/run.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/__init__.py
+-rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/database.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/
+-rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/__init__.py
+-rw-rw-rw-   0        0        0     3039 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/slot.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/
+-rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/__init__.py
+-rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
+-rw-rw-rw-   0        0        0     3383 2022-12-14 01:26:41.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
+-rw-rw-rw-   0        0        0      608 2023-02-28 09:02:51.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
+-rw-rw-rw-   0        0        0     8892 2022-09-27 01:01:15.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/
+-rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/__init__.py
+-rw-rw-rw-   0        0        0     2067 2022-12-13 09:26:23.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/nose_engine.py
+-rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/oakgate_engine.py
+-rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_engine.py
+-rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/special_parameter.py
+-rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/sse_engine.py
+-rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_build.py
+-rw-rw-rw-   0        0        0     2724 2022-12-14 00:39:53.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_download.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/__init__.py
+-rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+-rw-rw-rw-   0        0        0     3914 2023-04-10 08:49:21.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
+-rw-rw-rw-   0        0        0     1992 2023-04-10 08:33:59.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
+-rw-rw-rw-   0        0        0     1581 2022-09-27 01:01:15.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
+-rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+-rw-rw-rw-   0        0        0     5467 2022-08-12 02:31:49.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/node_database.py
+-rw-rw-rw-   0        0        0    10711 2023-03-31 07:34:14.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/performance_database.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/
+-rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/__init__.py
+-rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
+-rw-rw-rw-   0        0        0     2052 2023-04-04 09:26:41.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/state.py
+-rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/status_file.py
+-rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_base.py
+-rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark.py
+-rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark_group.py
+-rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_case.py
+-rw-rw-rw-   0        0        0    21722 2023-04-04 09:26:41.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_pool.py
+-rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_reboot_handle.py
+-rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_result.py
+-rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_runner.py
+-rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/test_framework/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/
+-rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/
+-rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/__init__.py
+-rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.dll
+-rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.so
+-rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/build.py
+-rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/linux_nvme.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/
+-rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/__init__.py
+-rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/buf.py
+-rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ctype.py
+-rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/get_feature.py
+-rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ioctl.py
+-rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/nvme.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/
+-rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/__init__.py
+-rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/command.py
+-rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/features.py
+-rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/hmb.py
+-rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/identify.py
+-rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/log_page.py
+-rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/memory.py
+-rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/pcie.py
+-rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/registers.py
+-rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/utility_vu.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/
+-rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/diskpart.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio.py
+-rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio_linux.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/tool/
+-rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/fio/tool/fio
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/git/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/git/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.4/automation_rest_server/tool/git/git_operator.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/tool/iometer/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/tool/iometer/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.4/automation_rest_server/tool/iometer/iometer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/__init__.py
+-rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/buf.py
+-rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.4/automation_rest_server/utils/firmware_path.py
+-rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/log.py
+-rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.4/automation_rest_server/utils/message.py
+-rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/nose_xml.py
+-rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.4/automation_rest_server/utils/pip_operation.py
+-rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/process.py
+-rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.4/automation_rest_server/utils/ssh.py
+-rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.4/automation_rest_server/utils/system.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-10 10:02:28.000000 automation_rest_server-3.6.4/automation_rest_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-04-10 10:02:29.000000 automation_rest_server-3.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-04-10 10:02:07.000000 automation_rest_server-3.6.4/setup.py
```

### Comparing `automation_rest_server-3.6.3/LICENSE.txt` & `automation_rest_server-3.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/MANIFEST.in` & `automation_rest_server-3.6.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/PKG-INFO` & `automation_rest_server-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation_rest_server
-Version: 3.6.3
+Version: 3.6.4
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.3/automation_rest_server/configuration/config.yaml` & `automation_rest_server-3.6.4/automation_rest_server/configuration/config.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/configuration/firmware_build.yaml` & `automation_rest_server-3.6.4/automation_rest_server/configuration/firmware_build.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/configuration/pci.ids` & `automation_rest_server-3.6.4/automation_rest_server/configuration/pci.ids`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/models/helper.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/node_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/node_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_client/resource/test_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_client/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_client/web_rest_client.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_client/web_rest_client.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/reset_server.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/reset_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/benchmark_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/build_firmware_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/build_firmware_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/git_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/git_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/models/ftp_server.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/ftp_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/models/helper.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/oakgate_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/oakgate_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/operation_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/operation_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/state_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/state_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/stop_flag_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/stop_flag_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/test_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/rest_server/resource/upgrade_resource.py` & `automation_rest_server-3.6.4/automation_rest_server/rest_server/resource/upgrade_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/run.py` & `automation_rest_server-3.6.4/automation_rest_server/run.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/database.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/slot.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/nose_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/nose_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/oakgate_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/oakgate_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/perses_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/engine/sse_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/engine/sse_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_build.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_download.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/node_database.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/node_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/performance_database.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/performance_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/state.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/state.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/status_file.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/status_file.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_base.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_base.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_benchmark.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_benchmark_group.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_benchmark_group.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_case.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_case.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_pool.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_pool.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_reboot_handle.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_reboot_handle.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_result.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_result.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_runner.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_runner.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/test_framework/test_suite.py` & `automation_rest_server-3.6.4/automation_rest_server/test_framework/test_suite.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/buf.dll` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.dll`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/buf.so` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/buf.so`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/dll/build.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/dll/build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/linux_nvme.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/linux_nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/buf.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/ctype.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ctype.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/get_feature.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/get_feature.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/ioctl.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/ioctl.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/nvme.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/command.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/command.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/features.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/features.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/hmb.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/hmb.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/identify.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/identify.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/log_page.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/log_page.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/memory.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/memory.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/pcie.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/pcie.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/struct/registers.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/struct/registers.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/device/nvme/utility_vu.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/device/nvme/utility_vu.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/diskpart/diskpart.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/diskpart/diskpart.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/fio/fio.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/fio/fio_linux.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/fio/fio_linux.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/fio/tool/fio` & `automation_rest_server-3.6.4/automation_rest_server/tool/fio/tool/fio`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/git/git_operator.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/git/git_operator.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/tool/iometer/iometer.py` & `automation_rest_server-3.6.4/automation_rest_server/tool/iometer/iometer.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/buf.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/firmware_path.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/firmware_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,267 +81,273 @@
 00000500: 6d65 7465 7273 293a 0d0a 2020 2020 2020  meters):..      
 00000510: 2020 6261 7365 5f70 6174 6820 3d20 7061    base_path = pa
 00000520: 7261 6d65 7465 7273 2e67 6574 2822 6677  rameters.get("fw
 00000530: 5f70 6174 6822 2c20 2222 290d 0a20 2020  _path", "")..   
 00000540: 2020 2020 206e 616e 6420 3d20 7061 7261       nand = para
 00000550: 6d65 7465 7273 2e67 6574 2822 6e61 6e64  meters.get("nand
 00000560: 222c 2022 5256 3034 2229 0d0a 2020 2020  ", "RV04")..    
-00000570: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
-00000580: 6f73 2e6c 6973 7464 6972 2862 6173 655f  os.listdir(base_
-00000590: 7061 7468 293a 0d0a 2020 2020 2020 2020  path):..        
-000005a0: 2020 2020 6966 206e 616e 6420 696e 2069      if nand in i
-000005b0: 7465 6d20 616e 6420 6974 656d 2e65 6e64  tem and item.end
-000005c0: 7377 6974 6828 222e 6361 7022 293a 0d0a  swith(".cap"):..
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 7265 7475 726e 206f 732e 7061 7468 2e6a  return os.path.j
-000005f0: 6f69 6e28 6261 7365 5f70 6174 682c 2069  oin(base_path, i
-00000600: 7465 6d29 0d0a 0d0a 2020 2020 6465 6620  tem)....    def 
-00000610: 6765 745f 6677 5f70 6174 685f 6672 6f6d  get_fw_path_from
-00000620: 5f70 6172 616d 6574 6572 2873 656c 662c  _parameter(self,
-00000630: 2070 6172 616d 6574 6572 732c 2062 6173   parameters, bas
-00000640: 655f 7061 7468 3d22 2229 3a0d 0a20 2020  e_path=""):..   
-00000650: 2020 2020 206e 616e 6420 3d20 7061 7261       nand = para
-00000660: 6d65 7465 7273 2e67 6574 2822 6e61 6e64  meters.get("nand
-00000670: 222c 2022 4249 4353 3522 290d 0a20 2020  ", "BICS5")..   
-00000680: 2020 2020 2063 6f6d 6d69 7420 3d20 7061       commit = pa
-00000690: 7261 6d65 7465 7273 2e67 6574 2822 636f  rameters.get("co
-000006a0: 6d6d 6974 222c 2022 2229 0d0a 2020 2020  mmit", "")..    
-000006b0: 2020 2020 6677 5f70 6174 6820 3d20 7061      fw_path = pa
-000006c0: 7261 6d65 7465 7273 2e67 6574 2822 6677  rameters.get("fw
-000006d0: 5f70 6174 6822 2c20 6261 7365 5f70 6174  _path", base_pat
-000006e0: 6829 2069 6620 6261 7365 5f70 6174 6820  h) if base_path 
-000006f0: 3d3d 2022 2220 656c 7365 2062 6173 655f  == "" else base_
-00000700: 7061 7468 0d0a 2020 2020 2020 2020 6966  path..        if
-00000710: 206e 6f74 206f 732e 7061 7468 2e69 7366   not os.path.isf
-00000720: 696c 6528 6677 5f70 6174 6829 3a0d 0a20  ile(fw_path):.. 
-00000730: 2020 2020 2020 2020 2020 206c 6f67 2e49             log.I
-00000740: 4e46 4f28 2266 7720 7061 7468 207b 7d20  NFO("fw path {} 
-00000750: 636f 6d6d 6974 207b 7d20 6e61 6e64 207b  commit {} nand {
-00000760: 7d22 2e66 6f72 6d61 7428 6677 5f70 6174  }".format(fw_pat
-00000770: 682c 2063 6f6d 6d69 742c 206e 616e 6429  h, commit, nand)
-00000780: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00000790: 775f 7061 7468 203d 2073 656c 662e 6765  w_path = self.ge
-000007a0: 745f 696d 6167 655f 7061 7468 2866 775f  t_image_path(fw_
-000007b0: 7061 7468 2c20 636f 6d6d 6974 2c20 6e61  path, commit, na
-000007c0: 6e64 290d 0a20 2020 2020 2020 206c 6f67  nd)..        log
-000007d0: 2e49 4e46 4f28 2247 6574 2070 6174 6820  .INFO("Get path 
-000007e0: 6672 6f6d 2070 6172 616d 6574 6572 733a  from parameters:
-000007f0: 207b 7d22 2e66 6f72 6d61 7428 6677 5f70   {}".format(fw_p
-00000800: 6174 6829 290d 0a20 2020 2020 2020 2072  ath))..        r
-00000810: 6574 7572 6e20 6677 5f70 6174 680d 0a0d  eturn fw_path...
-00000820: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00000830: 6f64 0d0a 2020 2020 6465 6620 6765 745f  od..    def get_
-00000840: 7370 695f 7061 7468 2870 6172 616d 6574  spi_path(paramet
-00000850: 6572 7329 3a0d 0a20 2020 2020 2020 2073  ers):..        s
-00000860: 7069 203d 204e 6f6e 650d 0a20 2020 2020  pi = None..     
-00000870: 2020 2066 775f 7061 7468 203d 2070 6172     fw_path = par
-00000880: 616d 6574 6572 732e 6765 7428 2266 775f  ameters.get("fw_
-00000890: 7061 7468 222c 2022 2229 0d0a 2020 2020  path", "")..    
-000008a0: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
-000008b0: 7869 7374 7328 6677 5f70 6174 6829 3a0d  xists(fw_path):.
-000008c0: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-000008d0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-000008e0: 6469 726e 616d 6528 6677 5f70 6174 6829  dirname(fw_path)
-000008f0: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
-00000900: 6c65 2866 775f 7061 7468 2920 656c 7365  le(fw_path) else
-00000910: 2066 775f 7061 7468 0d0a 2020 2020 2020   fw_path..      
-00000920: 2020 2020 2020 6669 6c65 7320 3d20 5b0d        files = [.
-00000930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000940: 206f 732e 7061 7468 2e6a 6f69 6e28 6469   os.path.join(di
-00000950: 725f 7061 7468 2c20 6974 656d 2920 666f  r_path, item) fo
-00000960: 7220 6974 656d 2069 6e20 6f73 2e6c 6973  r item in os.lis
-00000970: 7464 6972 2864 6972 5f70 6174 6829 0d0a  tdir(dir_path)..
-00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000990: 6966 2022 5f53 5049 4150 505f 2220 696e  if "_SPIAPP_" in
-000009a0: 2069 7465 6d20 616e 6420 6974 656d 2e65   item and item.e
-000009b0: 6e64 7377 6974 6828 222e 6361 7022 290d  ndswith(".cap").
-000009c0: 0a20 2020 2020 2020 2020 2020 205d 0d0a  .            ]..
-000009d0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000009e0: 656e 2866 696c 6573 2920 3d3d 2030 3a0d  en(files) == 0:.
-000009f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a00: 206c 6f67 2e45 5252 2866 2263 616e 206e   log.ERR(f"can n
-00000a10: 6f74 2066 696e 6420 5f53 5049 4150 505f  ot find _SPIAPP_
-00000a20: 2066 696c 6520 696e 2064 6972 6563 746f   file in directo
-00000a30: 7279 3a20 7b64 6972 5f70 6174 687d 2229  ry: {dir_path}")
-00000a40: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00000a50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00000a60: 2020 2020 2073 7069 203d 2066 696c 6573       spi = files
-00000a70: 5b30 5d0d 0a20 2020 2020 2020 2072 6574  [0]..        ret
-00000a80: 7572 6e20 7370 690d 0a0d 0a20 2020 2040  urn spi....    @
-00000a90: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
-00000aa0: 2020 6465 6620 6368 616e 6765 5f70 6174    def change_pat
-00000ab0: 685f 7769 6e5f 325f 6c69 6e75 7828 7769  h_win_2_linux(wi
-00000ac0: 6e5f 7061 7468 293a 0d0a 2020 2020 2020  n_path):..      
-00000ad0: 2020 6966 2077 696e 5f70 6174 6820 6973    if win_path is
-00000ae0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00000af0: 2020 2020 2020 2020 7061 7468 5f74 656d          path_tem
-00000b00: 7020 3d20 7769 6e5f 7061 7468 2e72 6570  p = win_path.rep
-00000b10: 6c61 6365 2822 5c5c 5c5c 3137 322e 3239  lace("\\\\172.29
-00000b20: 2e31 3930 2e34 222c 2022 2f68 6f6d 6522  .190.4", "/home"
-00000b30: 290d 0a20 2020 2020 2020 2020 2020 206c  )..            l
-00000b40: 696e 7578 5f70 6174 6820 3d20 7061 7468  inux_path = path
-00000b50: 5f74 656d 702e 7265 706c 6163 6528 225c  _temp.replace("\
-00000b60: 5c22 2c20 222f 2229 0d0a 2020 2020 2020  \", "/")..      
-00000b70: 2020 2020 2020 6c6f 672e 494e 464f 2822        log.INFO("
-00000b80: 4765 7420 6c69 6e75 7820 7061 7468 3a20  Get linux path: 
-00000b90: 7b7d 222e 666f 726d 6174 286c 696e 7578  {}".format(linux
-00000ba0: 5f70 6174 6829 290d 0a20 2020 2020 2020  _path))..       
-00000bb0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00000bc0: 2020 2020 6c69 6e75 785f 7061 7468 203d      linux_path =
-00000bd0: 2022 6e6f 745f 6669 6e64 5f6c 696e 7578   "not_find_linux
-00000be0: 5f70 6174 6822 0d0a 2020 2020 2020 2020  _path"..        
-00000bf0: 7265 7475 726e 206c 696e 7578 5f70 6174  return linux_pat
-00000c00: 680d 0a0d 0a20 2020 2040 7374 6174 6963  h....    @static
-00000c10: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-00000c20: 6368 616e 6765 5f70 6174 685f 6c69 6e75  change_path_linu
-00000c30: 785f 325f 7769 6e28 6c69 6e75 785f 7061  x_2_win(linux_pa
-00000c40: 7468 293a 0d0a 2020 2020 2020 2020 6966  th):..        if
-00000c50: 206c 696e 7578 5f70 6174 6820 6973 206e   linux_path is n
-00000c60: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00000c70: 2020 2020 2020 6c69 6e75 785f 7061 7468        linux_path
-00000c80: 203d 206c 696e 7578 5f70 6174 682e 7265   = linux_path.re
-00000c90: 706c 6163 6528 222f 2f22 2c20 222f 2229  place("//", "/")
-00000ca0: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
-00000cb0: 7468 5f74 656d 7020 3d20 6c69 6e75 785f  th_temp = linux_
-00000cc0: 7061 7468 2e72 6570 6c61 6365 2822 2f68  path.replace("/h
-00000cd0: 6f6d 6522 2c20 225c 5c5c 5c31 3732 2e32  ome", "\\\\172.2
-00000ce0: 392e 3139 302e 3422 290d 0a20 2020 2020  9.190.4")..     
-00000cf0: 2020 2020 2020 2077 696e 5f70 6174 6820         win_path 
-00000d00: 3d20 7061 7468 5f74 656d 702e 7265 706c  = path_temp.repl
-00000d10: 6163 6528 222f 222c 2022 5c5c 2229 0d0a  ace("/", "\\")..
-00000d20: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
-00000d30: 494e 464f 2822 4765 7420 7769 6e20 7061  INFO("Get win pa
-00000d40: 7468 3a20 7b7d 222e 666f 726d 6174 2877  th: {}".format(w
-00000d50: 696e 5f70 6174 6829 290d 0a20 2020 2020  in_path))..     
-00000d60: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000d70: 2020 2020 2020 7769 6e5f 7061 7468 203d        win_path =
-00000d80: 2022 6e6f 745f 6669 6e64 5f77 696e 5f70   "not_find_win_p
-00000d90: 6174 6822 0d0a 2020 2020 2020 2020 7265  ath"..        re
-00000da0: 7475 726e 2077 696e 5f70 6174 680d 0a0d  turn win_path...
-00000db0: 0a20 2020 2064 6566 2067 6574 5f64 6566  .    def get_def
-00000dc0: 6175 6c74 5f62 6173 655f 7061 7468 5f65  ault_base_path_e
-00000dd0: 6e68 616e 6365 2873 656c 662c 2070 6172  nhance(self, par
-00000de0: 616d 6574 6572 7329 3a0d 0a20 2020 2020  ameters):..     
-00000df0: 2020 2069 6620 2262 6173 655f 7061 7468     if "base_path
-00000e00: 2220 696e 2070 6172 616d 6574 6572 732e  " in parameters.
-00000e10: 6b65 7973 2829 3a20 2023 2066 6f72 206f  keys():  # for o
-00000e20: 616b 6761 7465 0d0a 2020 2020 2020 2020  akgate..        
-00000e30: 2020 2020 7265 7475 726e 2070 6172 616d      return param
-00000e40: 6574 6572 735b 2262 6173 655f 7061 7468  eters["base_path
-00000e50: 225d 0d0a 2020 2020 2020 2020 6966 2022  "]..        if "
-00000e60: 6677 5f70 6174 6822 2069 6e20 7061 7261  fw_path" in para
-00000e70: 6d65 7465 7273 2e6b 6579 7328 293a 2020  meters.keys():  
-00000e80: 2023 2066 6f72 2070 6572 7365 730d 0a20   # for perses.. 
-00000e90: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00000ea0: 7061 7468 203d 2070 6172 616d 6574 6572  path = parameter
-00000eb0: 735b 2266 775f 7061 7468 225d 0d0a 2020  s["fw_path"]..  
-00000ec0: 2020 2020 2020 2020 2020 6966 2022 3137            if "17
-00000ed0: 322e 3239 2e31 3930 2e34 2220 696e 2074  2.29.190.4" in t
-00000ee0: 656d 705f 7061 7468 3a0d 0a20 2020 2020  emp_path:..     
-00000ef0: 2020 2020 2020 2020 2020 2069 6620 2277             if "w
-00000f00: 696e 2220 696e 2073 7973 2e70 6c61 7466  in" in sys.platf
-00000f10: 6f72 6d2e 6c6f 7765 7228 293a 0d0a 2020  orm.lower():..  
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 2020 6261 7365 5f70 6174 6820 3d20 7465    base_path = te
-00000f40: 6d70 5f70 6174 680d 0a20 2020 2020 2020  mp_path..       
-00000f50: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 2020 6261 7365 5f70 6174 6820 3d20      base_path = 
-00000f80: 7365 6c66 2e63 6861 6e67 655f 7061 7468  self.change_path
-00000f90: 5f77 696e 5f32 5f6c 696e 7578 2874 656d  _win_2_linux(tem
-00000fa0: 705f 7061 7468 290d 0a20 2020 2020 2020  p_path)..       
-00000fb0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000fc0: 2020 2020 2020 2020 2020 2020 6261 7365              base
-00000fd0: 5f70 6174 6820 3d20 7465 6d70 5f70 6174  _path = temp_pat
-00000fe0: 680d 0a20 2020 2020 2020 2065 6c73 653a  h..        else:
-00000ff0: 0d0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
-00001000: 7365 5f70 6174 6820 3d20 7365 6c66 2e67  se_path = self.g
-00001010: 6574 5f64 6566 6175 6c74 5f62 6173 655f  et_default_base_
-00001020: 7061 7468 2829 0d0a 2020 2020 2020 2020  path()..        
-00001030: 6c6f 672e 494e 464f 2822 4765 7420 6261  log.INFO("Get ba
-00001040: 7365 2070 6174 683a 207b 7d22 2e66 6f72  se path: {}".for
-00001050: 6d61 7428 6261 7365 5f70 6174 6829 290d  mat(base_path)).
-00001060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001070: 6261 7365 5f70 6174 680d 0a0d 0a20 2020  base_path....   
-00001080: 2064 6566 2067 656e 6572 6174 655f 6f61   def generate_oa
-00001090: 6b67 6174 655f 696d 6167 6573 2873 656c  kgate_images(sel
-000010a0: 662c 2070 6172 616d 6574 6572 7329 3a0d  f, parameters):.
-000010b0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-000010c0: 7061 726d 203d 2064 6963 7428 290d 0a20  parm = dict().. 
-000010d0: 2020 2020 2020 206e 616e 6420 3d20 7061         nand = pa
-000010e0: 7261 6d65 7465 7273 2e67 6574 2822 6e61  rameters.get("na
-000010f0: 6e64 222c 2022 414c 4c22 290d 0a20 2020  nd", "ALL")..   
-00001100: 2020 2020 2066 6f72 2069 6d61 6765 5f6b       for image_k
-00001110: 6579 2069 6e20 5b22 6261 7365 5f69 6d61  ey in ["base_ima
-00001120: 6765 222c 2022 7461 7267 6574 5f69 6d61  ge", "target_ima
-00001130: 6765 225d 3a0d 0a20 2020 2020 2020 2020  ge"]:..         
-00001140: 2020 2069 6620 696d 6167 655f 6b65 7920     if image_key 
-00001150: 696e 2070 6172 616d 6574 6572 733a 0d0a  in parameters:..
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 696d 6167 655f 7061 7468 203d 2070 6172  image_path = par
-00001180: 616d 6574 6572 732e 6765 7428 696d 6167  ameters.get(imag
-00001190: 655f 6b65 7929 0d0a 2020 2020 2020 2020  e_key)..        
-000011a0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-000011b0: 7468 2e69 7364 6972 2869 6d61 6765 5f70  th.isdir(image_p
-000011c0: 6174 6829 3a0d 0a20 2020 2020 2020 2020  ath):..         
-000011d0: 2020 2020 2020 2020 2020 2072 6574 203d             ret =
-000011e0: 2073 656c 662e 6765 745f 696d 6167 655f   self.get_image_
-000011f0: 7061 7468 2869 6d61 6765 5f70 6174 682c  path(image_path,
-00001200: 2022 222c 206e 616e 6429 0d0a 2020 2020   "", nand)..    
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 6966 2072 6574 2069 7320 6e6f 7420 4e6f  if ret is not No
-00001230: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00001240: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00001250: 7075 745f 7061 726d 5b69 6d61 6765 5f6b  put_parm[image_k
-00001260: 6579 5d20 3d20 7265 740d 0a20 2020 2020  ey] = ret..     
-00001270: 2020 2072 6574 7572 6e20 6f75 7470 7574     return output
-00001280: 5f70 6172 6d0d 0a0d 0a20 2020 2064 6566  _parm....    def
-00001290: 2075 7064 6174 655f 7065 7273 6573 5f66   update_perses_f
-000012a0: 775f 7061 7468 2873 656c 662c 2070 6172  w_path(self, par
-000012b0: 616d 6574 6572 7329 3a0d 0a20 2020 2020  ameters):..     
-000012c0: 2020 2069 6620 2266 775f 7061 7468 2220     if "fw_path" 
-000012d0: 696e 2070 6172 616d 6574 6572 732e 6b65  in parameters.ke
-000012e0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-000012f0: 2020 2069 6620 2277 696e 2220 696e 2070     if "win" in p
-00001300: 6c61 7466 6f72 6d2e 7379 7374 656d 2829  latform.system()
-00001310: 2e6c 6f77 6572 2829 3a0d 0a20 2020 2020  .lower():..     
-00001320: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00001330: 7061 7468 203d 2073 656c 662e 6368 616e  path = self.chan
-00001340: 6765 5f70 6174 685f 6c69 6e75 785f 325f  ge_path_linux_2_
-00001350: 7769 6e28 7061 7261 6d65 7465 7273 5b22  win(parameters["
-00001360: 6677 5f70 6174 6822 5d29 0d0a 2020 2020  fw_path"])..    
-00001370: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00001380: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001390: 656d 705f 7061 7468 203d 2073 656c 662e  emp_path = self.
-000013a0: 6368 616e 6765 5f70 6174 685f 7769 6e5f  change_path_win_
-000013b0: 325f 6c69 6e75 7828 7061 7261 6d65 7465  2_linux(paramete
-000013c0: 7273 5b22 6677 5f70 6174 6822 5d29 0d0a  rs["fw_path"])..
-000013d0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000013e0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-000013f0: 7061 7468 203d 2073 656c 662e 6765 745f  path = self.get_
-00001400: 6465 6661 756c 745f 6261 7365 5f70 6174  default_base_pat
-00001410: 685f 656e 6861 6e63 6528 7061 7261 6d65  h_enhance(parame
-00001420: 7465 7273 290d 0a20 2020 2020 2020 2066  ters)..        f
-00001430: 775f 7061 7468 203d 2073 656c 662e 6765  w_path = self.ge
-00001440: 745f 6677 5f70 6174 685f 6672 6f6d 5f70  t_fw_path_from_p
-00001450: 6172 616d 6574 6572 2870 6172 616d 6574  arameter(paramet
-00001460: 6572 732c 2074 656d 705f 7061 7468 290d  ers, temp_path).
-00001470: 0a20 2020 2020 2020 2069 6620 6677 5f70  .        if fw_p
-00001480: 6174 6820 6973 206e 6f74 204e 6f6e 653a  ath is not None:
-00001490: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-000014a0: 672e 494e 464f 2822 7570 6461 7465 5f70  g.INFO("update_p
-000014b0: 6572 7365 735f 6677 5f70 6174 683a 207b  erses_fw_path: {
-000014c0: 7d22 2e66 6f72 6d61 7428 6677 5f70 6174  }".format(fw_pat
-000014d0: 6829 290d 0a20 2020 2020 2020 2020 2020  h))..           
-000014e0: 2070 6172 616d 6574 6572 735b 2266 775f   parameters["fw_
-000014f0: 7061 7468 225d 203d 2066 775f 7061 7468  path"] = fw_path
-00001500: 0d0a 2020 2020 2020 2020 2020 2020 6f73  ..            os
-00001510: 2e65 6e76 6972 6f6e 5b22 6677 5f70 6174  .environ["fw_pat
-00001520: 6822 5d20 3d20 6677 5f70 6174 680d 0a20  h"] = fw_path.. 
-00001530: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00001540: 2020 2020 2020 2020 2020 6c6f 672e 5741            log.WA
-00001550: 524e 2822 4e6f 7420 6669 6e64 2070 6174  RN("Not find pat
-00001560: 683a 2070 6572 7365 735f 6677 5f70 6174  h: perses_fw_pat
-00001570: 6822 290d 0a20 2020 2020 2020 2070 7269  h")..        pri
-00001580: 6e74 2870 6172 616d 6574 6572 7329 0d0a  nt(parameters)..
-00001590: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-000015a0: 6172 616d 6574 6572 730d 0a              arameters..
+00000570: 2020 2020 6469 725f 7061 7468 203d 206f      dir_path = o
+00000580: 732e 7061 7468 2e64 6972 6e61 6d65 2862  s.path.dirname(b
+00000590: 6173 655f 7061 7468 2920 6966 206f 732e  ase_path) if os.
+000005a0: 7061 7468 2e69 7366 696c 6528 6261 7365  path.isfile(base
+000005b0: 5f70 6174 6829 2065 6c73 6520 6261 7365  _path) else base
+000005c0: 5f70 6174 680d 0a20 2020 2020 2020 2066  _path..        f
+000005d0: 6f72 2069 7465 6d20 696e 206f 732e 6c69  or item in os.li
+000005e0: 7374 6469 7228 6469 725f 7061 7468 293a  stdir(dir_path):
+000005f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000600: 206e 616e 6420 696e 2069 7465 6d20 616e   nand in item an
+00000610: 6420 6974 656d 2e65 6e64 7377 6974 6828  d item.endswith(
+00000620: 222e 6361 7022 293a 0d0a 2020 2020 2020  ".cap"):..      
+00000630: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000640: 206f 732e 7061 7468 2e6a 6f69 6e28 6469   os.path.join(di
+00000650: 725f 7061 7468 2c20 6974 656d 290d 0a0d  r_path, item)...
+00000660: 0a20 2020 2064 6566 2067 6574 5f66 775f  .    def get_fw_
+00000670: 7061 7468 5f66 726f 6d5f 7061 7261 6d65  path_from_parame
+00000680: 7465 7228 7365 6c66 2c20 7061 7261 6d65  ter(self, parame
+00000690: 7465 7273 2c20 6261 7365 5f70 6174 683d  ters, base_path=
+000006a0: 2222 293a 0d0a 2020 2020 2020 2020 6e61  ""):..        na
+000006b0: 6e64 203d 2070 6172 616d 6574 6572 732e  nd = parameters.
+000006c0: 6765 7428 226e 616e 6422 2c20 2242 4943  get("nand", "BIC
+000006d0: 5335 2229 0d0a 2020 2020 2020 2020 636f  S5")..        co
+000006e0: 6d6d 6974 203d 2070 6172 616d 6574 6572  mmit = parameter
+000006f0: 732e 6765 7428 2263 6f6d 6d69 7422 2c20  s.get("commit", 
+00000700: 2222 290d 0a20 2020 2020 2020 2066 775f  "")..        fw_
+00000710: 7061 7468 203d 2070 6172 616d 6574 6572  path = parameter
+00000720: 732e 6765 7428 2266 775f 7061 7468 222c  s.get("fw_path",
+00000730: 2062 6173 655f 7061 7468 2920 6966 2062   base_path) if b
+00000740: 6173 655f 7061 7468 203d 3d20 2222 2065  ase_path == "" e
+00000750: 6c73 6520 6261 7365 5f70 6174 680d 0a20  lse base_path.. 
+00000760: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
+00000770: 2e70 6174 682e 6973 6669 6c65 2866 775f  .path.isfile(fw_
+00000780: 7061 7468 293a 0d0a 2020 2020 2020 2020  path):..        
+00000790: 2020 2020 6c6f 672e 494e 464f 2822 6677      log.INFO("fw
+000007a0: 2070 6174 6820 7b7d 2063 6f6d 6d69 7420   path {} commit 
+000007b0: 7b7d 206e 616e 6420 7b7d 222e 666f 726d  {} nand {}".form
+000007c0: 6174 2866 775f 7061 7468 2c20 636f 6d6d  at(fw_path, comm
+000007d0: 6974 2c20 6e61 6e64 2929 0d0a 2020 2020  it, nand))..    
+000007e0: 2020 2020 2020 2020 6677 5f70 6174 6820          fw_path 
+000007f0: 3d20 7365 6c66 2e67 6574 5f69 6d61 6765  = self.get_image
+00000800: 5f70 6174 6828 6677 5f70 6174 682c 2063  _path(fw_path, c
+00000810: 6f6d 6d69 742c 206e 616e 6429 0d0a 2020  ommit, nand)..  
+00000820: 2020 2020 2020 6c6f 672e 494e 464f 2822        log.INFO("
+00000830: 4765 7420 7061 7468 2066 726f 6d20 7061  Get path from pa
+00000840: 7261 6d65 7465 7273 3a20 7b7d 222e 666f  rameters: {}".fo
+00000850: 726d 6174 2866 775f 7061 7468 2929 0d0a  rmat(fw_path))..
+00000860: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000870: 775f 7061 7468 0d0a 0d0a 2020 2020 4073  w_path....    @s
+00000880: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
+00000890: 2064 6566 2067 6574 5f73 7069 5f70 6174   def get_spi_pat
+000008a0: 6828 7061 7261 6d65 7465 7273 293a 0d0a  h(parameters):..
+000008b0: 2020 2020 2020 2020 7370 6920 3d20 4e6f          spi = No
+000008c0: 6e65 0d0a 2020 2020 2020 2020 6677 5f70  ne..        fw_p
+000008d0: 6174 6820 3d20 7061 7261 6d65 7465 7273  ath = parameters
+000008e0: 2e67 6574 2822 6677 5f70 6174 6822 2c20  .get("fw_path", 
+000008f0: 2222 290d 0a20 2020 2020 2020 2069 6620  "")..        if 
+00000900: 6f73 2e70 6174 682e 6578 6973 7473 2866  os.path.exists(f
+00000910: 775f 7061 7468 293a 0d0a 2020 2020 2020  w_path):..      
+00000920: 2020 2020 2020 6469 725f 7061 7468 203d        dir_path =
+00000930: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+00000940: 2866 775f 7061 7468 2920 6966 206f 732e  (fw_path) if os.
+00000950: 7061 7468 2e69 7366 696c 6528 6677 5f70  path.isfile(fw_p
+00000960: 6174 6829 2065 6c73 6520 6677 5f70 6174  ath) else fw_pat
+00000970: 680d 0a20 2020 2020 2020 2020 2020 2066  h..            f
+00000980: 696c 6573 203d 205b 0d0a 2020 2020 2020  iles = [..      
+00000990: 2020 2020 2020 2020 2020 6f73 2e70 6174            os.pat
+000009a0: 682e 6a6f 696e 2864 6972 5f70 6174 682c  h.join(dir_path,
+000009b0: 2069 7465 6d29 2066 6f72 2069 7465 6d20   item) for item 
+000009c0: 696e 206f 732e 6c69 7374 6469 7228 6469  in os.listdir(di
+000009d0: 725f 7061 7468 290d 0a20 2020 2020 2020  r_path)..       
+000009e0: 2020 2020 2020 2020 2069 6620 225f 5350           if "_SP
+000009f0: 4941 5050 5f22 2069 6e20 6974 656d 2061  IAPP_" in item a
+00000a00: 6e64 2069 7465 6d2e 656e 6473 7769 7468  nd item.endswith
+00000a10: 2822 2e63 6170 2229 0d0a 2020 2020 2020  (".cap")..      
+00000a20: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+00000a30: 2020 2020 2069 6620 6c65 6e28 6669 6c65       if len(file
+00000a40: 7329 203d 3d20 303a 0d0a 2020 2020 2020  s) == 0:..      
+00000a50: 2020 2020 2020 2020 2020 6c6f 672e 4552            log.ER
+00000a60: 5228 6622 6361 6e20 6e6f 7420 6669 6e64  R(f"can not find
+00000a70: 205f 5350 4941 5050 5f20 6669 6c65 2069   _SPIAPP_ file i
+00000a80: 6e20 6469 7265 6374 6f72 793a 207b 6469  n directory: {di
+00000a90: 725f 7061 7468 7d22 290d 0a20 2020 2020  r_path}")..     
+00000aa0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+00000ac0: 6920 3d20 6669 6c65 735b 305d 0d0a 2020  i = files[0]..  
+00000ad0: 2020 2020 2020 7265 7475 726e 2073 7069        return spi
+00000ae0: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+00000af0: 6574 686f 640d 0a20 2020 2064 6566 2063  ethod..    def c
+00000b00: 6861 6e67 655f 7061 7468 5f77 696e 5f32  hange_path_win_2
+00000b10: 5f6c 696e 7578 2877 696e 5f70 6174 6829  _linux(win_path)
+00000b20: 3a0d 0a20 2020 2020 2020 2069 6620 7769  :..        if wi
+00000b30: 6e5f 7061 7468 2069 7320 6e6f 7420 4e6f  n_path is not No
+00000b40: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00000b50: 2070 6174 685f 7465 6d70 203d 2077 696e   path_temp = win
+00000b60: 5f70 6174 682e 7265 706c 6163 6528 225c  _path.replace("\
+00000b70: 5c5c 5c31 3732 2e32 392e 3139 302e 3422  \\\172.29.190.4"
+00000b80: 2c20 222f 686f 6d65 2229 0d0a 2020 2020  , "/home")..    
+00000b90: 2020 2020 2020 2020 6c69 6e75 785f 7061          linux_pa
+00000ba0: 7468 203d 2070 6174 685f 7465 6d70 2e72  th = path_temp.r
+00000bb0: 6570 6c61 6365 2822 5c5c 222c 2022 2f22  eplace("\\", "/"
+00000bc0: 290d 0a20 2020 2020 2020 2020 2020 206c  )..            l
+00000bd0: 6f67 2e49 4e46 4f28 2247 6574 206c 696e  og.INFO("Get lin
+00000be0: 7578 2070 6174 683a 207b 7d22 2e66 6f72  ux path: {}".for
+00000bf0: 6d61 7428 6c69 6e75 785f 7061 7468 2929  mat(linux_path))
+00000c00: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00000c10: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
+00000c20: 7578 5f70 6174 6820 3d20 226e 6f74 5f66  ux_path = "not_f
+00000c30: 696e 645f 6c69 6e75 785f 7061 7468 220d  ind_linux_path".
+00000c40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000c50: 6c69 6e75 785f 7061 7468 0d0a 0d0a 2020  linux_path....  
+00000c60: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
+00000c70: 0a20 2020 2064 6566 2063 6861 6e67 655f  .    def change_
+00000c80: 7061 7468 5f6c 696e 7578 5f32 5f77 696e  path_linux_2_win
+00000c90: 286c 696e 7578 5f70 6174 6829 3a0d 0a20  (linux_path):.. 
+00000ca0: 2020 2020 2020 2069 6620 6c69 6e75 785f         if linux_
+00000cb0: 7061 7468 2069 7320 6e6f 7420 4e6f 6e65  path is not None
+00000cc0: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
+00000cd0: 696e 7578 5f70 6174 6820 3d20 6c69 6e75  inux_path = linu
+00000ce0: 785f 7061 7468 2e72 6570 6c61 6365 2822  x_path.replace("
+00000cf0: 2f2f 222c 2022 2f22 290d 0a20 2020 2020  //", "/")..     
+00000d00: 2020 2020 2020 2070 6174 685f 7465 6d70         path_temp
+00000d10: 203d 206c 696e 7578 5f70 6174 682e 7265   = linux_path.re
+00000d20: 706c 6163 6528 222f 686f 6d65 222c 2022  place("/home", "
+00000d30: 5c5c 5c5c 3137 322e 3239 2e31 3930 2e34  \\\\172.29.190.4
+00000d40: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00000d50: 7769 6e5f 7061 7468 203d 2070 6174 685f  win_path = path_
+00000d60: 7465 6d70 2e72 6570 6c61 6365 2822 2f22  temp.replace("/"
+00000d70: 2c20 225c 5c22 290d 0a20 2020 2020 2020  , "\\")..       
+00000d80: 2020 2020 206c 6f67 2e49 4e46 4f28 2247       log.INFO("G
+00000d90: 6574 2077 696e 2070 6174 683a 207b 7d22  et win path: {}"
+00000da0: 2e66 6f72 6d61 7428 7769 6e5f 7061 7468  .format(win_path
+00000db0: 2929 0d0a 2020 2020 2020 2020 656c 7365  ))..        else
+00000dc0: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
+00000dd0: 696e 5f70 6174 6820 3d20 226e 6f74 5f66  in_path = "not_f
+00000de0: 696e 645f 7769 6e5f 7061 7468 220d 0a20  ind_win_path".. 
+00000df0: 2020 2020 2020 2072 6574 7572 6e20 7769         return wi
+00000e00: 6e5f 7061 7468 0d0a 0d0a 2020 2020 6465  n_path....    de
+00000e10: 6620 6765 745f 6465 6661 756c 745f 6261  f get_default_ba
+00000e20: 7365 5f70 6174 685f 656e 6861 6e63 6528  se_path_enhance(
+00000e30: 7365 6c66 2c20 7061 7261 6d65 7465 7273  self, parameters
+00000e40: 293a 0d0a 2020 2020 2020 2020 6966 2022  ):..        if "
+00000e50: 6261 7365 5f70 6174 6822 2069 6e20 7061  base_path" in pa
+00000e60: 7261 6d65 7465 7273 2e6b 6579 7328 293a  rameters.keys():
+00000e70: 2020 2320 666f 7220 6f61 6b67 6174 650d    # for oakgate.
+00000e80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00000e90: 7572 6e20 7061 7261 6d65 7465 7273 5b22  urn parameters["
+00000ea0: 6261 7365 5f70 6174 6822 5d0d 0a20 2020  base_path"]..   
+00000eb0: 2020 2020 2069 6620 2266 775f 7061 7468       if "fw_path
+00000ec0: 2220 696e 2070 6172 616d 6574 6572 732e  " in parameters.
+00000ed0: 6b65 7973 2829 3a20 2020 2320 666f 7220  keys():   # for 
+00000ee0: 7065 7273 6573 0d0a 2020 2020 2020 2020  perses..        
+00000ef0: 2020 2020 7465 6d70 5f70 6174 6820 3d20      temp_path = 
+00000f00: 7061 7261 6d65 7465 7273 5b22 6677 5f70  parameters["fw_p
+00000f10: 6174 6822 5d0d 0a20 2020 2020 2020 2020  ath"]..         
+00000f20: 2020 2069 6620 2231 3732 2e32 392e 3139     if "172.29.19
+00000f30: 302e 3422 2069 6e20 7465 6d70 5f70 6174  0.4" in temp_pat
+00000f40: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
+00000f50: 2020 2020 6966 2022 7769 6e22 2069 6e20      if "win" in 
+00000f60: 7379 732e 706c 6174 666f 726d 2e6c 6f77  sys.platform.low
+00000f70: 6572 2829 3a0d 0a20 2020 2020 2020 2020  er():..         
+00000f80: 2020 2020 2020 2020 2020 2062 6173 655f             base_
+00000f90: 7061 7468 203d 2074 656d 705f 7061 7468  path = temp_path
+00000fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000fb0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000fc0: 2020 2020 2020 2020 2020 2020 2062 6173               bas
+00000fd0: 655f 7061 7468 203d 2073 656c 662e 6368  e_path = self.ch
+00000fe0: 616e 6765 5f70 6174 685f 7769 6e5f 325f  ange_path_win_2_
+00000ff0: 6c69 6e75 7828 7465 6d70 5f70 6174 6829  linux(temp_path)
+00001000: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00001010: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00001020: 2020 2020 2062 6173 655f 7061 7468 203d       base_path =
+00001030: 2074 656d 705f 7061 7468 0d0a 2020 2020   temp_path..    
+00001040: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001050: 2020 2020 2020 2062 6173 655f 7061 7468         base_path
+00001060: 203d 2073 656c 662e 6765 745f 6465 6661   = self.get_defa
+00001070: 756c 745f 6261 7365 5f70 6174 6828 290d  ult_base_path().
+00001080: 0a20 2020 2020 2020 206c 6f67 2e49 4e46  .        log.INF
+00001090: 4f28 2247 6574 2062 6173 6520 7061 7468  O("Get base path
+000010a0: 3a20 7b7d 222e 666f 726d 6174 2862 6173  : {}".format(bas
+000010b0: 655f 7061 7468 2929 0d0a 2020 2020 2020  e_path))..      
+000010c0: 2020 7265 7475 726e 2062 6173 655f 7061    return base_pa
+000010d0: 7468 0d0a 0d0a 2020 2020 6465 6620 6765  th....    def ge
+000010e0: 6e65 7261 7465 5f6f 616b 6761 7465 5f69  nerate_oakgate_i
+000010f0: 6d61 6765 7328 7365 6c66 2c20 7061 7261  mages(self, para
+00001100: 6d65 7465 7273 293a 0d0a 2020 2020 2020  meters):..      
+00001110: 2020 6f75 7470 7574 5f70 6172 6d20 3d20    output_parm = 
+00001120: 6469 6374 2829 0d0a 2020 2020 2020 2020  dict()..        
+00001130: 6e61 6e64 203d 2070 6172 616d 6574 6572  nand = parameter
+00001140: 732e 6765 7428 226e 616e 6422 2c20 2241  s.get("nand", "A
+00001150: 4c4c 2229 0d0a 2020 2020 2020 2020 666f  LL")..        fo
+00001160: 7220 696d 6167 655f 6b65 7920 696e 205b  r image_key in [
+00001170: 2262 6173 655f 696d 6167 6522 2c20 2274  "base_image", "t
+00001180: 6172 6765 745f 696d 6167 6522 5d3a 0d0a  arget_image"]:..
+00001190: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000011a0: 6d61 6765 5f6b 6579 2069 6e20 7061 7261  mage_key in para
+000011b0: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+000011c0: 2020 2020 2020 2020 2069 6d61 6765 5f70           image_p
+000011d0: 6174 6820 3d20 7061 7261 6d65 7465 7273  ath = parameters
+000011e0: 2e67 6574 2869 6d61 6765 5f6b 6579 290d  .get(image_key).
+000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001200: 2069 6620 6f73 2e70 6174 682e 6973 6469   if os.path.isdi
+00001210: 7228 696d 6167 655f 7061 7468 293a 0d0a  r(image_path):..
+00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001230: 2020 2020 7265 7420 3d20 7365 6c66 2e67      ret = self.g
+00001240: 6574 5f69 6d61 6765 5f70 6174 6828 696d  et_image_path(im
+00001250: 6167 655f 7061 7468 2c20 2222 2c20 6e61  age_path, "", na
+00001260: 6e64 290d 0a20 2020 2020 2020 2020 2020  nd)..           
+00001270: 2020 2020 2020 2020 2069 6620 7265 7420           if ret 
+00001280: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 2020 2020 2020 6f75 7470 7574 5f70 6172        output_par
+000012b0: 6d5b 696d 6167 655f 6b65 795d 203d 2072  m[image_key] = r
+000012c0: 6574 0d0a 2020 2020 2020 2020 7265 7475  et..        retu
+000012d0: 726e 206f 7574 7075 745f 7061 726d 0d0a  rn output_parm..
+000012e0: 0d0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
+000012f0: 5f70 6572 7365 735f 6677 5f70 6174 6828  _perses_fw_path(
+00001300: 7365 6c66 2c20 7061 7261 6d65 7465 7273  self, parameters
+00001310: 293a 0d0a 2020 2020 2020 2020 6966 2022  ):..        if "
+00001320: 6677 5f70 6174 6822 2069 6e20 7061 7261  fw_path" in para
+00001330: 6d65 7465 7273 2e6b 6579 7328 293a 0d0a  meters.keys():..
+00001340: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00001350: 7769 6e22 2069 6e20 706c 6174 666f 726d  win" in platform
+00001360: 2e73 7973 7465 6d28 292e 6c6f 7765 7228  .system().lower(
+00001370: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001380: 2020 2020 7465 6d70 5f70 6174 6820 3d20      temp_path = 
+00001390: 7365 6c66 2e63 6861 6e67 655f 7061 7468  self.change_path
+000013a0: 5f6c 696e 7578 5f32 5f77 696e 2870 6172  _linux_2_win(par
+000013b0: 616d 6574 6572 735b 2266 775f 7061 7468  ameters["fw_path
+000013c0: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
+000013d0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000013e0: 2020 2020 2020 2020 7465 6d70 5f70 6174          temp_pat
+000013f0: 6820 3d20 7365 6c66 2e63 6861 6e67 655f  h = self.change_
+00001400: 7061 7468 5f77 696e 5f32 5f6c 696e 7578  path_win_2_linux
+00001410: 2870 6172 616d 6574 6572 735b 2266 775f  (parameters["fw_
+00001420: 7061 7468 225d 290d 0a20 2020 2020 2020  path"])..       
+00001430: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00001440: 2020 2020 7465 6d70 5f70 6174 6820 3d20      temp_path = 
+00001450: 7365 6c66 2e67 6574 5f64 6566 6175 6c74  self.get_default
+00001460: 5f62 6173 655f 7061 7468 5f65 6e68 616e  _base_path_enhan
+00001470: 6365 2870 6172 616d 6574 6572 7329 0d0a  ce(parameters)..
+00001480: 2020 2020 2020 2020 6677 5f70 6174 6820          fw_path 
+00001490: 3d20 7365 6c66 2e67 6574 5f66 775f 7061  = self.get_fw_pa
+000014a0: 7468 5f66 726f 6d5f 7061 7261 6d65 7465  th_from_paramete
+000014b0: 7228 7061 7261 6d65 7465 7273 2c20 7465  r(parameters, te
+000014c0: 6d70 5f70 6174 6829 0d0a 2020 2020 2020  mp_path)..      
+000014d0: 2020 6966 2066 775f 7061 7468 2069 7320    if fw_path is 
+000014e0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+000014f0: 2020 2020 2020 206c 6f67 2e49 4e46 4f28         log.INFO(
+00001500: 2275 7064 6174 655f 7065 7273 6573 5f66  "update_perses_f
+00001510: 775f 7061 7468 3a20 7b7d 222e 666f 726d  w_path: {}".form
+00001520: 6174 2866 775f 7061 7468 2929 0d0a 2020  at(fw_path))..  
+00001530: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+00001540: 7465 7273 5b22 6677 5f70 6174 6822 5d20  ters["fw_path"] 
+00001550: 3d20 6677 5f70 6174 680d 0a20 2020 2020  = fw_path..     
+00001560: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
+00001570: 6e5b 2266 775f 7061 7468 225d 203d 2066  n["fw_path"] = f
+00001580: 775f 7061 7468 0d0a 2020 2020 2020 2020  w_path..        
+00001590: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000015a0: 2020 206c 6f67 2e57 4152 4e28 224e 6f74     log.WARN("Not
+000015b0: 2066 696e 6420 7061 7468 3a20 7065 7273   find path: pers
+000015c0: 6573 5f66 775f 7061 7468 2229 0d0a 2020  es_fw_path")..  
+000015d0: 2020 2020 2020 7072 696e 7428 7061 7261        print(para
+000015e0: 6d65 7465 7273 290d 0a20 2020 2020 2020  meters)..       
+000015f0: 2072 6574 7572 6e20 7061 7261 6d65 7465   return paramete
+00001600: 7273 0d0a                                rs..
```

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/log.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/log.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/nose_xml.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/nose_xml.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/pip_operation.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/pip_operation.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/process.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/process.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/ssh.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server/utils/system.py` & `automation_rest_server-3.6.4/automation_rest_server/utils/system.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/automation_rest_server.egg-info/PKG-INFO` & `automation_rest_server-3.6.4/automation_rest_server.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation-rest-server
-Version: 3.6.3
+Version: 3.6.4
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.3/automation_rest_server.egg-info/SOURCES.txt` & `automation_rest_server-3.6.4/automation_rest_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.3/setup.py` & `automation_rest_server-3.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 packages = ["automation_rest_server"]
 #python setup.py sdist upload  
 #python setup.py bdist_wheel
 
 setup(
     name = 'automation_rest_server',
-    version = '3.6.3',
+    version = '3.6.4',
     keywords = ['runner', 'server'],
     description = 'NVMe production server',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
```

