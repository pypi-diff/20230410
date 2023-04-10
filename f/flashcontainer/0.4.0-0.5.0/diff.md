# Comparing `tmp/flashcontainer-0.4.0.tar.gz` & `tmp/flashcontainer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcontainer-0.4.0.tar", last modified: Fri Mar 24 14:54:44 2023, max compression
+gzip compressed data, was "flashcontainer-0.5.0.tar", last modified: Mon Apr 10 12:06:48 2023, max compression
```

## Comparing `flashcontainer-0.4.0.tar` & `flashcontainer-0.5.0.tar`

### file list

```diff
@@ -1,101 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.278459 flashcontainer-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.266459 flashcontainer-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.270459 flashcontainer-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.270459 flashcontainer-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    39391 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/Concept.png
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/Developing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-03-24 14:54:44.278459 flashcontainer-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.270459 flashcontainer-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.270459 flashcontainer-0.4.0/examples/arduino/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.270459 flashcontainer-0.4.0/examples/arduino/.pio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.270459 flashcontainer-0.4.0/examples/arduino/.pio/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/arduino/.pio/build/ATmega328P/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12596 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/.pio/build/ATmega328P/firmware.elf
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/.pio/build/ATmega328P/firmware.hex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/arduino/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/avr5.xn
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/example.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/gen_param.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)       71 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/gen_param.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/arduino/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/include/README
--rw-r--r--   0 runner    (1001) docker     (123)    43240 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/output.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/arduino/param/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/param/param.c
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/param/param.h
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/param/param.hex
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/param/param.ld
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/param/param.pyhexdump
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/param/param.xml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/platformio.ini
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/run_simavr.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/run_simavr.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/arduino/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/arduino/test/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/arduino/test/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/aurix_bmhdr/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/aurix_bmhdr/bmhdr.mao
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/aurix_bmhdr/bmhdr.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/aurix_bmhdr/example.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/aurix_bmhdr/run.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/aurix_bmhdr/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/examples/safety/
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/safety/example.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/safety/run.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/safety/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/examples/safety/safety.xml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/overview.plantuml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-24 14:54:44.278459 flashcontainer-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.270459 flashcontainer-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.274459 flashcontainer-0.4.0/src/flashcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/a2lwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/byteconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/cfilewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)    17191 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/gnuldwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/hexwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/packageinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/pargen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/pargen_1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/pyhexdumpwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/src/flashcontainer/xmlparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.278459 flashcontainer-0.4.0/src/flashcontainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-03-24 14:54:44.000000 flashcontainer-0.4.0/src/flashcontainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-24 14:54:44.000000 flashcontainer-0.4.0/src/flashcontainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:54:44.000000 flashcontainer-0.4.0/src/flashcontainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-24 14:54:44.000000 flashcontainer-0.4.0/src/flashcontainer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 14:54:44.000000 flashcontainer-0.4.0/src/flashcontainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-24 14:54:44.000000 flashcontainer-0.4.0/src/flashcontainer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.278459 flashcontainer-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.278459 flashcontainer-0.4.0/tests/collateral/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/collateral/fail_validation.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/collateral/invalid.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:54:44.278459 flashcontainer-0.4.0/tests/example/
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/example/example.xml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/example/run.bat
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/example/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/test_byteconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/test_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/test_model_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/test_pargen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-03-24 14:54:25.000000 flashcontainer-0.4.0/tests/test_xmlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.318603 flashcontainer-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.306602 flashcontainer-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.310603 flashcontainer-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.310603 flashcontainer-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39391 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/Concept.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/Developing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-04-10 12:06:48.322603 flashcontainer-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.310603 flashcontainer-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.310603 flashcontainer-0.5.0/examples/arduino/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.306602 flashcontainer-0.5.0/examples/arduino/.pio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.306602 flashcontainer-0.5.0/examples/arduino/.pio/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.310603 flashcontainer-0.5.0/examples/arduino/.pio/build/ATmega328P/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12596 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/.pio/build/ATmega328P/firmware.elf
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/.pio/build/ATmega328P/firmware.hex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.310603 flashcontainer-0.5.0/examples/arduino/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/avr5.xn
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/example.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/gen_param.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)       71 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/gen_param.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.310603 flashcontainer-0.5.0/examples/arduino/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/include/README
+-rw-r--r--   0 runner    (1001) docker     (123)    43240 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/output.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.314603 flashcontainer-0.5.0/examples/arduino/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/param/param.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/param/param.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/param/param.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/param/param.ld
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/param/param.pyhexdump
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/param/param.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/platformio.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/run_simavr.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/run_simavr.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.314603 flashcontainer-0.5.0/examples/arduino/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.314603 flashcontainer-0.5.0/examples/arduino/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/arduino/test/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.314603 flashcontainer-0.5.0/examples/aurix_bmhdr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/aurix_bmhdr/bmhdr.mao
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/aurix_bmhdr/bmhdr.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/aurix_bmhdr/example.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/aurix_bmhdr/run.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/aurix_bmhdr/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.314603 flashcontainer-0.5.0/examples/safety/
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/safety/example.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/safety/run.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/safety/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/examples/safety/safety.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/overview.plantuml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 12:06:48.322603 flashcontainer-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.306602 flashcontainer-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.318603 flashcontainer-0.5.0/src/flashcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/a2lwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/byteconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/cfilewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17191 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/fileargparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/gnuldwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/hexwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/packageinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/pargen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/pargen_1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/pyhexdumpwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/tc3xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/tc3xx_abmhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/tc3xx_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/src/flashcontainer/xmlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.318603 flashcontainer-0.5.0/src/flashcontainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-04-10 12:06:48.000000 flashcontainer-0.5.0/src/flashcontainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-10 12:06:48.000000 flashcontainer-0.5.0/src/flashcontainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:06:48.000000 flashcontainer-0.5.0/src/flashcontainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-10 12:06:48.000000 flashcontainer-0.5.0/src/flashcontainer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 12:06:48.000000 flashcontainer-0.5.0/src/flashcontainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 12:06:48.000000 flashcontainer-0.5.0/src/flashcontainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.318603 flashcontainer-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.318603 flashcontainer-0.5.0/tests/collateral/
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/collateral/abmhd_ref.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/collateral/abmhd_ref.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/collateral/fail_validation.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/collateral/invalid.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:48.318603 flashcontainer-0.5.0/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/example/example.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/example/run.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/example/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/test_byteconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/test_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/test_model_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/test_pargen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/test_tc3xx_abmhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-04-10 12:06:24.000000 flashcontainer-0.5.0/tests/test_xmlparser.py
```

### Comparing `flashcontainer-0.4.0/.github/workflows/push.yaml` & `flashcontainer-0.5.0/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/.github/workflows/python-package.yml` & `flashcontainer-0.5.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/.gitignore` & `flashcontainer-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/.pylintrc` & `flashcontainer-0.5.0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 # R0901)
 ignored-parents=
 
 # Maximum number of arguments for function / method.
 max-args=6
 
 # Maximum number of attributes for a class (see R0902).
-max-attributes=7
+max-attributes=10
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr=5
 
 # Maximum number of branch for function / method body.
 max-branches=12
 
@@ -322,15 +322,15 @@
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
-max-line-length=100
+max-line-length=120
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
```

### Comparing `flashcontainer-0.4.0/.vscode/launch.json` & `flashcontainer-0.5.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/.vscode/settings.json` & `flashcontainer-0.5.0/.vscode/settings.json`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     "python.testing.unittestEnabled": false,
     "python.testing.pytestEnabled": true,
     "python.linting.enabled": true,
     "python.linting.flake8Enabled": false,
     "python.linting.flake8Args": [
             "--max-line-length=120"
     ],
+    "python.linting.pylintArgs": [
+        "--rcfile=${workspaceFolder}/.pylintrc"
+    ],
     "cSpell.words": [
         "flashcontainer"
     ],
     "cSpell.enabled": true,
     "cSpell.enableFiletypes": [
         "markdown"
     ],
```

### Comparing `flashcontainer-0.4.0/Concept.png` & `flashcontainer-0.5.0/Concept.png`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/Developing.md` & `flashcontainer-0.5.0/Developing.md`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/LICENSE` & `flashcontainer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/PKG-INFO` & `flashcontainer-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-Metadata-Version: 2.1
-Name: flashcontainer
-Version: 0.4.0
-Summary: A tooling for flashable parameter data container generation
-Author: Haju Schulz
-Author-email: Haju Schulz <haju.schulz@online.de>
-License: BSD License
-Project-URL: repository, https://github.com/nhjschulz/flashcontainer
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# Pargen - A Tool for Flashable Parameter Container Creation
-
-Pargen is an embedded development tool for generating parameters values that
-can be stored in flash memory and maintained independently from the application.
-It allows to alter/update parameter values without recompilations.
+# Tools for Creating Flashable Parameter Container
 
 ![License](https://img.shields.io/badge/License-BSD%203--Clause-green)
 [![Python package](https://github.com/nhjschulz/flashcontainer/actions/workflows/push.yaml/badge.svg?branch=master)](https://github.com/nhjschulz/flashcontainer/actions/workflows/push.yaml)
 
+## Pargen - Parameter File Generator
+
+The main tool in flashcontainer is called Pargen. Pargen is generating data files
+for parameter values or other data structures that can to be stored in flash memory.
+It allows to change the data without recompilation by reading definitions from an
+XML file.
+
+Flashcontainter also includes tailored front ends for Pargen to simplify special
+use cases. See the [TC3xx tool](#generating-tc3xx-boot-mode-header-structures)
+description chapter for generating Infineon Aurix TC3xx boot mode headers structures.
+
 ## Concept and Features
 
 ![Concept](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/nhjschulz/flashcontainer/master/overview.plantuml)
 
 * Read input from a schema validated XML file
 * Generate C-Source stubs for embedding into the application source amd testing environments
 * Generate Intel Hex files for flashing with a programmer
@@ -69,18 +55,18 @@
       --static, -s          create static comment output without dynamic elements like date and time
       --modify name=value, -m name=value
                             modify parameter value using name=value notation
       --version             show program's version number and exit
     
     Copyright (c) 2022-2023 Haju Schulz <haju.schulz@online.de>. Visit https://github.com/nhjschulz/flashcontainer for full documentation and examples.
 
- The Pargen 
+ The flashcontainer 
 [Developing](https://github.com/nhjschulz/flashcontainer/blob/master/Developing.md/)
 page on Github explains how to use unreleased development builds
-or how to setup a development environment for Pargen.
+or how to setup a development environment.
 
 ## XML Definitions File
 
 The flash container configuration for Pargen is a XML
 definition file with the format explained below.
 
 ### TL;DR
@@ -166,15 +152,15 @@
 |Attribute  |Description              |optional|default|
 |-----------|-------------------------|--------|-------|
 | name      | The block name.         |   No   |       |
 | offset    | Memory start offset inside container. Value may be "." to use the next free offset inside the container.|No||
 | length    | Number of bytes covered by this block|No|
 | align     | block alignment to the next 1,2,4,8 bytes boundary|Yes|1|
 | fill      | byte value used to fill gaps.|Yes| 0x00 |
-| endianness| LE or BE: Little or or big endian byte order |Yes|LE|
+| endianness| LE or BE: Little or big endian byte order |Yes|LE|
 
 #### Block Child Elements
 
 |Element  |Description              | Multiplicity |
 |---------|-------------------------|--------------|
 | comment | Optional comment text for this block| 0..1|
 | header  | Optional header with id, version and length information | 0..1  |
@@ -324,14 +310,59 @@
 #### Crc Element Example
 
     <pd:crc offset="0x008" name="CRCBMHD" type="uint32">
       <pd:memory from="0x0000" to="0x0007" access="32" swap="true"/>
       <pd:config polynomial="0x04C11DB7" init="0xFFFFFFFF" rev_in="true" rev_out="true" final_xor="true" ></pd:config>
     </pd:crc>
 
+
+## Generating TC3xx Boot Mode Header Structures
+
+The tc3xx tool is used to generate Pargen definition XML files for boot mode header
+structures. A Boot mode header structure is a data block in flash memory, which is
+defined by Infineon TC3xx processors. It gets processed by startup software to 
+select which image to boot into.
+
+General usage of the tc3xx command:
+
+    tc3xx  [-h] [--version] {tool name} ...
+
+
+### TC3xx ABMHD - Alternate Boot Mode Header Generator
+
+Tc3xx supports the *abmhd* tool to a generate an alternate boot mode header structure for firmware hex files. 
+The *tc3xx abmhd* tool is controlled by options and produces a Pargen definition file. The definitions file is 
+written to stdout id no output file option is given. This allows to "pipe" the definitions directly into Pargen.
+
+*tc3xx abmhd* usage:
+
+    usage: tc3xx abmhd [-h] [--stad STADABM] [--from CHKSTART] [--to CHKEND] [--abmhdid ABMHDID] [--output filename] ADDRESS HEXFILE    
+
+    Generate TC3XX alternate boot mode header Pargen definition file.   
+
+    Example:
+        tc3xx abmhd --stad 0x80028000 --from 0x8002000 --to 0x8004000  0x80000100 fw.hex | pargen --ihex -f abmhd -   
+
+    positional arguments:
+      ADDRESS               flash address of alternate boot mode header.
+      HEXFILE               name of hexfile with user data content    
+
+    options:
+      -h, --help            show this help message and exit
+      --stad STADABM, -s STADABM
+                            user code start address (default: lowest address in hexfile)
+      --from CHKSTART, -f CHKSTART
+                            begin of range to be checked (default: lowest address in hexfile)
+      --to CHKEND, -t CHKEND
+                            end of range to be checked (default: highest address in hexfile + 1)
+      --abmhdid ABMHDID, -i ABMHDID
+                            alternate Boot Mode Header Identifier value (default=0xFA7CB359)
+      --output filename, -o filename
+                            file name of generated Pargen xml file (default: <stdout>)
+
 ## Issues, Ideas And Bugs
 
 If you have further ideas or you found some bugs, great! Create an
 [issue](https://github.com/nhjschulz/flashcontainer/issues)
 or if you are able and willing to fix it by yourself, clone
 the repository and create a pull request.
```

### Comparing `flashcontainer-0.4.0/README.md` & `flashcontainer-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,44 @@
-# Pargen - A Tool for Flashable Parameter Container Creation
+Metadata-Version: 2.1
+Name: flashcontainer
+Version: 0.5.0
+Summary: A tooling for flashable parameter data container generation
+Author: Haju Schulz
+Author-email: Haju Schulz <haju.schulz@online.de>
+License: BSD License
+Project-URL: repository, https://github.com/nhjschulz/flashcontainer
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
 
-Pargen is an embedded development tool for generating parameters values that
-can be stored in flash memory and maintained independently from the application.
-It allows to alter/update parameter values without recompilations.
+# Tools for Creating Flashable Parameter Container
 
 ![License](https://img.shields.io/badge/License-BSD%203--Clause-green)
 [![Python package](https://github.com/nhjschulz/flashcontainer/actions/workflows/push.yaml/badge.svg?branch=master)](https://github.com/nhjschulz/flashcontainer/actions/workflows/push.yaml)
 
+## Pargen - Parameter File Generator
+
+The main tool in flashcontainer is called Pargen. Pargen is generating data files
+for parameter values or other data structures that can to be stored in flash memory.
+It allows to change the data without recompilation by reading definitions from an
+XML file.
+
+Flashcontainter also includes tailored front ends for Pargen to simplify special
+use cases. See the [TC3xx tool](#generating-tc3xx-boot-mode-header-structures)
+description chapter for generating Infineon Aurix TC3xx boot mode headers structures.
+
 ## Concept and Features
 
 ![Concept](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/nhjschulz/flashcontainer/master/overview.plantuml)
 
 * Read input from a schema validated XML file
 * Generate C-Source stubs for embedding into the application source amd testing environments
 * Generate Intel Hex files for flashing with a programmer
@@ -48,18 +76,18 @@
       --static, -s          create static comment output without dynamic elements like date and time
       --modify name=value, -m name=value
                             modify parameter value using name=value notation
       --version             show program's version number and exit
     
     Copyright (c) 2022-2023 Haju Schulz <haju.schulz@online.de>. Visit https://github.com/nhjschulz/flashcontainer for full documentation and examples.
 
- The Pargen 
+ The flashcontainer 
 [Developing](https://github.com/nhjschulz/flashcontainer/blob/master/Developing.md/)
 page on Github explains how to use unreleased development builds
-or how to setup a development environment for Pargen.
+or how to setup a development environment.
 
 ## XML Definitions File
 
 The flash container configuration for Pargen is a XML
 definition file with the format explained below.
 
 ### TL;DR
@@ -145,15 +173,15 @@
 |Attribute  |Description              |optional|default|
 |-----------|-------------------------|--------|-------|
 | name      | The block name.         |   No   |       |
 | offset    | Memory start offset inside container. Value may be "." to use the next free offset inside the container.|No||
 | length    | Number of bytes covered by this block|No|
 | align     | block alignment to the next 1,2,4,8 bytes boundary|Yes|1|
 | fill      | byte value used to fill gaps.|Yes| 0x00 |
-| endianness| LE or BE: Little or or big endian byte order |Yes|LE|
+| endianness| LE or BE: Little or big endian byte order |Yes|LE|
 
 #### Block Child Elements
 
 |Element  |Description              | Multiplicity |
 |---------|-------------------------|--------------|
 | comment | Optional comment text for this block| 0..1|
 | header  | Optional header with id, version and length information | 0..1  |
@@ -303,14 +331,59 @@
 #### Crc Element Example
 
     <pd:crc offset="0x008" name="CRCBMHD" type="uint32">
       <pd:memory from="0x0000" to="0x0007" access="32" swap="true"/>
       <pd:config polynomial="0x04C11DB7" init="0xFFFFFFFF" rev_in="true" rev_out="true" final_xor="true" ></pd:config>
     </pd:crc>
 
+
+## Generating TC3xx Boot Mode Header Structures
+
+The tc3xx tool is used to generate Pargen definition XML files for boot mode header
+structures. A Boot mode header structure is a data block in flash memory, which is
+defined by Infineon TC3xx processors. It gets processed by startup software to 
+select which image to boot into.
+
+General usage of the tc3xx command:
+
+    tc3xx  [-h] [--version] {tool name} ...
+
+
+### TC3xx ABMHD - Alternate Boot Mode Header Generator
+
+Tc3xx supports the *abmhd* tool to a generate an alternate boot mode header structure for firmware hex files. 
+The *tc3xx abmhd* tool is controlled by options and produces a Pargen definition file. The definitions file is 
+written to stdout id no output file option is given. This allows to "pipe" the definitions directly into Pargen.
+
+*tc3xx abmhd* usage:
+
+    usage: tc3xx abmhd [-h] [--stad STADABM] [--from CHKSTART] [--to CHKEND] [--abmhdid ABMHDID] [--output filename] ADDRESS HEXFILE    
+
+    Generate TC3XX alternate boot mode header Pargen definition file.   
+
+    Example:
+        tc3xx abmhd --stad 0x80028000 --from 0x8002000 --to 0x8004000  0x80000100 fw.hex | pargen --ihex -f abmhd -   
+
+    positional arguments:
+      ADDRESS               flash address of alternate boot mode header.
+      HEXFILE               name of hexfile with user data content    
+
+    options:
+      -h, --help            show this help message and exit
+      --stad STADABM, -s STADABM
+                            user code start address (default: lowest address in hexfile)
+      --from CHKSTART, -f CHKSTART
+                            begin of range to be checked (default: lowest address in hexfile)
+      --to CHKEND, -t CHKEND
+                            end of range to be checked (default: highest address in hexfile + 1)
+      --abmhdid ABMHDID, -i ABMHDID
+                            alternate Boot Mode Header Identifier value (default=0xFA7CB359)
+      --output filename, -o filename
+                            file name of generated Pargen xml file (default: <stdout>)
+
 ## Issues, Ideas And Bugs
 
 If you have further ideas or you found some bugs, great! Create an
 [issue](https://github.com/nhjschulz/flashcontainer/issues)
 or if you are able and willing to fix it by yourself, clone
 the repository and create a pull request.
```

### Comparing `flashcontainer-0.4.0/examples/README.md` & `flashcontainer-0.5.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/.pio/build/ATmega328P/firmware.elf` & `flashcontainer-0.5.0/examples/arduino/.pio/build/ATmega328P/firmware.elf`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/.pio/build/ATmega328P/firmware.hex` & `flashcontainer-0.5.0/examples/arduino/.pio/build/ATmega328P/firmware.hex`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/avr5.xn` & `flashcontainer-0.5.0/examples/arduino/avr5.xn`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/example.md` & `flashcontainer-0.5.0/examples/arduino/example.md`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/include/README` & `flashcontainer-0.5.0/examples/arduino/include/README`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/output.map` & `flashcontainer-0.5.0/examples/arduino/output.map`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/param/param.c` & `flashcontainer-0.5.0/examples/arduino/param/param.c`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/param/param.h` & `flashcontainer-0.5.0/examples/arduino/param/param.h`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/param/param.hex` & `flashcontainer-0.5.0/examples/arduino/param/param.hex`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/param/param.ld` & `flashcontainer-0.5.0/examples/arduino/param/param.ld`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/param/param.pyhexdump` & `flashcontainer-0.5.0/examples/arduino/param/param.pyhexdump`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/param/param.xml` & `flashcontainer-0.5.0/examples/arduino/param/param.xml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/platformio.ini` & `flashcontainer-0.5.0/examples/arduino/platformio.ini`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/src/main.cpp` & `flashcontainer-0.5.0/examples/arduino/src/main.cpp`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/arduino/test/README` & `flashcontainer-0.5.0/examples/arduino/test/README`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/aurix_bmhdr/bmhdr.mao` & `flashcontainer-0.5.0/examples/aurix_bmhdr/bmhdr.mao`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/aurix_bmhdr/bmhdr.xml` & `flashcontainer-0.5.0/examples/aurix_bmhdr/bmhdr.xml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/aurix_bmhdr/example.md` & `flashcontainer-0.5.0/examples/aurix_bmhdr/example.md`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/safety/example.md` & `flashcontainer-0.5.0/examples/safety/example.md`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/examples/safety/safety.xml` & `flashcontainer-0.5.0/examples/safety/safety.xml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/overview.plantuml` & `flashcontainer-0.5.0/overview.plantuml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/pyproject.toml` & `flashcontainer-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel", "toml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flashcontainer"
-version = "0.4.0"
+version = "0.5.0"
 requires-python = ">=3.8"
 description = "A tooling for flashable parameter data container generation"
 readme = "README.md"
 license = {text = "BSD License"}
 authors = [
   {name = "Haju Schulz", email = "haju.schulz@online.de"}
 ]
@@ -38,12 +38,14 @@
 ]
 
 [project.urls]
 repository = "https://github.com/nhjschulz/flashcontainer"
 
 [project.scripts]
 pargen = "flashcontainer.pargen:pargen_cli"
+tc3xx = "flashcontainer.tc3xx:tc3xx_cli"
+
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
```

### Comparing `flashcontainer-0.4.0/setup.cfg` & `flashcontainer-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/__init__.py` & `flashcontainer-0.5.0/src/flashcontainer/__init__.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/__main__.py` & `flashcontainer-0.5.0/src/flashcontainer/__main__.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/a2lwriter.py` & `flashcontainer-0.5.0/src/flashcontainer/a2lwriter.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/byteconv.py` & `flashcontainer-0.5.0/src/flashcontainer/byteconv.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 
 import struct
 import json5
 
 import flashcontainer.datamodel as DM
 
 class ByteConvert:
-    """Byte to Text convertiona
+    """Byte to Text conversions
     """
 
     @staticmethod
     def get_type_size(ptype: DM.ParamType) -> int:
-        """Get bytesize of type"""
+        """Get byte size of type"""
 
         return DM.TYPE_DATA[ptype].size
 
     @staticmethod
     def json_to_bytes(ptype: DM.ParamType,  endianess: DM.Endianness, value_str: str) -> bytearray:
         """Convert from json string into raw bytes """
```

### Comparing `flashcontainer-0.4.0/src/flashcontainer/cfilewriter.py` & `flashcontainer-0.5.0/src/flashcontainer/cfilewriter.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/checksum.py` & `flashcontainer-0.5.0/src/flashcontainer/checksum.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/datamodel.py` & `flashcontainer-0.5.0/src/flashcontainer/datamodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,19 +512,19 @@
                 pfx += f"{self.ctx_block.name}:"
 
         logging.error(pfx + msg)
 
         self.result = False
 
 
-# A tuple holding additional information for datamodel types
+# A tuple holding additional information for data model types
 #
 # fmt: format character used in struct.pack/unpack
-# size: # if bytes used by one elemnent of this type
-# witdh: preferned print width
+# size: # if bytes used by one element of this type
+# width: preferred print width
 # ctype: C-Language type
 TypeData = namedtuple('TypeData', ['fmt', 'size', 'width', 'signed', 'ctype'])
 
 TYPE_DATA = {
     ParamType.UINT32:  TypeData("L", 4, 10, False, "uint32_t"),
     ParamType.UINT8:   TypeData("B", 1, 4, False, "uint8_t"),
     ParamType.UINT16:  TypeData("H", 2, 6, False, "uint16_t"),
```

### Comparing `flashcontainer-0.4.0/src/flashcontainer/gnuldwriter.py` & `flashcontainer-0.5.0/src/flashcontainer/gnuldwriter.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/hexwriter.py` & `flashcontainer-0.5.0/src/flashcontainer/hexwriter.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/packageinfo.py` & `flashcontainer-0.5.0/src/flashcontainer/packageinfo.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/pargen.py` & `flashcontainer-0.5.0/src/flashcontainer/pargen.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 import datetime
-import argparse
 import logging
 import uuid
 import sys
 import os
 from enum import Enum
 from pathlib import Path
 from typing import List, Dict
@@ -44,14 +43,15 @@
 from flashcontainer.hexwriter import HexWriter
 from flashcontainer.xmlparser import XmlParser
 from flashcontainer.cfilewriter import CFileWriter
 from flashcontainer.gnuldwriter import GnuLdWriter
 from flashcontainer.pyhexdumpwriter import PyHexDumpWriter
 from flashcontainer.a2lwriter import A2lWriter
 from flashcontainer.packageinfo import __version__, __email__, __repository__
+from flashcontainer.fileargparse import FileArgumentParser
 import flashcontainer.datamodel as DM
 
 # List of output writers
 _WRITER = [
     {
         "key": "ihex",
         "class": HexWriter,
@@ -75,35 +75,25 @@
     {
         "key": "pyhexdump",
         "class": PyHexDumpWriter,
         "help": "generate pyHexDump print configuration file"
     }
 ]
 
-class FileArgumentParser(argparse.ArgumentParser):
-    """Argument parser with support for argument files."""
-
-    def convert_arg_line_to_args(self, arg_line):
-        return arg_line.split()
-
 def pargen_cli() -> int:
     """ cmd line interface for pagen"""
 
     logging.basicConfig(encoding='utf-8', level=logging.WARN)
 
     name = "pargen"
     about = f"{name} {__version__}: A tool for generating flashable parameter container."
 
     parser = FileArgumentParser(
         prog=name,
-        description=about,
-        fromfile_prefix_chars='@',
-        epilog=
-            f"Copyright (c) 2022-2023 {__email__}. "
-            f" Visit {__repository__} for full documentation and examples."
+        description=about
     )
 
     for writer in _WRITER:
         parser.add_argument("--" + writer["key"], action='store_true', help=writer["help"])
 
     parser.add_argument(
         '--destdir', '-o', nargs=1, metavar="directory",
@@ -120,72 +110,78 @@
     parser.add_argument(
         "--modify", "-m", nargs=1,  action='append', metavar="name=value",
         help='modify parameter value using name=value notation'
     )
 
     parser.add_argument('--version', action='version', version=f'%(prog)s {__version__}')
 
-    parser.add_argument('file', nargs=1, help='name of the XML parameter definition file')
+    parser.add_argument(
+       'file',
+        nargs=1, help='name of the XML parameter definition file (or - for stdin)')
 
     args = parser.parse_args()
 
-    # parse modifiy option values into string tuple list of (name, value) pairs.
+    # parse modify option values into string tuple list of (name, value) pairs.
     modify_values = {}
     for modval_str in (args.modify or []):
         seperator = modval_str[0].find('=')
         if -1 == seperator:
             logging.error("invalid modify option  %s. Expect <name>=<val>.", modval_str[0])
             return Error.ERROR_INVALID_OPTION
 
         modify_values[modval_str[0][:seperator]] = modval_str[0][seperator+1:]
 
-    print(modify_values)
     writers = []
 
     for writer in _WRITER:
         if getattr(args, writer["key"]):
             writers.append(writer["class"])
 
+    base_name = None
+    if args.filename is not None:
+        base_name = args.filename[0]
+
     return pargen(
         cfgfile=args.file[0],
-        filename=args.filename,
+        filename=base_name,
         outdir=Path(args.destdir[0]),
         static=args.static,
         writers=writers,
         modifier=modify_values)
 
 class Error(Enum):
     """Pargen error codes """
 
     ERROR_OK = 0
     ERROR_FILE_NOT_FOUND = 1
     ERROR_INVALID_FORMAT = 2
     ERROR_VALIDATION_FAIL = 3
     ERROR_EXCEPTION = 4
-    ERROR_INVALID_OPTION =5
+    ERROR_INVALID_OPTION = 5
 
 def pargen(
         cfgfile: str,
         filename: str,
         outdir: Path,
         static: bool,
         writers: List[DM.Walker],
         modifier: Dict[str, str] = None) -> int:
     """ Parameter generator tool entry point"""
 
     # Create output directory (if necessary)
     destdir = Path.resolve(outdir)
     destdir.mkdir(parents=True, exist_ok=True)
 
-    outfilename = filename
-    if outfilename is None:
-        outfilename = os.path.basename(cfgfile)
-    outfilename = Path(outfilename).stem
-
-    if Path(cfgfile).is_file():
+    base_name = Path(os.path.basename(cfgfile)).stem
+    if filename is not None:
+        base_name = Path(filename).stem
+    if "-" == cfgfile:
+        print("Processing definitions from <stdin>\n")
+        model = XmlParser.from_file(sys.stdin, modifier)
+    elif Path(cfgfile).is_file():
         print(f"Processing definitions from {cfgfile}\n")
         model = XmlParser.from_file(cfgfile, modifier)
     else:
         logging.error("file not found: %s", cfgfile)
         return Error.ERROR_FILE_NOT_FOUND.value
 
     if model is None:
@@ -197,15 +193,15 @@
         "VERSION": __version__,
         "INPUT": cfgfile,
         "GUID": uuid.uuid4(),
         "CMDLINE": ' '.join(sys.argv[0:]),
         "DATETIME": datetime.datetime.now(),
         "MODEL": model,
         "DESTDIR": destdir,
-        "BASENAME": outfilename,
+        "BASENAME": base_name,
         "STATICOUTPUT": static
         }
 
     if model.validate(param) is False:
         return Error.ERROR_VALIDATION_FAIL.value
 
     if 0 == len(writers):
```

### Comparing `flashcontainer-0.4.0/src/flashcontainer/pargen_1.0.xsd` & `flashcontainer-0.5.0/src/flashcontainer/pargen_1.0.xsd`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/pyhexdumpwriter.py` & `flashcontainer-0.5.0/src/flashcontainer/pyhexdumpwriter.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/src/flashcontainer/xmlparser.py` & `flashcontainer-0.5.0/src/flashcontainer/xmlparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     @classmethod
     def from_file(cls, file: str, values: Dict[str, str] = None) -> DM.Model:
         """Parser entry point returning model instance"""
         return cls.parse(file, values)
 
     @staticmethod
     def parse(file: str, values: Dict[str, str]) -> DM.Model:
-        """ Parse given XML file into datamodel. """
+        """ Parse given XML file into data model. """
         model = None
         try:
-            logging.info("Loading parameter definitons from %s.", file)
+            logging.info("Loading parameter definitions from %s.", file)
             schema = ET.XMLSchema(ET.parse(schema_file))
             xml_doc = ET.parse(file, ET.XMLParser(remove_comments=True))
             schema.assertValid(xml_doc)
             XmlParser._update_values(xml_doc.getroot(), values)
             model = XmlParser._build_model(xml_doc.getroot(), file)
 
         except ET.DocumentInvalid as err:
@@ -263,17 +263,17 @@
 
     @staticmethod
     def calc_addr(base_addr: int, running_addr: int, offset_str: str, alignment: int) -> int:
         """Calculate address from address input or '.'
 
         Args:
             base_addr(int): Start address of parent element
-            running_addr(int): Next unused adderss in parent element
+            running_addr(int): Next unused address in parent element
             offset_str(str): address information from XML
-            alignment(int): optional address alignement to 1,2,4,8... boundary
+            alignment(int): optional address alignment to 1,2,4,8... boundary
 
         Returns:
             Aligned address if integer is passed or aligned next free address for '.'
         """
 
         if "." == offset_str:
             result_addr = running_addr
```

### Comparing `flashcontainer-0.4.0/src/flashcontainer.egg-info/PKG-INFO` & `flashcontainer-0.5.0/src/flashcontainer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcontainer
-Version: 0.4.0
+Version: 0.5.0
 Summary: A tooling for flashable parameter data container generation
 Author: Haju Schulz
 Author-email: Haju Schulz <haju.schulz@online.de>
 License: BSD License
 Project-URL: repository, https://github.com/nhjschulz/flashcontainer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,23 +15,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# Pargen - A Tool for Flashable Parameter Container Creation
-
-Pargen is an embedded development tool for generating parameters values that
-can be stored in flash memory and maintained independently from the application.
-It allows to alter/update parameter values without recompilations.
+# Tools for Creating Flashable Parameter Container
 
 ![License](https://img.shields.io/badge/License-BSD%203--Clause-green)
 [![Python package](https://github.com/nhjschulz/flashcontainer/actions/workflows/push.yaml/badge.svg?branch=master)](https://github.com/nhjschulz/flashcontainer/actions/workflows/push.yaml)
 
+## Pargen - Parameter File Generator
+
+The main tool in flashcontainer is called Pargen. Pargen is generating data files
+for parameter values or other data structures that can to be stored in flash memory.
+It allows to change the data without recompilation by reading definitions from an
+XML file.
+
+Flashcontainter also includes tailored front ends for Pargen to simplify special
+use cases. See the [TC3xx tool](#generating-tc3xx-boot-mode-header-structures)
+description chapter for generating Infineon Aurix TC3xx boot mode headers structures.
+
 ## Concept and Features
 
 ![Concept](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/nhjschulz/flashcontainer/master/overview.plantuml)
 
 * Read input from a schema validated XML file
 * Generate C-Source stubs for embedding into the application source amd testing environments
 * Generate Intel Hex files for flashing with a programmer
@@ -69,18 +76,18 @@
       --static, -s          create static comment output without dynamic elements like date and time
       --modify name=value, -m name=value
                             modify parameter value using name=value notation
       --version             show program's version number and exit
     
     Copyright (c) 2022-2023 Haju Schulz <haju.schulz@online.de>. Visit https://github.com/nhjschulz/flashcontainer for full documentation and examples.
 
- The Pargen 
+ The flashcontainer 
 [Developing](https://github.com/nhjschulz/flashcontainer/blob/master/Developing.md/)
 page on Github explains how to use unreleased development builds
-or how to setup a development environment for Pargen.
+or how to setup a development environment.
 
 ## XML Definitions File
 
 The flash container configuration for Pargen is a XML
 definition file with the format explained below.
 
 ### TL;DR
@@ -166,15 +173,15 @@
 |Attribute  |Description              |optional|default|
 |-----------|-------------------------|--------|-------|
 | name      | The block name.         |   No   |       |
 | offset    | Memory start offset inside container. Value may be "." to use the next free offset inside the container.|No||
 | length    | Number of bytes covered by this block|No|
 | align     | block alignment to the next 1,2,4,8 bytes boundary|Yes|1|
 | fill      | byte value used to fill gaps.|Yes| 0x00 |
-| endianness| LE or BE: Little or or big endian byte order |Yes|LE|
+| endianness| LE or BE: Little or big endian byte order |Yes|LE|
 
 #### Block Child Elements
 
 |Element  |Description              | Multiplicity |
 |---------|-------------------------|--------------|
 | comment | Optional comment text for this block| 0..1|
 | header  | Optional header with id, version and length information | 0..1  |
@@ -324,14 +331,59 @@
 #### Crc Element Example
 
     <pd:crc offset="0x008" name="CRCBMHD" type="uint32">
       <pd:memory from="0x0000" to="0x0007" access="32" swap="true"/>
       <pd:config polynomial="0x04C11DB7" init="0xFFFFFFFF" rev_in="true" rev_out="true" final_xor="true" ></pd:config>
     </pd:crc>
 
+
+## Generating TC3xx Boot Mode Header Structures
+
+The tc3xx tool is used to generate Pargen definition XML files for boot mode header
+structures. A Boot mode header structure is a data block in flash memory, which is
+defined by Infineon TC3xx processors. It gets processed by startup software to 
+select which image to boot into.
+
+General usage of the tc3xx command:
+
+    tc3xx  [-h] [--version] {tool name} ...
+
+
+### TC3xx ABMHD - Alternate Boot Mode Header Generator
+
+Tc3xx supports the *abmhd* tool to a generate an alternate boot mode header structure for firmware hex files. 
+The *tc3xx abmhd* tool is controlled by options and produces a Pargen definition file. The definitions file is 
+written to stdout id no output file option is given. This allows to "pipe" the definitions directly into Pargen.
+
+*tc3xx abmhd* usage:
+
+    usage: tc3xx abmhd [-h] [--stad STADABM] [--from CHKSTART] [--to CHKEND] [--abmhdid ABMHDID] [--output filename] ADDRESS HEXFILE    
+
+    Generate TC3XX alternate boot mode header Pargen definition file.   
+
+    Example:
+        tc3xx abmhd --stad 0x80028000 --from 0x8002000 --to 0x8004000  0x80000100 fw.hex | pargen --ihex -f abmhd -   
+
+    positional arguments:
+      ADDRESS               flash address of alternate boot mode header.
+      HEXFILE               name of hexfile with user data content    
+
+    options:
+      -h, --help            show this help message and exit
+      --stad STADABM, -s STADABM
+                            user code start address (default: lowest address in hexfile)
+      --from CHKSTART, -f CHKSTART
+                            begin of range to be checked (default: lowest address in hexfile)
+      --to CHKEND, -t CHKEND
+                            end of range to be checked (default: highest address in hexfile + 1)
+      --abmhdid ABMHDID, -i ABMHDID
+                            alternate Boot Mode Header Identifier value (default=0xFA7CB359)
+      --output filename, -o filename
+                            file name of generated Pargen xml file (default: <stdout>)
+
 ## Issues, Ideas And Bugs
 
 If you have further ideas or you found some bugs, great! Create an
 [issue](https://github.com/nhjschulz/flashcontainer/issues)
 or if you are able and willing to fix it by yourself, clone
 the repository and create a pull request.
```

### Comparing `flashcontainer-0.4.0/src/flashcontainer.egg-info/SOURCES.txt` & `flashcontainer-0.5.0/src/flashcontainer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -47,32 +47,39 @@
 src/flashcontainer/__init__.py
 src/flashcontainer/__main__.py
 src/flashcontainer/a2lwriter.py
 src/flashcontainer/byteconv.py
 src/flashcontainer/cfilewriter.py
 src/flashcontainer/checksum.py
 src/flashcontainer/datamodel.py
+src/flashcontainer/fileargparse.py
 src/flashcontainer/gnuldwriter.py
 src/flashcontainer/hexwriter.py
 src/flashcontainer/packageinfo.py
 src/flashcontainer/pargen.py
 src/flashcontainer/pargen_1.0.xsd
 src/flashcontainer/pyhexdumpwriter.py
+src/flashcontainer/tc3xx.py
+src/flashcontainer/tc3xx_abmhd.py
+src/flashcontainer/tc3xx_cmd.py
 src/flashcontainer/xmlparser.py
 src/flashcontainer.egg-info/PKG-INFO
 src/flashcontainer.egg-info/SOURCES.txt
 src/flashcontainer.egg-info/dependency_links.txt
 src/flashcontainer.egg-info/entry_points.txt
 src/flashcontainer.egg-info/requires.txt
 src/flashcontainer.egg-info/top_level.txt
 tests/__init__.py
 tests/test_byteconv.py
 tests/test_checksum.py
 tests/test_datamodel.py
 tests/test_model_validate.py
 tests/test_pargen.py
+tests/test_tc3xx_abmhd.py
 tests/test_xmlparser.py
+tests/collateral/abmhd_ref.hex
+tests/collateral/abmhd_ref.xml
 tests/collateral/fail_validation.xml
 tests/collateral/invalid.xml
 tests/example/example.xml
 tests/example/run.bat
 tests/example/run.sh
```

### Comparing `flashcontainer-0.4.0/tests/collateral/fail_validation.xml` & `flashcontainer-0.5.0/tests/collateral/fail_validation.xml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/collateral/invalid.xml` & `flashcontainer-0.5.0/tests/collateral/invalid.xml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/example/example.xml` & `flashcontainer-0.5.0/tests/example/example.xml`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/test_byteconv.py` & `flashcontainer-0.5.0/tests/test_byteconv.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/test_checksum.py` & `flashcontainer-0.5.0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/test_datamodel.py` & `flashcontainer-0.5.0/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/test_model_validate.py` & `flashcontainer-0.5.0/tests/test_model_validate.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/test_pargen.py` & `flashcontainer-0.5.0/tests/test_pargen.py`

 * *Files identical despite different names*

### Comparing `flashcontainer-0.4.0/tests/test_xmlparser.py` & `flashcontainer-0.5.0/tests/test_xmlparser.py`

 * *Files identical despite different names*

