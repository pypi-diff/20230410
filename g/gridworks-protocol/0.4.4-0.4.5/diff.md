# Comparing `tmp/gridworks_protocol-0.4.4.tar.gz` & `tmp/gridworks_protocol-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.4.4.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.4.5.tar", max compression
```

## Comparing `gridworks_protocol-0.4.4.tar` & `gridworks_protocol-0.4.5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1070 2023-04-10 11:44:26.168876 gridworks_protocol-0.4.4/LICENSE
--rw-r--r--   0        0        0     2552 2023-04-10 11:44:26.168876 gridworks_protocol-0.4.4/README.md
--rw-r--r--   0        0        0     2287 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/__init__.py
--rw-r--r--   0        0        0     6610 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/api_types.py
--rw-r--r--   0        0        0     1339 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0     1488 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      995 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1112 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/relay_cac.py
--rw-r--r--   0        0        0     1118 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0     1580 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0     1388 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1094 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1659 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0     1479 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1357 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1267 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/relay_component.py
--rw-r--r--   0        0        0     1465 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0     1308 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      165 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    14718 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0     1957 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    12051 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/decoders.py
--rw-r--r--   0        0        0      451 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     3583 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     1119 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0     2657 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     3480 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     1823 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     1148 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0       89 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      464 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      446 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3168 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3058 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0     4045 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/topic.py
--rw-r--r--   0        0        0     6632 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0     5474 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0     6119 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0    10192 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     3892 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     3603 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    21265 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    13413 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0     7187 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_boolean_actuator_component.py
--rw-r--r--   0        0        0     8451 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     5798 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     4973 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     5584 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     5327 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    12792 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11884 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    13663 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    12350 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8389 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0     9471 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0    21597 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0     9935 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    11300 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0     7622 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     2761 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0    11124 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/relay_cac_gt.py
--rw-r--r--   0        0        0     7616 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/relay_component_gt.py
--rw-r--r--   0        0        0    11736 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0     8096 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0    20796 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0     7280 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     6007 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    18344 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    14059 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    12227 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     2556 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/utils.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.4/setup.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-10 13:49:57.918573 gridworks_protocol-0.4.5/LICENSE
+-rw-r--r--   0        0        0     2552 2023-04-10 13:49:57.918573 gridworks_protocol-0.4.5/README.md
+-rw-r--r--   0        0        0     2287 2023-04-10 13:50:09.642840 gridworks_protocol-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     6610 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/api_types.py
+-rw-r--r--   0        0        0     1339 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0     1488 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      995 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1112 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/relay_cac.py
+-rw-r--r--   0        0        0     1118 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0     1580 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0     1388 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1094 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1659 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0     1479 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1357 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1267 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/relay_component.py
+-rw-r--r--   0        0        0     1465 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0     1308 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      165 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    14718 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0     1957 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    12051 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/decoders.py
+-rw-r--r--   0        0        0      451 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     3486 2023-04-10 13:50:09.642840 gridworks_protocol-0.4.5/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     1119 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0     2657 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     3480 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     1823 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     1148 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0       89 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      464 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      446 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3168 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3058 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0     4045 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/topic.py
+-rw-r--r--   0        0        0     6632 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0     5474 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0     6119 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0    10192 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     3892 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     3603 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    21265 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    13413 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     7187 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_boolean_actuator_component.py
+-rw-r--r--   0        0        0     8451 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0     5798 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     4973 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     5584 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     5327 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    12792 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11884 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    13663 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    12350 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8389 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0     9471 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0    21597 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0     9935 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    11300 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7622 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     2761 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0    11124 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/relay_cac_gt.py
+-rw-r--r--   0        0        0     7616 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/relay_component_gt.py
+-rw-r--r--   0        0        0    11736 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0     8096 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0    20796 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7280 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     6007 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    18219 2023-04-10 13:50:09.642840 gridworks_protocol-0.4.5/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    14059 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    12227 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     2556 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/utils.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.5/setup.py
+-rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.5/PKG-INFO
```

### Comparing `gridworks_protocol-0.4.4/LICENSE` & `gridworks_protocol-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/README.md` & `gridworks_protocol-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/pyproject.toml` & `gridworks_protocol-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.4.4"
+version = "0.4.5"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
```

### Comparing `gridworks_protocol-0.4.4/src/gwproto/__init__.py` & `gridworks_protocol-0.4.5/src/gwproto/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/api_types.py` & `gridworks_protocol-0.4.5/src/gwproto/api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/relay_cac.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/relay_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/component_attribute_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/relay_component.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/relay_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/hardware_layout.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.4.5/src/gwproto/data_classes/sh_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/decoders.py` & `gridworks_protocol-0.4.5/src/gwproto/decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.4.5/src/gwproto/enums/actor_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,24 @@
       * HomeAlone (32d3d19f, 000): HomeAlone is an abstract Spaceheat Actor responsible for dispatching the SCADA when it is not talking with the AtomicTNode.
       * BooleanActuator (fddd0064, 000): A SpaceheatNode representing a generic boolean actuator capable of turning on (closing a circuit) or turning off (opening a circuit).
       * PowerMeter (2ea112b9, 000): A SpaceheatNode representing the power meter that is used to settle financial transactions with the TerminalAsset. That is, this is the power meter whose accuracy is certified in the creation of the TerminalAsset GNode via creation of the TaDeed.. [More Info](https://gridworks.readthedocs.io/en/latest/terminal-asset.html).
       * Atn (b103058f, 000): A SpaceheatNode representing the AtomicTNode. Note that the code running the AtomicTNode is not local within the SCADA code, except for a stub used for testing purposes.. [More Info](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html).
       * SimpleSensor (dae4b2f0, 000): A SpaceheatNode representing a sensor that measures a single category of quantity (for example, temperature) for a single object (for example, on a pipe).. [More Info](https://gridworks-protocol.readthedocs.io/en/latest/simple-sensor.html).
       * MultipurposeSensor (7c483ad0, 000): A sensor that either reads multiple kinds of readings from the same sensing device (for example reads current and voltage), reads multiple different objects (temperature from two different thermisters) or both.. [More Info](https://gridworks-protocol.readthedocs.io/en/latest/multipurpose-sensor.html).
       * Thermostat (4a9c1785, 000): A SpaceheatNode representing a thermostat.
-      * Relay (311835f6, 001): A SpaceheatNode representing an electric relay
     """
     NoActor = auto()
     Scada = auto()
     HomeAlone = auto()
     BooleanActuator = auto()
     PowerMeter = auto()
     Atn = auto()
     SimpleSensor = auto()
     MultipurposeSensor = auto()
     Thermostat = auto()
-    Relay = auto()
     
     @classmethod
     def default(cls) -> "ActorClass":
         """
         Returns default value NoActor
         """
         return cls.NoActor
```

### Comparing `gridworks_protocol-0.4.4/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.4.5/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.4.5/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/enums/role.py` & `gridworks_protocol-0.4.5/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.4.5/src/gwproto/enums/telemetry_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/enums/unit.py` & `gridworks_protocol-0.4.5/src/gwproto/enums/unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/message.py` & `gridworks_protocol-0.4.5/src/gwproto/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.4.5/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/messages/event.py` & `gridworks_protocol-0.4.5/src/gwproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/messages/misc.py` & `gridworks_protocol-0.4.5/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/property_format.py` & `gridworks_protocol-0.4.5/src/gwproto/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/topic.py` & `gridworks_protocol-0.4.5/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/__init__.py` & `gridworks_protocol-0.4.5/src/gwproto/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/component_attribute_class_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.4.5/src/gwproto/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.4.5/src/gwproto/types/egauge_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.4.5/src/gwproto/types/egauge_register_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_boolean_actuator_component.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_boolean_actuator_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.4.5/src/gwproto/types/gt_telemetry.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.4.5/src/gwproto/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.4.5/src/gwproto/types/power_watts.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/relay_cac_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/relay_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/relay_component_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/relay_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_component_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.4.5/src/gwproto/types/snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.4.5/src/gwproto/types/spaceheat_node_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         "32d3d19f",
         "fddd0064",
         "2ea112b9",
         "b103058f",
         "dae4b2f0",
         "7c483ad0",
         "4a9c1785",
-        "311835f6",
     ]
 
     @classmethod
     def is_symbol(cls, candidate: str) -> bool:
         if candidate in cls.symbols:
             return True
         return False
@@ -47,15 +46,14 @@
     HomeAlone = auto()
     BooleanActuator = auto()
     PowerMeter = auto()
     Atn = auto()
     SimpleSensor = auto()
     MultipurposeSensor = auto()
     Thermostat = auto()
-    Relay = auto()
 
     @classmethod
     def default(cls) -> "ShActorClass000":
         return cls.NoActor
 
     @classmethod
     def values(cls) -> List[str]:
@@ -85,28 +83,26 @@
         "32d3d19f": ShActorClass000.HomeAlone,
         "fddd0064": ShActorClass000.BooleanActuator,
         "2ea112b9": ShActorClass000.PowerMeter,
         "b103058f": ShActorClass000.Atn,
         "dae4b2f0": ShActorClass000.SimpleSensor,
         "7c483ad0": ShActorClass000.MultipurposeSensor,
         "4a9c1785": ShActorClass000.Thermostat,
-        "311835f6": ShActorClass000.Relay,
     }
 
     versioned_enum_to_type_dict: Dict[ShActorClass000, str] = {
         ShActorClass000.NoActor: "00000000",
         ShActorClass000.Scada: "6d37aa41",
         ShActorClass000.HomeAlone: "32d3d19f",
         ShActorClass000.BooleanActuator: "fddd0064",
         ShActorClass000.PowerMeter: "2ea112b9",
         ShActorClass000.Atn: "b103058f",
         ShActorClass000.SimpleSensor: "dae4b2f0",
         ShActorClass000.MultipurposeSensor: "7c483ad0",
         ShActorClass000.Thermostat: "4a9c1785",
-        ShActorClass000.Relay: "311835f6",
     }
 
 
 class ShNodeRole000SchemaEnum:
     enum_name: str = "sh.node.role.000"
     symbols: List[str] = [
         "00000000",
```

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.4.5/src/gwproto/types/telemetry_reporting_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.4.5/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/src/gwproto/utils.py` & `gridworks_protocol-0.4.5/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.4/setup.py` & `gridworks_protocol-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 install_requires = \
 ['fastapi-utils>=0.2.1,<0.3.0',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'gridworks-protocol',
-    'version': '0.4.4',
+    'version': '0.4.5',
     'description': 'Gridworks Protocol',
     'long_description': "# Gridworks Protocol\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-protocol.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/gridworks-protocol.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-protocol)][python version]\n[![License](https://img.shields.io/pypi/l/gridworks-protocol)][license]\n\n[![Read the documentation at https://gridworks-protocol.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-protocol/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-protocol/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-protocol/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/gridworks-protocol/\n[status]: https://pypi.org/project/gridworks-protocol/\n[python version]: https://pypi.org/project/gridworks-protocol\n[read the docs]: https://gridworks-protocol.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-protocol/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-protocol\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Gridworks Protocol_ via [pip] from [PyPI]:\n\n```console\n$ pip install gridworks-protocol\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Gridworks Protocol_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-protocol/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-protocol/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-protocol/blob/main/CONTRIBUTING.md\n",
     'author': 'Jessica Millar',
     'author_email': 'jmillar@gridworks-consulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegridelectric/gridworks-protocol',
```

### Comparing `gridworks_protocol-0.4.4/PKG-INFO` & `gridworks_protocol-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.4.4
+Version: 0.4.5
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```
