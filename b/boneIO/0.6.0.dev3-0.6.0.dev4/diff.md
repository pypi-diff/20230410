# Comparing `tmp/boneIO-0.6.0.dev3.tar.gz` & `tmp/boneIO-0.6.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneIO-0.6.0.dev3.tar", last modified: Wed Feb  8 19:50:21 2023, max compression
+gzip compressed data, was "boneIO-0.6.0.dev4.tar", last modified: Mon Apr 10 19:09:14 2023, max compression
```

## Comparing `boneIO-0.6.0.dev3.tar` & `boneIO-0.6.0.dev4.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0    35149 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/LICENSE
--rw-r--r--   0        0        0      474 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/README.md
--rw-r--r--   0        0        0      147 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/__init__.py
--rw-r--r--   0        0        0     3155 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/bonecli.py
--rw-r--r--   0        0        0     2908 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/const.py
--rw-r--r--   0        0        0     8454 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/cover.py
--rw-r--r--   0        0        0        0 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/__init__.py
--rw-r--r--   0        0        0      168 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/adc.yaml
--rw-r--r--   0        0        0      326 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/config.yaml
--rw-r--r--   0        0        0      150 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/cover.yaml
--rw-r--r--   0        0        0     2883 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/input.yaml
--rw-r--r--   0        0        0     3392 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/led32x4A.yaml
--rw-r--r--   0        0        0     1691 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/output24x16A.yaml
--rw-r--r--   0        0        0     2403 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/example_config/output32x5A.yaml
--rw-r--r--   0        0        0    19372 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/fonts/danube__.ttf
--rw-r--r--   0        0        0     1972 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/__init__.py
--rw-r--r--   0        0        0      985 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/async_updater.py
--rw-r--r--   0        0        0     1311 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/config.py
--rw-r--r--   0        0        0     5579 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/events.py
--rw-r--r--   0        0        0      637 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/exceptions.py
--rw-r--r--   0        0        0      885 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/filter.py
--rw-r--r--   0        0        0     2710 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/gpio.py
--rw-r--r--   0        0        0     6129 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/ha_discovery.py
--rw-r--r--   0        0        0    13488 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/loader.py
--rw-r--r--   0        0        0     1801 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/logger.py
--rw-r--r--   0        0        0      759 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/mqtt.py
--rw-r--r--   0        0        0      351 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/oled.py
--rw-r--r--   0        0        0     2430 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/onewire/W1ThermSensor.py
--rw-r--r--   0        0        0      448 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/onewire/__init__.py
--rw-r--r--   0        0        0     5169 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/onewire/ds2482.py
--rw-r--r--   0        0        0     2497 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/onewire/onewire.py
--rw-r--r--   0        0        0     1066 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/queue.py
--rw-r--r--   0        0        0     1994 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/state_manager.py
--rw-r--r--   0        0        0     5693 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/stats.py
--rw-r--r--   0        0        0     5806 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/timeperiod.py
--rw-r--r--   0        0        0      508 2023-02-08 19:49:48.284728 boneIO-0.6.0.dev3/boneio/helper/util.py
--rw-r--r--   0        0        0    11304 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/helper/yaml_util.py
--rw-r--r--   0        0        0       99 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/input/__init__.py
--rw-r--r--   0        0        0     4391 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/input/gpio.py
--rw-r--r--   0        0        0    20179 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/manager.py
--rw-r--r--   0        0        0     4176 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/modbus.py
--rw-r--r--   0        0        0     6983 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/mqtt_client.py
--rw-r--r--   0        0        0     5244 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/oled.py
--rw-r--r--   0        0        0      181 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/relay/__init__.py
--rw-r--r--   0        0        0     2629 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/relay/basic.py
--rw-r--r--   0        0        0     1163 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/relay/gpio.py
--rw-r--r--   0        0        0     2669 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/relay/mcp.py
--rw-r--r--   0        0        0     4873 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/relay/pca.py
--rw-r--r--   0        0        0     2287 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/runner.py
--rw-r--r--   0        0        0     1009 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/actions.yaml
--rw-r--r--   0        0        0      129 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/actions_sensor.yaml
--rw-r--r--   0        0        0      124 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/actions_switch.yaml
--rw-r--r--   0        0        0      286 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/filters.yaml
--rw-r--r--   0        0        0      304 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/filters_adc.yaml
--rw-r--r--   0        0        0       75 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/id.yaml
--rw-r--r--   0        0        0    12551 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/schema.yaml
--rw-r--r--   0        0        0       65 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/temp_unit.yaml
--rw-r--r--   0        0        0      133 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/schema/update_interval.yaml
--rw-r--r--   0        0        0      431 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/__init__.py
--rw-r--r--   0        0        0     1281 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/adc.py
--rw-r--r--   0        0        0     1289 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/gpio.py
--rw-r--r--   0        0        0     8500 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/modbus/__init__.py
--rw-r--r--   0        0        0     8810 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/modbus/dts1964_3f.json
--rw-r--r--   0        0        0      526 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/modbus/pt100.json
--rw-r--r--   0        0        0     2735 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/modbus/r4dcb08.json
--rw-r--r--   0        0        0     4145 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/modbus/sdm120.json
--rw-r--r--   0        0        0    10969 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/modbus/sdm630.json
--rw-r--r--   0        0        0     5592 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/modbus/sofar.json
--rw-r--r--   0        0        0     1659 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/temp/__init__.py
--rw-r--r--   0        0        0     2485 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/temp/dallas.py
--rw-r--r--   0        0        0      243 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/temp/lm75.py
--rw-r--r--   0        0        0      271 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/sensor/temp/mcp9808.py
--rw-r--r--   0        0        0       41 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/boneio/version.py
--rw-r--r--   0        0        0     1845 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/pyproject.toml
--rw-r--r--   0        0        0      166 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/tests/32_5_config.yaml
--rw-r--r--   0        0        0      224 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/tests/bandit.yaml
--rw-r--r--   0        0        0     1070 2023-02-08 19:49:48.288728 boneIO-0.6.0.dev3/tests/relay_32_5.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/LICENSE
+-rw-r--r--   0        0        0      474 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/README.md
+-rw-r--r--   0        0        0      147 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/__init__.py
+-rw-r--r--   0        0        0     3155 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/bonecli.py
+-rw-r--r--   0        0        0     2924 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/const.py
+-rw-r--r--   0        0        0     8454 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/cover.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/__init__.py
+-rw-r--r--   0        0        0      168 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/adc.yaml
+-rw-r--r--   0        0        0      326 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/config.yaml
+-rw-r--r--   0        0        0      150 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/cover.yaml
+-rw-r--r--   0        0        0     2883 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/input.yaml
+-rw-r--r--   0        0        0     3392 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/led32x4A.yaml
+-rw-r--r--   0        0        0     1691 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/output24x16A.yaml
+-rw-r--r--   0        0        0     2403 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/output32x5A.yaml
+-rw-r--r--   0        0        0    19372 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/fonts/danube__.ttf
+-rw-r--r--   0        0        0     2039 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/__init__.py
+-rw-r--r--   0        0        0      985 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/async_updater.py
+-rw-r--r--   0        0        0     1169 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/click_timer.py
+-rw-r--r--   0        0        0     1311 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/config.py
+-rw-r--r--   0        0        0     7494 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/events.py
+-rw-r--r--   0        0        0      637 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/exceptions.py
+-rw-r--r--   0        0        0      885 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/filter.py
+-rw-r--r--   0        0        0     2718 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/gpio.py
+-rw-r--r--   0        0        0     6129 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/ha_discovery.py
+-rw-r--r--   0        0        0    13488 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/loader.py
+-rw-r--r--   0        0        0     1801 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/logger.py
+-rw-r--r--   0        0        0      759 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/mqtt.py
+-rw-r--r--   0        0        0      351 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/oled.py
+-rw-r--r--   0        0        0     2430 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/W1ThermSensor.py
+-rw-r--r--   0        0        0      448 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/__init__.py
+-rw-r--r--   0        0        0     5169 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/ds2482.py
+-rw-r--r--   0        0        0     2497 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/onewire.py
+-rw-r--r--   0        0        0     1066 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/queue.py
+-rw-r--r--   0        0        0     1994 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/state_manager.py
+-rw-r--r--   0        0        0     5693 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/stats.py
+-rw-r--r--   0        0        0     5806 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/timeperiod.py
+-rw-r--r--   0        0        0      508 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/util.py
+-rw-r--r--   0        0        0    11304 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/yaml_util.py
+-rw-r--r--   0        0        0       99 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/input/__init__.py
+-rw-r--r--   0        0        0     2583 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/input/gpio.py
+-rw-r--r--   0        0        0    20273 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/manager.py
+-rw-r--r--   0        0        0     4176 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/modbus.py
+-rw-r--r--   0        0        0     6983 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/mqtt_client.py
+-rw-r--r--   0        0        0     5244 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/oled.py
+-rw-r--r--   0        0        0      181 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/__init__.py
+-rw-r--r--   0        0        0     2629 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/basic.py
+-rw-r--r--   0        0        0     1163 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/gpio.py
+-rw-r--r--   0        0        0     2669 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/mcp.py
+-rw-r--r--   0        0        0     4873 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/pca.py
+-rw-r--r--   0        0        0     2287 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/runner.py
+-rw-r--r--   0        0        0     1030 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/actions.yaml
+-rw-r--r--   0        0        0      129 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/actions_sensor.yaml
+-rw-r--r--   0        0        0      124 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/actions_switch.yaml
+-rw-r--r--   0        0        0      286 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/filters.yaml
+-rw-r--r--   0        0        0      304 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/filters_adc.yaml
+-rw-r--r--   0        0        0       75 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/id.yaml
+-rw-r--r--   0        0        0    12551 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/schema.yaml
+-rw-r--r--   0        0        0       65 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/temp_unit.yaml
+-rw-r--r--   0        0        0      133 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/update_interval.yaml
+-rw-r--r--   0        0        0      431 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/__init__.py
+-rw-r--r--   0        0        0     1281 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/adc.py
+-rw-r--r--   0        0        0     1289 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/gpio.py
+-rw-r--r--   0        0        0     8500 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/__init__.py
+-rw-r--r--   0        0        0     8810 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/dts1964_3f.json
+-rw-r--r--   0        0        0      526 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/pt100.json
+-rw-r--r--   0        0        0     2735 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/r4dcb08.json
+-rw-r--r--   0        0        0     4145 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm120.json
+-rw-r--r--   0        0        0    10969 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm630.json
+-rw-r--r--   0        0        0     5592 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/sofar.json
+-rw-r--r--   0        0        0     1659 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/__init__.py
+-rw-r--r--   0        0        0     2485 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/dallas.py
+-rw-r--r--   0        0        0      243 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/lm75.py
+-rw-r--r--   0        0        0      271 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/mcp9808.py
+-rw-r--r--   0        0        0       41 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/version.py
+-rw-r--r--   0        0        0     1871 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/tests/32_5_config.yaml
+-rw-r--r--   0        0        0      224 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/tests/bandit.yaml
+-rw-r--r--   0        0        0     1070 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/tests/relay_32_5.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.0.dev4/PKG-INFO
```

### Comparing `boneIO-0.6.0.dev3/LICENSE` & `boneIO-0.6.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/bonecli.py` & `boneIO-0.6.0.dev4/boneio/bonecli.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/const.py` & `boneIO-0.6.0.dev4/boneio/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 NONE = "none"
 
 # MISCELLANEOUS CONSTS
 RELAY = "relay"
 LED = "led"
 ON = "ON"
 OFF = "OFF"
+TOGGLE = "TOGGLE"
 STATE = "state"
 BRIGHTNESS = "brightness"
 SET_BRIGHTNESS = "set_brightness"
 ENABLED = "enabled"
 OUTPUT = "output"
 PIN = "pin"
 ID = "id"
@@ -51,15 +52,15 @@
     "uart1": {ID: "/dev/ttyS1", TX: "P9.24", RX: "P9.26"},
     "uart2": {ID: "/dev/ttyS2", TX: "P9.21", RX: "P9.22"},
     "uart3": {ID: "/dev/ttyS3", TX: "P9.42", RX: None},
     "uart4": {ID: "/dev/ttyS4", TX: "P9.13", RX: "P9.11"},
     "uart5": {ID: "/dev/ttyS5", TX: "P8.37", RX: "P8.38"},
 }
 
-relay_actions = {ON: "turn_on", OFF: "turn_off", "TOGGLE": "toggle"}
+relay_actions = {ON: "turn_on", OFF: "turn_off", TOGGLE: "toggle"}
 
 # HA CONSTS
 HOMEASSISTANT = "homeassistant"
 HA_DISCOVERY = "ha_discovery"
 OUTPUT_TYPE = "output_type"
 SHOW_HA = "show_in_ha"
```

### Comparing `boneIO-0.6.0.dev3/boneio/cover.py` & `boneIO-0.6.0.dev4/boneio/cover.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/example_config/input.yaml` & `boneIO-0.6.0.dev4/boneio/example_config/input.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/example_config/led32x4A.yaml` & `boneIO-0.6.0.dev4/boneio/example_config/led32x4A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/example_config/output24x16A.yaml` & `boneIO-0.6.0.dev4/boneio/example_config/output24x16A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/example_config/output32x5A.yaml` & `boneIO-0.6.0.dev4/boneio/example_config/output32x5A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/fonts/danube__.ttf` & `boneIO-0.6.0.dev4/boneio/fonts/danube__.ttf`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/__init__.py` & `boneIO-0.6.0.dev4/boneio/helper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Helper dir for BoneIO."""
 
 from boneio.helper.exceptions import GPIOInputException, GPIOOutputException, I2CError
+from boneio.helper.click_timer import ClickTimer
 from boneio.helper.gpio import (
     GpioBaseClass,
     configure_pin,
     edge_detect,
     read_input,
     setup_input,
     setup_output,
@@ -66,8 +67,9 @@
     "UniqueQueue",
     "schema_file",
     "load_config_from_string",
     "load_config_from_file",
     "TimePeriod",
     "callback",
     "is_callback",
+    "ClickTimer",
 ]
```

### Comparing `boneIO-0.6.0.dev3/boneio/helper/async_updater.py` & `boneIO-0.6.0.dev4/boneio/helper/async_updater.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/config.py` & `boneIO-0.6.0.dev4/boneio/helper/config.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/exceptions.py` & `boneIO-0.6.0.dev4/boneio/helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/filter.py` & `boneIO-0.6.0.dev4/boneio/helper/filter.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/gpio.py` & `boneIO-0.6.0.dev4/boneio/helper/gpio.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def write_output(pin: str, value: str) -> None:
     """Write a value to a GPIO."""
 
     GPIO.output(pin, value)
 
 
-def read_input(pin: str, on_state: Gpio_States = LOW) -> None:
+def read_input(pin: str, on_state: Gpio_States = LOW) -> bool:
     """Read a value from a GPIO."""
     return GPIO.input(pin) is on_state
 
 
 def edge_detect(
     pin: str, callback: Callable, bounce: int = 0, edge: Gpio_Edges = FALLING
 ) -> None:
@@ -93,10 +93,10 @@
         gpio_mode = kwargs.get(GPIO_MODE, GPIO_STR)
         self._bounce_time = kwargs.get("bounce_time", TimePeriod(milliseconds=10))
         self._loop = asyncio.get_running_loop()
         self._press_callback = press_callback
         setup_input(pin=self._pin, pull_mode=gpio_mode)
 
     @property
-    def is_pressed(self):
+    def is_pressed(self) -> bool:
         """Is button pressed."""
         return read_input(self._pin)
```

### Comparing `boneIO-0.6.0.dev3/boneio/helper/ha_discovery.py` & `boneIO-0.6.0.dev4/boneio/helper/ha_discovery.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/loader.py` & `boneIO-0.6.0.dev4/boneio/helper/loader.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/logger.py` & `boneIO-0.6.0.dev4/boneio/helper/logger.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/mqtt.py` & `boneIO-0.6.0.dev4/boneio/helper/mqtt.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/onewire/W1ThermSensor.py` & `boneIO-0.6.0.dev4/boneio/helper/onewire/W1ThermSensor.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/onewire/ds2482.py` & `boneIO-0.6.0.dev4/boneio/helper/onewire/ds2482.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/onewire/onewire.py` & `boneIO-0.6.0.dev4/boneio/helper/onewire/onewire.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/queue.py` & `boneIO-0.6.0.dev4/boneio/helper/queue.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/state_manager.py` & `boneIO-0.6.0.dev4/boneio/helper/state_manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/stats.py` & `boneIO-0.6.0.dev4/boneio/helper/stats.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/timeperiod.py` & `boneIO-0.6.0.dev4/boneio/helper/timeperiod.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/helper/yaml_util.py` & `boneIO-0.6.0.dev4/boneio/helper/yaml_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from collections import OrderedDict
 from typing import Any, Tuple
 
 from cerberus import TypeDefinition, Validator
 from yaml import MarkedYAMLError, SafeLoader, YAMLError, load
 
-from boneio.const import COVER, ID, OUTPUT
+from boneio.const import COVER, ID, OUTPUT, TOGGLE
 from boneio.helper.exceptions import ConfigurationException
 from boneio.helper.timeperiod import TimePeriod
 
 schema_file = os.path.join(os.path.dirname(__file__), "../schema/schema.yaml")
 _LOGGER = logging.getLogger(__name__)
 
 SECRET_YAML = "secrets.yaml"
@@ -99,17 +99,15 @@
 )
 BoneIOLoader.add_constructor(
     "!include_dir_named", BoneIOLoader.construct_include_dir_named
 )
 BoneIOLoader.add_constructor(
     "!include_dir_merge_named", BoneIOLoader.construct_include_dir_merge_named
 )
-BoneIOLoader.add_constructor(
-    "!include_files", BoneIOLoader.construct_include_files
-)
+BoneIOLoader.add_constructor("!include_files", BoneIOLoader.construct_include_files)
 
 
 def filter_yaml_files(files):
     return [
         f
         for f in files
         if (
@@ -242,15 +240,15 @@
     def _normalize_coerce_lower(self, value):
         return str(value).lower()
 
     def _normalize_coerce_upper(self, value):
         return str(value).upper()
 
     def _normalize_coerce_actions_output(self, value):
-        return str(value).lower()
+        return str(value).upper()
 
     def _normalize_coerce_str(self, value):
         return str(value)
 
     def _normalize_coerce_check_actions(self, value):
         _path = self.document_path
         parent = self.root_document[_path[0]][_path[1]]
@@ -320,8 +318,8 @@
             out = self.root_document
             for _p in self.document_path:
                 out = out[_p]
             return out
 
         parent = get_parent()
         if parent["action"] == COVER:
-            return "toggle"
+            return TOGGLE
```

### Comparing `boneIO-0.6.0.dev3/boneio/manager.py` & `boneIO-0.6.0.dev4/boneio/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,16 @@
                 device = action_definition.get(PIN)
                 if not device:
                     continue
                 relay = self._output.get(device.replace(" ", ""))
                 action = relay_actions.get(action_definition["action_output"])
                 if relay and action:
                     getattr(relay, action)()
+                else:
+                    _LOGGER.warn("PIN %s for action not found", device)
             elif action_definition[ACTION] == MQTT:
                 action_topic = action_definition.get(TOPIC)
                 action_payload = action_definition.get("action_mqtt_msg")
                 if action_topic and action_payload:
                     self.send_message(
                         topic=action_topic, payload=action_payload, retain=False
                     )
```

### Comparing `boneIO-0.6.0.dev3/boneio/modbus.py` & `boneIO-0.6.0.dev4/boneio/modbus.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/mqtt_client.py` & `boneIO-0.6.0.dev4/boneio/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/oled.py` & `boneIO-0.6.0.dev4/boneio/oled.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/relay/basic.py` & `boneIO-0.6.0.dev4/boneio/relay/basic.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/relay/gpio.py` & `boneIO-0.6.0.dev4/boneio/relay/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/relay/mcp.py` & `boneIO-0.6.0.dev4/boneio/relay/mcp.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/relay/pca.py` & `boneIO-0.6.0.dev4/boneio/relay/pca.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/runner.py` & `boneIO-0.6.0.dev4/boneio/runner.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/schema/actions.yaml` & `boneIO-0.6.0.dev4/boneio/schema/actions.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -19,24 +19,25 @@
     required: False
     nullable: True
     allowed:
       ['toggle', 'open', 'close', 'stop', 'toggle_open', 'toggle_close']
     default_setter: toggle_cover
     dependencies:
       action: ['cover']
+    coerce:
+      - actions_output
     meta:
       label: If cover action chosen then what action to perform.
   action_output:
     type: string
     allowed: ['toggle', 'on', 'off']
     default: toggle
     dependencies:
       action: ['output']
     coerce:
-      - lower
       - actions_output
     meta:
       label: If output action chosen then what action to perform.
   action_mqtt_msg:
     type: string
     dependencies:
       action: ['mqtt']
```

### Comparing `boneIO-0.6.0.dev3/boneio/schema/schema.yaml` & `boneIO-0.6.0.dev4/boneio/schema/schema.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/adc.py` & `boneIO-0.6.0.dev4/boneio/sensor/adc.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/gpio.py` & `boneIO-0.6.0.dev4/boneio/sensor/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/modbus/__init__.py` & `boneIO-0.6.0.dev4/boneio/sensor/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/modbus/dts1964_3f.json` & `boneIO-0.6.0.dev4/boneio/sensor/modbus/dts1964_3f.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/modbus/pt100.json` & `boneIO-0.6.0.dev4/boneio/sensor/modbus/pt100.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/modbus/r4dcb08.json` & `boneIO-0.6.0.dev4/boneio/sensor/modbus/r4dcb08.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/modbus/sdm120.json` & `boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm120.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/modbus/sdm630.json` & `boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm630.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/modbus/sofar.json` & `boneIO-0.6.0.dev4/boneio/sensor/modbus/sofar.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/temp/__init__.py` & `boneIO-0.6.0.dev4/boneio/sensor/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/boneio/sensor/temp/dallas.py` & `boneIO-0.6.0.dev4/boneio/sensor/temp/dallas.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/pyproject.toml` & `boneIO-0.6.0.dev4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     "luma.core>=2.3.1",
     "luma.oled>=3.8.1",
     "pymodbus>=2.5.3",
     "pyserial-asyncio>=0.6",
     "PyYAML>=6.0",
     "Adafruit-BBIO>=1.2.0",
     "psutil>=5.9.1",
-    "adafruit-circuitpython-onewire>=2.0.1",
+    "adafruit-circuitpython-onewire>=2.0.4",
     "w1thermsensor[async]>=2.0.0",
     "adafruit-circuitpython-pca9685>=3.4.6",
 ]
 requires-python = ">=3.7"
-version = "0.6.0.dev3"
+version = "0.6.0.dev4"
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.urls]
 Homepage = "https://boneio.eu"
 Repository = "https://github.com/boneIO-eu/app_bbb"
@@ -50,14 +50,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=22.6.0",
     "isort>=5.10.1",
     "pre-commit>=2.19.0",
     "flake8>=4.0.1",
     "bandit>=1.7.4",
+    "setuptools>=67.6.1",
 ]
 
 [tool.pdm.scripts]
 lint = "pre-commit run --all-files"
 
 [tool.black]
 line-length = 88
```

### Comparing `boneIO-0.6.0.dev3/tests/relay_32_5.py` & `boneIO-0.6.0.dev4/tests/relay_32_5.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev3/PKG-INFO` & `boneIO-0.6.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boneIO
-Version: 0.6.0.dev3
+Version: 0.6.0.dev4
 Summary: Python App for BoneIO
 License: GNU General Public License v3.0
 Author-email: Paweł Szafer <pszafer@gmail.com>
 Requires-Python: >=3.7
 Project-URL: Changelog, https://github.com/boneIO-eu/app_bbb/releases
 Project-URL: Documentation, https://boneio.eu/docs/intro/
 Project-URL: Homepage, https://boneio.eu
```

