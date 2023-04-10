# Comparing `tmp/cloudshell-snmp-autoload-1.0.3.zip` & `tmp/cloudshell-snmp-autoload-2.0.1.zip`

## zipinfo {}

```diff
@@ -1,70 +1,92 @@
-Zip file size: 38029 bytes, number of entries: 68
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/
--rw-r--r--  2.0 unx       35 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/MANIFEST.in
--rw-r--r--  2.0 unx    11358 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/LICENSE
--rw-r--r--  2.0 unx       48 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/test_requirements.txt
--rw-r--r--  2.0 unx       63 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/requirements.txt
--rw-r--r--  2.0 unx      871 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/setup.py
--rw-r--r--  2.0 unx     1096 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tox.ini
--rw-r--r--  2.0 unx      373 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/PKG-INFO
--rw-r--r--  2.0 unx      781 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/README.md
--rw-r--r--  2.0 unx       60 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/dev_requirements.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/version.txt
--rw-r--r--  2.0 unx       38 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/setup.cfg
--rw-r--r--  2.0 unx       66 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/requires.txt
--rw-r--r--  2.0 unx       17 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/top_level.txt
--rw-r--r--  2.0 unx      373 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     2091 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/__init__.py
--rw-r--r--  2.0 unx     5304 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/snmp_system_info.py
--rw-r--r--  2.0 unx     6184 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/snmp_if_table.py
--rw-r--r--  2.0 unx     7999 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/snmp_entity_table.py
--rw-r--r--  2.0 unx    11759 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/generic_snmp_autoload.py
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/__init__.py
--rw-r--r--  2.0 unx      364 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
--rw-r--r--  2.0 unx     1747 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/entity_constants.py
--rw-r--r--  2.0 unx      874 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/port_constants.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/__init__.py
--rw-r--r--  2.0 unx     1523 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/snmpv2_data.py
--rw-r--r--  2.0 unx     3044 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/snmp_port_attr_tables.py
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/__init__.py
--rw-r--r--  2.0 unx     4696 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/snmp_if_port_entity.py
--rw-r--r--  2.0 unx     1212 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/snmp_if_port_channel_entity.py
--rw-r--r--  2.0 unx     4009 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/snmp_if_entity.py
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/__init__.py
--rw-r--r--  2.0 unx      758 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/snmp_entity_element.py
--rw-r--r--  2.0 unx     3459 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/snmp_entity_base.py
--rw-r--r--  2.0 unx     4312 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/snmp_entity_struct.py
--rw-r--r--  2.0 unx        0 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/__init__.py
--rw-r--r--  2.0 unx     1179 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/entity_quali_mib_table.py
--rw-r--r--  2.0 unx      977 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
--rw-r--r--  2.0 unx        0 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/__init__.py
--rw-r--r--  2.0 unx     1883 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/port_mapper.py
--rw-r--r--  2.0 unx     2534 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/port_parent_validator.py
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/snmp_autoload_error.py
--rw-r--r--  2.0 unx      312 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/snmp_oid_template.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/cloudshell/
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/cloudshell/__init__.py
--rw-r--r--  2.0 unx      515 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/cloudshell/test_snmp_if_table.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/autoload/
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 22-Apr-18 17:34 cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/autoload/__init__.py
-68 files, 82881 bytes uncompressed, 23695 bytes compressed:  71.4%
+Zip file size: 69088 bytes, number of entries: 90
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/
+-rw-r--r--  2.0 unx    11358 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/LICENSE
+-rw-r--r--  2.0 unx      304 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/PKG-INFO
+-rw-r--r--  2.0 unx     1060 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tox.ini
+-rw-r--r--  2.0 unx      854 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/setup.py
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/dev_requirements.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/setup.cfg
+-rw-r--r--  2.0 unx      781 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/README.md
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/version.txt
+-rw-r--r--  2.0 unx       35 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/MANIFEST.in
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/requirements.txt
+-rw-r--r--  2.0 unx       55 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/test_requirements.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/requires.txt
+-rw-r--r--  2.0 unx      304 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3297 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/SOURCES.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/__init__.py
+-rw-r--r--  2.0 unx     7632 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/generic_snmp_autoload.py
+-rw-r--r--  2.0 unx      364 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/__init__.py
+-rw-r--r--  2.0 unx     1841 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/port_constants.py
+-rw-r--r--  2.0 unx     1771 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/entity_constants.py
+-rw-r--r--  2.0 unx      971 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
+-rw-r--r--  2.0 unx     7000 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_helper.py
+-rw-r--r--  2.0 unx    12017 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/module_helper.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/entity_helper.py
+-rw-r--r--  2.0 unx     2502 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_parent_validator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/__init__.py
+-rw-r--r--  2.0 unx      256 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_name_helper.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/snmp_autoload_error.py
+-rw-r--r--  2.0 unx     8359 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/__init__.py
+-rw-r--r--  2.0 unx     4935 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/system_info_table.py
+-rw-r--r--  2.0 unx    10402 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/physical_entities_table.py
+-rw-r--r--  2.0 unx     3432 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_mapping_table.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/__init__.py
+-rw-r--r--  2.0 unx     1515 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/snmpv2_data.py
+-rw-r--r--  2.0 unx     2361 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/
+-rw-r--r--  2.0 unx     1315 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py
+-rw-r--r--  2.0 unx     1019 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/__init__.py
+-rw-r--r--  2.0 unx     2892 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py
+-rw-r--r--  2.0 unx     1633 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_service_interface.py
+-rw-r--r--  2.0 unx     7295 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py
+-rw-r--r--  2.0 unx     4271 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_port_ip_tables.py
+-rw-r--r--  2.0 unx     1569 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/__init__.py
+-rw-r--r--  2.0 unx     1683 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_duplex_table.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/__init__.py
+-rw-r--r--  2.0 unx   186031 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/port_snmp_data.py
+-rw-r--r--  2.0 unx     1241 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/test_snmp_if_table.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/__init__.py
+-rw-r--r--  2.0 unx     3023 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_port_helper.py
+-rw-r--r--  2.0 unx     6305 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/__init__.py
+-rw-r--r--  2.0 unx     4657 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_module_helper.py
+-rw-r--r--  2.0 unx     3425 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
+-rw-r--r--  2.0 unx     2742 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/__init__.py
+-rw-r--r--  2.0 unx     1422 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/if_port_data.py
+-rw-r--r--  2.0 unx    93295 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/physical_entities_data.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/__init__.py
+90 files, 411648 bytes uncompressed, 48994 bytes compressed:  88.1%
```

## zipnote {}

```diff
@@ -1,205 +1,271 @@
-Filename: cloudshell-snmp-autoload-1.0.3/
+Filename: cloudshell-snmp-autoload-2.0.1/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/
+Filename: cloudshell-snmp-autoload-2.0.1/tests/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/MANIFEST.in
+Filename: cloudshell-snmp-autoload-2.0.1/LICENSE
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/LICENSE
+Filename: cloudshell-snmp-autoload-2.0.1/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/test_requirements.txt
+Filename: cloudshell-snmp-autoload-2.0.1/tox.ini
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/requirements.txt
+Filename: cloudshell-snmp-autoload-2.0.1/setup.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/setup.py
+Filename: cloudshell-snmp-autoload-2.0.1/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tox.ini
+Filename: cloudshell-snmp-autoload-2.0.1/setup.cfg
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/PKG-INFO
+Filename: cloudshell-snmp-autoload-2.0.1/README.md
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/README.md
+Filename: cloudshell-snmp-autoload-2.0.1/version.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/dev_requirements.txt
+Filename: cloudshell-snmp-autoload-2.0.1/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/version.txt
+Filename: cloudshell-snmp-autoload-2.0.1/requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/setup.cfg
+Filename: cloudshell-snmp-autoload-2.0.1/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/requires.txt
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/top_level.txt
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/PKG-INFO
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/dependency_links.txt
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/SOURCES.txt
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/snmp_system_info.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/generic_snmp_autoload.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/snmp_if_table.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/snmp_entity_table.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/generic_snmp_autoload.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/port_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/entity_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/entity_constants.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/port_constants.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/module_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/entity_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_parent_validator.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/snmpv2_data.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_name_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/snmp_port_attr_tables.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/snmp_autoload_error.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/snmp_if_port_entity.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/snmp_if_port_channel_entity.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/if_entity/snmp_if_entity.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/system_info_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/physical_entities_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/snmp_entity_element.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_mapping_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/snmp_entity_base.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/entity/snmp_entity_struct.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/entity_quali_mib_table.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/snmpv2_data.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/port_mapper.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/port_parent_validator.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/snmp_autoload_error.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/core/snmp_oid_template.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/cloudshell/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_service_interface.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/cloudshell/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/cloudshell/test_snmp_if_table.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_port_ip_tables.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/autoload/
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-1.0.3/tests/cloudshell/snmp/autoload/__init__.py
+Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_duplex_table.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/port_snmp_data.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/test_snmp_if_table.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_port_helper.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_module_helper.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/if_port_data.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/physical_entities_data.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-snmp-autoload-1.0.3/LICENSE` & `cloudshell-snmp-autoload-2.0.1/LICENSE`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-1.0.3/tox.ini` & `cloudshell-snmp-autoload-2.0.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
 envlist =
-    py{27,37,39}-{master,dev}
+    py{37,39}-{master,dev}
     pre-commit
     build
 distshare = dist
 
 [testenv]
 skip_install:
     dev: true
@@ -25,20 +25,18 @@
 deps = pre-commit
 commands = pre-commit run --all-files --show-diff-on-failure
 
 [testenv:build]
 skip_install = true
 commands =
     python setup.py -q sdist --format zip
-    python setup.py -q bdist_wheel --universal
+    python setup.py -q bdist_wheel
 
 [isort]
 profile=black
 forced_separate = cloudshell.snmp.autoload,tests
-skip = mibs
 
 [flake8]
 max-line-length = 88
 ;we don't need have docstrings in every func, class and package
 ;and W503 is not PEP 8 compliant
-ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203
-exclude = mibs
+ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203,E501
```

## Comparing `cloudshell-snmp-autoload-1.0.3/README.md` & `cloudshell-snmp-autoload-2.0.1/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-1.0.3/cloudshell_snmp_autoload.egg-info/SOURCES.txt` & `cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,44 +7,62 @@
 test_requirements.txt
 tox.ini
 version.txt
 cloudshell/__init__.py
 cloudshell/snmp/__init__.py
 cloudshell/snmp/autoload/__init__.py
 cloudshell/snmp/autoload/generic_snmp_autoload.py
-cloudshell/snmp/autoload/snmp_entity_table.py
-cloudshell/snmp/autoload/snmp_if_table.py
-cloudshell/snmp/autoload/snmp_system_info.py
 cloudshell/snmp/autoload/constants/__init__.py
 cloudshell/snmp/autoload/constants/entity_constants.py
 cloudshell/snmp/autoload/constants/port_constants.py
 cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
-cloudshell/snmp/autoload/core/__init__.py
-cloudshell/snmp/autoload/core/snmp_autoload_error.py
-cloudshell/snmp/autoload/core/snmp_oid_template.py
-cloudshell/snmp/autoload/domain/__init__.py
-cloudshell/snmp/autoload/domain/snmp_port_attr_tables.py
-cloudshell/snmp/autoload/domain/snmpv2_data.py
-cloudshell/snmp/autoload/domain/entity/__init__.py
-cloudshell/snmp/autoload/domain/entity/snmp_entity_base.py
-cloudshell/snmp/autoload/domain/entity/snmp_entity_element.py
-cloudshell/snmp/autoload/domain/entity/snmp_entity_struct.py
-cloudshell/snmp/autoload/domain/if_entity/__init__.py
-cloudshell/snmp/autoload/domain/if_entity/snmp_if_entity.py
-cloudshell/snmp/autoload/domain/if_entity/snmp_if_port_channel_entity.py
-cloudshell/snmp/autoload/domain/if_entity/snmp_if_port_entity.py
+cloudshell/snmp/autoload/exceptions/__init__.py
+cloudshell/snmp/autoload/exceptions/snmp_autoload_error.py
 cloudshell/snmp/autoload/helper/__init__.py
-cloudshell/snmp/autoload/helper/entity_quali_mib_table.py
+cloudshell/snmp/autoload/helper/entity_helper.py
+cloudshell/snmp/autoload/helper/module_helper.py
+cloudshell/snmp/autoload/helper/port_helper.py
+cloudshell/snmp/autoload/helper/port_name_helper.py
+cloudshell/snmp/autoload/helper/port_parent_validator.py
 cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
-cloudshell/snmp/autoload/service/__init__.py
-cloudshell/snmp/autoload/service/port_mapper.py
-cloudshell/snmp/autoload/service/port_parent_validator.py
+cloudshell/snmp/autoload/services/__init__.py
+cloudshell/snmp/autoload/services/physical_entities_table.py
+cloudshell/snmp/autoload/services/port_mapping_table.py
+cloudshell/snmp/autoload/services/port_table.py
+cloudshell/snmp/autoload/services/system_info_table.py
+cloudshell/snmp/autoload/snmp/__init__.py
+cloudshell/snmp/autoload/snmp/snmpv2_data.py
+cloudshell/snmp/autoload/snmp/entities/__init__.py
+cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py
+cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py
+cloudshell/snmp/autoload/snmp/tables/__init__.py
+cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py
+cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py
+cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py
+cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/__init__.py
+cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py
+cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_port_ip_tables.py
+cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py
+cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_duplex_table.py
+cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py
+cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_service_interface.py
 cloudshell_snmp_autoload.egg-info/PKG-INFO
 cloudshell_snmp_autoload.egg-info/SOURCES.txt
 cloudshell_snmp_autoload.egg-info/dependency_links.txt
 cloudshell_snmp_autoload.egg-info/requires.txt
 cloudshell_snmp_autoload.egg-info/top_level.txt
 tests/__init__.py
 tests/cloudshell/__init__.py
-tests/cloudshell/test_snmp_if_table.py
 tests/cloudshell/snmp/__init__.py
-tests/cloudshell/snmp/autoload/__init__.py
+tests/cloudshell/snmp/port_snmp_data.py
+tests/cloudshell/snmp/test_snmp_if_table.py
+tests/cloudshell/snmp/autoload/__init__.py
+tests/cloudshell/snmp/autoload/data/__init__.py
+tests/cloudshell/snmp/autoload/data/if_port_data.py
+tests/cloudshell/snmp/autoload/data/physical_entities_data.py
+tests/cloudshell/snmp/autoload/helper/__init__.py
+tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
+tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
+tests/cloudshell/snmp/autoload/helper/test_module_helper.py
+tests/cloudshell/snmp/autoload/helper/test_port_helper.py
+tests/cloudshell/snmp/autoload/services/__init__.py
+tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
```

## Comparing `cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/snmp_system_info.py` & `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/system_info_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import re
 
-from cloudshell.shell.flows.autoload.autoload_utils import get_device_name
+from cloudshell.snmp.autoload.snmp.snmpv2_data import SnmpV2MibData
 
-from cloudshell.snmp.autoload.domain.snmpv2_data import SnmpV2MibData
 
-
-class SnmpSystemInfo(object):
+class SnmpSystemInfo:
     DEVICE_MODEL_PATTERN = re.compile(r"::(?P<model>\S+$)")
     VENDOR_OID_PATTERN = re.compile(r"1.3.6.1.4.1.\d+")
     OS_VERSION_PATTERN = re.compile(r"Version (?P<os_version>[^\s,]+)")
 
     def __init__(self, snmp_handler, logger, vendor=None):
         self._vendor = vendor
         self._snmp_handler = snmp_handler
@@ -49,25 +47,23 @@
             )
         if isinstance(supported_os_pattern, list):
             supported_os_pattern = re.compile(
                 "|".join(supported_os_pattern), re.IGNORECASE | re.DOTALL
             )
 
         system_description = self._snmp_v2_obj.get_system_description()
-        self._logger.debug(
-            "Detected system description: '{0}'".format(system_description)
-        )
+        self._logger.debug(f"Detected system description: '{system_description}'")
         if system_description:
             result = supported_os_pattern.search(str(system_description))
 
             if result:
                 return True
             else:
                 error_message = (
-                    "Incompatible driver! Please use this driver for '{0}' "
+                    "Incompatible driver! Please use this driver for '{}' "
                     "operation system(s)".format(supported_os_pattern.pattern)
                 )
         else:
             error_message = "Unable to identify device firmware type"
 
         self._logger.error(error_message)
         return False
@@ -90,15 +86,15 @@
         """Get device model from the SNMPv2 mib.
 
         :return: device model
         :rtype: str
         """
         if not self._vendor:
             sys_obj_id = self._snmp_v2_obj.get_system_object_id()
-            sys_obj_id_oid = ".".join(map(str, sys_obj_id.raw_value))
+            sys_obj_id_oid = str(sys_obj_id.raw_value)
             oid_match = self.VENDOR_OID_PATTERN.search(sys_obj_id_oid)
             if oid_match:
                 self._vendor = self._snmp_handler.translate_oid(
                     oid_match.group()
                 ).capitalize()
 
         return self._vendor
@@ -128,19 +124,12 @@
         resource.system_name = self._snmp_v2_obj.get_system_name()
         resource.location = self._snmp_v2_obj.get_system_location()
         resource.os_version = self._get_device_os_version()
         vendor = self._get_vendor()
         resource.vendor = vendor
 
         raw_model = self._get_device_model()
-        model = re.sub(r"^{}".format(vendor), "", raw_model, flags=re.IGNORECASE)
-        resource.model = model
-        resource.model_name = self._get_model_name(raw_model)
+        model = re.sub(rf"^{vendor}", "", raw_model, flags=re.IGNORECASE)
+        resource.model = model.capitalize()
+        resource.model_name = model.capitalize()
 
         self._logger.info("Building Root completed")
-
-    def _get_model_name(self, model):
-        if self._device_model_map_path:
-            return (
-                get_device_name(file_name=self._device_model_map_path, sys_obj_id=model)
-                or model
-            )
```

## Comparing `cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/constants/entity_constants.py` & `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/entity_constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import re
-from collections import OrderedDict
 
 from cloudshell.snmp.core.domain.snmp_oid import SnmpMibObject
 
-from cloudshell.snmp.autoload.core.snmp_oid_template import SnmpMibOidTemplate
-
 ENTITY_VALID_CLASS_PATTERN = re.compile(
     r"stack|chassis|module|port|powerSupply|container|backplane"
 )
 
-ENTITY_POSITION = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalParentRelPos")
-ENTITY_DESCRIPTION = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalDescr")
-ENTITY_NAME = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalName")
-ENTITY_PARENT_ID = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalContainedIn")
-ENTITY_CLASS = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalClass")
-ENTITY_VENDOR_TYPE = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalVendorType")
-ENTITY_MODEL = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalModelName")
-ENTITY_SERIAL = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalSerialNum")
-ENTITY_OS_VERSION = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalSoftwareRev")
-ENTITY_HW_VERSION = SnmpMibOidTemplate("ENTITY-MIB", "entPhysicalHardwareRev")
-# ENTITY_TO_IF_ID = SnmpMibOidTemplate("ENTITY-MIB", "entAliasMappingIdentifier") # noqa: E501
+CONTAINER_MATCH_PATTERN = re.compile(r"^\S+container", re.IGNORECASE)
+CHASSIS_MATCH_PATTERN = re.compile(r"^\S+chassis", re.IGNORECASE)
+MODULE_MATCH_PATTERN = re.compile(r"^\S+module", re.IGNORECASE)
+PORT_MATCH_PATTERN = re.compile(r"^\S+port", re.IGNORECASE)
+POWER_SUPPLY_MATCH_PATTERN = re.compile(r"^\S+powersupply", re.IGNORECASE)
+
+ENTITY_VENDOR_TYPE_TO_CLASS_MAP = {
+    CONTAINER_MATCH_PATTERN: "container",
+    CHASSIS_MATCH_PATTERN: "chassis",
+    MODULE_MATCH_PATTERN: "module",
+    PORT_MATCH_PATTERN: "port",
+    POWER_SUPPLY_MATCH_PATTERN: "powerSupply",
+}
+
+ENTITY_POSITION = SnmpMibObject("ENTITY-MIB", "entPhysicalParentRelPos")
+ENTITY_DESCRIPTION = SnmpMibObject("ENTITY-MIB", "entPhysicalDescr")
+ENTITY_NAME = SnmpMibObject("ENTITY-MIB", "entPhysicalName")
+ENTITY_PARENT_ID = SnmpMibObject("ENTITY-MIB", "entPhysicalContainedIn")
+ENTITY_CLASS = SnmpMibObject("ENTITY-MIB", "entPhysicalClass")
+ENTITY_VENDOR_TYPE = SnmpMibObject("ENTITY-MIB", "entPhysicalVendorType")
+ENTITY_MODEL = SnmpMibObject("ENTITY-MIB", "entPhysicalModelName")
+ENTITY_SERIAL = SnmpMibObject("ENTITY-MIB", "entPhysicalSerialNum")
+ENTITY_OS_VERSION = SnmpMibObject("ENTITY-MIB", "entPhysicalSoftwareRev")
+ENTITY_HW_VERSION = SnmpMibObject("ENTITY-MIB", "entPhysicalHardwareRev")
 ENTITY_TO_IF_ID = SnmpMibObject("ENTITY-MIB", "entAliasMappingIdentifier")
 
-ENTITY_VENDOR_TYPE_TO_CLASS_MAP = OrderedDict(
-    [
-        (re.compile(r"^\S+container", re.IGNORECASE), "container"),
-        (re.compile(r"^\S+chassis", re.IGNORECASE), "chassis"),
-        (re.compile(r"^\S+module", re.IGNORECASE), "module"),
-        (re.compile(r"^\S+port", re.IGNORECASE), "port"),
-        (re.compile(r"^\S+powersupply", re.IGNORECASE), "powerSupply"),
-    ]
-)
-
-
-ENTITY_TO_CONTAINER_PATTERN = re.compile(
-    r"powershelf|^\S+sfp|^\S+xfr|^\S+xfp|"
-    r"^\S+Container10GigBasePort|^\S+ModulePseAsicPlim"
-)
+ENTITY_TABLE_REQUIRED_COLUMNS = [
+    ENTITY_POSITION,
+    ENTITY_DESCRIPTION,
+    ENTITY_NAME,
+    ENTITY_PARENT_ID,
+    ENTITY_CLASS,
+    ENTITY_VENDOR_TYPE,
+    ENTITY_MODEL,
+    ENTITY_SERIAL,
+    ENTITY_OS_VERSION,
+    ENTITY_HW_VERSION,
+]
```

## Comparing `cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/domain/snmpv2_data.py` & `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/snmpv2_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cloudshell.snmp.autoload.constants import snmpv_v2_constants
 
 
-class SnmpV2MibData(object):
+class SnmpV2MibData:
     def __init__(self, snmp_handler, logger):
         self._snmp_handler = snmp_handler
         self._logger = logger
         self._sys_descr = ""
         self._sys_location = None
         self._sys_contact = None
         self._sys_object_id = None
```

## Comparing `cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py` & `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
     :param autoload_details:
     :return:
     """
     logger.debug("-------------------- <RESOURCES> ----------------------")
     for resource in autoload_details.resources:
         logger.debug(
-            "{0:15}, {1:20}, {2}".format(
+            "{:15}, {:20}, {}".format(
                 str(resource.relative_address),
                 resource.name,
                 resource.unique_identifier,
             )
         )
     logger.debug("-------------------- </RESOURCES> ----------------------")
 
     logger.debug("-------------------- <ATTRIBUTES> ---------------------")
     for attribute in autoload_details.attributes:
         logger.debug(
-            "-- {0:15}, {1:60}, {2}".format(
+            "-- {:15}, {:60}, {}".format(
                 str(attribute.relative_address),
                 attribute.attribute_name,
                 attribute.attribute_value,
             )
         )
     logger.debug("-------------------- </ATTRIBUTES> ---------------------")
```

## Comparing `cloudshell-snmp-autoload-1.0.3/cloudshell/snmp/autoload/service/port_parent_validator.py` & `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_parent_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import re
 
 
-class PortParentValidator(object):
+class PortParentValidator:
     MIN_PORT_ID_LENGTH = 3  # Skipping Port names with less then 3 digits
 
     def __init__(self, logger):
         self._logger = logger
 
     def validate_port_parent_ids(self, port):
         name = port.if_entity.if_name or port.if_entity.if_descr_name
-        self._logger.debug("Start port {} parent modules id validation".format(name))
+        self._logger.debug(f"Start port {name} parent modules id validation")
         parent_ids = port.parent.full_id  # ["0", "11"]
         parent_ids_list = parent_ids.split("/")
         if re.search(parent_ids, name, re.IGNORECASE):
-            self._logger.debug("Port {} parent modules ids are valid.".format(name))
+            self._logger.debug(f"Port {name} parent modules ids are valid.")
             return
         else:
             parent_ids_from_port_match = re.search(r"\d+(/\d+)*$", name, re.IGNORECASE)
             if parent_ids_from_port_match:
                 parent_ids_from_port = (
                     parent_ids_from_port_match.group()
                 )  # ["0", "7", "0", "0"]
@@ -25,15 +25,15 @@
                 if len(parent_ids_from_port_list) > len(parent_ids_list):  # > 1:
                     parent_ids_from_port_list = parent_ids_from_port_list[
                         : len(parent_ids_list)
                     ]  # ["0", "7"]
 
                     self._set_port_parent_ids(port, parent_ids_from_port_list)
                     self._logger.debug(
-                        "Completed port {} parent modules id validation".format(name)
+                        f"Completed port {name} parent modules id validation"
                     )
                 else:
                     self._logger.debug(
                         "Failed to validate port {} parent modules ids. "
                         "Skipping.".format(name)
                     )
```

