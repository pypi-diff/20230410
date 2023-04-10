# Comparing `tmp/runtimepy-1.2.0.tar.gz` & `tmp/runtimepy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.2.0.tar", last modified: Sun Apr  9 08:16:17 2023, max compression
+gzip compressed data, was "runtimepy-1.3.0.tar", last modified: Sun Apr  9 21:33:47 2023, max compression
```

## Comparing `runtimepy-1.2.0.tar` & `runtimepy-1.3.0.tar`

### file list

```diff
@@ -1,131 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 08:14:51.000000 runtimepy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-09 08:16:17.256465 runtimepy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-09 08:14:51.000000 runtimepy-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-09 08:14:51.000000 runtimepy-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.240465 runtimepy-1.2.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.240465 runtimepy-1.2.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.236465 runtimepy-1.2.0/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mixins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/udp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/task/basic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.240465 runtimepy-1.2.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:16:17.256465 runtimepy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 08:14:51.000000 runtimepy-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 08:14:51.000000 runtimepy-1.2.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-09 08:14:51.000000 runtimepy-1.2.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 08:14:51.000000 runtimepy-1.2.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.883755 runtimepy-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 21:32:26.000000 runtimepy-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-09 21:33:47.883755 runtimepy-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-09 21:32:26.000000 runtimepy-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-09 21:32:26.000000 runtimepy-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.855755 runtimepy-1.3.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.855755 runtimepy-1.3.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.859755 runtimepy-1.3.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.859755 runtimepy-1.3.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.859755 runtimepy-1.3.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.863755 runtimepy-1.3.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.843755 runtimepy-1.3.0/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.863755 runtimepy-1.3.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.867755 runtimepy-1.3.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.867755 runtimepy-1.3.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/mixins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.867755 runtimepy-1.3.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.867755 runtimepy-1.3.0/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.871755 runtimepy-1.3.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.871755 runtimepy-1.3.0/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.871755 runtimepy-1.3.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.871755 runtimepy-1.3.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.871755 runtimepy-1.3.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/udp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.875755 runtimepy-1.3.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.875755 runtimepy-1.3.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.879755 runtimepy-1.3.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.879755 runtimepy-1.3.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.879755 runtimepy-1.3.0/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.879755 runtimepy-1.3.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.883755 runtimepy-1.3.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.883755 runtimepy-1.3.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/task/basic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.883755 runtimepy-1.3.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.883755 runtimepy-1.3.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.883755 runtimepy-1.3.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-09 21:32:26.000000 runtimepy-1.3.0/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.855755 runtimepy-1.3.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-09 21:33:47.000000 runtimepy-1.3.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-09 21:33:47.000000 runtimepy-1.3.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:33:47.000000 runtimepy-1.3.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 21:33:47.000000 runtimepy-1.3.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-09 21:33:47.000000 runtimepy-1.3.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 21:33:47.000000 runtimepy-1.3.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 21:33:47.883755 runtimepy-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 21:32:26.000000 runtimepy-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:47.883755 runtimepy-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 21:32:26.000000 runtimepy-1.3.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-09 21:32:26.000000 runtimepy-1.3.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 21:32:26.000000 runtimepy-1.3.0/tests/test_resources.py
```

### Comparing `runtimepy-1.2.0/LICENSE` & `runtimepy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/PKG-INFO` & `runtimepy-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.2.0
+Version: 1.3.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ce3f1316217e521947cc4b3047971525
+    hash=7c98e655e98208996b70a51005eccaca
     =====================================
 -->
 
-# runtimepy ([1.2.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.3.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.2.0/README.md` & `runtimepy-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ce3f1316217e521947cc4b3047971525
+    hash=7c98e655e98208996b70a51005eccaca
     =====================================
 -->
 
-# runtimepy ([1.2.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.3.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.2.0/pyproject.toml` & `runtimepy-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.2.0"
+version = "1.3.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-1.2.0/runtimepy/app.py` & `runtimepy-1.3.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/__init__.py` & `runtimepy-1.3.0/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/environment/__init__.py` & `runtimepy-1.3.0/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/environment/array.py` & `runtimepy-1.3.0/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/environment/base.py` & `runtimepy-1.3.0/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/environment/create.py` & `runtimepy-1.3.0/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/environment/file.py` & `runtimepy-1.3.0/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/environment/names.py` & `runtimepy-1.3.0/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/channel/registry.py` & `runtimepy-1.3.0/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/codec/protocol/base.py` & `runtimepy-1.3.0/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/codec/protocol/json.py` & `runtimepy-1.3.0/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/commands/all.py` & `runtimepy-1.3.0/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/commands/arbiter.py` & `runtimepy-1.3.0/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/commands/tui.py` & `runtimepy-1.3.0/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.3.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.3.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,21 @@
 
   servers:
     type: array
     items:
       $ref: package://runtimepy/schemas/ServerConnectionConfig.yaml
 
   app:
+    # This is the default application.
+    # default: "runtimepy.net.apps.init_only"
     type: string
-    default: "runtimepy.net.arbiter.base.init_only"
+
+  # Application configuration data.
+  config:
+    type: object
 
   factories:
     type: array
     items:
       type: object
       required: [name]
       additionalProperties: false
```

### Comparing `runtimepy-1.2.0/runtimepy/entry.py` & `runtimepy-1.3.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/enum/__init__.py` & `runtimepy-1.3.0/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/enum/registry.py` & `runtimepy-1.3.0/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/enum/type.py` & `runtimepy-1.3.0/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/mapping.py` & `runtimepy-1.3.0/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/mixins/enum.py` & `runtimepy-1.3.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/mixins/regex.py` & `runtimepy-1.3.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/__init__.py` & `runtimepy-1.3.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/arbiter/base.py` & `runtimepy-1.3.0/runtimepy/net/arbiter/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,39 +7,49 @@
 from contextlib import AsyncExitStack as _AsyncExitStack
 from inspect import isawaitable as _isawaitable
 from typing import Awaitable as _Awaitable
 from typing import Callable as _Callable
 from typing import Iterable as _Iterable
 from typing import List as _List
 from typing import MutableMapping as _MutableMapping
+from typing import NamedTuple
 from typing import Union as _Union
 
 # third-party
 from vcorelib.asyncio import run_handle_stop as _run_handle_stop
+from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.logging import LoggerMixin as _LoggerMixin
 from vcorelib.logging import LoggerType as _LoggerType
 from vcorelib.namespace import Namespace as _Namespace
 from vcorelib.namespace import NamespaceMixin as _NamespaceMixin
 
 # internal
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 
 ConnectionMap = _MutableMapping[str, _Connection]
-NetworkApplication = _Callable[
-    [_AsyncExitStack, ConnectionMap], _Awaitable[int]
-]
+
+
+class AppInfo(NamedTuple):
+    """References provided to network applications."""
+
+    stack: _AsyncExitStack
+    connections: ConnectionMap
+    stop: _asyncio.Event
+    config: _JsonObject
+
+
+NetworkApplication = _Callable[[AppInfo], _Awaitable[int]]
 ServerTask = _Awaitable[None]
 
 
-async def init_only(stack: _AsyncExitStack, connections: ConnectionMap) -> int:
+async def init_only(app: AppInfo) -> int:
     """A network application that doesn't do anything."""
 
-    del stack
-    del connections
+    del app
     return 0
 
 
 class BaseConnectionArbiter(_NamespaceMixin, _LoggerMixin):
     """
     A class implementing a base connection-manager for a broader application.
     """
@@ -47,14 +57,15 @@
     def __init__(
         self,
         manager: _ConnectionManager = None,
         stop_sig: _asyncio.Event = None,
         namespace: _Namespace = None,
         logger: _LoggerType = None,
         app: NetworkApplication = init_only,
+        config: _JsonObject = None,
     ) -> None:
         """Initialize this connection arbiter."""
 
         _LoggerMixin.__init__(self, logger=logger)
 
         if manager is None:
             manager = _ConnectionManager()
@@ -66,14 +77,19 @@
 
         _NamespaceMixin.__init__(self, namespace=namespace)
 
         # A fallback application. Set a class attribute so this can be more
         # easily externally updated.
         self._app = app
 
+        # Application configuration data.
+        if config is None:
+            config = {}
+        self._config = config
+
         # Keep track of connection objects.
         self._connections: ConnectionMap = {}
         self._deferred_connections: _MutableMapping[
             str, _Awaitable[_Connection]
         ] = {}
 
         self._servers: _List[ServerTask] = []
@@ -115,15 +131,18 @@
                 self._register_connection(connection, name)
 
             result = True
 
         return result
 
     async def _entry(
-        self, app: NetworkApplication = None, check_connections: bool = True
+        self,
+        app: NetworkApplication = None,
+        check_connections: bool = True,
+        config: _JsonObject = None,
     ) -> int:
         """
         Ensures connections are given a chance to initialize, run the
         application, clean up connections and return the application's result.
         """
 
         result = -1
@@ -154,48 +173,61 @@
             ):
                 async with _AsyncExitStack() as stack:
                     self.logger.info("Application starting.")
 
                     if app is None:
                         app = self._app
 
-                    result = await app(stack, self._connections)
+                    result = await app(
+                        AppInfo(
+                            stack,
+                            self._connections,
+                            self.stop_sig,
+                            config if config is not None else self._config,
+                        )
+                    )
                     self.logger.info("Application returned %d.", result)
 
         finally:
             for conn in self._connections.values():
                 conn.disable(f"app exit {result}")
             self.stop_sig.set()
 
         return result
 
     async def app(
         self,
         app: NetworkApplication = None,
         check_connections: bool = True,
+        config: _JsonObject = None,
     ) -> int:
         """
         Run the application alongside the connection manager and server tasks.
         """
 
         result = await _asyncio.gather(
-            self._entry(app, check_connections=check_connections),
+            self._entry(
+                app, check_connections=check_connections, config=config
+            ),
             self.manager.manage(self.stop_sig),
             *self._servers,
         )
         return int(result[0])
 
     def run(
         self,
         app: NetworkApplication = None,
         eloop: _asyncio.AbstractEventLoop = None,
         signals: _Iterable[int] = None,
         check_connections: bool = True,
+        config: _JsonObject = None,
     ) -> int:
         """Run the application until the stop signal is set."""
 
         return _run_handle_stop(
             self.stop_sig,
-            self.app(app=app, check_connections=check_connections),
+            self.app(
+                app=app, check_connections=check_connections, config=config
+            ),
             eloop=eloop,
             signals=signals,
         )
```

### Comparing `runtimepy-1.2.0/runtimepy/net/arbiter/config.py` & `runtimepy-1.3.0/runtimepy/net/arbiter/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 # built-in
 import socket as _socket
 from typing import Any as _Any
 from typing import Dict as _Dict
 from typing import List as _List
+from typing import Optional as _Optional
 from typing import cast as _cast
 
 # third-party
 from vcorelib.dict.env import dict_resolve_env_vars, list_resolve_env_vars
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.paths import Pathlike as _Pathlike
 
@@ -39,15 +40,19 @@
             self.ports[item["name"]] = get_free_socket_name(
                 local=normalize_host(item["host"], item["port"]),
                 kind=_socket.SOCK_STREAM
                 if item["type"] == "tcp"
                 else _socket.SOCK_DGRAM,
             ).port
 
-        self.app: str = data["app"]  # type: ignore
+        self.app: _Optional[str] = data.get("app")  # type: ignore
+        self.config: _Optional[_JsonObject] = _cast(
+            _JsonObject, data.get("config")
+        )
+
         self.factories: _List[_Any] = data.get("factories", [])  # type: ignore
         self.clients: _List[_Any] = data.get("clients", [])  # type: ignore
         self.servers: _List[_Any] = data.get("servers", [])  # type: ignore
 
     def asdict(self) -> _JsonObject:
         """Obtain a dictionary representing this instance."""
         return self.data
@@ -87,15 +92,18 @@
     """
     A class implementing a configuration loading interface for the connection
     arbiter.
     """
 
     async def load_config(self, path: _Pathlike) -> None:
         """Load a client and server configuration to the arbiter."""
-        await self.process_config(ConnectionArbiterConfig.decode(path))
+
+        await self.process_config(
+            ConnectionArbiterConfig.decode(path, includes_key="includes")
+        )
 
     async def process_config(self, config: ConnectionArbiterConfig) -> None:
         """Register clients and servers from a configuration object."""
 
         # Registier factories.
         for factory in config.factories:
             name = factory["name"]
@@ -137,9 +145,14 @@
                     server.get("args", []), env=config.ports  # type: ignore
                 ),
                 **dict_resolve_env_vars(
                     server.get("kwargs", {}), env=config.ports  # type: ignore
                 ),
             ), f"Couldn't register a '{factory}' server!"
 
-        # Set the new (default) application entry.
-        self.set_app(config.app)
+        # Set the new application entry if it's set.
+        if config.app is not None:
+            self.set_app(config.app)
+
+        # Update application configuration data if necessary.
+        if config.config is not None:
+            self._config = config.config
```

### Comparing `runtimepy-1.2.0/runtimepy/net/arbiter/factory.py` & `runtimepy-1.3.0/runtimepy/net/arbiter/factory.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/arbiter/imports.py` & `runtimepy-1.3.0/runtimepy/net/arbiter/imports.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.3.0/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/arbiter/udp.py` & `runtimepy-1.3.0/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.3.0/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/connection.py` & `runtimepy-1.3.0/runtimepy/net/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,7 +189,21 @@
             # Attempt to get the next message.
             data = await queue.get()
 
             # Process it.
             if data is not None:
                 await self._send_binay_message(data)
                 queue.task_done()
+
+
+class EchoConnection(Connection):
+    """A connection that just echoes what it was sent."""
+
+    async def process_text(self, data: str) -> bool:
+        """Process a text frame."""
+        self.send_text(data)
+        return True
+
+    async def process_binary(self, data: bytes) -> bool:
+        """Process a binary frame."""
+        self.send_binary(data)
+        return True
```

### Comparing `runtimepy-1.2.0/runtimepy/net/manager.py` & `runtimepy-1.3.0/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/mixin.py` & `runtimepy-1.3.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/tcp/connection.py` & `runtimepy-1.3.0/runtimepy/net/tcp/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # third-party
 from vcorelib.logging import LoggerType as _LoggerType
 
 # internal
 from runtimepy.net import sockname as _sockname
 from runtimepy.net.connection import BinaryMessage as _BinaryMessage
 from runtimepy.net.connection import Connection as _Connection
+from runtimepy.net.connection import EchoConnection as _EchoConnection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 from runtimepy.net.mixin import (
     BinaryMessageQueueMixin as _BinaryMessageQueueMixin,
 )
 from runtimepy.net.mixin import TransportMixin as _TransportMixin
 
 LOG = _getLogger(__name__)
@@ -190,7 +191,11 @@
 
         assert conn1 is not None
         return conn1, conn2
 
     async def close(self) -> None:
         """Close this connection."""
         self._transport.close()
+
+
+class EchoTcpConnection(TcpConnection, _EchoConnection):
+    """An echo connection for TCP."""
```

### Comparing `runtimepy-1.2.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.3.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.3.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/net/udp/connection.py` & `runtimepy-1.3.0/runtimepy/net/udp/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # third-party
 from vcorelib.logging import LoggerType as _LoggerType
 
 # internal
 from runtimepy.net import IpHost, get_free_socket
 from runtimepy.net.connection import BinaryMessage as _BinaryMessage
 from runtimepy.net.connection import Connection as _Connection
+from runtimepy.net.connection import EchoConnection as _EchoConnection
 from runtimepy.net.mixin import TransportMixin as _TransportMixin
 
 LOG = _getLogger(__name__)
 
 
 class UdpQueueProtocol(_DatagramProtocol):
     """A simple UDP protocol that populates a message queue."""
@@ -142,7 +143,19 @@
 
             if message is not None:
                 result = await self.process_datagram(message[0], message[1])
 
             # If we failed to read a message, disable.
             if not result:
                 self.disable("read processing error")
+
+
+class EchoUdpConnection(UdpConnection, _EchoConnection):
+    """An echo connection for UDP."""
+
+    async def process_datagram(
+        self, data: bytes, addr: _Tuple[str, int]
+    ) -> bool:
+        """Process a datagram."""
+
+        self.sendto(data, addr=addr)
+        return True
```

### Comparing `runtimepy-1.2.0/runtimepy/net/websocket/connection.py` & `runtimepy-1.3.0/runtimepy/net/websocket/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 )
 from websockets.server import WebSocketServer as _WebSocketServer
 from websockets.server import serve as _serve
 
 # internal
 from runtimepy.net import sockname as _sockname
 from runtimepy.net.connection import BinaryMessage, Connection
+from runtimepy.net.connection import EchoConnection as _EchoConnection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 
 T = _TypeVar("T", bound="WebsocketConnection")
 ConnectionInit = _Callable[[T], _Awaitable[bool]]
 V = _TypeVar("V")
 LOG = _getLogger(__name__)
 
@@ -202,7 +203,11 @@
                 serving_callback(server)
 
             LOG.info("WebSocket Application starting.")
             await manager.manage(stop_sig)
             LOG.info("WebSocket Application stopped.")
 
         LOG.info("WebSocket Server closed.")
+
+
+class EchoWebsocketConnection(WebsocketConnection, _EchoConnection):
+    """An echo connection for WebSocket."""
```

### Comparing `runtimepy-1.2.0/runtimepy/primitives/__init__.py` & `runtimepy-1.3.0/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/array.py` & `runtimepy-1.3.0/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/base.py` & `runtimepy-1.3.0/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/bool.py` & `runtimepy-1.3.0/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/byte_order.py` & `runtimepy-1.3.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/field/__init__.py` & `runtimepy-1.3.0/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/field/fields.py` & `runtimepy-1.3.0/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.3.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.3.0/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/float.py` & `runtimepy-1.3.0/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/int.py` & `runtimepy-1.3.0/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/string.py` & `runtimepy-1.3.0/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/type/__init__.py` & `runtimepy-1.3.0/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/type/base.py` & `runtimepy-1.3.0/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/type/float.py` & `runtimepy-1.3.0/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/primitives/type/int.py` & `runtimepy-1.3.0/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/registry/__init__.py` & `runtimepy-1.3.0/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/registry/bool.py` & `runtimepy-1.3.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/registry/item.py` & `runtimepy-1.3.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/registry/name.py` & `runtimepy-1.3.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/schemas.py` & `runtimepy-1.3.0/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/task/__init__.py` & `runtimepy-1.3.0/runtimepy/task/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/task/basic/__init__.py` & `runtimepy-1.3.0/runtimepy/task/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/tui/channels/__init__.py` & `runtimepy-1.3.0/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy/tui/task.py` & `runtimepy-1.3.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.3.0/runtimepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.2.0
+Version: 1.3.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ce3f1316217e521947cc4b3047971525
+    hash=7c98e655e98208996b70a51005eccaca
     =====================================
 -->
 
-# runtimepy ([1.2.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.3.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.2.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.3.0/runtimepy.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -48,22 +48,24 @@
 runtimepy/mixins/__init__.py
 runtimepy/mixins/enum.py
 runtimepy/mixins/regex.py
 runtimepy/net/__init__.py
 runtimepy/net/connection.py
 runtimepy/net/manager.py
 runtimepy/net/mixin.py
+runtimepy/net/apps/__init__.py
 runtimepy/net/arbiter/__init__.py
 runtimepy/net/arbiter/base.py
 runtimepy/net/arbiter/config.py
 runtimepy/net/arbiter/factory.py
 runtimepy/net/arbiter/imports.py
 runtimepy/net/arbiter/tcp.py
 runtimepy/net/arbiter/udp.py
 runtimepy/net/arbiter/websocket.py
+runtimepy/net/factories/__init__.py
 runtimepy/net/tcp/__init__.py
 runtimepy/net/tcp/connection.py
 runtimepy/net/tcp/telnet/__init__.py
 runtimepy/net/tcp/telnet/codes.py
 runtimepy/net/udp/__init__.py
 runtimepy/net/udp/connection.py
 runtimepy/net/websocket/__init__.py
```

### Comparing `runtimepy-1.2.0/setup.py` & `runtimepy-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/tests/test_entry.py` & `runtimepy-1.3.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.2.0/tests/test_mapping.py` & `runtimepy-1.3.0/tests/test_mapping.py`

 * *Files identical despite different names*

