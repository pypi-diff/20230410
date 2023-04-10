# Comparing `tmp/ipfabric-6.2.0b3.tar.gz` & `tmp/ipfabric-6.2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.2.0b3.tar", max compression
+gzip compressed data, was "ipfabric-6.2.0b4.tar", max compression
```

## Comparing `ipfabric-6.2.0b3.tar` & `ipfabric-6.2.0b4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1790 2023-03-16 16:58:08.617128 ipfabric-6.2.0b3/ipfabric/__init__.py
--rw-r--r--   0        0        0    17674 2023-04-04 14:05:32.118649 ipfabric-6.2.0b3/ipfabric/api.py
--rw-r--r--   0        0        0     9218 2023-04-04 13:54:22.367500 ipfabric-6.2.0b3/ipfabric/client.py
--rw-r--r--   0        0        0      322 2023-02-08 21:33:38.498830 ipfabric-6.2.0b3/ipfabric/models/__init__.py
--rw-r--r--   0        0        0     6054 2023-03-14 15:20:54.722357 ipfabric-6.2.0b3/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2786 2023-03-14 15:45:17.816340 ipfabric-6.2.0b3/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0     2110 2023-02-09 13:14:16.640525 ipfabric-6.2.0b3/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     5669 2023-02-09 13:14:16.640525 ipfabric-6.2.0b3/ipfabric/models/jobs.py
--rw-r--r--   0        0        0    11726 2023-02-08 20:33:50.375972 ipfabric-6.2.0b3/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0    12162 2023-03-14 14:52:33.106216 ipfabric-6.2.0b3/ipfabric/models/table.py
--rw-r--r--   0        0        0     2830 2023-02-09 13:14:16.655535 ipfabric-6.2.0b3/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1156 2023-02-25 14:47:47.471307 ipfabric-6.2.0b3/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      488 2023-02-08 13:05:11.993384 ipfabric-6.2.0b3/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2173 2023-02-08 13:05:11.998383 ipfabric-6.2.0b3/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1002 2023-02-08 13:05:12.003471 ipfabric-6.2.0b3/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     7018 2023-02-25 14:47:47.471307 ipfabric-6.2.0b3/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      324 2023-02-08 13:05:12.011503 ipfabric-6.2.0b3/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0      843 2023-02-08 13:05:12.016497 ipfabric-6.2.0b3/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      470 2023-02-08 13:05:12.021499 ipfabric-6.2.0b3/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     5644 2023-02-08 13:05:12.027499 ipfabric-6.2.0b3/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2045 2023-02-25 14:47:47.482435 ipfabric-6.2.0b3/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     2783 2023-02-25 14:47:47.482435 ipfabric-6.2.0b3/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0      759 2023-02-08 13:05:12.031562 ipfabric-6.2.0b3/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      633 2023-02-08 13:05:12.031562 ipfabric-6.2.0b3/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     3529 2023-02-25 14:51:16.763228 ipfabric-6.2.0b3/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1231 2023-02-08 13:05:12.050282 ipfabric-6.2.0b3/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1078 2023-02-08 13:05:12.065065 ipfabric-6.2.0b3/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     4773 2023-02-25 14:51:16.794519 ipfabric-6.2.0b3/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2159 2023-02-08 13:05:12.078066 ipfabric-6.2.0b3/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      431 2023-02-08 13:05:12.083210 ipfabric-6.2.0b3/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2062 2023-02-08 13:05:12.088455 ipfabric-6.2.0b3/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2228 2023-02-08 13:05:12.092469 ipfabric-6.2.0b3/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0      856 2023-02-08 13:05:12.097528 ipfabric-6.2.0b3/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0      867 2023-02-08 13:05:12.097528 ipfabric-6.2.0b3/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.0b3/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3602 2023-02-09 20:02:01.172909 ipfabric-6.2.0b3/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6187 2023-02-08 13:05:11.963806 ipfabric-6.2.0b3/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.0b3/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.0b3/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.0b3/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     1413 2023-01-31 20:32:11.592169 ipfabric-6.2.0b3/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     4326 2023-02-09 18:30:40.306993 ipfabric-6.2.0b3/ipfabric/settings/user_mgmt.py
--rw-r--r--   0        0        0     1875 2023-02-08 14:40:46.626939 ipfabric-6.2.0b3/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     6439 2023-02-09 20:02:01.204437 ipfabric-6.2.0b3/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.0b3/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     7876 2023-03-30 17:03:49.576728 ipfabric-6.2.0b3/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.0b3/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/4/__init__.py
--rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/4/dashboard.json
--rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/4/groups.json
--rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/4/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-03 16:42:03.278481 ipfabric-6.2.0b3/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     5784 2023-01-31 20:32:11.624088 ipfabric-6.2.0b3/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0     2519 2023-02-09 19:07:57.301096 ipfabric-6.2.0b3/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2396 2023-02-09 18:58:27.499064 ipfabric-6.2.0b3/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2573 2023-03-24 18:58:14.154592 ipfabric-6.2.0b3/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.0b3/LICENSE
--rw-r--r--   0        0        0     2016 2023-04-04 14:07:08.012899 ipfabric-6.2.0b3/pyproject.toml
--rw-r--r--   0        0        0     3705 2023-04-04 13:32:24.957368 ipfabric-6.2.0b3/README.md
--rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 ipfabric-6.2.0b3/setup.py
--rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 ipfabric-6.2.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1790 2023-03-16 16:58:08.617128 ipfabric-6.2.0b4/ipfabric/__init__.py
+-rw-r--r--   0        0        0    17132 2023-04-05 16:49:28.923924 ipfabric-6.2.0b4/ipfabric/api.py
+-rw-r--r--   0        0        0     9218 2023-04-04 13:54:22.367500 ipfabric-6.2.0b4/ipfabric/client.py
+-rw-r--r--   0        0        0      322 2023-02-08 21:33:38.498830 ipfabric-6.2.0b4/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0     6054 2023-03-14 15:20:54.722357 ipfabric-6.2.0b4/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2786 2023-03-14 15:45:17.816340 ipfabric-6.2.0b4/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0     2110 2023-02-09 13:14:16.640525 ipfabric-6.2.0b4/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     5669 2023-02-09 13:14:16.640525 ipfabric-6.2.0b4/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0    12119 2023-04-05 17:31:47.761633 ipfabric-6.2.0b4/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0    12162 2023-03-14 14:52:33.106216 ipfabric-6.2.0b4/ipfabric/models/table.py
+-rw-r--r--   0        0        0     2830 2023-02-09 13:14:16.655535 ipfabric-6.2.0b4/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1156 2023-02-25 14:47:47.471307 ipfabric-6.2.0b4/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      488 2023-02-08 13:05:11.993384 ipfabric-6.2.0b4/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2173 2023-02-08 13:05:11.998383 ipfabric-6.2.0b4/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1002 2023-02-08 13:05:12.003471 ipfabric-6.2.0b4/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     7018 2023-02-25 14:47:47.471307 ipfabric-6.2.0b4/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      324 2023-02-08 13:05:12.011503 ipfabric-6.2.0b4/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0      843 2023-02-08 13:05:12.016497 ipfabric-6.2.0b4/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      470 2023-02-08 13:05:12.021499 ipfabric-6.2.0b4/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     5644 2023-02-08 13:05:12.027499 ipfabric-6.2.0b4/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2045 2023-02-25 14:47:47.482435 ipfabric-6.2.0b4/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     2783 2023-02-25 14:47:47.482435 ipfabric-6.2.0b4/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0      759 2023-02-08 13:05:12.031562 ipfabric-6.2.0b4/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      633 2023-02-08 13:05:12.031562 ipfabric-6.2.0b4/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     3529 2023-02-25 14:51:16.763228 ipfabric-6.2.0b4/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1231 2023-02-08 13:05:12.050282 ipfabric-6.2.0b4/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1078 2023-02-08 13:05:12.065065 ipfabric-6.2.0b4/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     4773 2023-02-25 14:51:16.794519 ipfabric-6.2.0b4/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2159 2023-02-08 13:05:12.078066 ipfabric-6.2.0b4/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      431 2023-02-08 13:05:12.083210 ipfabric-6.2.0b4/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2062 2023-02-08 13:05:12.088455 ipfabric-6.2.0b4/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2228 2023-02-08 13:05:12.092469 ipfabric-6.2.0b4/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0      856 2023-02-08 13:05:12.097528 ipfabric-6.2.0b4/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0      867 2023-02-08 13:05:12.097528 ipfabric-6.2.0b4/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.0b4/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3602 2023-02-09 20:02:01.172909 ipfabric-6.2.0b4/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6187 2023-02-08 13:05:11.963806 ipfabric-6.2.0b4/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.0b4/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.0b4/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.0b4/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     1413 2023-01-31 20:32:11.592169 ipfabric-6.2.0b4/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     5247 2023-04-05 17:31:47.706534 ipfabric-6.2.0b4/ipfabric/settings/user_mgmt.py
+-rw-r--r--   0        0        0     1875 2023-02-08 14:40:46.626939 ipfabric-6.2.0b4/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     6439 2023-02-09 20:02:01.204437 ipfabric-6.2.0b4/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.0b4/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     7876 2023-03-30 17:03:49.576728 ipfabric-6.2.0b4/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.0b4/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/__init__.py
+-rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/dashboard.json
+-rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/groups.json
+-rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/__init__.py
+-rw-r--r--   0        0        0     4511 2023-04-03 16:42:03.278481 ipfabric-6.2.0b4/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     5784 2023-01-31 20:32:11.624088 ipfabric-6.2.0b4/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0     2519 2023-02-09 19:07:57.301096 ipfabric-6.2.0b4/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2396 2023-02-09 18:58:27.499064 ipfabric-6.2.0b4/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2573 2023-03-24 18:58:14.154592 ipfabric-6.2.0b4/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.0b4/LICENSE
+-rw-r--r--   0        0        0     2016 2023-04-05 18:08:11.041198 ipfabric-6.2.0b4/pyproject.toml
+-rw-r--r--   0        0        0     3705 2023-04-04 13:32:24.957368 ipfabric-6.2.0b4/README.md
+-rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 ipfabric-6.2.0b4/setup.py
+-rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 ipfabric-6.2.0b4/PKG-INFO
```

### Comparing `ipfabric-6.2.0b3/ipfabric/__init__.py` & `ipfabric-6.2.0b4/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/api.py` & `ipfabric-6.2.0b4/ipfabric/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,18 @@
 
     @property
     def hostname(self):
         resp = self.get("/os/hostname")
         if resp.status_code == 200:
             return resp.json()["hostname"]
         elif resp.status_code == 403:
-            logger.critical(f'API_INSUFFICIENT_RIGHTS for user "{self.user.username}" on GET "/os/hostname".')
+            msg = f'API_INSUFFICIENT_RIGHTS for user "{self.user.username}" '
+            if self.user.token:
+                msg += f'token "{self.user.token.description}" '
+            logger.critical(msg + 'on GET "/os/hostname".')
             return None
         else:
             resp.raise_for_status()
 
     def _web_endpoints(self, base_url):
         resp = self.get(urljoin(base_url, "/api/oas/openapi-extended.json"))
         resp.raise_for_status()
@@ -363,28 +366,14 @@
         version
         initialVersion
         """
         res = self.get("/snapshots")
         res.raise_for_status()
         return {s["id"]: s for s in res.json()}
 
-    def _get_snapshot_settings(self, snapshot_id):
-        ae_tasks = dict(graphCache=None, historicalData=None, intentVerification=None)
-        res = self.get(f"/snapshots/{snapshot_id}/settings")
-        try:
-            res.raise_for_status()
-            disabled = res.json().get("disabledPostDiscoveryActions", list())
-            [ae_tasks.update({t: True if t in disabled else False}) for t in ae_tasks]
-        except httpx.HTTPError:
-            logger.warning(
-                "User/Token does not have access to `snapshots/:key/settings`; "
-                "cannot get status of Assurance Engine tasks."
-            )
-        return ae_tasks
-
     def get_snapshots(self):
         """Gets all snapshots from IP Fabric and returns a dictionary of {ID:   Snapshot_info}
 
         Returns:
             Dictionary with ID as key and dictionary with info as the value
         """
         payload = {"columns": SNAPSHOT_COLUMNS, "sort": {"order": "desc", "column": "tsEnd"}}
```

### Comparing `ipfabric-6.2.0b3/ipfabric/client.py` & `ipfabric-6.2.0b4/ipfabric/client.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/intent.py` & `ipfabric-6.2.0b4/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/intent_check.py` & `ipfabric-6.2.0b4/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/inventory.py` & `ipfabric-6.2.0b4/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/jobs.py` & `ipfabric-6.2.0b4/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/snapshot.py` & `ipfabric-6.2.0b4/ipfabric/models/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,29 +216,36 @@
             with open(path, "wb") as fp:
                 fp.write(filename.read())
             return path
         logger.error(f"Download job did not finish within {retry * timeout} seconds, could not get file.")
         return None
 
     def get_snapshot_settings(self, ipf: Union[IPFClient, IPFabricAPI]):
+        settings = None
+        msg = "API_INSUFFICIENT_RIGHTS to `snapshots/:key/settings` " + ipf.user.error_msg
+
+        if ipf.user.get_snapshots_settings is False:
+            logger.debug(f"Could not get Snapshot {self.snapshot_id} Settings:" + msg)
+            return settings
         res = ipf.get(f"/snapshots/{self.snapshot_id}/settings")
         try:
             res.raise_for_status()
-            return res.json()
+            settings = res.json()
+            if ipf.user.get_snapshots_settings is None:
+                ipf.user.set_snapshots_settings(True)
         except HTTPError:
-            logger.warning(
-                "User/Token does not have access to `snapshots/:key/settings`; "
-                "cannot get status of Assurance Engine tasks."
-            )
-        return None
+            logger.debug(f"Could not get Snapshot {self.snapshot_id} Settings:" + msg)
+            logger.warning(msg)
+            ipf.user.set_snapshots_settings(False)
+        return settings
 
     def get_assurance_engine_settings(self, ipf: Union[IPFClient, IPFabricAPI]):
         settings = self.get_snapshot_settings(ipf)
         if settings is None:
-            logger.error(f"Could not get Snapshot {self.snapshot_id} Settings to verify Assurance Engine tasks.")
+            logger.debug(f"Could not get Snapshot {self.snapshot_id} Settings to verify Assurance Engine tasks.")
             return None
         disabled = settings.get("disabledPostDiscoveryActions", list())
         self.disabled_graph_cache = True if "graphCache" in disabled else False
         self.disabled_historical_data = True if "historicalData" in disabled else False
         self.disabled_intent_verification = True if "intentVerification" in disabled else False
         return dict(
             disabled_graph_cache=self.disabled_graph_cache,
```

### Comparing `ipfabric-6.2.0b3/ipfabric/models/table.py` & `ipfabric-6.2.0b4/ipfabric/models/table.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/__init__.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/addressing.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/dhcp.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/fhrp.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/interfaces.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/management.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/mpls.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/multicast.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/neighbors.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/oam.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/platforms.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/port_channels.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/qos.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/routing.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/sdn.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/security.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/stp.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/vlans.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/models/technology/wireless.py` & `ipfabric-6.2.0b4/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/__init__.py` & `ipfabric-6.2.0b4/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/api_tokens.py` & `ipfabric-6.2.0b4/ipfabric/settings/api_tokens.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/attributes.py` & `ipfabric-6.2.0b4/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/authentication.py` & `ipfabric-6.2.0b4/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/discovery.py` & `ipfabric-6.2.0b4/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/seeds.py` & `ipfabric-6.2.0b4/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/site_separation.py` & `ipfabric-6.2.0b4/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/user_mgmt.py` & `ipfabric-6.2.0b4/ipfabric/settings/user_mgmt.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,43 @@
     sso_provider: Optional[Any] = Field(alias="ssoProvider")
     domains: Optional[Any] = Field(alias="domainSuffixes")
     role_names: Optional[list] = Field(alias="roleNames", default_factory=list)
     role_ids: list = Field(alias="roleIds")
     ldap_id: Optional[Any] = Field(alias="ldapId")
     timezone: Optional[str]
     token: Optional[Token]
+    _get_snapshots_settings: Optional[bool] = None
+
+    class Config:
+        underscore_attrs_are_private = True
+
+    @property
+    def is_admin(self):
+        return (
+            True
+            if (self.token and "admin" in self.token.role_ids) or (not self.token and "admin" in self.role_ids)
+            else False
+        )
+
+    @property
+    def get_snapshots_settings(self):
+        """If the User/Token has access to snapshots/:key/settings Endpoint."""
+        if self._get_snapshots_settings is None and self.is_admin:
+            self._get_snapshots_settings = True
+        return self._get_snapshots_settings
+
+    def set_snapshots_settings(self, v: bool):
+        self._get_snapshots_settings = v
+
+    @property
+    def error_msg(self):
+        msg = f'User "{self.username}" '
+        if self.token:
+            msg += f'Token "{self.token.description}" '
+        return msg
 
 
 class Role(BaseModel):
     role_id: str = Field(alias="id")
     name: str
     description: Optional[str]
     role_type: str = Field(alias="type")
```

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/vendor_api.py` & `ipfabric-6.2.0b4/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.2.0b4/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/configuration.py` & `ipfabric-6.2.0b4/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/discovery_history.py` & `ipfabric-6.2.0b4/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/4/dashboard.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/4/groups.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v4/4/intents.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/0/dashboard.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/0/groups.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v5/0/intents.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/0/dashboard.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/0/groups.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/factory_defaults/v6/0/intents.json` & `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/nist.py` & `ipfabric-6.2.0b4/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/restore_intents.py` & `ipfabric-6.2.0b4/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/shared.py` & `ipfabric-6.2.0b4/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.2.0b4/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.2.0b4/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/LICENSE` & `ipfabric-6.2.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/pyproject.toml` & `ipfabric-6.2.0b4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.2.0b3"
+version = "v6.2.0b4"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
```

### Comparing `ipfabric-6.2.0b3/README.md` & `ipfabric-6.2.0b4/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b3/setup.py` & `ipfabric-6.2.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
               'openpyxl>=3.0.9,<4.0.0',
               'tabulate>=0.8.9,<0.10.0',
               'python-json-logger>=2.0.4,<3.0.0',
               'pyyaml>=6.0,<7.0']}
 
 setup_kwargs = {
     'name': 'ipfabric',
-    'version': '6.2.0b3',
+    'version': '6.2.0b4',
     'description': 'Python package for interacting with IP Fabric',
     'long_description': '# IP Fabric \n\nIPFabric is a Python module for connecting to and communicating against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation. \n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token=\'<TOKEN>\'` or `username=\'<USER>\', password=\'<PASS>\'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth=\'TOKEN\')`\n  - User/Pass: `IPFClient(auth=(\'USER\', \'PASS\'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API\'s are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK\'s match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric\n```\n\n## Introduction\n\nPlease take a look at [API Programmability - Part 1: The Basics](https://ipfabric.io/blog/api-programmability-part-1/)\nfor instructions on creating an API token.\n\nMost of the methods and features can be located in [Examples](examples) to show how to use this package. \nAnother great introduction to this package can be found at [API Programmability - Part 2: Python](https://ipfabric.io/blog/api-programmability-python/)\n\n## Diagrams\n\nDiagramming in IP Fabric version v4.3 and above has been moved to it\'s own package.\n\nDiagramming will move back to this project in v7.0\n\n```\npip install ipfabric-diagrams\n```\n\n## Authentication\n### Username/Password\nSupply in client:\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=(\'user\', \'pass\'))\n```\n\n### Token\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=\'token\')\n```\n\n### Environment \nThe easiest way to use this package is with a `.env` file.  You can copy the sample and edit it with your environment variables. \n\n```commandline\ncp sample.env .env\n```\n\nThis contains the following variables which can also be set as environment variables instead of a .env file.\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_TOKEN=TOKEN\nIPF_VERIFY=true\n```\n\nOr if using Username/Password:\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_USERNAME=USER\nIPF_PASSWORD=PASS\n```\n\n## Development\n\n### Poetry Installation\n\nIPFabric uses [Poetry](https://pypi.org/project/poetry/) to make setting up a virtual environment with all dependencies\ninstalled quick and easy.\n\nInstall poetry globally:\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo run examples, install extras:\n```\npoetry install ipfabric -E examples\n```\n\n### Test and Build\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric\npoetry update\n```\n',
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric',
```

### Comparing `ipfabric-6.2.0b3/PKG-INFO` & `ipfabric-6.2.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.2.0b3
+Version: 6.2.0b4
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
```

