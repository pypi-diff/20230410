# Comparing `tmp/gridworks_protocol-0.4.3.tar.gz` & `tmp/gridworks_protocol-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.4.3.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.4.4.tar", max compression
```

## Comparing `gridworks_protocol-0.4.3.tar` & `gridworks_protocol-0.4.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1070 2023-04-09 21:31:14.387178 gridworks_protocol-0.4.3/LICENSE
--rw-r--r--   0        0        0     2552 2023-04-09 21:31:14.387178 gridworks_protocol-0.4.3/README.md
--rw-r--r--   0        0        0     2287 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/__init__.py
--rw-r--r--   0        0        0     6695 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/api_types.py
--rw-r--r--   0        0        0     1152 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/boolean_actuator_cac.py
--rw-r--r--   0        0        0     1339 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0     1488 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      995 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1118 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0     1580 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0     1388 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1094 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1348 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/boolean_actuator_component.py
--rw-r--r--   0        0        0     1659 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0     1479 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1357 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1465 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0     1308 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      165 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    14778 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0     1957 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    12051 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/decoders.py
--rw-r--r--   0        0        0      451 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     3462 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     1119 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0     2657 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     3480 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     1823 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     1148 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0       89 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      464 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      446 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3168 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3058 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0     4045 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/topic.py
--rw-r--r--   0        0        0     6756 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0    11376 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/types/boolean_actuator_cac_gt.py
--rw-r--r--   0        0        0     7878 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/types/boolean_actuator_component_gt.py
--rw-r--r--   0        0        0     5474 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0     6119 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0    10192 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     3892 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     3603 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    21265 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    13413 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0     7187 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_boolean_actuator_component.py
--rw-r--r--   0        0        0     8451 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     5798 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     4973 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     5584 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     5327 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    12792 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11884 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    13663 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    12350 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8389 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0     9471 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0    21597 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0     9935 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    11300 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0     7622 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     2761 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0    11736 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0     8096 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0    20796 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0     7280 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     6007 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    18219 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    14059 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    12227 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     2556 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/utils.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.3/setup.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-10 11:44:26.168876 gridworks_protocol-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2552 2023-04-10 11:44:26.168876 gridworks_protocol-0.4.4/README.md
+-rw-r--r--   0        0        0     2287 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     6610 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/api_types.py
+-rw-r--r--   0        0        0     1339 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0     1488 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      995 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1112 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/relay_cac.py
+-rw-r--r--   0        0        0     1118 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0     1580 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0     1388 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1094 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1659 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0     1479 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1357 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1267 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/relay_component.py
+-rw-r--r--   0        0        0     1465 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0     1308 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      165 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    14718 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0     1957 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    12051 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/decoders.py
+-rw-r--r--   0        0        0      451 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     3583 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     1119 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0     2657 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     3480 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     1823 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     1148 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0       89 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      464 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      446 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3168 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3058 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0     4045 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2023-04-10 11:44:26.172876 gridworks_protocol-0.4.4/src/gwproto/topic.py
+-rw-r--r--   0        0        0     6632 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0     5474 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0     6119 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0    10192 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     3892 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     3603 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    21265 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    13413 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     7187 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_boolean_actuator_component.py
+-rw-r--r--   0        0        0     8451 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0     5798 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     4973 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     5584 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     5327 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    12792 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11884 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    13663 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    12350 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8389 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0     9471 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0    21597 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0     9935 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    11300 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7622 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     2761 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0    11124 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/relay_cac_gt.py
+-rw-r--r--   0        0        0     7616 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/relay_component_gt.py
+-rw-r--r--   0        0        0    11736 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0     8096 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0    20796 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7280 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     6007 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    18344 2023-04-10 11:44:39.702179 gridworks_protocol-0.4.4/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    14059 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    12227 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     2556 2023-04-10 11:44:26.176877 gridworks_protocol-0.4.4/src/gwproto/utils.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.4/setup.py
+-rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.4/PKG-INFO
```

### Comparing `gridworks_protocol-0.4.3/LICENSE` & `gridworks_protocol-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/README.md` & `gridworks_protocol-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/pyproject.toml` & `gridworks_protocol-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.4.3"
+version = "0.4.4"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/__init__.py` & `gridworks_protocol-0.4.4/src/gwproto/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/api_types.py` & `gridworks_protocol-0.4.4/src/gwproto/api_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """ List of all the types used"""
 from typing import Dict
 from typing import List
 from typing import no_type_check
 
-from gwproto.types import BooleanActuatorCacGt_Maker
-from gwproto.types import BooleanActuatorComponentGt_Maker
 from gwproto.types import ComponentAttributeClassGt_Maker
 from gwproto.types import ComponentGt_Maker
 from gwproto.types import DataChannel_Maker
 from gwproto.types import EgaugeIo_Maker
 from gwproto.types import EgaugeRegisterConfig_Maker
 from gwproto.types import ElectricMeterCacGt_Maker
 from gwproto.types import ElectricMeterComponentGt_Maker
@@ -24,14 +22,16 @@
 from gwproto.types import GtTelemetry_Maker
 from gwproto.types import HeartbeatB_Maker
 from gwproto.types import MultipurposeSensorCacGt_Maker
 from gwproto.types import MultipurposeSensorComponentGt_Maker
 from gwproto.types import PipeFlowSensorCacGt_Maker
 from gwproto.types import PipeFlowSensorComponentGt_Maker
 from gwproto.types import PowerWatts_Maker
+from gwproto.types import RelayCacGt_Maker
+from gwproto.types import RelayComponentGt_Maker
 from gwproto.types import ResistiveHeaterCacGt_Maker
 from gwproto.types import ResistiveHeaterComponentGt_Maker
 from gwproto.types import SimpleTempSensorCacGt_Maker
 from gwproto.types import SimpleTempSensorComponentGt_Maker
 from gwproto.types import SnapshotSpaceheat_Maker
 from gwproto.types import SpaceheatNodeGt_Maker
 from gwproto.types import TelemetryReportingConfig_Maker
@@ -40,16 +40,14 @@
 
 TypeMakerByName: Dict[str, HeartbeatB_Maker] = {}
 
 
 @no_type_check
 def type_makers() -> List[HeartbeatB_Maker]:
     return [
-        BooleanActuatorCacGt_Maker,
-        BooleanActuatorComponentGt_Maker,
         ComponentAttributeClassGt_Maker,
         ComponentGt_Maker,
         DataChannel_Maker,
         EgaugeIo_Maker,
         EgaugeRegisterConfig_Maker,
         ElectricMeterCacGt_Maker,
         ElectricMeterComponentGt_Maker,
@@ -65,14 +63,16 @@
         GtTelemetry_Maker,
         HeartbeatB_Maker,
         MultipurposeSensorCacGt_Maker,
         MultipurposeSensorComponentGt_Maker,
         PipeFlowSensorCacGt_Maker,
         PipeFlowSensorComponentGt_Maker,
         PowerWatts_Maker,
+        RelayCacGt_Maker,
+        RelayComponentGt_Maker,
         ResistiveHeaterCacGt_Maker,
         ResistiveHeaterComponentGt_Maker,
         SimpleTempSensorCacGt_Maker,
         SimpleTempSensorComponentGt_Maker,
         SnapshotSpaceheat_Maker,
         SpaceheatNodeGt_Maker,
         TelemetryReportingConfig_Maker,
@@ -87,16 +87,14 @@
 def version_by_type_name() -> Dict[str, str]:
     """
     Returns:
         Dict[str, str]: Keys are TypeNames, values are versions
     """
 
     v: Dict[str, str] = {
-        "boolean.actuator.cac.gt": "000",
-        "boolean.actuator.component.gt": "000",
         "component.attribute.class.gt": "000",
         "component.gt": "000",
         "data.channel": "000",
         "egauge.io": "000",
         "egauge.register.config": "000",
         "electric.meter.cac.gt": "000",
         "electric.meter.component.gt": "000",
@@ -112,14 +110,16 @@
         "gt.telemetry": "110",
         "heartbeat.b": "001",
         "multipurpose.sensor.cac.gt": "000",
         "multipurpose.sensor.component.gt": "000",
         "pipe.flow.sensor.cac.gt": "000",
         "pipe.flow.sensor.component.gt": "000",
         "power.watts": "000",
+        "relay.cac.gt": "000",
+        "relay.component.gt": "000",
         "resistive.heater.cac.gt": "000",
         "resistive.heater.component.gt": "000",
         "simple.temp.sensor.cac.gt": "000",
         "simple.temp.sensor.component.gt": "000",
         "snapshot.spaceheat": "000",
         "spaceheat.node.gt": "100",
         "telemetry.reporting.config": "000",
@@ -132,16 +132,14 @@
 def status_by_versioned_type_name() -> Dict[str, str]:
     """
     Returns:
         Dict[str, str]: Keys are versioned TypeNames, values are type status
     """
 
     v: Dict[str, str] = {
-        "boolean.actuator.cac.gt.000": "Active",
-        "boolean.actuator.component.gt.000": "Pending",
         "component.attribute.class.gt.000": "Active",
         "component.gt.000": "Active",
         "data.channel.000": "Active",
         "egauge.io.000": "Active",
         "egauge.register.config.000": "Active",
         "electric.meter.cac.gt.000": "Active",
         "electric.meter.component.gt.000": "Active",
@@ -157,14 +155,16 @@
         "gt.telemetry.110": "Active",
         "heartbeat.b.001": "Active",
         "multipurpose.sensor.cac.gt.000": "Active",
         "multipurpose.sensor.component.gt.000": "Active",
         "pipe.flow.sensor.cac.gt.000": "Active",
         "pipe.flow.sensor.component.gt.000": "Active",
         "power.watts.000": "Active",
+        "relay.cac.gt.000": "Active",
+        "relay.component.gt.000": "Active",
         "resistive.heater.cac.gt.000": "Active",
         "resistive.heater.component.gt.000": "Active",
         "simple.temp.sensor.cac.gt.000": "Active",
         "simple.temp.sensor.component.gt.000": "Active",
         "snapshot.spaceheat.000": "Active",
         "spaceheat.node.gt.100": "Active",
         "telemetry.reporting.config.000": "Active",
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/boolean_actuator_cac.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/relay_cac.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""BooleanActuatorCac definition"""
+"""RelayCac definition"""
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.enums import MakeModel
 from gwproto.enums import TelemetryName
 
 
-class BooleanActuatorCac(ComponentAttributeClass):
-    by_id: Dict[str, "BooleanActuatorCac"] = {}
+class RelayCac(ComponentAttributeClass):
+    by_id: Dict[str, "RelayCac"] = {}
 
     def __init__(
         self,
         component_attribute_class_id: str,
         make_model: MakeModel,
         typical_response_time_ms: Optional[int],
         display_name: Optional[str] = None,
@@ -20,15 +20,15 @@
         super(self.__class__, self).__init__(
             component_attribute_class_id=component_attribute_class_id,
             display_name=display_name,
         )
 
         self.typical_response_time_ms = typical_response_time_ms
         self.make_model = make_model
-        BooleanActuatorCac.by_id[self.component_attribute_class_id] = self
+        RelayCac.by_id[self.component_attribute_class_id] = self
         ComponentAttributeClass.by_id[self.component_attribute_class_id] = self
 
     def __repr__(self):
         return f"{self.make_model.value} {self.display_name}"
 
     @property
     def telemetry_name(self):
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/component_attribute_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/boolean_actuator_component.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-"""BooleanActuatorComponent definition"""
+"""ResistiveHeaterComponent definition"""
 from typing import Dict
 from typing import Optional
 
-from gwproto.data_classes.cacs.boolean_actuator_cac import BooleanActuatorCac
+from gwproto.data_classes.cacs.resistive_heater_cac import ResistiveHeaterCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
 
 
-class BooleanActuatorComponent(Component):
-    by_id: Dict[str, "BooleanActuatorComponent"] = {}
+class ResistiveHeaterComponent(Component):
+    by_id: Dict[str, "ResistiveHeaterComponent"] = {}
 
     def __init__(
         self,
         component_id: str,
         component_attribute_class_id: str,
-        normally_open: bool,
-        display_name: Optional[str] = None,
-        gpio: Optional[int] = None,
+        tested_max_hot_milli_ohms: Optional[int] = None,
+        tested_max_cold_milli_ohms: Optional[int] = None,
         hw_uid: Optional[str] = None,
+        display_name: Optional[str] = None,
     ):
         super(self.__class__, self).__init__(
             display_name=display_name,
             component_id=component_id,
             hw_uid=hw_uid,
             component_attribute_class_id=component_attribute_class_id,
         )
-        self.normally_open = normally_open
-        self.gpio = gpio
-
-        BooleanActuatorComponent.by_id[self.component_id] = self
+        self.tested_max_hot_milli_ohms = tested_max_hot_milli_ohms
+        self.tested_max_cold_milli_ohms = tested_max_cold_milli_ohms
+        ResistiveHeaterComponent.by_id[self.component_id] = self
         Component.by_id[self.component_id] = self
 
     @property
-    def cac(self) -> BooleanActuatorCac:
-        return BooleanActuatorCac.by_id[self.component_attribute_class_id]
+    def cac(self) -> ResistiveHeaterCac:
+        return ResistiveHeaterCac.by_id[self.component_attribute_class_id]
 
     @property
     def make_model(self) -> MakeModel:
         return self.cac.make_model
 
     def __repr__(self):
         return f"{self.display_name}  ({self.cac.make_model.value})"
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/relay_component.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-"""ResistiveHeaterComponent definition"""
+"""RelayComponent definition"""
 from typing import Dict
 from typing import Optional
 
-from gwproto.data_classes.cacs.resistive_heater_cac import ResistiveHeaterCac
+from gwproto.data_classes.cacs.relay_cac import RelayCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
 
 
-class ResistiveHeaterComponent(Component):
-    by_id: Dict[str, "ResistiveHeaterComponent"] = {}
+class RelayComponent(Component):
+    by_id: Dict[str, "RelayComponent"] = {}
 
     def __init__(
         self,
         component_id: str,
         component_attribute_class_id: str,
-        tested_max_hot_milli_ohms: Optional[int] = None,
-        tested_max_cold_milli_ohms: Optional[int] = None,
-        hw_uid: Optional[str] = None,
+        normally_open: bool,
         display_name: Optional[str] = None,
+        gpio: Optional[int] = None,
+        hw_uid: Optional[str] = None,
     ):
         super(self.__class__, self).__init__(
             display_name=display_name,
             component_id=component_id,
             hw_uid=hw_uid,
             component_attribute_class_id=component_attribute_class_id,
         )
-        self.tested_max_hot_milli_ohms = tested_max_hot_milli_ohms
-        self.tested_max_cold_milli_ohms = tested_max_cold_milli_ohms
-        ResistiveHeaterComponent.by_id[self.component_id] = self
+        self.normally_open = normally_open
+        self.gpio = gpio
+
+        RelayComponent.by_id[self.component_id] = self
         Component.by_id[self.component_id] = self
 
     @property
-    def cac(self) -> ResistiveHeaterCac:
-        return ResistiveHeaterCac.by_id[self.component_attribute_class_id]
+    def cac(self) -> RelayCac:
+        return RelayCac.by_id[self.component_attribute_class_id]
 
     @property
     def make_model(self) -> MakeModel:
         return self.cac.make_model
 
     def __repr__(self):
         return f"{self.display_name}  ({self.cac.make_model.value})"
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/hardware_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 from gwproto.data_classes.errors import DataClassLoadingError
 from gwproto.data_classes.sh_node import ShNode
 from gwproto.data_classes.telemetry_tuple import TelemetryTuple
 from gwproto.enums import ActorClass
 from gwproto.enums import Role
 from gwproto.enums import TelemetryName
 from gwproto.types import ElectricMeterCacGt_Maker
-from gwproto.types import GtBooleanActuatorCac_Maker
-from gwproto.types import GtBooleanActuatorComponent_Maker
 from gwproto.types import MultipurposeSensorCacGt_Maker
 from gwproto.types import PipeFlowSensorCacGt_Maker
 from gwproto.types import PipeFlowSensorComponentGt_Maker
+from gwproto.types import RelayCacGt_Maker
+from gwproto.types import RelayComponentGt_Maker
 from gwproto.types import ResistiveHeaterCacGt_Maker
 from gwproto.types import ResistiveHeaterComponentGt_Maker
 from gwproto.types import SimpleTempSensorCacGt_Maker
 from gwproto.types import SimpleTempSensorComponentGt_Maker
 from gwproto.types import SpaceheatNodeGt_Maker
 from gwproto.types.electric_meter_component_gt import ElectricMeterComponentGt_Maker
 from gwproto.types.multipurpose_sensor_component_gt import (
@@ -57,15 +57,15 @@
     src_dict: dict
     exception: Exception
 
 
 def load_cacs(layout: dict, raise_errors: bool = True) -> list[LoadError]:
     errors: list[LoadError] = []
     for type_name, maker_class in [
-        ("BooleanActuatorCacs", GtBooleanActuatorCac_Maker),
+        ("RelayCacs", RelayCacGt_Maker),
         ("ResistiveHeaterCacs", ResistiveHeaterCacGt_Maker),
         ("ElectricMeterCacs", ElectricMeterCacGt_Maker),
         ("PipeFlowSensorCacs", PipeFlowSensorCacGt_Maker),
         ("MultipurposeSensorCacs", MultipurposeSensorCacGt_Maker),
         ("SimpleTempSensorCacs", SimpleTempSensorCacGt_Maker),
     ]:
         for d in layout[type_name]:
@@ -86,15 +86,15 @@
             errors.append(LoadError("OtherCacs", d, e))
     return errors
 
 
 def load_components(layout: dict, raise_errors: bool = True) -> list[LoadError]:
     errors: list[LoadError] = []
     for type_name, maker_class in [
-        ("BooleanActuatorComponents", GtBooleanActuatorComponent_Maker),
+        ("RelayComponents", RelayComponentGt_Maker),
         ("ResistiveHeaterComponents", ResistiveHeaterComponentGt_Maker),
         ("ElectricMeterComponents", ElectricMeterComponentGt_Maker),
         ("PipeFlowSensorComponents", PipeFlowSensorComponentGt_Maker),
         ("MultipurposeSensorComponents", MultipurposeSensorComponentGt_Maker),
         ("SimpleTempSensorComponents", SimpleTempSensorComponentGt_Maker),
     ]:
         for d in layout[type_name]:
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.4.4/src/gwproto/data_classes/sh_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/decoders.py` & `gridworks_protocol-0.4.4/src/gwproto/decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.4.4/src/gwproto/enums/actor_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Enum with TypeName sh.actor.class, Version 000, Status Active"""
+""" Enum with TypeName sh.actor.class, Version 001, Status Active"""
 from enum import auto
 from typing import List
 
 from fastapi_utils.enums import StrEnum
 
 
 class ActorClass(StrEnum):
@@ -11,30 +11,32 @@
     [More Info](https://gridworks-protocol.readthedocs.io/en/latest/actor-class.html).
 
     Name (EnumSymbol, Version): description
     
       * NoActor (00000000, 000): A SpaceheatNode that does not have any code running on its behalf within the SCADA, but is instead only a reference object (for example, a tank of hot water or a resistive element) that can be discussed (for example, the power drawn by the resistive element can be measured) or evaluated (for example, a set of 5 different temperatures in different places on the tank can be used to estimate total thermal energy in the tank).
       * Scada (6d37aa41, 000): The SCADA actor is the prime piece of code running and supervising other ProActors within the SCADA code. It is also responsible for managing the state of TalkingWith the AtomicTNode, as well maintaining and reporting a boolean state variable that indicates whether it is following dispatch commands from the AtomicTNode XOR following dispatch commands from its own HomeAlone actor.
       * HomeAlone (32d3d19f, 000): HomeAlone is an abstract Spaceheat Actor responsible for dispatching the SCADA when it is not talking with the AtomicTNode.
-      * BooleanActuator (fddd0064, 000): A SpaceheatNode representing an electric relay, that can be turned off (open circuit) or on (closed circuit).
+      * BooleanActuator (fddd0064, 000): A SpaceheatNode representing a generic boolean actuator capable of turning on (closing a circuit) or turning off (opening a circuit).
       * PowerMeter (2ea112b9, 000): A SpaceheatNode representing the power meter that is used to settle financial transactions with the TerminalAsset. That is, this is the power meter whose accuracy is certified in the creation of the TerminalAsset GNode via creation of the TaDeed.. [More Info](https://gridworks.readthedocs.io/en/latest/terminal-asset.html).
       * Atn (b103058f, 000): A SpaceheatNode representing the AtomicTNode. Note that the code running the AtomicTNode is not local within the SCADA code, except for a stub used for testing purposes.. [More Info](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html).
       * SimpleSensor (dae4b2f0, 000): A SpaceheatNode representing a sensor that measures a single category of quantity (for example, temperature) for a single object (for example, on a pipe).. [More Info](https://gridworks-protocol.readthedocs.io/en/latest/simple-sensor.html).
       * MultipurposeSensor (7c483ad0, 000): A sensor that either reads multiple kinds of readings from the same sensing device (for example reads current and voltage), reads multiple different objects (temperature from two different thermisters) or both.. [More Info](https://gridworks-protocol.readthedocs.io/en/latest/multipurpose-sensor.html).
       * Thermostat (4a9c1785, 000): A SpaceheatNode representing a thermostat.
+      * Relay (311835f6, 001): A SpaceheatNode representing an electric relay
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
+    Relay = auto()
     
     @classmethod
     def default(cls) -> "ActorClass":
         """
         Returns default value NoActor
         """
         return cls.NoActor
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.4.4/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.4.4/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/enums/role.py` & `gridworks_protocol-0.4.4/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.4.4/src/gwproto/enums/telemetry_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/enums/unit.py` & `gridworks_protocol-0.4.4/src/gwproto/enums/unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.4.4/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.4.4/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/message.py` & `gridworks_protocol-0.4.4/src/gwproto/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.4.4/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/messages/event.py` & `gridworks_protocol-0.4.4/src/gwproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/messages/misc.py` & `gridworks_protocol-0.4.4/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/property_format.py` & `gridworks_protocol-0.4.4/src/gwproto/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/topic.py` & `gridworks_protocol-0.4.4/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/__init__.py` & `gridworks_protocol-0.4.4/src/gwproto/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """ List of all the schema types """
 
-from gwproto.types.boolean_actuator_cac_gt import BooleanActuatorCacGt
-from gwproto.types.boolean_actuator_cac_gt import BooleanActuatorCacGt_Maker
-from gwproto.types.boolean_actuator_component_gt import BooleanActuatorComponentGt
-from gwproto.types.boolean_actuator_component_gt import BooleanActuatorComponentGt_Maker
 from gwproto.types.component_attribute_class_gt import ComponentAttributeClassGt
 from gwproto.types.component_attribute_class_gt import ComponentAttributeClassGt_Maker
 from gwproto.types.component_gt import ComponentGt
 from gwproto.types.component_gt import ComponentGt_Maker
 from gwproto.types.data_channel import DataChannel
 from gwproto.types.data_channel import DataChannel_Maker
 from gwproto.types.egauge_io import EgaugeIo
@@ -52,14 +48,18 @@
 from gwproto.types.multipurpose_sensor_cac_gt import MultipurposeSensorCacGt_Maker
 from gwproto.types.pipe_flow_sensor_cac_gt import PipeFlowSensorCacGt
 from gwproto.types.pipe_flow_sensor_cac_gt import PipeFlowSensorCacGt_Maker
 from gwproto.types.pipe_flow_sensor_component_gt import PipeFlowSensorComponentGt
 from gwproto.types.pipe_flow_sensor_component_gt import PipeFlowSensorComponentGt_Maker
 from gwproto.types.power_watts import PowerWatts
 from gwproto.types.power_watts import PowerWatts_Maker
+from gwproto.types.relay_cac_gt import RelayCacGt
+from gwproto.types.relay_cac_gt import RelayCacGt_Maker
+from gwproto.types.relay_component_gt import RelayComponentGt
+from gwproto.types.relay_component_gt import RelayComponentGt_Maker
 from gwproto.types.resistive_heater_cac_gt import ResistiveHeaterCacGt
 from gwproto.types.resistive_heater_cac_gt import ResistiveHeaterCacGt_Maker
 from gwproto.types.resistive_heater_component_gt import ResistiveHeaterComponentGt
 from gwproto.types.resistive_heater_component_gt import ResistiveHeaterComponentGt_Maker
 from gwproto.types.simple_temp_sensor_cac_gt import SimpleTempSensorCacGt
 from gwproto.types.simple_temp_sensor_cac_gt import SimpleTempSensorCacGt_Maker
 from gwproto.types.simple_temp_sensor_component_gt import SimpleTempSensorComponentGt
@@ -73,18 +73,14 @@
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig_Maker
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat_Maker
 
 
 __all__ = [
-    "BooleanActuatorCacGt",
-    "BooleanActuatorCacGt_Maker",
-    "BooleanActuatorComponentGt",
-    "BooleanActuatorComponentGt_Maker",
     "ComponentAttributeClassGt",
     "ComponentAttributeClassGt_Maker",
     "ComponentGt",
     "ComponentGt_Maker",
     "DataChannel",
     "DataChannel_Maker",
     "EgaugeIo",
@@ -123,14 +119,18 @@
     # "MultipurposeSensorComponentGt_Maker",
     "PipeFlowSensorCacGt",
     "PipeFlowSensorCacGt_Maker",
     "PipeFlowSensorComponentGt",
     "PipeFlowSensorComponentGt_Maker",
     "PowerWatts",
     "PowerWatts_Maker",
+    "RelayCacGt",
+    "RelayCacGt_Maker",
+    "RelayComponentGt",
+    "RelayComponentGt_Maker",
     "ResistiveHeaterCacGt",
     "ResistiveHeaterCacGt_Maker",
     "ResistiveHeaterComponentGt",
     "ResistiveHeaterComponentGt_Maker",
     "SimpleTempSensorCacGt",
     "SimpleTempSensorCacGt_Maker",
     "SimpleTempSensorComponentGt",
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/boolean_actuator_cac_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/relay_cac_gt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Type boolean.actuator.cac.gt, version 000"""
+"""Type relay.cac.gt, version 000"""
 import json
 from enum import auto
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
 
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.data_classes.cacs.boolean_actuator_cac import BooleanActuatorCac
+from gwproto.data_classes.cacs.relay_cac import RelayCac
 from gwproto.enums import MakeModel as EnumMakeModel
 from gwproto.errors import MpSchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatMakeModel000SchemaEnum:
     enum_name: str = "spaceheat.make.model.000"
@@ -154,18 +154,19 @@
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[3]) != 4:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[4]) != 12:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
 
 
-class BooleanActuatorCacGt(BaseModel):
-    """Type for tracking Boolean Actuator ComponentAttributeClasses.
+class RelayCacGt(BaseModel):
+    """Type for tracking Relay ComponentAttributeClasses.
 
-    GridWorks Spaceheat SCADA uses the GridWorks GNodeRegistry structures and abstractions for managing relational device data. The Cac, or ComponentAttributeClass, is part of this structure.
+    GridWorks Spaceheat SCADA uses the GridWorks GNodeRegistry structures and abstractions for
+    managing relational device data. The Cac, or ComponentAttributeClass, is part of this structure.
     [More info](https://g-node-registry.readthedocs.io/en/latest/component-attribute-class.html).
     """
 
     ComponentAttributeClassId: str = Field(
         title="ComponentAttributeClassId",
     )
     MakeModel: EnumMakeModel = Field(
@@ -174,15 +175,15 @@
     DisplayName: Optional[str] = Field(
         title="DisplayName",
         default=None,
     )
     TypicalResponseTimeMs: int = Field(
         title="TypicalResponseTimeMs",
     )
-    TypeName: Literal["boolean.actuator.cac.gt"] = "boolean.actuator.cac.gt"
+    TypeName: Literal["relay.cac.gt"] = "relay.cac.gt"
     Version: str = "000"
 
     @validator("ComponentAttributeClassId")
     def _check_component_attribute_class_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
@@ -207,55 +208,55 @@
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
     def __hash__(self):
         return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
 
-class BooleanActuatorCacGt_Maker:
-    type_name = "boolean.actuator.cac.gt"
+class RelayCacGt_Maker:
+    type_name = "relay.cac.gt"
     version = "000"
 
     def __init__(
         self,
         component_attribute_class_id: str,
         make_model: EnumMakeModel,
         display_name: Optional[str],
         typical_response_time_ms: int,
     ):
-        self.tuple = BooleanActuatorCacGt(
+        self.tuple = RelayCacGt(
             ComponentAttributeClassId=component_attribute_class_id,
             MakeModel=make_model,
             DisplayName=display_name,
             TypicalResponseTimeMs=typical_response_time_ms,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: BooleanActuatorCacGt) -> str:
+    def tuple_to_type(cls, tuple: RelayCacGt) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> BooleanActuatorCacGt:
+    def type_to_tuple(cls, t: str) -> RelayCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise MpSchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise MpSchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> BooleanActuatorCacGt:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> RelayCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
@@ -264,51 +265,51 @@
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "TypicalResponseTimeMs" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing TypicalResponseTimeMs")
         if "TypeName" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing TypeName")
 
-        return BooleanActuatorCacGt(
+        return RelayCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             DisplayName=d2["DisplayName"],
             TypicalResponseTimeMs=d2["TypicalResponseTimeMs"],
             TypeName=d2["TypeName"],
             Version="000",
         )
 
     @classmethod
-    def tuple_to_dc(cls, t: BooleanActuatorCacGt) -> BooleanActuatorCac:
-        if t.ComponentAttributeClassId in BooleanActuatorCac.by_id.keys():
-            dc = BooleanActuatorCac.by_id[t.ComponentAttributeClassId]
+    def tuple_to_dc(cls, t: RelayCacGt) -> RelayCac:
+        if t.ComponentAttributeClassId in RelayCac.by_id.keys():
+            dc = RelayCac.by_id[t.ComponentAttributeClassId]
         else:
-            dc = BooleanActuatorCac(
+            dc = RelayCac(
                 component_attribute_class_id=t.ComponentAttributeClassId,
                 make_model=t.MakeModel,
                 display_name=t.DisplayName,
                 typical_response_time_ms=t.TypicalResponseTimeMs,
             )
 
         return dc
 
     @classmethod
-    def dc_to_tuple(cls, dc: BooleanActuatorCac) -> BooleanActuatorCacGt:
-        t = BooleanActuatorCacGt_Maker(
+    def dc_to_tuple(cls, dc: RelayCac) -> RelayCacGt:
+        t = RelayCacGt_Maker(
             component_attribute_class_id=dc.component_attribute_class_id,
             make_model=dc.make_model,
             display_name=dc.display_name,
             typical_response_time_ms=dc.typical_response_time_ms,
         ).tuple
         return t
 
     @classmethod
-    def type_to_dc(cls, t: str) -> BooleanActuatorCac:
+    def type_to_dc(cls, t: str) -> RelayCac:
         return cls.tuple_to_dc(cls.type_to_tuple(t))
 
     @classmethod
-    def dc_to_type(cls, dc: BooleanActuatorCac) -> str:
+    def dc_to_type(cls, dc: RelayCac) -> str:
         return cls.dc_to_tuple(dc).as_type()
 
     @classmethod
-    def dict_to_dc(cls, d: dict[Any, str]) -> BooleanActuatorCac:
+    def dict_to_dc(cls, d: dict[Any, str]) -> RelayCac:
         return cls.tuple_to_dc(cls.dict_to_tuple(d))
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/boolean_actuator_component_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_boolean_actuator_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Type boolean.actuator.component.gt, version 000"""
+"""Type gt.boolean.actuator.component, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
 
 from pydantic import BaseModel
@@ -46,19 +46,22 @@
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[3]) != 4:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[4]) != 12:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
 
 
-class BooleanActuatorComponentGt(BaseModel):
-    """Type for tracking Boolean ActuatorComponents.
+class GtBooleanActuatorComponent(BaseModel):
+    """Type for tracking Boolean ActuatorComponents
 
-    GridWorks Spaceheat SCADA uses the GridWorks GNodeRegistry structures and abstractions for managing relational device data. The Component associated to a SpaceheatNode is part of this structure.
-    [More info](https://g-node-registry.readthedocs.io/en/latest/component.html).
+    GridWorks Spaceheat SCADA uses the GridWorks GNodeRegistry structures and
+    abstractionsfor managing relational device data. The Component associated
+    to a SpaceheatNode is part of this structure.
+
+    [More info](https://g-node-registry.readthedocs.io/en/latest/component.html)
     """
 
     ComponentId: str = Field(
         title="ComponentId",
     )
     ComponentAttributeClassId: str = Field(
         title="ComponentAttributeClassId",
@@ -71,19 +74,15 @@
         title="Gpio",
         default=None,
     )
     HwUid: Optional[str] = Field(
         title="HwUid",
         default=None,
     )
-    NormallyOpen: bool = Field(
-        title="Normally Open",
-        description="Normally open relay default in the open position, meaning that when they're not in use, there is no contact between the circuits. When power is introduced, an electromagnet pulls the first circuit into contact with the second, thereby closing the circuit and allowing power to flow through",
-    )
-    TypeName: Literal["boolean.actuator.component.gt"] = "boolean.actuator.component.gt"
+    TypeName: Literal["gt.boolean.actuator.component"] = "gt.boolean.actuator.component"
     Version: str = "000"
 
     @validator("ComponentId")
     def _check_component_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
@@ -115,111 +114,104 @@
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
     def __hash__(self):
         return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
 
-class BooleanActuatorComponentGt_Maker:
-    type_name = "boolean.actuator.component.gt"
+class GtBooleanActuatorComponent_Maker:
+    type_name = "gt.boolean.actuator.component"
     version = "000"
 
     def __init__(
         self,
         component_id: str,
         component_attribute_class_id: str,
         display_name: Optional[str],
         gpio: Optional[int],
         hw_uid: Optional[str],
-        normally_open: bool,
     ):
-        self.tuple = BooleanActuatorComponentGt(
+        self.tuple = GtBooleanActuatorComponent(
             ComponentId=component_id,
             ComponentAttributeClassId=component_attribute_class_id,
             DisplayName=display_name,
             Gpio=gpio,
             HwUid=hw_uid,
-            NormallyOpen=normally_open,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: BooleanActuatorComponentGt) -> str:
+    def tuple_to_type(cls, tuple: GtBooleanActuatorComponent) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> BooleanActuatorComponentGt:
+    def type_to_tuple(cls, t: str) -> GtBooleanActuatorComponent:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise MpSchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise MpSchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> BooleanActuatorComponentGt:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> GtBooleanActuatorComponent:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "Gpio" not in d2.keys():
             d2["Gpio"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
-        if "NormallyOpen" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing NormallyOpen")
         if "TypeName" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing TypeName")
 
-        return BooleanActuatorComponentGt(
+        return GtBooleanActuatorComponent(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             Gpio=d2["Gpio"],
             HwUid=d2["HwUid"],
-            NormallyOpen=d2["NormallyOpen"],
             TypeName=d2["TypeName"],
             Version="000",
         )
 
     @classmethod
-    def tuple_to_dc(cls, t: BooleanActuatorComponentGt) -> BooleanActuatorComponent:
+    def tuple_to_dc(cls, t: GtBooleanActuatorComponent) -> BooleanActuatorComponent:
         if t.ComponentId in BooleanActuatorComponent.by_id.keys():
             dc = BooleanActuatorComponent.by_id[t.ComponentId]
         else:
             dc = BooleanActuatorComponent(
                 component_id=t.ComponentId,
                 component_attribute_class_id=t.ComponentAttributeClassId,
                 display_name=t.DisplayName,
                 gpio=t.Gpio,
                 hw_uid=t.HwUid,
-                normally_open=t.NormallyOpen,
             )
 
         return dc
 
     @classmethod
-    def dc_to_tuple(cls, dc: BooleanActuatorComponent) -> BooleanActuatorComponentGt:
-        t = BooleanActuatorComponentGt_Maker(
+    def dc_to_tuple(cls, dc: BooleanActuatorComponent) -> GtBooleanActuatorComponent:
+        t = GtBooleanActuatorComponent_Maker(
             component_id=dc.component_id,
             component_attribute_class_id=dc.component_attribute_class_id,
             display_name=dc.display_name,
             gpio=dc.gpio,
             hw_uid=dc.hw_uid,
-            normally_open=dc.normally_open,
         ).tuple
         return t
 
     @classmethod
     def type_to_dc(cls, t: str) -> BooleanActuatorComponent:
         return cls.tuple_to_dc(cls.type_to_tuple(t))
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/component_attribute_class_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.4.4/src/gwproto/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.4.4/src/gwproto/types/egauge_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.4.4/src/gwproto/types/egauge_register_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/electric_meter_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_boolean_actuator_component.py` & `gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""Type gt.boolean.actuator.component, version 000"""
+"""Type resistive.heater.component.gt, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.data_classes.components.boolean_actuator_component import (
-    BooleanActuatorComponent,
+from gwproto.data_classes.components.resistive_heater_component import (
+    ResistiveHeaterComponent,
 )
 from gwproto.errors import MpSchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
@@ -46,43 +46,46 @@
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[3]) != 4:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[4]) != 12:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
 
 
-class GtBooleanActuatorComponent(BaseModel):
-    """Type for tracking Boolean ActuatorComponents
+class ResistiveHeaterComponentGt(BaseModel):
+    """Type for tracking Resistive Heater Components.
 
     GridWorks Spaceheat SCADA uses the GridWorks GNodeRegistry structures and
-    abstractionsfor managing relational device data. The Component associated
+    abstractions for managing relational device data. The Component associated
     to a SpaceheatNode is part of this structure.
-
-    [More info](https://g-node-registry.readthedocs.io/en/latest/component.html)
+    [More info](https://g-node-registry.readthedocs.io/en/latest/component.html).
     """
 
     ComponentId: str = Field(
         title="ComponentId",
     )
     ComponentAttributeClassId: str = Field(
         title="ComponentAttributeClassId",
     )
     DisplayName: Optional[str] = Field(
         title="DisplayName",
         default=None,
     )
-    Gpio: Optional[int] = Field(
-        title="Gpio",
-        default=None,
-    )
     HwUid: Optional[str] = Field(
         title="HwUid",
         default=None,
     )
-    TypeName: Literal["gt.boolean.actuator.component"] = "gt.boolean.actuator.component"
+    TestedMaxHotMilliOhms: Optional[int] = Field(
+        title="TestedMaxHotMilliOhms",
+        default=None,
+    )
+    TestedMaxColdMilliOhms: Optional[int] = Field(
+        title="TestedMaxColdMilliOhms",
+        default=None,
+    )
+    TypeName: Literal["resistive.heater.component.gt"] = "resistive.heater.component.gt"
     Version: str = "000"
 
     @validator("ComponentId")
     def _check_component_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
@@ -101,124 +104,133 @@
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         if d["DisplayName"] is None:
             del d["DisplayName"]
-        if d["Gpio"] is None:
-            del d["Gpio"]
         if d["HwUid"] is None:
             del d["HwUid"]
+        if d["TestedMaxHotMilliOhms"] is None:
+            del d["TestedMaxHotMilliOhms"]
+        if d["TestedMaxColdMilliOhms"] is None:
+            del d["TestedMaxColdMilliOhms"]
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
     def __hash__(self):
         return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
 
-class GtBooleanActuatorComponent_Maker:
-    type_name = "gt.boolean.actuator.component"
+class ResistiveHeaterComponentGt_Maker:
+    type_name = "resistive.heater.component.gt"
     version = "000"
 
     def __init__(
         self,
         component_id: str,
         component_attribute_class_id: str,
         display_name: Optional[str],
-        gpio: Optional[int],
         hw_uid: Optional[str],
+        tested_max_hot_milli_ohms: Optional[int],
+        tested_max_cold_milli_ohms: Optional[int],
     ):
-        self.tuple = GtBooleanActuatorComponent(
+        self.tuple = ResistiveHeaterComponentGt(
             ComponentId=component_id,
             ComponentAttributeClassId=component_attribute_class_id,
             DisplayName=display_name,
-            Gpio=gpio,
             HwUid=hw_uid,
+            TestedMaxHotMilliOhms=tested_max_hot_milli_ohms,
+            TestedMaxColdMilliOhms=tested_max_cold_milli_ohms,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: GtBooleanActuatorComponent) -> str:
+    def tuple_to_type(cls, tuple: ResistiveHeaterComponentGt) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> GtBooleanActuatorComponent:
+    def type_to_tuple(cls, t: str) -> ResistiveHeaterComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise MpSchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise MpSchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> GtBooleanActuatorComponent:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> ResistiveHeaterComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
-        if "Gpio" not in d2.keys():
-            d2["Gpio"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
+        if "TestedMaxHotMilliOhms" not in d2.keys():
+            d2["TestedMaxHotMilliOhms"] = None
+        if "TestedMaxColdMilliOhms" not in d2.keys():
+            d2["TestedMaxColdMilliOhms"] = None
         if "TypeName" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing TypeName")
 
-        return GtBooleanActuatorComponent(
+        return ResistiveHeaterComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
-            Gpio=d2["Gpio"],
             HwUid=d2["HwUid"],
+            TestedMaxHotMilliOhms=d2["TestedMaxHotMilliOhms"],
+            TestedMaxColdMilliOhms=d2["TestedMaxColdMilliOhms"],
             TypeName=d2["TypeName"],
             Version="000",
         )
 
     @classmethod
-    def tuple_to_dc(cls, t: GtBooleanActuatorComponent) -> BooleanActuatorComponent:
-        if t.ComponentId in BooleanActuatorComponent.by_id.keys():
-            dc = BooleanActuatorComponent.by_id[t.ComponentId]
+    def tuple_to_dc(cls, t: ResistiveHeaterComponentGt) -> ResistiveHeaterComponent:
+        if t.ComponentId in ResistiveHeaterComponent.by_id.keys():
+            dc = ResistiveHeaterComponent.by_id[t.ComponentId]
         else:
-            dc = BooleanActuatorComponent(
+            dc = ResistiveHeaterComponent(
                 component_id=t.ComponentId,
                 component_attribute_class_id=t.ComponentAttributeClassId,
                 display_name=t.DisplayName,
-                gpio=t.Gpio,
                 hw_uid=t.HwUid,
+                tested_max_hot_milli_ohms=t.TestedMaxHotMilliOhms,
+                tested_max_cold_milli_ohms=t.TestedMaxColdMilliOhms,
             )
 
         return dc
 
     @classmethod
-    def dc_to_tuple(cls, dc: BooleanActuatorComponent) -> GtBooleanActuatorComponent:
-        t = GtBooleanActuatorComponent_Maker(
+    def dc_to_tuple(cls, dc: ResistiveHeaterComponent) -> ResistiveHeaterComponentGt:
+        t = ResistiveHeaterComponentGt_Maker(
             component_id=dc.component_id,
             component_attribute_class_id=dc.component_attribute_class_id,
             display_name=dc.display_name,
-            gpio=dc.gpio,
             hw_uid=dc.hw_uid,
+            tested_max_hot_milli_ohms=dc.tested_max_hot_milli_ohms,
+            tested_max_cold_milli_ohms=dc.tested_max_cold_milli_ohms,
         ).tuple
         return t
 
     @classmethod
-    def type_to_dc(cls, t: str) -> BooleanActuatorComponent:
+    def type_to_dc(cls, t: str) -> ResistiveHeaterComponent:
         return cls.tuple_to_dc(cls.type_to_tuple(t))
 
     @classmethod
-    def dc_to_type(cls, dc: BooleanActuatorComponent) -> str:
+    def dc_to_type(cls, dc: ResistiveHeaterComponent) -> str:
         return cls.dc_to_tuple(dc).as_type()
 
     @classmethod
-    def dict_to_dc(cls, d: dict[Any, str]) -> BooleanActuatorComponent:
+    def dict_to_dc(cls, d: dict[Any, str]) -> ResistiveHeaterComponent:
         return cls.tuple_to_dc(cls.dict_to_tuple(d))
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.4.4/src/gwproto/types/gt_telemetry.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.4.4/src/gwproto/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.4.4/src/gwproto/types/power_watts.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.4.4/src/gwproto/types/snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.4.4/src/gwproto/types/spaceheat_node_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "32d3d19f",
         "fddd0064",
         "2ea112b9",
         "b103058f",
         "dae4b2f0",
         "7c483ad0",
         "4a9c1785",
+        "311835f6",
     ]
 
     @classmethod
     def is_symbol(cls, candidate: str) -> bool:
         if candidate in cls.symbols:
             return True
         return False
@@ -46,14 +47,15 @@
     HomeAlone = auto()
     BooleanActuator = auto()
     PowerMeter = auto()
     Atn = auto()
     SimpleSensor = auto()
     MultipurposeSensor = auto()
     Thermostat = auto()
+    Relay = auto()
 
     @classmethod
     def default(cls) -> "ShActorClass000":
         return cls.NoActor
 
     @classmethod
     def values(cls) -> List[str]:
@@ -83,26 +85,28 @@
         "32d3d19f": ShActorClass000.HomeAlone,
         "fddd0064": ShActorClass000.BooleanActuator,
         "2ea112b9": ShActorClass000.PowerMeter,
         "b103058f": ShActorClass000.Atn,
         "dae4b2f0": ShActorClass000.SimpleSensor,
         "7c483ad0": ShActorClass000.MultipurposeSensor,
         "4a9c1785": ShActorClass000.Thermostat,
+        "311835f6": ShActorClass000.Relay,
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
+        ShActorClass000.Relay: "311835f6",
     }
 
 
 class ShNodeRole000SchemaEnum:
     enum_name: str = "sh.node.role.000"
     symbols: List[str] = [
         "00000000",
```

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.4.4/src/gwproto/types/telemetry_reporting_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.4.4/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/src/gwproto/utils.py` & `gridworks_protocol-0.4.4/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.3/setup.py` & `gridworks_protocol-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 install_requires = \
 ['fastapi-utils>=0.2.1,<0.3.0',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'gridworks-protocol',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'Gridworks Protocol',
     'long_description': "# Gridworks Protocol\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-protocol.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/gridworks-protocol.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-protocol)][python version]\n[![License](https://img.shields.io/pypi/l/gridworks-protocol)][license]\n\n[![Read the documentation at https://gridworks-protocol.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-protocol/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-protocol/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-protocol/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/gridworks-protocol/\n[status]: https://pypi.org/project/gridworks-protocol/\n[python version]: https://pypi.org/project/gridworks-protocol\n[read the docs]: https://gridworks-protocol.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-protocol/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-protocol\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Gridworks Protocol_ via [pip] from [PyPI]:\n\n```console\n$ pip install gridworks-protocol\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Gridworks Protocol_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-protocol/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-protocol/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-protocol/blob/main/CONTRIBUTING.md\n",
     'author': 'Jessica Millar',
     'author_email': 'jmillar@gridworks-consulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegridelectric/gridworks-protocol',
```

### Comparing `gridworks_protocol-0.4.3/PKG-INFO` & `gridworks_protocol-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.4.3
+Version: 0.4.4
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

