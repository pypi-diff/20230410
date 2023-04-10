# Comparing `tmp/systembridgebackend-3.6.3.dev5.tar.gz` & `tmp/systembridgebackend-3.6.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-3.6.3.dev5.tar", last modified: Sat Feb 18 15:17:27 2023, max compression
+gzip compressed data, was "systembridgebackend-3.6.3.dev6.tar", last modified: Mon Apr 10 15:36:50 2023, max compression
```

## Comparing `systembridgebackend-3.6.3.dev5.tar` & `systembridgebackend-3.6.3.dev6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.282072 systembridgebackend-3.6.3.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-18 15:17:27.282072 systembridgebackend-3.6.3.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 15:17:27.282072 systembridgebackend-3.6.3.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-18 15:17:25.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/battery/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/battery/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/cpu/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/disk/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/disk/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/display/
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/display/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/gpu/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/memory/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/network/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/network/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/sensors/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/system/
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/system/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.282072 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.282072 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/autostart/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/autostart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/autostart/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/autostart/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/remote_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.282072 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/shortcuts/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/shortcuts/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-18 15:17:10.000000 systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:17:27.278072 systembridgebackend-3.6.3.dev5/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-18 15:17:27.000000 systembridgebackend-3.6.3.dev5/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-18 15:17:27.000000 systembridgebackend-3.6.3.dev5/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 15:17:27.000000 systembridgebackend-3.6.3.dev5/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-18 15:17:27.000000 systembridgebackend-3.6.3.dev5/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-18 15:17:27.000000 systembridgebackend-3.6.3.dev5/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-10 15:36:48.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/battery/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/battery/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/cpu/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/disk/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/display/
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/display/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/gpu/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/memory/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/network/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/sensors/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/system/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/autostart/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/autostart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/autostart/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/autostart/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/remote_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.080907 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/shortcuts/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/shortcuts/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-10 15:36:25.000000 systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:36:50.076907 systembridgebackend-3.6.3.dev6/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-10 15:36:50.000000 systembridgebackend-3.6.3.dev6/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-10 15:36:50.000000 systembridgebackend-3.6.3.dev6/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:36:50.000000 systembridgebackend-3.6.3.dev6/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-10 15:36:50.000000 systembridgebackend-3.6.3.dev6/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:36:50.000000 systembridgebackend-3.6.3.dev6/systembridgebackend.egg-info/top_level.txt
```

### Comparing `systembridgebackend-3.6.3.dev5/pyproject.toml` & `systembridgebackend-3.6.3.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/setup.py` & `systembridgebackend-3.6.3.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/__main__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/data.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/gui.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/gui.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/icon.ico` & `systembridgebackend-3.6.3.dev6/systembridgebackend/icon.ico`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/icon.png` & `systembridgebackend-3.6.3.dev6/systembridgebackend/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/battery/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/battery/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/battery/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/battery/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/cpu/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/cpu/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/cpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/disk/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/disk/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/disk/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/display/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/display/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/display/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/display/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/gpu/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/gpu/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/gpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/listeners.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/memory/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/memory/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/network/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/network/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/network/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/network/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/sensors/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/sensors/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/sensors/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/system/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/system/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/system/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/system/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/modules/update.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/modules/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/server/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/server/api.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/server/mdns.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/server/websocket.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/action.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/autostart/__init__.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/autostart/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/autostart/linux.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/autostart/linux.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/autostart/windows.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/autostart/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/keyboard.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/media.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/power.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/shortcuts/linux.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/shortcuts/linux.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend/utilities/shortcuts/windows.py` & `systembridgebackend-3.6.3.dev6/systembridgebackend/utilities/shortcuts/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev5/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-3.6.3.dev6/systembridgebackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*
