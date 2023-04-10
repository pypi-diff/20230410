# Comparing `tmp/libfwevt-python-20220925.tar.gz` & `tmp/libfwevt-python-20230410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwevt-python-20220925.tar", last modified: Thu Nov  3 08:07:14 2022, max compression
+gzip compressed data, was "libfwevt-python-20230410.tar", last modified: Mon Apr 10 14:01:08 2023, max compression
```

## Comparing `libfwevt-python-20220925.tar` & `libfwevt-python-20230410.tar`

### file list

```diff
@@ -1,641 +1,641 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2739 2022-11-03 06:28:21.000000 libfwevt-20220925/libfwevt.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libfwevt/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_provider.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt.rc.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_document.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_notify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1689 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5591 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2022-11-03 06:32:42.000000 libfwevt-20220925/libfwevt/libfwevt.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2011 2022-07-24 08:18:24.000000 libfwevt-20220925/libfwevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_token.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_event.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_level.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)   168398 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_document.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9032 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_tag.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8950 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_task.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_template_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_support.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_event.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_keyword.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_extern.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_keyword.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_libcdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8481 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_opcode.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8232 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5589 2022-11-03 06:32:42.000000 libfwevt-20220925/libfwevt/libfwevt_definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_task.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_manifest.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_channel.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2645 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_template_value.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_libfvalue.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_manifest.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_opcode.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_provider.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33211 2022-11-03 06:32:30.000000 libfwevt-20220925/libfwevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36400 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_template.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   151450 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_tag.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9577 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/fwevt_template.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_xml_token.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8352 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_level.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_libfguid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2022-11-03 06:31:56.000000 libfwevt-20220925/libfwevt/libfwevt_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3882 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_template.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9050 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_support.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2022-11-03 06:28:24.000000 libfwevt-20220925/libfwevt/libfwevt_map.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:11.000000 libfwevt-20220925/common/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-11-03 06:28:23.000000 libfwevt-20220925/common/config_msc.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2022-11-03 06:28:23.000000 libfwevt-20220925/common/byte_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2022-11-03 06:28:23.000000 libfwevt-20220925/common/common.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2022-11-03 06:28:23.000000 libfwevt-20220925/common/system_string.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2022-11-03 06:28:20.000000 libfwevt-20220925/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7235 2022-11-03 06:32:42.000000 libfwevt-20220925/common/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7236 2022-11-03 06:28:23.000000 libfwevt-20220925/common/types.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2243 2022-11-03 06:28:23.000000 libfwevt-20220925/common/config_winapi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2022-11-03 06:28:23.000000 libfwevt-20220925/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12255 2022-11-03 06:32:42.000000 libfwevt-20220925/common/config.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2022-11-03 06:28:23.000000 libfwevt-20220925/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22039 2022-11-03 06:32:30.000000 libfwevt-20220925/common/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2022-11-03 06:28:23.000000 libfwevt-20220925/common/file_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2022-11-03 06:28:23.000000 libfwevt-20220925/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11564 2022-11-03 06:32:30.000000 libfwevt-20220925/common/config.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2022-11-03 06:28:23.000000 libfwevt-20220925/common/wide_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26439 2022-11-03 06:32:30.000000 libfwevt-20220925/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2022-11-03 06:32:10.000000 libfwevt-20220925/libfguid/libfguid_extern.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   422667 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_xml_document.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3901 2022-11-03 06:31:56.000000 libfwevt-20220925/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31728 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_template.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_libfwevt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_macros.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3431 2022-11-03 06:31:56.000000 libfwevt-20220925/tests/test_python_module.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5346 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11335 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11198 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_opcode.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11439 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_keyword.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2074 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89615 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15846 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_event.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71222 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_xml_tag.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1645 2022-11-03 06:28:24.000000 libfwevt-20220925/tests/test_manpage.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6064 2022-11-03 06:31:56.000000 libfwevt-20220925/tests/pyfwevt_test_manifest.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11384 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9238 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_xml_token.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20972 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10785 2022-11-03 06:31:56.000000 libfwevt-20220925/tests/pyfwevt_test_provider.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37784 2022-11-03 06:28:24.000000 libfwevt-20220925/tests/test_runner.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/pyfwevt_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55507 2022-11-03 06:32:31.000000 libfwevt-20220925/tests/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10018 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_map.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2022-11-03 06:28:25.000000 libfwevt-20220925/tests/fwevt_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20604 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_xml_template_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11188 2022-11-03 06:31:28.000000 libfwevt-20220925/tests/fwevt_test_level.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2022-11-03 06:32:30.000000 libfwevt-20220925/missing
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2590 2022-04-26 06:03:46.000000 libfwevt-20220925/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55818 2022-11-03 06:32:27.000000 libfwevt-20220925/aclocal.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2022-11-03 06:28:21.000000 libfwevt-20220925/COPYING
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      308 2022-11-03 06:28:21.000000 libfwevt-20220925/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:11.000000 libfwevt-20220925/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:11.000000 libfwevt-20220925/include/libfwevt/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5106 2022-11-03 06:28:23.000000 libfwevt-20220925/include/libfwevt/definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2022-11-03 06:28:23.000000 libfwevt-20220925/include/libfwevt/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5265 2022-11-03 06:32:42.000000 libfwevt-20220925/include/libfwevt/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-11-03 06:31:56.000000 libfwevt-20220925/include/libfwevt/features.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5396 2022-11-03 06:28:23.000000 libfwevt-20220925/include/libfwevt/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-11-03 06:32:42.000000 libfwevt-20220925/include/libfwevt/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5104 2022-11-03 06:32:42.000000 libfwevt-20220925/include/libfwevt/definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2022-11-03 06:28:23.000000 libfwevt-20220925/include/libfwevt/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      471 2022-11-03 06:28:21.000000 libfwevt-20220925/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24555 2022-11-03 06:32:42.000000 libfwevt-20220925/include/libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25017 2022-11-03 06:32:30.000000 libfwevt-20220925/include/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    24555 2022-11-03 06:28:23.000000 libfwevt-20220925/include/libfwevt.h.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2022-11-03 06:32:30.000000 libfwevt-20220925/install-sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/pyfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_map.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5826 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_template.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_integer.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_channels.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2391 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_tasks.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2506 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_manifest.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2022-07-24 05:32:44.000000 libfwevt-20220925/pyfwevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5543 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_level.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_libfwevt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_levels.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1800 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9328 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_events.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9926 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_channel.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2096 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_event.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_opcode.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14318 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_keywords.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_providers.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10708 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_task.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_maps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9390 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_opcodes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5566 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9206 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_maps.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2022-11-03 06:31:28.000000 libfwevt-20220925/pyfwevt/pyfwevt_templates.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62291 2022-11-03 06:32:31.000000 libfwevt-20220925/pyfwevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_keyword.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_providers.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_opcode.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2901 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50707 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2433 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_opcodes.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_tasks.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9236 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_levels.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_provider.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_events.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_channels.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_level.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2022-11-03 06:31:27.000000 libfwevt-20220925/pyfwevt/pyfwevt_keywords.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2022-11-03 06:31:28.000000 libfwevt-20220925/pyfwevt/pyfwevt_templates.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2022-11-03 06:28:24.000000 libfwevt-20220925/pyfwevt/pyfwevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2022-11-03 06:32:30.000000 libfwevt-20220925/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:11.000000 libfwevt-20220925/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      121 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2022-11-03 06:32:42.000000 libfwevt-20220925/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/libfwevt-python3.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2022-11-03 06:28:25.000000 libfwevt-20220925/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:11.000000 libfwevt-20220925/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/source/format
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/rules
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/libfwevt.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2022-11-03 06:28:21.000000 libfwevt-20220925/dpkg/libfwevt-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29610 2022-11-03 06:32:30.000000 libfwevt-20220925/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2022-11-03 06:32:09.000000 libfwevt-20220925/libfdatetime/libfdatetime_filetime.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/pyfwevt-python2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1965 2022-11-03 06:28:22.000000 libfwevt-20220925/pyfwevt-python2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62166 2022-11-03 06:32:31.000000 libfwevt-20220925/pyfwevt-python2/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29849 2022-11-03 06:32:30.000000 libfwevt-20220925/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2022-11-03 06:32:07.000000 libfwevt-20220925/libcthreads/libcthreads_queue.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-11-03 06:28:23.000000 libfwevt-20220925/AUTHORS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2022-11-03 06:32:30.000000 libfwevt-20220925/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      132 2016-02-02 07:37:21.000000 libfwevt-20220925/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22240 2022-11-03 06:32:31.000000 libfwevt-20220925/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11783 2022-11-03 06:31:56.000000 libfwevt-20220925/manuals/libfwevt.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-11 04:25:12.000000 libfwevt-20220925/ABOUT-NLS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8769 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libfwevt/libfwevt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5157 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_support/fwevt_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libfguid/libfguid.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1223 2022-11-03 06:31:56.000000 libfwevt-20220925/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_provider/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_manifest/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_template/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_template/fwevt_test_template.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_tag/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5568 2022-11-03 06:31:56.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_level/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_level/fwevt_test_level.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/pyfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8480 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/pyfwevt/pyfwevt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5151 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_error/fwevt_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_template_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5436 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_map/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_map/fwevt_test_map.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_event/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_event/fwevt_test_event.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_document/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2022-11-03 06:31:56.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_channel/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libuna/libuna.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_token/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20218 2022-11-03 06:32:31.000000 libfwevt-20220925/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_opcode/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_keyword/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19630 2022-11-03 06:31:56.000000 libfwevt-20220925/msvscpp/libfwevt.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/msvscpp/fwevt_test_task/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5394 2022-11-03 06:28:39.000000 libfwevt-20220925/msvscpp/fwevt_test_task/fwevt_test_task.vcproj
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    10199 2022-11-03 06:28:39.000000 libfwevt-20220925/setup.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2022-11-03 06:32:30.000000 libfwevt-20220925/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2022-11-03 06:32:42.000000 libfwevt-20220925/libfwevt.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 06:28:21.000000 libfwevt-20220925/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/ossfuzz/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      868 2021-11-20 11:04:16.000000 libfwevt-20220925/ossfuzz/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      972 2022-11-03 06:28:24.000000 libfwevt-20220925/ossfuzz/ossfuzz_libfwevt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2022-11-03 06:28:24.000000 libfwevt-20220925/ossfuzz/manifest_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29873 2022-11-03 06:32:31.000000 libfwevt-20220925/ossfuzz/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2022-11-03 06:28:24.000000 libfwevt-20220925/ossfuzz/xml_document_fuzzer.cc
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2022-11-03 06:32:31.000000 libfwevt-20220925/test-driver
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1559321 2022-11-03 06:32:29.000000 libfwevt-20220925/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50561 2022-11-03 06:32:31.000000 libfwevt-20220925/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2022-11-03 06:32:19.000000 libfwevt-20220925/libuna/libuna_codepage_iso_8859_16.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2876 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84540 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6272 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32274 2022-11-03 06:32:30.000000 libfwevt-20220925/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2022-11-03 06:32:15.000000 libfwevt-20220925/libfvalue/libfvalue_definitions.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/pyfwevt-python3/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1965 2022-11-03 06:28:22.000000 libfwevt-20220925/pyfwevt-python3/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62166 2022-11-03 06:32:31.000000 libfwevt-20220925/pyfwevt-python3/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38224 2022-11-03 06:32:30.000000 libfwevt-20220925/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      425 2021-12-03 05:42:29.000000 libfwevt-20220925/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:11.000000 libfwevt-20220925/m4/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-11-18 19:42:05.000000 libfwevt-20220925/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/gettext.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-08-27 05:06:23.000000 libfwevt-20220925/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2022-11-03 06:32:25.000000 libfwevt-20220925/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/lib-ld.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-09-06 03:53:36.000000 libfwevt-20220925/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-11-18 20:24:51.000000 libfwevt-20220925/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2022-11-03 06:32:25.000000 libfwevt-20220925/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/nls.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-09-06 03:53:36.000000 libfwevt-20220925/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/host-cpu-c-abi.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-09-06 03:53:36.000000 libfwevt-20220925/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2022-11-03 06:32:25.000000 libfwevt-20220925/m4/ltversion.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16825 2022-04-26 06:02:48.000000 libfwevt-20220925/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2022-11-03 06:32:25.000000 libfwevt-20220925/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/po.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2014-09-28 19:03:26.000000 libfwevt-20220925/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-12-27 06:01:12.000000 libfwevt-20220925/m4/common.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-09-06 03:53:36.000000 libfwevt-20220925/m4/libcerror.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-09-06 03:53:36.000000 libfwevt-20220925/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2022-11-03 06:32:25.000000 libfwevt-20220925/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-11 04:25:12.000000 libfwevt-20220925/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-07-30 20:03:40.000000 libfwevt-20220925/m4/types.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2020-08-27 05:06:23.000000 libfwevt-20220925/m4/libfvalue.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2022-11-03 06:28:21.000000 libfwevt-20220925/COPYING.LESSER
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26384 2022-11-03 06:32:30.000000 libfwevt-20220925/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2022-11-03 06:32:04.000000 libfwevt-20220925/libcerror/libcerror_system.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26871 2022-11-03 06:32:30.000000 libfwevt-20220925/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2022-11-03 06:32:06.000000 libfwevt-20220925/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2022-11-03 06:32:25.000000 libfwevt-20220925/ltmain.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2022-11-03 06:32:30.000000 libfwevt-20220925/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-11 04:25:12.000000 libfwevt-20220925/config.rpath
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2022-11-03 06:32:31.000000 libfwevt-20220925/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:13.000000 libfwevt-20220925/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-11 04:25:12.000000 libfwevt-20220925/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-11 04:25:12.000000 libfwevt-20220925/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2014-09-28 18:22:12.000000 libfwevt-20220925/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-11 04:25:12.000000 libfwevt-20220925/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2014-09-28 18:22:12.000000 libfwevt-20220925/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-04 13:53:58.000000 libfwevt-20220925/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-11 04:25:12.000000 libfwevt-20220925/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2014-09-28 18:22:12.000000 libfwevt-20220925/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1810 2022-11-03 06:32:42.000000 libfwevt-20220925/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-11 04:25:12.000000 libfwevt-20220925/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-11 04:25:12.000000 libfwevt-20220925/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2014-09-28 18:22:12.000000 libfwevt-20220925/po/boldquot.sed
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-11-03 08:07:12.000000 libfwevt-20220925/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65251 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5714 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29443 2022-11-03 06:32:30.000000 libfwevt-20220925/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2022-11-03 06:32:03.000000 libfwevt-20220925/libcdata/libcdata_btree.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      759 2022-11-03 06:28:21.000000 libfwevt-20220925/acinclude.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      536 2022-11-03 06:28:20.000000 libfwevt-20220925/libfwevt.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5466 2022-11-03 06:31:56.000000 libfwevt-20220925/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      443 2022-11-03 08:07:14.113339 libfwevt-20220925/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2739 2023-04-10 13:32:40.000000 libfwevt-20230410/libfwevt.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:04.000000 libfwevt-20230410/libfwevt/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_provider.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt.rc.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_document.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_notify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1689 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5591 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2023-04-10 13:45:27.000000 libfwevt-20230410/libfwevt/libfwevt.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2011 2022-07-24 08:18:24.000000 libfwevt-20230410/libfwevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_token.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_event.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_level.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)   168398 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_document.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9032 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_tag.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8950 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_task.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_template_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_support.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_event.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_keyword.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_extern.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_keyword.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_libcdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8481 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_opcode.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8232 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5589 2023-04-10 13:45:27.000000 libfwevt-20230410/libfwevt/libfwevt_definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_task.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_manifest.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_channel.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2645 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_template_value.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_libfvalue.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_manifest.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_opcode.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_provider.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33211 2023-04-10 13:45:18.000000 libfwevt-20230410/libfwevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36400 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_template.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   151450 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_tag.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9577 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/fwevt_template.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_xml_token.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8352 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_level.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_libfguid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3882 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_template.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9050 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_support.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2023-04-10 13:32:43.000000 libfwevt-20230410/libfwevt/libfwevt_map.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/common/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-04-10 13:32:43.000000 libfwevt-20230410/common/config_msc.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-04-10 13:32:43.000000 libfwevt-20230410/common/byte_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-04-10 13:32:43.000000 libfwevt-20230410/common/common.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-04-10 13:32:43.000000 libfwevt-20230410/common/system_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-04-10 13:32:40.000000 libfwevt-20230410/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2023-04-10 13:45:27.000000 libfwevt-20230410/common/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-04-10 13:32:43.000000 libfwevt-20230410/common/types.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-04-10 13:32:43.000000 libfwevt-20230410/common/config_winapi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-04-10 13:32:43.000000 libfwevt-20230410/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12255 2023-04-10 13:45:27.000000 libfwevt-20230410/common/config.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-04-10 13:32:43.000000 libfwevt-20230410/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22039 2023-04-10 13:45:17.000000 libfwevt-20230410/common/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-04-10 13:32:43.000000 libfwevt-20230410/common/file_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-04-10 13:32:43.000000 libfwevt-20230410/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11564 2023-04-10 13:45:17.000000 libfwevt-20230410/common/config.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-04-10 13:32:43.000000 libfwevt-20230410/common/wide_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:00.000000 libfwevt-20230410/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26439 2023-04-10 13:45:17.000000 libfwevt-20230410/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-10 13:45:04.000000 libfwevt-20230410/libfguid/libfguid_extern.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:06.000000 libfwevt-20230410/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   422667 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_xml_document.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3901 2023-04-10 13:33:36.000000 libfwevt-20230410/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31728 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_template.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_libfwevt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_macros.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3431 2023-04-10 13:33:36.000000 libfwevt-20230410/tests/test_python_module.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5346 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11335 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11198 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_opcode.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11439 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_keyword.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2074 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89615 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15846 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_event.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71222 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_xml_tag.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1645 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/test_manpage.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6064 2023-04-10 13:33:36.000000 libfwevt-20230410/tests/pyfwevt_test_manifest.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11384 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9238 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_xml_token.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20972 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10785 2023-04-10 13:33:36.000000 libfwevt-20230410/tests/pyfwevt_test_provider.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37784 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/test_runner.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/pyfwevt_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55507 2023-04-10 13:45:18.000000 libfwevt-20230410/tests/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10018 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_map.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2023-04-10 13:32:44.000000 libfwevt-20230410/tests/fwevt_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20604 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_xml_template_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11188 2023-04-10 13:33:21.000000 libfwevt-20230410/tests/fwevt_test_level.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-04-10 13:45:17.000000 libfwevt-20230410/missing
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2590 2022-04-26 06:03:46.000000 libfwevt-20230410/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55818 2023-04-10 13:45:15.000000 libfwevt-20230410/aclocal.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-04-10 13:32:40.000000 libfwevt-20230410/COPYING
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      308 2023-04-10 13:32:40.000000 libfwevt-20230410/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/include/libfwevt/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5106 2023-04-10 13:32:43.000000 libfwevt-20230410/include/libfwevt/definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-04-10 13:32:43.000000 libfwevt-20230410/include/libfwevt/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5265 2023-04-10 13:45:27.000000 libfwevt-20230410/include/libfwevt/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-10 13:33:36.000000 libfwevt-20230410/include/libfwevt/features.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5396 2023-04-10 13:32:43.000000 libfwevt-20230410/include/libfwevt/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-10 13:45:27.000000 libfwevt-20230410/include/libfwevt/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5104 2023-04-10 13:45:27.000000 libfwevt-20230410/include/libfwevt/definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2023-04-10 13:32:43.000000 libfwevt-20230410/include/libfwevt/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      471 2023-04-10 13:32:40.000000 libfwevt-20230410/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24555 2023-04-10 13:45:27.000000 libfwevt-20230410/include/libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25017 2023-04-10 13:45:17.000000 libfwevt-20230410/include/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    24555 2023-04-10 13:32:43.000000 libfwevt-20230410/include/libfwevt.h.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-04-10 13:45:17.000000 libfwevt-20230410/install-sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:04.000000 libfwevt-20230410/pyfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_map.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5826 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_template.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_integer.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_channels.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2391 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_tasks.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2506 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_manifest.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2022-07-24 05:32:44.000000 libfwevt-20230410/pyfwevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5543 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_level.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_libfwevt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_levels.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1800 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9328 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_events.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9926 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_channel.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2096 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_event.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_opcode.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14318 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_keywords.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_providers.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10708 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_task.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_maps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9390 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_opcodes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5566 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9206 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_maps.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_templates.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62291 2023-04-10 13:45:18.000000 libfwevt-20230410/pyfwevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_keyword.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_providers.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_opcode.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2901 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50707 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2433 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_opcodes.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_tasks.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9236 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_levels.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_provider.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_events.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_channels.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_level.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_keywords.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2023-04-10 13:33:36.000000 libfwevt-20230410/pyfwevt/pyfwevt_templates.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2023-04-10 13:32:44.000000 libfwevt-20230410/pyfwevt/pyfwevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-04-10 13:45:17.000000 libfwevt-20230410/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/dpkg/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      121 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-04-10 13:45:27.000000 libfwevt-20230410/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/libfwevt-python3.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2023-04-10 13:32:44.000000 libfwevt-20230410/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/source/format
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/rules
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/libfwevt.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-04-10 13:32:40.000000 libfwevt-20230410/dpkg/libfwevt-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:00.000000 libfwevt-20230410/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29610 2023-04-10 13:45:17.000000 libfwevt-20230410/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-04-10 13:45:02.000000 libfwevt-20230410/libfdatetime/libfdatetime_filetime.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:05.000000 libfwevt-20230410/pyfwevt-python2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1965 2023-04-10 13:32:41.000000 libfwevt-20230410/pyfwevt-python2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62166 2023-04-10 13:45:18.000000 libfwevt-20230410/pyfwevt-python2/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29849 2023-04-10 13:45:17.000000 libfwevt-20230410/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-04-10 13:45:00.000000 libfwevt-20230410/libcthreads/libcthreads_queue.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2023-04-10 13:32:42.000000 libfwevt-20230410/AUTHORS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-04-10 13:45:17.000000 libfwevt-20230410/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:06.000000 libfwevt-20230410/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      132 2016-02-02 07:37:21.000000 libfwevt-20230410/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22240 2023-04-10 13:45:18.000000 libfwevt-20230410/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11783 2023-04-10 13:33:36.000000 libfwevt-20230410/manuals/libfwevt.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-11 04:25:12.000000 libfwevt-20230410/ABOUT-NLS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8769 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libfwevt/libfwevt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5157 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_support/fwevt_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libfguid/libfguid.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1223 2023-04-10 13:33:20.000000 libfwevt-20230410/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_provider/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_manifest/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_template/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_template/fwevt_test_template.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_tag/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5568 2023-04-10 13:33:20.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_level/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_level/fwevt_test_level.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/pyfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8480 2023-04-10 13:33:21.000000 libfwevt-20230410/msvscpp/pyfwevt/pyfwevt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5151 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_error/fwevt_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_template_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5436 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_map/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_map/fwevt_test_map.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_event/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_event/fwevt_test_event.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_document/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2023-04-10 13:33:20.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_channel/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libuna/libuna.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_token/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20218 2023-04-10 13:45:18.000000 libfwevt-20230410/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_opcode/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_keyword/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19630 2023-04-10 13:33:21.000000 libfwevt-20230410/msvscpp/libfwevt.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/msvscpp/fwevt_test_task/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5394 2023-04-10 13:33:00.000000 libfwevt-20230410/msvscpp/fwevt_test_task/fwevt_test_task.vcproj
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11454 2023-04-10 13:33:00.000000 libfwevt-20230410/setup.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-04-10 13:45:17.000000 libfwevt-20230410/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2023-04-10 13:45:27.000000 libfwevt-20230410/libfwevt.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 13:32:40.000000 libfwevt-20230410/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:07.000000 libfwevt-20230410/ossfuzz/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      868 2021-11-20 11:04:16.000000 libfwevt-20230410/ossfuzz/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      972 2023-04-10 13:32:43.000000 libfwevt-20230410/ossfuzz/ossfuzz_libfwevt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2023-04-10 13:32:43.000000 libfwevt-20230410/ossfuzz/manifest_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29873 2023-04-10 13:45:18.000000 libfwevt-20230410/ossfuzz/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2023-04-10 13:32:43.000000 libfwevt-20230410/ossfuzz/xml_document_fuzzer.cc
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-04-10 13:45:18.000000 libfwevt-20230410/test-driver
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1562213 2023-04-10 13:45:16.000000 libfwevt-20230410/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:59.000000 libfwevt-20230410/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50561 2023-04-10 13:45:18.000000 libfwevt-20230410/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-04-10 13:45:07.000000 libfwevt-20230410/libuna/libuna_codepage_iso_8859_16.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:02.000000 libfwevt-20230410/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2876 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84540 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6272 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32274 2023-04-10 13:45:18.000000 libfwevt-20230410/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2023-04-10 13:45:05.000000 libfwevt-20230410/libfvalue/libfvalue_definitions.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:05.000000 libfwevt-20230410/pyfwevt-python3/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1965 2023-04-10 13:32:41.000000 libfwevt-20230410/pyfwevt-python3/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62166 2023-04-10 13:45:18.000000 libfwevt-20230410/pyfwevt-python3/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38224 2023-04-10 13:45:17.000000 libfwevt-20230410/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      425 2021-12-03 05:42:29.000000 libfwevt-20230410/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:57.000000 libfwevt-20230410/m4/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-11-18 19:42:05.000000 libfwevt-20230410/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/gettext.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-08-27 05:06:23.000000 libfwevt-20230410/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-04-10 13:45:12.000000 libfwevt-20230410/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/lib-ld.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-09-06 03:53:36.000000 libfwevt-20230410/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-11-18 20:24:51.000000 libfwevt-20230410/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-04-10 13:45:12.000000 libfwevt-20230410/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/nls.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-09-06 03:53:36.000000 libfwevt-20230410/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/host-cpu-c-abi.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-09-06 03:53:36.000000 libfwevt-20230410/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-04-10 13:45:12.000000 libfwevt-20230410/m4/ltversion.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-01-12 04:30:49.000000 libfwevt-20230410/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-04-10 13:45:12.000000 libfwevt-20230410/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/po.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2014-09-28 19:03:26.000000 libfwevt-20230410/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-12-27 06:01:12.000000 libfwevt-20230410/m4/common.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-09-06 03:53:36.000000 libfwevt-20230410/m4/libcerror.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-09-06 03:53:36.000000 libfwevt-20230410/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-04-10 13:45:12.000000 libfwevt-20230410/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-11 04:25:12.000000 libfwevt-20230410/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-07-30 20:03:40.000000 libfwevt-20230410/m4/types.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2020-08-27 05:06:23.000000 libfwevt-20230410/m4/libfvalue.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-04-10 13:32:40.000000 libfwevt-20230410/COPYING.LESSER
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26384 2023-04-10 13:45:17.000000 libfwevt-20230410/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-04-10 13:44:58.000000 libfwevt-20230410/libcerror/libcerror_system.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26871 2023-04-10 13:45:17.000000 libfwevt-20230410/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-04-10 13:44:59.000000 libfwevt-20230410/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-04-10 13:45:12.000000 libfwevt-20230410/ltmain.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-04-10 13:45:17.000000 libfwevt-20230410/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-11 04:25:12.000000 libfwevt-20230410/config.rpath
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-04-10 13:45:18.000000 libfwevt-20230410/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:01:06.000000 libfwevt-20230410/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-11 04:25:12.000000 libfwevt-20230410/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-11 04:25:12.000000 libfwevt-20230410/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2014-09-28 18:22:12.000000 libfwevt-20230410/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-11 04:25:12.000000 libfwevt-20230410/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2014-09-28 18:22:12.000000 libfwevt-20230410/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-04 13:53:58.000000 libfwevt-20230410/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-11 04:25:12.000000 libfwevt-20230410/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2014-09-28 18:22:12.000000 libfwevt-20230410/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1810 2023-04-10 13:45:27.000000 libfwevt-20230410/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-11 04:25:12.000000 libfwevt-20230410/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-11 04:25:12.000000 libfwevt-20230410/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2014-09-28 18:22:12.000000 libfwevt-20230410/po/boldquot.sed
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 14:00:58.000000 libfwevt-20230410/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29443 2023-04-10 13:45:17.000000 libfwevt-20230410/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-04-10 13:44:56.000000 libfwevt-20230410/libcdata/libcdata_btree.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      759 2023-04-10 13:32:40.000000 libfwevt-20230410/acinclude.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      536 2023-04-10 13:32:40.000000 libfwevt-20230410/libfwevt.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5466 2023-04-10 13:32:40.000000 libfwevt-20230410/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      351 2023-04-10 14:01:08.472124 libfwevt-20230410/PKG-INFO
```

### Comparing `libfwevt-20220925/libfwevt.spec.in` & `libfwevt-20230410/libfwevt.spec.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfwevt/libfwevt_provider.c` & `libfwevt-20230410/libfwevt/libfwevt_provider.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Provider functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_libcerror.h` & `libfwevt-20230410/libfwevt/libfwevt_libcerror.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt.rc.in` & `libfwevt-20230410/libfwevt/libfwevt.rc.in`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support the Windows XML Event Log (EVTX) data types\0"
       VALUE "FileVersion",		"@VERSION@" "\0"
       VALUE "InternalName",		"libfwevt.dll\0"
-      VALUE "LegalCopyright",		"(C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>\0"
+      VALUE "LegalCopyright",		"(C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwevt.dll\0"
       VALUE "ProductName",		"libfwevt\0"
       VALUE "ProductVersion",		"@VERSION@" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwevt/\0"
     END
   END
   BLOCK "VarFileInfo"
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_document.h` & `libfwevt-20230410/libfwevt/libfwevt_xml_document.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows Event Log binary XML document functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_notify.h` & `libfwevt-20230410/libfwevt/libfwevt_notify.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_debug.h` & `libfwevt-20230410/libfwevt/libfwevt_debug.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_definitions.h.in` & `libfwevt-20230410/libfwevt/libfwevt_definitions.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt.rc` & `libfwevt-20230410/libfwevt/libfwevt.rc`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support the Windows XML Event Log (EVTX) data types\0"
-      VALUE "FileVersion",		"20220925" "\0"
+      VALUE "FileVersion",		"20230410" "\0"
       VALUE "InternalName",		"libfwevt.dll\0"
-      VALUE "LegalCopyright",		"(C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>\0"
+      VALUE "LegalCopyright",		"(C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwevt.dll\0"
       VALUE "ProductName",		"libfwevt\0"
-      VALUE "ProductVersion",		"20220925" "\0"
+      VALUE "ProductVersion",		"20230410" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwevt/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwevt-20220925/libfwevt/Makefile.am` & `libfwevt-20230410/libfwevt/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_token.h` & `libfwevt-20230410/libfwevt/libfwevt_xml_token.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows Event Log binary XML token functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_event.h` & `libfwevt-20230410/libfwevt/libfwevt_event.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Event functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_level.h` & `libfwevt-20230410/libfwevt/libfwevt_level.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Level functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_document.c` & `libfwevt-20230410/libfwevt/libfwevt_xml_document.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows Event Log binary XML document functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_map.c` & `libfwevt-20230410/libfwevt/libfwevt_map.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Map functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_tag.h` & `libfwevt-20230410/libfwevt/libfwevt_xml_tag.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * XML tag functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_task.c` & `libfwevt-20230410/libfwevt/libfwevt_task.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Task functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_template_value.h` & `libfwevt-20230410/libfwevt/libfwevt_xml_template_value.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Binary XML template value functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_notify.c` & `libfwevt-20230410/libfwevt/libfwevt_notify.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_support.c` & `libfwevt-20230410/libfwevt/libfwevt_support.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt.c` & `libfwevt-20230410/libfwevt/libfwevt.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library to support the Windows XML Event Log (EVTX) data types
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_event.c` & `libfwevt-20230410/libfwevt/libfwevt_event.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Event functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_keyword.h` & `libfwevt-20230410/libfwevt/libfwevt_keyword.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Keyword functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_extern.h` & `libfwevt-20230410/libfwevt/libfwevt_extern.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_keyword.c` & `libfwevt-20230410/libfwevt/libfwevt_keyword.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Keyword functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_libuna.h` & `libfwevt-20230410/libfwevt/libfwevt_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_libcdata.h` & `libfwevt-20230410/libfwevt/libfwevt_libcdata.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_opcode.c` & `libfwevt-20230410/libfwevt/libfwevt_opcode.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Opcode functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_debug.c` & `libfwevt-20230410/libfwevt/libfwevt_debug.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_definitions.h` & `libfwevt-20230410/libfwevt/libfwevt_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwevt/definitions.h> are copied here
  * for local use of libfwevt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWEVT_VERSION						20220925
+#define LIBFWEVT_VERSION						20230410
 
 /* The version string
  */
-#define LIBFWEVT_VERSION_STRING						"20220925"
+#define LIBFWEVT_VERSION_STRING						"20230410"
 
 /* The byte order definitions
  */
 #define LIBFWEVT_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWEVT_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The binary XML document read flags
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_task.h` & `libfwevt-20230410/libfwevt/libfwevt_task.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Task functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_manifest.c` & `libfwevt-20230410/libfwevt/libfwevt_manifest.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Map functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_channel.h` & `libfwevt-20230410/libfwevt/libfwevt_channel.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Channel functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_types.h` & `libfwevt-20230410/libfwevt/libfwevt_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_template_value.c` & `libfwevt-20230410/libfwevt/libfwevt_xml_template_value.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Binary XML template value functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_libfvalue.h` & `libfwevt-20230410/libfwevt/libfwevt_libfvalue.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfvalue header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_manifest.h` & `libfwevt-20230410/libfwevt/libfwevt_manifest.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Manifest functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_opcode.h` & `libfwevt-20230410/libfwevt/libfwevt_opcode.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Opcode functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_provider.h` & `libfwevt-20230410/libfwevt/libfwevt_provider.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Provider functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/Makefile.in` & `libfwevt-20230410/libfwevt/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfwevt/libfwevt_template.c` & `libfwevt-20230410/libfwevt/libfwevt_template.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Template functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_tag.c` & `libfwevt-20230410/libfwevt/libfwevt_xml_tag.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * XML tag functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/fwevt_template.h` & `libfwevt-20230410/libfwevt/fwevt_template.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The Windows Event Template (WEVT_TEMPLATE) definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_error.h` & `libfwevt-20230410/libfwevt/libfwevt_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_xml_token.c` & `libfwevt-20230410/libfwevt/libfwevt_xml_token.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows Event Log binary XML token functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_level.c` & `libfwevt-20230410/libfwevt/libfwevt_level.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Level functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_libfguid.h` & `libfwevt-20230410/libfvalue/libfvalue_libfguid.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfguid header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,35 +15,37 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWEVT_LIBFGUID_H )
-#define _LIBFWEVT_LIBFGUID_H
+#if !defined( _LIBFVALUE_LIBFGUID_H )
+#define _LIBFVALUE_LIBFGUID_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBFGUID for local use of libfguid
  */
 #if defined( HAVE_LOCAL_LIBFGUID )
 
 #include <libfguid_definitions.h>
 #include <libfguid_identifier.h>
 #include <libfguid_types.h>
 
-#else
+/* Note that libfvalue does not require to have libfguid support
+ */
+#elif defined( HAVE_LIBFGUID )
 
 /* If libtool DLL support is enabled set LIBFGUID_DLL_IMPORT
  * before including libfguid.h
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBFGUID_DLL_IMPORT
 #endif
 
 #include <libfguid.h>
 
 #endif /* defined( HAVE_LOCAL_LIBFGUID ) */
 
-#endif /* !defined( _LIBFWEVT_LIBFGUID_H ) */
+#endif /* !defined( _LIBFVALUE_LIBFGUID_H ) */
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_unused.h` & `libfwevt-20230410/libfwevt/libfwevt_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_error.c` & `libfwevt-20230410/libfwevt/libfwevt_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_libcnotify.h` & `libfwevt-20230410/libfvalue/libfvalue_libcnotify.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcnotify header
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWEVT_LIBCNOTIFY_H )
-#define _LIBFWEVT_LIBCNOTIFY_H
+#if !defined( _LIBFVALUE_LIBCNOTIFY_H )
+#define _LIBFVALUE_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_template.h` & `libfwevt-20230410/libfwevt/libfwevt_template.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Template functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_channel.c` & `libfwevt-20230410/libfwevt/libfwevt_channel.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Channel functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_support.h` & `libfwevt-20230410/libfwevt/libfwevt_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfwevt/libfwevt_map.h` & `libfwevt-20230410/libfwevt/libfwevt_map.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Map functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/config_msc.h` & `libfwevt-20230410/common/config_msc.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Configuration for the Microsoft Visual Studio C++ compiler
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/byte_stream.h` & `libfwevt-20230410/common/byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/common.h` & `libfwevt-20230410/common/common.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Common include file
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/system_string.h` & `libfwevt-20230410/common/system_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System character string functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/types.h` & `libfwevt-20230410/common/types.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Type and type-support definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -56,15 +56,18 @@
 
 #define PRIc_SYSTEM "c"
 #define PRIs_SYSTEM "s"
 
 #endif /* defined( WINAPI ) && ( defined( _UNICODE ) || defined( UNICODE ) ) */
 
 /* Fallback for systems without PRI definitions
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( PRId8 )
 #define PRId8 "d"
 #endif
 
 #if !defined( PRId16 )
 #define PRId16 "d"
 #endif
@@ -212,14 +215,16 @@
 
 #else
 #define PRIx64 "llx"
 
 #endif
 #endif /* !defined( PRIx64 ) */
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Fallback for systems without printf %jd definition
  */
 #if defined( HAVE_PRINTF_JD )
 #define PRIjd	"jd"
 #define PRIji	"ji"
 #define PRIju	"ju"
 #define PRIjx	"jx"
```

### Comparing `libfwevt-20220925/common/types.h.in` & `libfwevt-20230410/common/types.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Type and type-support definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -56,15 +56,18 @@
 
 #define PRIc_SYSTEM "c"
 #define PRIs_SYSTEM "s"
 
 #endif /* defined( WINAPI ) && ( defined( _UNICODE ) || defined( UNICODE ) ) */
 
 /* Fallback for systems without PRI definitions
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( PRId8 )
 #define PRId8 "d"
 #endif
 
 #if !defined( PRId16 )
 #define PRId16 "d"
 #endif
@@ -212,14 +215,16 @@
 
 #else
 #define PRIx64 "llx"
 
 #endif
 #endif /* !defined( PRIx64 ) */
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Fallback for systems without printf %jd definition
  */
 #if defined( HAVE_PRINTF_JD )
 #define PRIjd	"jd"
 #define PRIji	"ji"
 #define PRIju	"ju"
 #define PRIjx	"jx"
```

### Comparing `libfwevt-20220925/common/config_winapi.h` & `libfwevt-20230410/common/config_winapi.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Configuration file for WINAPI
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -41,23 +41,28 @@
 /* Define the size of the integer for WINAPI
  */
 #if !defined( SIZEOF_INT )
 #define SIZEOF_INT			4
 #endif
 
 /* Define the size of size_t for WINAPI
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( SIZEOF_SIZE_T )
 #if __WORDSIZE == 64
 #define SIZEOF_SIZE_T			8
 #else
 #define SIZEOF_SIZE_T			4
 #endif
 #endif
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Define the size of the wide character for WINAPI
  */
 #if !defined( SIZEOF_WCHAR_T )
 #define SIZEOF_WCHAR_T			2
 #endif
 
 /* Enable the DllMain function
```

### Comparing `libfwevt-20220925/common/memory.h` & `libfwevt-20230410/common/memory.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/config.h` & `libfwevt-20230410/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -364,24 +364,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwevt"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwevt 20220925"
+#define PACKAGE_STRING "libfwevt 20230410"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwevt"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20220925"
+#define PACKAGE_VERSION "20230410"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -399,15 +399,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20220925"
+#define VERSION "20230410"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwevt-20220925/common/narrow_string.h` & `libfwevt-20230410/common/narrow_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Narrow character string functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/Makefile.in` & `libfwevt-20230410/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/common/file_stream.h` & `libfwevt-20230410/common/file_stream.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * FILE stream functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/config_borlandc.h` & `libfwevt-20230410/common/config_borlandc.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Configuration for the Borland/CodeGear C++ Builder compiler
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/common/config.h.in` & `libfwevt-20230410/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/common/wide_string.h` & `libfwevt-20230410/common/wide_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Wide character string functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libfguid/libfguid_identifier.c` & `libfwevt-20230410/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_support.c` & `libfwevt-20230410/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/Makefile.am` & `libfwevt-20230410/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_support.h` & `libfwevt-20230410/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_definitions.h` & `libfwevt-20230410/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_identifier.h` & `libfwevt-20230410/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_unused.h` & `libfwevt-20230410/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_error.h` & `libfwevt-20230410/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_libcerror.h` & `libfwevt-20230410/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/Makefile.in` & `libfwevt-20230410/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_error.c` & `libfwevt-20230410/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_types.h` & `libfwevt-20230410/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfguid/libfguid_extern.h` & `libfwevt-20230410/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/tests/fwevt_test_xml_document.c` & `libfwevt-20230410/tests/fwevt_test_xml_document.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library xml_document type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/test_library.sh` & `libfwevt-20230410/tests/test_library.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/tests/fwevt_test_template.c` & `libfwevt-20230410/tests/fwevt_test_template.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library template type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_libfwevt.h` & `libfwevt-20230410/tests/fwevt_test_libfwevt.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfwevt header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_macros.h` & `libfwevt-20230410/tests/fwevt_test_macros.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Macros for testing
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/test_python_module.sh` & `libfwevt-20230410/tests/test_python_module.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/tests/fwevt_test_libcnotify.h` & `libfwevt-20230410/tests/fwevt_test_libcnotify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/Makefile.am` & `libfwevt-20230410/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/tests/fwevt_test_channel.c` & `libfwevt-20230410/tests/fwevt_test_channel.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library channel type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_opcode.c` & `libfwevt-20230410/tests/fwevt_test_opcode.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library opcode type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_memory.c` & `libfwevt-20230410/tests/fwevt_test_memory.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory allocation functions for testing
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_keyword.c` & `libfwevt-20230410/tests/fwevt_test_keyword.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library keyword type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_support.c` & `libfwevt-20230410/tests/fwevt_test_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library support functions test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_provider.c` & `libfwevt-20230410/tests/fwevt_test_provider.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library provider type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_event.c` & `libfwevt-20230410/tests/fwevt_test_event.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library event type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_libfvalue.h` & `libfwevt-20230410/tests/fwevt_test_libfvalue.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfvalue header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_xml_tag.c` & `libfwevt-20230410/tests/fwevt_test_xml_tag.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library xml_tag type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/test_manpage.sh` & `libfwevt-20230410/tests/test_manpage.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/tests/fwevt_test_libcerror.h` & `libfwevt-20230410/tests/fwevt_test_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/pyfwevt_test_manifest.py` & `libfwevt-20230410/tests/pyfwevt_test_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Python-bindings manifest type test script
 #
-# Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+# Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
 #
 # Refer to AUTHORS for acknowledgements.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_task.c` & `libfwevt-20230410/tests/fwevt_test_task.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library task type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_xml_token.c` & `libfwevt-20230410/tests/fwevt_test_xml_token.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library xml_token type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_manifest.c` & `libfwevt-20230410/tests/fwevt_test_manifest.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library manifest type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/pyfwevt_test_provider.py` & `libfwevt-20230410/tests/pyfwevt_test_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Python-bindings provider type test script
 #
-# Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+# Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
 #
 # Refer to AUTHORS for acknowledgements.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/test_runner.sh` & `libfwevt-20230410/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/tests/fwevt_test_unused.h` & `libfwevt-20230410/tests/fwevt_test_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_libuna.h` & `libfwevt-20230410/tests/fwevt_test_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/pyfwevt_test_support.py` & `libfwevt-20230410/tests/pyfwevt_test_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Python-bindings support functions test script
 #
-# Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+# Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
 #
 # Refer to AUTHORS for acknowledgements.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/Makefile.in` & `libfwevt-20230410/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/tests/fwevt_test_error.c` & `libfwevt-20230410/tests/fwevt_test_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library error functions test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_map.c` & `libfwevt-20230410/tests/fwevt_test_map.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library map type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_memory.h` & `libfwevt-20230410/tests/fwevt_test_memory.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory allocation functions for testing
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_xml_template_value.c` & `libfwevt-20230410/tests/fwevt_test_xml_template_value.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library xml_template_value type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/tests/fwevt_test_level.c` & `libfwevt-20230410/tests/fwevt_test_level.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library level type test program
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/missing` & `libfwevt-20230410/missing`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/Makefile.am` & `libfwevt-20230410/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/aclocal.m4` & `libfwevt-20230410/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/COPYING` & `libfwevt-20230410/COPYING`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/include/libfwevt/definitions.h.in` & `libfwevt-20230410/include/libfwevt/definitions.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions for libfwevt
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/libfwevt/extern.h` & `libfwevt-20230410/include/libfwevt/extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * The extern definition
  *
  * This header should be included in header files that export or import
  * library functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/libfwevt/types.h` & `libfwevt-20230410/include/libfwevt/types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Type definitions for libfwevt
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/libfwevt/features.h.in` & `libfwevt-20230410/include/libfwevt/features.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Features of libfwevt
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/libfwevt/types.h.in` & `libfwevt-20230410/include/libfwevt/types.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Type definitions for libfwevt
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/libfwevt/features.h` & `libfwevt-20230410/include/libfwevt/features.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Features of libfwevt
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/libfwevt/definitions.h` & `libfwevt-20230410/include/libfwevt/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions for libfwevt
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWEVT_DEFINITIONS_H )
 #define _LIBFWEVT_DEFINITIONS_H
 
 #include <libfwevt/types.h>
 
-#define LIBFWEVT_VERSION							20220925
+#define LIBFWEVT_VERSION							20230410
 
 /* The version string
  */
-#define LIBFWEVT_VERSION_STRING							"20220925"
+#define LIBFWEVT_VERSION_STRING							"20230410"
 
 /* The byte order definitions
  */
 enum LIBFWEVT_ENDIAN
 {
 	LIBFWEVT_ENDIAN_BIG							= (int) 'b',
 	LIBFWEVT_ENDIAN_LITTLE							= (int) 'l'
```

### Comparing `libfwevt-20220925/include/libfwevt/error.h` & `libfwevt-20230410/include/libfwevt/error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The error code definitions for libfwevt
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/libfwevt.h` & `libfwevt-20230410/include/libfwevt.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library to support the Windows XML Event Log (EVTX) data types
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/include/Makefile.in` & `libfwevt-20230410/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/include/libfwevt.h.in` & `libfwevt-20230410/include/libfwevt.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Library to support the Windows XML Event Log (EVTX) data types
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/install-sh` & `libfwevt-20230410/install-sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_map.h` & `libfwevt-20230410/pyfwevt/pyfwevt_map.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_map_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_template.c` & `libfwevt-20230410/pyfwevt/pyfwevt_template.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_template_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_integer.h` & `libfwevt-20230410/pyfwevt/pyfwevt_integer.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Integer functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_error.h` & `libfwevt-20230410/pyfwevt/pyfwevt_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_channels.h` & `libfwevt-20230410/pyfwevt/pyfwevt_channels.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of channels
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_keyword.c` & `libfwevt-20230410/pyfwevt/pyfwevt_keyword.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_keyword_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_tasks.h` & `libfwevt-20230410/pyfwevt/pyfwevt_tasks.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of tasks
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_manifest.h` & `libfwevt-20230410/pyfwevt/pyfwevt_manifest.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_manifest_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/Makefile.am` & `libfwevt-20230410/pyfwevt/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_level.c` & `libfwevt-20230410/pyfwevt/pyfwevt_level.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_level_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_libfwevt.h` & `libfwevt-20230410/pyfwevt/pyfwevt_libfwevt.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libfwevt header
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt.h` & `libfwevt-20230410/pyfwevt/pyfwevt.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python bindings module for libfwevt (pyfwevt)
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_levels.h` & `libfwevt-20230410/pyfwevt/pyfwevt_levels.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of levels
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_template.h` & `libfwevt-20230410/pyfwevt/pyfwevt_template.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_template_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_events.c` & `libfwevt-20230410/pyfwevt/pyfwevt_events.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of events
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_event.c` & `libfwevt-20230410/pyfwevt/pyfwevt_event.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_event_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_channel.h` & `libfwevt-20230410/pyfwevt/pyfwevt_channel.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_channel_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_libfguid.h` & `libfwevt-20230410/pyfwevt/pyfwevt_libfguid.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfguid header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_event.h` & `libfwevt-20230410/pyfwevt/pyfwevt_event.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_event_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_opcode.h` & `libfwevt-20230410/pyfwevt/pyfwevt_opcode.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_opcode_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_unused.h` & `libfwevt-20230410/pyfwevt/pyfwevt_unused.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_manifest.c` & `libfwevt-20230410/pyfwevt/pyfwevt_manifest.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_manifest_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_keywords.h` & `libfwevt-20230410/pyfwevt/pyfwevt_keywords.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of keywords
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_providers.h` & `libfwevt-20230410/pyfwevt/pyfwevt_providers.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of providers
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt.c` & `libfwevt-20230410/pyfwevt/pyfwevt.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python bindings module for libfwevt (pyfwevt)
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_libcerror.h` & `libfwevt-20230410/pyfwevt/pyfwevt_libcerror.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_task.h` & `libfwevt-20230410/pyfwevt/pyfwevt_task.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_task_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_map.c` & `libfwevt-20230410/pyfwevt/pyfwevt_map.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_map_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_maps.h` & `libfwevt-20230410/pyfwevt/pyfwevt_maps.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of maps
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_opcodes.c` & `libfwevt-20230410/pyfwevt/pyfwevt_opcodes.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of opcodes
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_task.c` & `libfwevt-20230410/pyfwevt/pyfwevt_task.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_task_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_maps.c` & `libfwevt-20230410/pyfwevt/pyfwevt_maps.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of maps
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_templates.c` & `libfwevt-20230410/pyfwevt/pyfwevt_templates.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of templates
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/Makefile.in` & `libfwevt-20230410/pyfwevt/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_keyword.h` & `libfwevt-20230410/pyfwevt/pyfwevt_keyword.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_keyword_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_providers.c` & `libfwevt-20230410/pyfwevt/pyfwevt_providers.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of providers
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_integer.c` & `libfwevt-20230410/pyfwevt/pyfwevt_integer.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Integer functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_opcode.c` & `libfwevt-20230410/pyfwevt/pyfwevt_opcode.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_opcode_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_guid.c` & `libfwevt-20230410/pyfwevt/pyfwevt_guid.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * GUID functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_provider.c` & `libfwevt-20230410/pyfwevt/pyfwevt_provider.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_provider_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_opcodes.h` & `libfwevt-20230410/pyfwevt/pyfwevt_opcodes.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of opcodes
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_guid.h` & `libfwevt-20230410/pyfwevt/pyfwevt_guid.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * GUID functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_tasks.c` & `libfwevt-20230410/pyfwevt/pyfwevt_tasks.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of tasks
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_levels.c` & `libfwevt-20230410/pyfwevt/pyfwevt_levels.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of levels
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_python.h` & `libfwevt-20230410/pyfwevt/pyfwevt_python.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The python header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_provider.h` & `libfwevt-20230410/pyfwevt/pyfwevt_provider.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_provider_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_channel.c` & `libfwevt-20230410/pyfwevt/pyfwevt_channel.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_channel_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_events.h` & `libfwevt-20230410/pyfwevt/pyfwevt_events.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of events
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_channels.c` & `libfwevt-20230410/pyfwevt/pyfwevt_channels.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of channels
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_level.h` & `libfwevt-20230410/pyfwevt/pyfwevt_level.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object wrapper of libfwevt_level_t
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_keywords.c` & `libfwevt-20230410/pyfwevt/pyfwevt_keywords.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of keywords
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_templates.h` & `libfwevt-20230410/pyfwevt/pyfwevt_templates.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Python object definition of the sequence and iterator object of templates
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/pyfwevt/pyfwevt_error.c` & `libfwevt-20230410/pyfwevt/pyfwevt_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/INSTALL` & `libfwevt-20230410/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/dpkg/copyright` & `libfwevt-20230410/dpkg/copyright`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Format: http://www.debian.org/doc/packaging-manuals/copyright-format/1.0/
 Upstream-Name: libfwevt
 Source: https://github.com/libyal/libfwevt
 
 Files: *
-Copyright: 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+Copyright: 2011-2023, Joachim Metz <joachim.metz@gmail.com>
 License: LGPL-3.0+
 
 License: LGPL-3.0+
  This package is free software; you can redistribute it and/or
  modify it under the terms of the GNU Lesser General Public
  License as published by the Free Software Foundation; either
  version 3 of the License, or (at your option) any later version.
```

### Comparing `libfwevt-20220925/dpkg/rules` & `libfwevt-20230410/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/dpkg/control` & `libfwevt-20230410/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_support.c` & `libfwevt-20230410/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_systemtime.h` & `libfwevt-20230410/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_error.h` & `libfwevt-20230410/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/Makefile.am` & `libfwevt-20230410/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_unused.h` & `libfwevt-20230410/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_error.c` & `libfwevt-20230410/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_posix_time.c` & `libfwevt-20230410/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_fat_date_time.h` & `libfwevt-20230410/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_types.h` & `libfwevt-20230410/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_floatingtime.c` & `libfwevt-20230410/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_hfs_time.h` & `libfwevt-20230410/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_support.h` & `libfwevt-20230410/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_extern.h` & `libfwevt-20230410/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_filetime.h` & `libfwevt-20230410/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_date_time_values.c` & `libfwevt-20230410/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_floatingtime.h` & `libfwevt-20230410/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_libcerror.h` & `libfwevt-20230410/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/Makefile.in` & `libfwevt-20230410/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwevt-20230410/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_date_time_values.h` & `libfwevt-20230410/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_hfs_time.c` & `libfwevt-20230410/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_posix_time.h` & `libfwevt-20230410/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_fat_date_time.c` & `libfwevt-20230410/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwevt-20230410/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_definitions.h` & `libfwevt-20230410/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_systemtime.c` & `libfwevt-20230410/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfdatetime/libfdatetime_filetime.c` & `libfwevt-20230410/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/pyfwevt-python2/Makefile.am` & `libfwevt-20230410/pyfwevt-python2/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/pyfwevt-python2/Makefile.in` & `libfwevt-20230410/pyfwevt-python2/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_thread_pool.h` & `libfwevt-20230410/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_thread_pool.c` & `libfwevt-20230410/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_repeating_thread.c` & `libfwevt-20230410/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_error.c` & `libfwevt-20230410/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/Makefile.am` & `libfwevt-20230410/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_unused.h` & `libfwevt-20230410/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_condition.h` & `libfwevt-20230410/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_definitions.h` & `libfwevt-20230410/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_thread.h` & `libfwevt-20230410/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_repeating_thread.h` & `libfwevt-20230410/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_read_write_lock.c` & `libfwevt-20230410/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_mutex.h` & `libfwevt-20230410/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_support.h` & `libfwevt-20230410/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_thread.c` & `libfwevt-20230410/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_mutex.c` & `libfwevt-20230410/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_types.h` & `libfwevt-20230410/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_lock.h` & `libfwevt-20230410/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_extern.h` & `libfwevt-20230410/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_error.h` & `libfwevt-20230410/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_queue.c` & `libfwevt-20230410/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_condition.c` & `libfwevt-20230410/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/Makefile.in` & `libfwevt-20230410/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_thread_attributes.c` & `libfwevt-20230410/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_libcerror.h` & `libfwevt-20230410/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_lock.c` & `libfwevt-20230410/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_support.c` & `libfwevt-20230410/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_read_write_lock.h` & `libfwevt-20230410/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_thread_attributes.h` & `libfwevt-20230410/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcthreads/libcthreads_queue.h` & `libfwevt-20230410/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/config.sub` & `libfwevt-20230410/config.sub`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/manuals/Makefile.in` & `libfwevt-20230410/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/manuals/libfwevt.3` & `libfwevt-20230410/manuals/libfwevt.3`

 * *Files 1% similar despite different names*

```diff
@@ -202,13 +202,13 @@
 .Sh FILES
 None
 .Sh BUGS
 Please report bugs of any kind on the project issue tracker: https://github.com/libyal/libfwevt/issues
 .Sh AUTHOR
 These man pages are generated from "libfwevt.h".
 .Sh COPYRIGHT
-Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>.
+Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>.
 .sp
 This is free software; see the source for copying conditions.
 There is NO warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 .Sh SEE ALSO
 the libfwevt.h include file
```

### Comparing `libfwevt-20220925/msvscpp/libfwevt/libfwevt.vcproj` & `libfwevt-20230410/msvscpp/libfwevt/libfwevt.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_support/fwevt_test_support.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_support/fwevt_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libfguid/libfguid.vcproj` & `libfwevt-20230410/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/Makefile.am` & `libfwevt-20230410/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_template/fwevt_test_template.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_template/fwevt_test_template.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_level/fwevt_test_level.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_level/fwevt_test_level.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/pyfwevt/pyfwevt.vcproj` & `libfwevt-20230410/msvscpp/pyfwevt/pyfwevt.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_error/fwevt_test_error.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_error/fwevt_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwevt-20230410/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libcthreads/libcthreads.vcproj` & `libfwevt-20230410/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_map/fwevt_test_map.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_map/fwevt_test_map.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_event/fwevt_test_event.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_event/fwevt_test_event.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libuna/libuna.vcproj` & `libfwevt-20230410/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libfvalue/libfvalue.vcproj` & `libfwevt-20230410/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/Makefile.in` & `libfwevt-20230410/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libcerror/libcerror.vcproj` & `libfwevt-20230410/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libcnotify/libcnotify.vcproj` & `libfwevt-20230410/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libfwevt.sln` & `libfwevt-20230410/msvscpp/libfwevt.sln`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/libcdata/libcdata.vcproj` & `libfwevt-20230410/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/msvscpp/fwevt_test_task/fwevt_test_task.vcproj` & `libfwevt-20230410/msvscpp/fwevt_test_task/fwevt_test_task.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/setup.py` & `libfwevt-20230410/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python
 #
 # Script to build and install Python-bindings.
-# Version: 20220806
+# Version: 20221217
 
 from __future__ import print_function
 
 import copy
+import datetime
 import glob
 import gzip
 import platform
 import os
 import shlex
 import shutil
 import subprocess
 import sys
 import tarfile
+import zipfile
 
 from distutils.ccompiler import new_compiler
 
 from setuptools import Extension
 from setuptools import setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.sdist import sdist
@@ -93,82 +95,108 @@
     compiler = new_compiler(compiler=self.compiler)
     if compiler.compiler_type == "msvc":
       self.define = [
           ("UNICODE", ""),
       ]
 
     else:
-      command = "sh configure --disable-shared-libs"
+      command = "sh configure --disable-nls --disable-shared-libs"
       output = self._RunCommand(command)
 
       print_line = False
       for line in output.split("\n"):
         line = line.rstrip()
         if line == "configure:":
           print_line = True
 
         if print_line:
           print(line)
 
       self.define = [
           ("HAVE_CONFIG_H", ""),
-          ("LOCALEDIR", "\"/usr/share/locale\""),
       ]
 
     build_ext.run(self)
 
 
 class custom_sdist(sdist):
   """Custom handler for the sdist command."""
 
   def run(self):
     """Builds a source distribution (sdist) package."""
-    if self.formats != ["gztar"]:
+    if self.formats != ["gztar"] and self.formats != ["zip"]:
       print("'setup.py sdist' unsupported format.")
       sys.exit(1)
 
     if glob.glob("*.tar.gz"):
       print("'setup.py sdist' remove existing *.tar.gz files from "
             "source directory.")
       sys.exit(1)
 
     command = "make dist"
     exit_code = subprocess.call(command, shell=True)
     if exit_code != 0:
       raise RuntimeError("Running: {0:s} failed.".format(command))
 
-    if not os.path.exists("dist"):
-      os.mkdir("dist")
+    if not os.path.exists(self.dist_dir):
+      os.mkdir(self.dist_dir)
 
     source_package_file = glob.glob("*.tar.gz")[0]
     source_package_prefix, _, source_package_suffix = (
         source_package_file.partition("-"))
     sdist_package_file = "{0:s}-python-{1:s}".format(
         source_package_prefix, source_package_suffix)
-    sdist_package_file = os.path.join("dist", sdist_package_file)
+    sdist_package_file = os.path.join(self.dist_dir, sdist_package_file)
     os.rename(source_package_file, sdist_package_file)
 
     # Create and add the PKG-INFO file to the source package.
-    with gzip.open(sdist_package_file, 'rb') as input_file:
-      with open(sdist_package_file[:-3], 'wb') as output_file:
+    with gzip.open(sdist_package_file, "rb") as input_file:
+      with open(sdist_package_file[:-3], "wb") as output_file:
         shutil.copyfileobj(input_file, output_file)
     os.remove(sdist_package_file)
 
     self.distribution.metadata.write_pkg_info(".")
     pkg_info_path = "{0:s}-{1:s}/PKG-INFO".format(
         source_package_prefix, source_package_suffix[:-7])
     with tarfile.open(sdist_package_file[:-3], "a:") as tar_file:
       tar_file.add("PKG-INFO", arcname=pkg_info_path)
     os.remove("PKG-INFO")
 
-    with open(sdist_package_file[:-3], 'rb') as input_file:
-      with gzip.open(sdist_package_file, 'wb') as output_file:
+    with open(sdist_package_file[:-3], "rb") as input_file:
+      with gzip.open(sdist_package_file, "wb") as output_file:
         shutil.copyfileobj(input_file, output_file)
     os.remove(sdist_package_file[:-3])
 
+    # Convert the .tar.gz into a .zip
+    if self.formats == ["zip"]:
+      zip_sdist_package_file = "{0:s}.zip".format(sdist_package_file[:-7])
+
+      with tarfile.open(sdist_package_file, "r|gz") as tar_file:
+        with zipfile.ZipFile(
+            zip_sdist_package_file, "w", zipfile.ZIP_DEFLATED) as zip_file:
+          for tar_file_entry in tar_file:
+            file_entry = tar_file.extractfile(tar_file_entry)
+            if tar_file_entry.isfile():
+              modification_time = datetime.datetime.fromtimestamp(
+                  tar_file_entry.mtime)
+              zip_modification_time = (
+                  modification_time.year, modification_time.month,
+                  modification_time.day, modification_time.hour,
+                  modification_time.minute, modification_time.second)
+              zip_info = zipfile.ZipInfo(
+                  date_time=zip_modification_time,
+                  filename=tar_file_entry.name)
+              zip_info.external_attr = (tar_file_entry.mode & 0xff) << 16
+
+              file_data = file_entry.read()
+              zip_file.writestr(zip_info, file_data)
+
+      os.remove(sdist_package_file)
+      sdist_package_file = zip_sdist_package_file
+
     # Inform distutils what files were created.
     dist_files = getattr(self.distribution, "dist_files", [])
     dist_files.append(("sdist", "", sdist_package_file))
 
 
 class ProjectInformation(object):
   """Project information."""
```

### Comparing `libfwevt-20220925/config.guess` & `libfwevt-20230410/config.guess`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfwevt.spec` & `libfwevt-20230410/libfwevt.spec`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfwevt
-Version: 20220925
+Version: 20230410
 Release: 1
 Summary: Library to support the Windows XML Event Log (EVTX) data types
 Group: System Environment/Libraries
 License: LGPLv3+
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwevt
 BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
@@ -81,10 +81,10 @@
 %defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Thu Nov  3 2022 Joachim Metz <joachim.metz@gmail.com> 20220925-1
+* Mon Apr 10 2023 Joachim Metz <joachim.metz@gmail.com> 20230410-1
 - Auto-generated
```

### Comparing `libfwevt-20220925/ossfuzz/Makefile.am` & `libfwevt-20230410/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/ossfuzz/ossfuzz_libfwevt.h` & `libfwevt-20230410/ossfuzz/ossfuzz_libfwevt.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfwevt header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/ossfuzz/manifest_fuzzer.cc` & `libfwevt-20230410/ossfuzz/manifest_fuzzer.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * OSS-Fuzz target for libfwevt manifest type
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/ossfuzz/Makefile.in` & `libfwevt-20230410/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/ossfuzz/xml_document_fuzzer.cc` & `libfwevt-20230410/ossfuzz/xml_document_fuzzer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * OSS-Fuzz target for libfwevt xml_document type
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/test-driver` & `libfwevt-20230410/test-driver`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/configure` & `libfwevt-20230410/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwevt 20220925.
+# Generated by GNU Autoconf 2.71 for libfwevt 20230410.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfwevt'
 PACKAGE_TARNAME='libfwevt'
-PACKAGE_VERSION='20220925'
-PACKAGE_STRING='libfwevt 20220925'
+PACKAGE_VERSION='20230410'
+PACKAGE_STRING='libfwevt 20230410'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwevt.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1584,15 +1584,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwevt 20220925 to adapt to many kinds of systems.
+\`configure' configures libfwevt 20230410 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1655,15 +1655,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwevt 20220925:";;
+     short | recursive ) echo "Configuration of libfwevt 20230410:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1860,15 +1860,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwevt configure 20220925
+libfwevt configure 20230410
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2581,15 +2581,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwevt $as_me 20220925, which was
+It was created by libfwevt $as_me 20230410, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4070,15 +4070,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwevt'
- VERSION='20220925'
+ VERSION='20230410'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -27029,37 +27029,37 @@
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libcdata" >&5
 printf %s "checking for libcdata... " >&6; }
 
 if test -n "$libcdata_CFLAGS"; then
     pkg_cv_libcdata_CFLAGS="$libcdata_CFLAGS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libcdata >= 20220115\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libcdata >= 20220115") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libcdata >= 20230108\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libcdata >= 20230108") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libcdata_CFLAGS=`$PKG_CONFIG --cflags "libcdata >= 20220115" 2>/dev/null`
+  pkg_cv_libcdata_CFLAGS=`$PKG_CONFIG --cflags "libcdata >= 20230108" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
 if test -n "$libcdata_LIBS"; then
     pkg_cv_libcdata_LIBS="$libcdata_LIBS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libcdata >= 20220115\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libcdata >= 20220115") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libcdata >= 20230108\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libcdata >= 20230108") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libcdata_LIBS=`$PKG_CONFIG --libs "libcdata >= 20220115" 2>/dev/null`
+  pkg_cv_libcdata_LIBS=`$PKG_CONFIG --libs "libcdata >= 20230108" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
@@ -27072,17 +27072,17 @@
 
 if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
         _pkg_short_errors_supported=yes
 else
         _pkg_short_errors_supported=no
 fi
         if test $_pkg_short_errors_supported = yes; then
-	        libcdata_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libcdata >= 20220115" 2>&1`
+	        libcdata_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libcdata >= 20230108" 2>&1`
         else
-	        libcdata_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libcdata >= 20220115" 2>&1`
+	        libcdata_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libcdata >= 20230108" 2>&1`
         fi
 	# Put the nasty error message in config.log where it belongs
 	echo "$libcdata_PKG_ERRORS" >&5
 
 	ac_cv_libcdata=check
 elif test $pkg_failed = untried; then
      	{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
@@ -28674,14 +28674,56 @@
 if test "x$ac_cv_lib_cdata_libcdata_list_insert_element" = xyes
 then :
   ac_cv_libcdata_dummy=yes
 else $as_nop
   ac_cv_libcdata=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libcdata_list_insert_element_with_existing in -lcdata" >&5
+printf %s "checking for libcdata_list_insert_element_with_existing in -lcdata... " >&6; }
+if test ${ac_cv_lib_cdata_libcdata_list_insert_element_with_existing+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lcdata  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libcdata_list_insert_element_with_existing ();
+int
+main (void)
+{
+return libcdata_list_insert_element_with_existing ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_cdata_libcdata_list_insert_element_with_existing=yes
+else $as_nop
+  ac_cv_lib_cdata_libcdata_list_insert_element_with_existing=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_cdata_libcdata_list_insert_element_with_existing" >&5
+printf "%s\n" "$ac_cv_lib_cdata_libcdata_list_insert_element_with_existing" >&6; }
+if test "x$ac_cv_lib_cdata_libcdata_list_insert_element_with_existing" = xyes
+then :
+  ac_cv_libcdata_dummy=yes
+else $as_nop
+  ac_cv_libcdata=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libcdata_list_insert_value in -lcdata" >&5
 printf %s "checking for libcdata_list_insert_value in -lcdata... " >&6; }
 if test ${ac_cv_lib_cdata_libcdata_list_insert_value+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -28716,14 +28758,56 @@
 if test "x$ac_cv_lib_cdata_libcdata_list_insert_value" = xyes
 then :
   ac_cv_libcdata_dummy=yes
 else $as_nop
   ac_cv_libcdata=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libcdata_list_insert_value_with_existing in -lcdata" >&5
+printf %s "checking for libcdata_list_insert_value_with_existing in -lcdata... " >&6; }
+if test ${ac_cv_lib_cdata_libcdata_list_insert_value_with_existing+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lcdata  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libcdata_list_insert_value_with_existing ();
+int
+main (void)
+{
+return libcdata_list_insert_value_with_existing ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_cdata_libcdata_list_insert_value_with_existing=yes
+else $as_nop
+  ac_cv_lib_cdata_libcdata_list_insert_value_with_existing=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_cdata_libcdata_list_insert_value_with_existing" >&5
+printf "%s\n" "$ac_cv_lib_cdata_libcdata_list_insert_value_with_existing" >&6; }
+if test "x$ac_cv_lib_cdata_libcdata_list_insert_value_with_existing" = xyes
+then :
+  ac_cv_libcdata_dummy=yes
+else $as_nop
+  ac_cv_libcdata=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libcdata_list_remove_element in -lcdata" >&5
 printf %s "checking for libcdata_list_remove_element in -lcdata... " >&6; }
 if test ${ac_cv_lib_cdata_libcdata_list_remove_element+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -47288,15 +47372,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwevt $as_me 20220925, which was
+This file was extended by libfwevt $as_me 20230410, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -47356,15 +47440,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwevt config.status 20220925
+libfwevt config.status 20230410
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwevt-20220925/libuna/libuna_url_stream.c` & `libfwevt-20230410/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_symbol.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_support.c` & `libfwevt-20230410/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_scsu.h` & `libfwevt-20230410/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_5.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_2.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1253.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_koi8_u.h` & `libfwevt-20230410/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1252.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf32_stream.c` & `libfwevt-20230410/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1257.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_cyrillic.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_thai.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf32_string.c` & `libfwevt-20230410/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_thai.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_874.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1251.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_libcerror.h` & `libfwevt-20230410/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_949.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_6.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1256.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_greek.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_russian.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_ukrainian.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_6.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_874.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1251.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1256.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_base16_stream.h` & `libfwevt-20230410/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_2.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/Makefile.am` & `libfwevt-20230410/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1257.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1254.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1255.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_unused.h` & `libfwevt-20230410/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1253.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_unicode_character.h` & `libfwevt-20230410/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_dingbats.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_scsu.c` & `libfwevt-20230410/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_byte_stream.c` & `libfwevt-20230410/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_celtic.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_croatian.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_3.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_15.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_roman.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf32_string.h` & `libfwevt-20230410/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_koi8_r.c` & `libfwevt-20230410/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_icelandic.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_936.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_base64_stream.h` & `libfwevt-20230410/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_celtic.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_950.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf8_string.h` & `libfwevt-20230410/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_936.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_unicode_character.c` & `libfwevt-20230410/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf8_string.c` & `libfwevt-20230410/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_base32_stream.c` & `libfwevt-20230410/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_950.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_error.h` & `libfwevt-20230410/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_932.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_turkish.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf8_stream.c` & `libfwevt-20230410/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_ukrainian.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_koi8_r.h` & `libfwevt-20230410/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_base16_stream.c` & `libfwevt-20230410/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1250.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_16.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_croatian.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_gaelic.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf16_stream.h` & `libfwevt-20230410/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_10.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_932.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf8_stream.h` & `libfwevt-20230410/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_url_stream.h` & `libfwevt-20230410/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_farsi.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_949.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_romanian.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_gaelic.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_8.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_types.h` & `libfwevt-20230410/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_arabic.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1252.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1250.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_russian.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf16_string.c` & `libfwevt-20230410/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_5.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_extern.h` & `libfwevt-20230410/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_4.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_byte_stream.h` & `libfwevt-20230410/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_roman.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf16_string.h` & `libfwevt-20230410/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_4.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_10.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_icelandic.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/Makefile.in` & `libfwevt-20230410/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf7_stream.h` & `libfwevt-20230410/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_symbol.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_base32_stream.h` & `libfwevt-20230410/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_turkish.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_inuit.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf16_stream.c` & `libfwevt-20230410/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf7_stream.c` & `libfwevt-20230410/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_support.h` & `libfwevt-20230410/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_utf32_stream.h` & `libfwevt-20230410/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_3.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_greek.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_definitions.h` & `libfwevt-20230410/libuna/libuna_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1255.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_14.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_13.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_8.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_9.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1254.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_cyrillic.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_arabic.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1258.c` & `libfwevt-20230410/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_farsi.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_15.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_7.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_dingbats.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_9.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_windows_1258.h` & `libfwevt-20230410/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_base64_stream.c` & `libfwevt-20230410/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_romanian.c` & `libfwevt-20230410/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_error.c` & `libfwevt-20230410/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_koi8_u.c` & `libfwevt-20230410/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_13.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_7.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_14.h` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_mac_inuit.h` & `libfwevt-20230410/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libuna/libuna_codepage_iso_8859_16.c` & `libfwevt-20230410/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_split_utf8_string.c` & `libfwevt-20230410/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_support.h` & `libfwevt-20230410/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_value_entry.c` & `libfwevt-20230410/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_libfwnt.h` & `libfwevt-20230410/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_utf8_string.h` & `libfwevt-20230410/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_libcerror.h` & `libfwevt-20230410/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_split_utf16_string.h` & `libfwevt-20230410/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_value.c` & `libfwevt-20230410/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_libcnotify.h` & `libfwevt-20230410/libfwevt/libfwevt_libcnotify.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The internal libcnotify header
+ * The libcnotify header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_LIBCNOTIFY_H )
-#define _LIBFVALUE_LIBCNOTIFY_H
+#if !defined( _LIBFWEVT_LIBCNOTIFY_H )
+#define _LIBFWEVT_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
-#endif
+#endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif
+#endif /* !defined( _LIBFWEVT_LIBCNOTIFY_H ) */
```

### Comparing `libfwevt-20220925/libfvalue/libfvalue_types.h` & `libfwevt-20230410/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/Makefile.am` & `libfwevt-20230410/libfvalue/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_integer.h` & `libfwevt-20230410/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_support.c` & `libfwevt-20230410/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_split_utf16_string.c` & `libfwevt-20230410/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_unused.h` & `libfwevt-20230410/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_floating_point.c` & `libfwevt-20230410/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_utf8_string.c` & `libfwevt-20230410/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_utf16_string.h` & `libfwevt-20230410/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_codepage.h` & `libfwevt-20230410/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_string.c` & `libfwevt-20230410/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_data_handle.c` & `libfwevt-20230410/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_libcdata.h` & `libfwevt-20230410/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_extern.h` & `libfwevt-20230410/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_libfdatetime.h` & `libfwevt-20230410/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_value_entry.h` & `libfwevt-20230410/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_split_utf8_string.h` & `libfwevt-20230410/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_value.h` & `libfwevt-20230410/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_binary_data.h` & `libfwevt-20230410/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_value_type.h` & `libfwevt-20230410/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_utf16_string.c` & `libfwevt-20230410/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_value_type.c` & `libfwevt-20230410/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/Makefile.in` & `libfwevt-20230410/libfvalue/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_libuna.h` & `libfwevt-20230410/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_error.c` & `libfwevt-20230410/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_error.h` & `libfwevt-20230410/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_filetime.c` & `libfwevt-20230410/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_table.c` & `libfwevt-20230410/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_libfguid.h` & `libfwevt-20230410/libfwevt/libfwevt_libfguid.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfguid header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,37 +15,35 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_LIBFGUID_H )
-#define _LIBFVALUE_LIBFGUID_H
+#if !defined( _LIBFWEVT_LIBFGUID_H )
+#define _LIBFWEVT_LIBFGUID_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBFGUID for local use of libfguid
  */
 #if defined( HAVE_LOCAL_LIBFGUID )
 
 #include <libfguid_definitions.h>
 #include <libfguid_identifier.h>
 #include <libfguid_types.h>
 
-/* Note that libfvalue does not require to have libfguid support
- */
-#elif defined( HAVE_LIBFGUID )
+#else
 
 /* If libtool DLL support is enabled set LIBFGUID_DLL_IMPORT
  * before including libfguid.h
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBFGUID_DLL_IMPORT
 #endif
 
 #include <libfguid.h>
 
 #endif /* defined( HAVE_LOCAL_LIBFGUID ) */
 
-#endif /* !defined( _LIBFVALUE_LIBFGUID_H ) */
+#endif /* !defined( _LIBFWEVT_LIBFGUID_H ) */
```

### Comparing `libfwevt-20220925/libfvalue/libfvalue_string.h` & `libfwevt-20230410/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_table.h` & `libfwevt-20230410/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_floating_point.h` & `libfwevt-20230410/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_binary_data.c` & `libfwevt-20230410/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_filetime.h` & `libfwevt-20230410/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_integer.c` & `libfwevt-20230410/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_data_handle.h` & `libfwevt-20230410/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfvalue/libfvalue_definitions.h` & `libfwevt-20230410/libfvalue/libfvalue_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/pyfwevt-python3/Makefile.am` & `libfwevt-20230410/pyfwevt-python3/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/pyfwevt-python3/Makefile.in` & `libfwevt-20230410/pyfwevt-python3/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/Makefile.in` & `libfwevt-20230410/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libuna.m4` & `libfwevt-20230410/m4/libuna.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/gettext.m4` & `libfwevt-20230410/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/tests.m4` & `libfwevt-20230410/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/lib-prefix.m4` & `libfwevt-20230410/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/ltoptions.m4` & `libfwevt-20230410/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/lib-ld.m4` & `libfwevt-20230410/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libcthreads.m4` & `libfwevt-20230410/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/lib-link.m4` & `libfwevt-20230410/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/python.m4` & `libfwevt-20230410/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libtool.m4` & `libfwevt-20230410/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/nls.m4` & `libfwevt-20230410/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libfdatetime.m4` & `libfwevt-20230410/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/host-cpu-c-abi.m4` & `libfwevt-20230410/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libcnotify.m4` & `libfwevt-20230410/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/ltversion.m4` & `libfwevt-20230410/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libcdata.m4` & `libfwevt-20230410/m4/libcdata.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20220417
+dnl Version: 20230108
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
@@ -22,15 +22,15 @@
         ])
       ],
       [dnl Check for a pkg-config file
       AS_IF(
         [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
         [PKG_CHECK_MODULES(
           [libcdata],
-          [libcdata >= 20220115],
+          [libcdata >= 20230108],
           [ac_cv_libcdata=yes],
           [ac_cv_libcdata=check])
         ])
       AS_IF(
         [test "x$ac_cv_libcdata" = xyes],
         [ac_cv_libcdata_CPPFLAGS="$pkg_cv_libcdata_CFLAGS"
         ac_cv_libcdata_LIBADD="$pkg_cv_libcdata_LIBS"])
@@ -236,19 +236,29 @@
         AC_CHECK_LIB(
           cdata,
           libcdata_list_insert_element,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
         AC_CHECK_LIB(
           cdata,
+          libcdata_list_insert_element_with_existing,
+          [ac_cv_libcdata_dummy=yes],
+          [ac_cv_libcdata=no])
+        AC_CHECK_LIB(
+          cdata,
           libcdata_list_insert_value,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
         AC_CHECK_LIB(
           cdata,
+          libcdata_list_insert_value_with_existing,
+          [ac_cv_libcdata_dummy=yes],
+          [ac_cv_libcdata=no])
+        AC_CHECK_LIB(
+          cdata,
           libcdata_list_remove_element,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         dnl List element functions
         AC_CHECK_LIB(
           cdata,
```

### Comparing `libfwevt-20220925/m4/progtest.m4` & `libfwevt-20230410/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/lt~obsolete.m4` & `libfwevt-20230410/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/po.m4` & `libfwevt-20230410/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/pthread.m4` & `libfwevt-20230410/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/common.m4` & `libfwevt-20230410/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libcerror.m4` & `libfwevt-20230410/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libfguid.m4` & `libfwevt-20230410/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/iconv.m4` & `libfwevt-20230410/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/ltsugar.m4` & `libfwevt-20230410/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/intlmacosx.m4` & `libfwevt-20230410/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/types.m4` & `libfwevt-20230410/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/m4/libfvalue.m4` & `libfwevt-20230410/m4/libfvalue.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/COPYING.LESSER` & `libfwevt-20230410/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_system.c` & `libfwevt-20230410/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_error.c` & `libfwevt-20230410/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_extern.h` & `libfwevt-20230410/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/Makefile.am` & `libfwevt-20230410/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_error.h` & `libfwevt-20230410/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_support.h` & `libfwevt-20230410/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_types.h` & `libfwevt-20230410/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_definitions.h` & `libfwevt-20230410/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_unused.h` & `libfwevt-20230410/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/Makefile.in` & `libfwevt-20230410/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_support.c` & `libfwevt-20230410/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcerror/libcerror_system.h` & `libfwevt-20230410/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_libcerror.h` & `libfwevt-20230410/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_unused.h` & `libfwevt-20230410/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_support.h` & `libfwevt-20230410/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_support.c` & `libfwevt-20230410/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/Makefile.am` & `libfwevt-20230410/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_print.c` & `libfwevt-20230410/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_verbose.c` & `libfwevt-20230410/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_stream.h` & `libfwevt-20230410/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_extern.h` & `libfwevt-20230410/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_stream.c` & `libfwevt-20230410/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/Makefile.in` & `libfwevt-20230410/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_print.h` & `libfwevt-20230410/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_verbose.h` & `libfwevt-20230410/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcnotify/libcnotify_definitions.h` & `libfwevt-20230410/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/ltmain.sh` & `libfwevt-20230410/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/compile` & `libfwevt-20230410/compile`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/config.rpath` & `libfwevt-20230410/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/depcomp` & `libfwevt-20230410/depcomp`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/en@quot.header` & `libfwevt-20230410/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/Rules-quot` & `libfwevt-20230410/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/remove-potcdate.sin` & `libfwevt-20230410/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/Makevars.in` & `libfwevt-20230410/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/en@boldquot.header` & `libfwevt-20230410/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/Makevars` & `libfwevt-20230410/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/insert-header.sin` & `libfwevt-20230410/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/po/Makefile.in.in` & `libfwevt-20230410/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcdata/libcdata_array.c` & `libfwevt-20230410/libcdata/libcdata_array.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Array functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_btree_node.c` & `libfwevt-20230410/libcdata/libcdata_btree_node.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Balanced tree node functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_tree_node.c` & `libfwevt-20230410/libcdata/libcdata_tree_node.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Tree functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_libcthreads.h` & `libfwevt-20230410/libcdata/libcdata_libcthreads.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_range_list_value.h` & `libfwevt-20230410/libcdata/libcdata_range_list_value.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Range list value
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_unused.h` & `libfwevt-20230410/libcdata/libcdata_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_range_list.h` & `libfwevt-20230410/libcdata/libcdata_range_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Range list
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/Makefile.am` & `libfwevt-20230410/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcdata/libcdata_range_list.c` & `libfwevt-20230410/libcdata/libcdata_range_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Range list
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_extern.h` & `libfwevt-20230410/libcdata/libcdata_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_support.c` & `libfwevt-20230410/libcdata/libcdata_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_list_element.h` & `libfwevt-20230410/libcdata/libcdata_list_element.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * List element functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_btree_values_list.c` & `libfwevt-20230410/libcdata/libcdata_btree_values_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Balanced tree values list functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_range_list_value.c` & `libfwevt-20230410/libcdata/libcdata_range_list_value.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Range list value
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_libcerror.h` & `libfwevt-20230410/libcdata/libcdata_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_error.c` & `libfwevt-20230410/libcdata/libcdata_error.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_error.h` & `libfwevt-20230410/libcdata/libcdata_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_support.h` & `libfwevt-20230410/libcdata/libcdata_support.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_btree_node.h` & `libfwevt-20230410/libcdata/libcdata_btree_node.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Balanced tree node functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_list.c` & `libfwevt-20230410/libcdata/libcdata_list.c`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * List functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -2102,26 +2102,74 @@
      int (*value_compare_function)(
             intptr_t *first_value,
             intptr_t *second_value,
             libcerror_error_t **error ),
      uint8_t insert_flags,
      libcerror_error_t **error )
 {
-	libcdata_internal_list_t *internal_list       = NULL;
-	libcdata_list_element_t *list_element         = NULL;
-	libcdata_list_element_t *next_element         = NULL;
-	libcdata_list_element_t *previous_element     = NULL;
-	intptr_t *value_to_insert                     = NULL;
-	static char *function                         = "libcdata_list_insert_element";
-	int element_index                             = 0;
-	int result                                    = 1;
+	libcdata_list_element_t *existing_element = NULL;
+	static char *function                     = "libcdata_list_insert_element";
+	int result                                = 0;
+
+	result = libcdata_list_insert_element_with_existing(
+	          list,
+	          element_to_insert,
+	          value_compare_function,
+	          insert_flags,
+	          &existing_element,
+	          error );
+
+	if( result == -1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_APPEND_FAILED,
+		 "%s: unable to insert element into list.",
+		 function );
+
+		return( -1 );
+	}
+	return( result );
+}
+
+/* Inserts a list element into the list
+ *
+ * Uses the value_compare_function to determine the order of the entries
+ * The value_compare_function should return LIBCDATA_COMPARE_LESS,
+ * LIBCDATA_COMPARE_EQUAL, LIBCDATA_COMPARE_GREATER if successful or -1 on error
+ *
+ * Duplicate entries are allowed by default and inserted after the last duplicate value.
+ * Only allowing unique entries can be enforced by setting the flag LIBCDATA_INSERT_FLAG_UNIQUE_ENTRIES
+ *
+ * Returns 1 if successful, 0 if the list element already exists or -1 on error
+ */
+int libcdata_list_insert_element_with_existing(
+     libcdata_list_t *list,
+     libcdata_list_element_t *element_to_insert,
+     int (*value_compare_function)(
+            intptr_t *first_value,
+            intptr_t *second_value,
+            libcerror_error_t **error ),
+     uint8_t insert_flags,
+     libcdata_list_element_t **existing_element,
+     libcerror_error_t **error )
+{
+	libcdata_internal_list_t *internal_list        = NULL;
+	libcdata_list_element_t *next_element          = NULL;
+	libcdata_list_element_t *previous_element      = NULL;
+	libcdata_list_element_t *safe_existing_element = NULL;
+	intptr_t *value_to_insert                      = NULL;
+	static char *function                          = "libcdata_list_insert_element_with_existing";
+	int element_index                              = 0;
+	int result                                     = 1;
 
 #if defined( HAVE_MULTI_THREAD_SUPPORT ) && !defined( HAVE_LOCAL_LIBCDATA )
-	libcdata_list_element_t *backup_first_element = NULL;
-	libcdata_list_element_t *backup_last_element  = NULL;
+	libcdata_list_element_t *backup_first_element  = NULL;
+	libcdata_list_element_t *backup_last_element   = NULL;
 #endif
 
 	if( list == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -2213,14 +2261,27 @@
 		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 		 "%s: unsupported insert flags: 0x%02" PRIx8 ".",
 		 function,
 		 insert_flags );
 
 		return( -1 );
 	}
+	if( existing_element == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid existing element.",
+		 function );
+
+		return( -1 );
+	}
+	*existing_element = NULL;
+
 	if( libcdata_list_element_get_elements(
 	     element_to_insert,
 	     &previous_element,
 	     &next_element,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -2270,42 +2331,47 @@
 		 "%s: unable to grab read/write lock for writing.",
 		 function );
 
 		return( -1 );
 	}
 	backup_first_element = internal_list->first_element;
 	backup_last_element  = internal_list->last_element;
-#endif
+
+#endif /* defined( HAVE_MULTI_THREAD_SUPPORT ) && !defined( HAVE_LOCAL_LIBCDATA ) */
 
 	result = libcdata_internal_list_insert_element_find_element(
 	          internal_list,
 	          value_to_insert,
 	          value_compare_function,
 	          insert_flags,
 	          &element_index,
-	          &list_element,
+	          &safe_existing_element,
 	          error );
 
 	if( result == -1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to find element in list.",
 		 function );
 
 		result = -1;
 	}
-	else if( result == 1 )
+	else if( result == 0 )
+	{
+		*existing_element = safe_existing_element;
+	}
+	else
 	{
-		if( list_element != NULL )
+		if( safe_existing_element != NULL )
 		{
 			if( libcdata_list_element_get_elements(
-			     list_element,
+			     safe_existing_element,
 			     &previous_element,
 			     &next_element,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -2317,15 +2383,15 @@
 				result = -1;
 			}
 		}
 		if( result == 1 )
 		{
 			if( libcdata_internal_list_insert_element_before_element(
 			     internal_list,
-			     list_element,
+			     safe_existing_element,
 			     element_to_insert,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_APPEND_FAILED,
@@ -2350,27 +2416,28 @@
 
 		goto on_error;
 	}
 #endif
 	return( result );
 
 #if defined( HAVE_MULTI_THREAD_SUPPORT ) && !defined( HAVE_LOCAL_LIBCDATA )
+
 on_error:
 	if( result == 1 )
 	{
 		libcdata_list_element_set_elements(
 		 element_to_insert,
 		 NULL,
 		 NULL,
 		 NULL );
 
-		if( list_element != NULL )
+		if( safe_existing_element != NULL )
 		{
 			libcdata_list_element_set_elements(
-			 list_element,
+			 safe_existing_element,
 			 previous_element,
 			 next_element,
 			 NULL );
 		}
 		else if( backup_last_element != NULL )
 		{
 			libcdata_list_element_set_next_element(
@@ -2380,15 +2447,16 @@
 		}
 		internal_list->first_element = backup_first_element;
 		internal_list->last_element  = backup_last_element;
 
 		internal_list->number_of_elements -= 1;
 	}
 	return( -1 );
-#endif
+
+#endif /* defined( HAVE_MULTI_THREAD_SUPPORT ) && !defined( HAVE_LOCAL_LIBCDATA ) */
 }
 
 /* Inserts a value to the list
  *
  * Creates a new list element
  *
  * Uses the value_compare_function to determine the order of the entries
@@ -2406,17 +2474,81 @@
      int (*value_compare_function)(
             intptr_t *first_value,
             intptr_t *second_value,
             libcerror_error_t **error ),
      uint8_t insert_flags,
      libcerror_error_t **error )
 {
-	libcdata_list_element_t *element = NULL;
-	static char *function            = "libcdata_list_insert_value";
-	int result                       = 1;
+	intptr_t *existing_value = NULL;
+	static char *function    = "libcdata_list_insert_value";
+	int result               = 0;
+
+	result = libcdata_list_insert_value_with_existing(
+	          list,
+	          value,
+	          value_compare_function,
+	          insert_flags,
+	          &existing_value,
+	          error );
+
+	if( result == -1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_APPEND_FAILED,
+		 "%s: unable to insert value into list.",
+		 function );
+
+		return( -1 );
+	}
+	return( result );
+}
+
+/* Inserts a value to the list
+ *
+ * Creates a new list element
+ *
+ * Uses the value_compare_function to determine the order of the entries
+ * The value_compare_function should return LIBCDATA_COMPARE_LESS,
+ * LIBCDATA_COMPARE_EQUAL, LIBCDATA_COMPARE_GREATER if successful or -1 on error
+ *
+ * Duplicate entries are allowed by default and inserted after the last duplicate value.
+ * Only allowing unique entries can be enforced by setting the flag LIBCDATA_INSERT_FLAG_UNIQUE_ENTRIES
+ *
+ * Returns 1 if successful, 0 if the list element already exists or -1 on error
+ */
+int libcdata_list_insert_value_with_existing(
+     libcdata_list_t *list,
+     intptr_t *value,
+     int (*value_compare_function)(
+            intptr_t *first_value,
+            intptr_t *second_value,
+            libcerror_error_t **error ),
+     uint8_t insert_flags,
+     intptr_t **existing_value,
+     libcerror_error_t **error )
+{
+	libcdata_list_element_t *element          = NULL;
+	libcdata_list_element_t *existing_element = NULL;
+	static char *function                     = "libcdata_list_insert_value_with_existing";
+	int result                                = 1;
+
+	if( existing_value == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid existing value.",
+		 function );
+
+		return( -1 );
+	}
+	*existing_value = NULL;
 
 	if( libcdata_list_element_initialize(
 	     &element,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -2437,19 +2569,20 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to set value of list element.",
 		 function );
 
 		goto on_error;
 	}
-	result = libcdata_list_insert_element(
+	result = libcdata_list_insert_element_with_existing(
 	          list,
 	          element,
 	          value_compare_function,
 	          insert_flags,
+	          &existing_element,
 	          error );
 
 	if( result == -1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -2471,14 +2604,28 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 			 "%s: unable to free list element.",
 			 function );
 
 			goto on_error;
 		}
+		if( libcdata_list_element_get_value(
+		     existing_element,
+		     existing_value,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+			 "%s: unable to retrieve value from existing list element.",
+			 function );
+
+			goto on_error;
+		}
 	}
 	return( result );
 
 on_error:
 	if( element != NULL )
 	{
 		libcdata_list_element_free(
```

### Comparing `libfwevt-20220925/libcdata/libcdata_tree_node.h` & `libfwevt-20230410/libcdata/libcdata_tree_node.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Tree functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_list.h` & `libfwevt-20230410/libcdata/libcdata_list.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * List functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -183,25 +183,49 @@
             intptr_t *first,
             intptr_t *second,
             libcerror_error_t **error ),
      uint8_t insert_flags,
      libcerror_error_t **error );
 
 LIBCDATA_EXTERN \
+int libcdata_list_insert_element_with_existing(
+     libcdata_list_t *list,
+     libcdata_list_element_t *element_to_insert,
+     int (*value_compare_function)(
+            intptr_t *first,
+            intptr_t *second,
+            libcerror_error_t **error ),
+     uint8_t insert_flags,
+     libcdata_list_element_t **existing_element,
+     libcerror_error_t **error );
+
+LIBCDATA_EXTERN \
 int libcdata_list_insert_value(
      libcdata_list_t *list,
      intptr_t *value,
      int (*value_compare_function)(
             intptr_t *first,
             intptr_t *second,
             libcerror_error_t **error ),
      uint8_t insert_flags,
      libcerror_error_t **error );
 
 LIBCDATA_EXTERN \
+int libcdata_list_insert_value_with_existing(
+     libcdata_list_t *list,
+     intptr_t *value,
+     int (*value_compare_function)(
+            intptr_t *first,
+            intptr_t *second,
+            libcerror_error_t **error ),
+     uint8_t insert_flags,
+     intptr_t **existing_value,
+     libcerror_error_t **error );
+
+LIBCDATA_EXTERN \
 int libcdata_list_remove_element(
      libcdata_list_t *list,
      libcdata_list_element_t *element_to_remove,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
```

### Comparing `libfwevt-20220925/libcdata/libcdata_types.h` & `libfwevt-20230410/libcdata/libcdata_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_list_element.c` & `libfwevt-20230410/libcdata/libcdata_list_element.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * List element functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/Makefile.in` & `libfwevt-20230410/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libcdata/libcdata_btree_values_list.h` & `libfwevt-20230410/libcdata/libcdata_btree_values_list.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Balanced tree values list functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_array.h` & `libfwevt-20230410/libcdata/libcdata_array.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Array functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_btree.h` & `libfwevt-20230410/libcdata/libcdata_btree.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Balanced tree type functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/libcdata/libcdata_definitions.h` & `libfwevt-20230410/libcdata/libcdata_definitions.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20220115
+#define LIBCDATA_VERSION				20230108
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20220115"
+#define LIBCDATA_VERSION_STRING				"20230108"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libfwevt-20220925/libcdata/libcdata_btree.c` & `libfwevt-20230410/libcdata/libcdata_btree.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Balanced tree type functions
  *
- * Copyright (C) 2006-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwevt-20220925/acinclude.m4` & `libfwevt-20230410/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/libfwevt.pc.in` & `libfwevt-20230410/libfwevt.pc.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20220925/configure.ac` & `libfwevt-20230410/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwevt],
- [20220925],
+ [20230410],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwevt.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
```

