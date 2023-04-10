# Comparing `tmp/flixy2app-0.1.tar.gz` & `tmp/flixy2app-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixy2app-0.1.tar", last modified: Mon Apr 10 12:29:25 2023, max compression
+gzip compressed data, was "flixy2app-0.2.tar", last modified: Mon Apr 10 12:47:04 2023, max compression
```

## Comparing `flixy2app-0.1.tar` & `flixy2app-0.2.tar`

### file list

```diff
@@ -1,65 +1,80 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.198179 flixy2app-0.1/
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 flixy2app-0.1/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       36 2023-04-10 11:52:11.000000 flixy2app-0.1/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      770 2023-04-10 12:29:25.197912 flixy2app-0.1/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      398 2023-04-10 12:09:24.000000 flixy2app-0.1/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.190993 flixy2app-0.1/flixy/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.191282 flixy2app-0.1/flixy/Demo/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       29 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/Demo/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      909 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/Demo/demo.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       57 2023-04-10 05:31:19.000000 flixy2app-0.1/flixy/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.191927 flixy2app-0.1/flixy/flixy/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      161 2023-04-09 19:45:54.000000 flixy2app-0.1/flixy/flixy/APP.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2963 2023-04-09 23:08:38.000000 flixy2app-0.1/flixy/flixy/PAGE.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.193212 flixy2app-0.1/flixy/flixy/Tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1944 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/Haptics.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      149 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/action.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      753 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/convert_rgb_to_hex.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       98 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/error_handle.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      242 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/get_parent.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1340 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/sounds.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.193622 flixy2app-0.1/flixy/flixy/Tools/subscribers/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:40.000000 flixy2app-0.1/flixy/flixy/Tools/subscribers/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      355 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/subscribers/call_on_change.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1534 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/Tools/subscribers/text_subscribe.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      709 2023-04-09 23:21:29.000000 flixy2app-0.1/flixy/flixy/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.195263 flixy2app-0.1/flixy/flixy/controls/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1470 2023-04-09 22:12:43.000000 flixy2app-0.1/flixy/flixy/controls/APPBAR.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1942 2023-04-09 21:43:35.000000 flixy2app-0.1/flixy/flixy/controls/BUTTON.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2879 2023-04-09 23:13:59.000000 flixy2app-0.1/flixy/flixy/controls/COLUMN.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       91 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/controls/CONTAINER.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2221 2023-04-09 23:28:15.000000 flixy2app-0.1/flixy/flixy/controls/NAVIGATOR.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2912 2023-04-09 23:11:48.000000 flixy2app-0.1/flixy/flixy/controls/ROW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1957 2023-04-09 23:11:34.000000 flixy2app-0.1/flixy/flixy/controls/SHEET.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1740 2023-04-09 22:06:30.000000 flixy2app-0.1/flixy/flixy/controls/TEXT.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3240 2023-04-09 22:54:23.000000 flixy2app-0.1/flixy/flixy/controls/TEXTFIELD.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1835 2023-04-09 22:54:56.000000 flixy2app-0.1/flixy/flixy/controls/TEXTVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3613 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/controls/WEBVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/controls/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8385 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/installer.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.195879 flixy2app-0.1/flixy/flixy/pythonista_ui/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1509 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/pythonista_ui/VIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    26900 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/pythonista_ui/WKWEBVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/pythonista_ui/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.196151 flixy2app-0.1/flixy/flixy/pythonista_ui/tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:50.000000 flixy2app-0.1/flixy/flixy/pythonista_ui/tools/__init__.py
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)    39335 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/pythonista_ui/tools/gestures.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5593 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/update.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.196425 flixy2app-0.1/flixy/flixy/widgets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/widgets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      196 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/flixy/widgets/on_top.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      131 2023-04-09 19:33:37.000000 flixy2app-0.1/flixy/info.txt
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.196916 flixy2app-0.1/flixy2app/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:59:37.000000 flixy2app-0.1/flixy2app/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-10 12:21:28.000000 flixy2app-0.1/flixy2app/converter.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      651 2023-04-10 12:23:39.000000 flixy2app-0.1/flixy2app/generate.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:29:25.197687 flixy2app-0.1/flixy2app.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      770 2023-04-10 12:29:25.000000 flixy2app-0.1/flixy2app.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1469 2023-04-10 12:29:25.000000 flixy2app-0.1/flixy2app.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-10 12:29:25.000000 flixy2app-0.1/flixy2app.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       26 2023-04-10 12:29:25.000000 flixy2app-0.1/flixy2app.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-10 12:29:25.000000 flixy2app-0.1/flixy2app.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 flixy2app-0.1/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-10 12:29:25.198280 flixy2app-0.1/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      624 2023-04-10 12:29:10.000000 flixy2app-0.1/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.079813 flixy2app-0.2/
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 flixy2app-0.2/LICENSE
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)       36 2023-04-10 11:52:11.000000 flixy2app-0.2/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      770 2023-04-10 12:47:04.079662 flixy2app-0.2/PKG-INFO
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      398 2023-04-10 12:09:24.000000 flixy2app-0.2/README.md
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.070755 flixy2app-0.2/flixy/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.071265 flixy2app-0.2/flixy/Demo/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       29 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Demo/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      909 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Demo/demo.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.071542 flixy2app-0.2/flixy/Learn/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:44:57.000000 flixy2app-0.2/flixy/Learn/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2859 2023-04-10 05:36:37.000000 flixy2app-0.2/flixy/Learn/learn.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.073202 flixy2app-0.2/flixy/Learn/lessons/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1381 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/Text.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:32:01.000000 flixy2app-0.2/flixy/Learn/lessons/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1187 2023-04-10 05:37:44.000000 flixy2app-0.2/flixy/Learn/lessons/app.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2235 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1908 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/column.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1755 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/navigate.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3088 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/page.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1843 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/row.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1598 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/sheet.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2872 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/textfield.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2079 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/Learn/lessons/webview.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       57 2023-04-10 05:31:19.000000 flixy2app-0.2/flixy/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.073952 flixy2app-0.2/flixy/flixy/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      161 2023-04-09 19:45:54.000000 flixy2app-0.2/flixy/flixy/APP.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2963 2023-04-09 23:08:38.000000 flixy2app-0.2/flixy/flixy/PAGE.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.074826 flixy2app-0.2/flixy/flixy/Tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1944 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/Haptics.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      149 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/action.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      753 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/convert_rgb_to_hex.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       98 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/error_handle.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      242 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/get_parent.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1340 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/sounds.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.075187 flixy2app-0.2/flixy/flixy/Tools/subscribers/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:40.000000 flixy2app-0.2/flixy/flixy/Tools/subscribers/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      355 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/subscribers/call_on_change.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1534 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/Tools/subscribers/text_subscribe.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      709 2023-04-09 23:21:29.000000 flixy2app-0.2/flixy/flixy/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.076779 flixy2app-0.2/flixy/flixy/controls/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1470 2023-04-09 22:12:43.000000 flixy2app-0.2/flixy/flixy/controls/APPBAR.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1942 2023-04-09 21:43:35.000000 flixy2app-0.2/flixy/flixy/controls/BUTTON.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2879 2023-04-09 23:13:59.000000 flixy2app-0.2/flixy/flixy/controls/COLUMN.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       91 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/controls/CONTAINER.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2221 2023-04-09 23:28:15.000000 flixy2app-0.2/flixy/flixy/controls/NAVIGATOR.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2912 2023-04-09 23:11:48.000000 flixy2app-0.2/flixy/flixy/controls/ROW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1957 2023-04-09 23:11:34.000000 flixy2app-0.2/flixy/flixy/controls/SHEET.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1740 2023-04-09 22:06:30.000000 flixy2app-0.2/flixy/flixy/controls/TEXT.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3240 2023-04-09 22:54:23.000000 flixy2app-0.2/flixy/flixy/controls/TEXTFIELD.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1835 2023-04-09 22:54:56.000000 flixy2app-0.2/flixy/flixy/controls/TEXTVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3613 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/controls/WEBVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/controls/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8385 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/installer.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.077183 flixy2app-0.2/flixy/flixy/pythonista_ui/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1509 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/pythonista_ui/VIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    26900 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/pythonista_ui/WKWEBVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/pythonista_ui/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.077423 flixy2app-0.2/flixy/flixy/pythonista_ui/tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:50.000000 flixy2app-0.2/flixy/flixy/pythonista_ui/tools/__init__.py
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)    39335 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/pythonista_ui/tools/gestures.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5593 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/update.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.077698 flixy2app-0.2/flixy/flixy/widgets/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/widgets/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      196 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/flixy/widgets/on_top.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      131 2023-04-09 19:33:37.000000 flixy2app-0.2/flixy/info.txt
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.078532 flixy2app-0.2/flixy2app/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:59:37.000000 flixy2app-0.2/flixy2app/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-10 12:21:28.000000 flixy2app-0.2/flixy2app/converter.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      651 2023-04-10 12:23:39.000000 flixy2app-0.2/flixy2app/generate.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:47:04.079413 flixy2app-0.2/flixy2app.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      770 2023-04-10 12:47:04.000000 flixy2app-0.2/flixy2app.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1841 2023-04-10 12:47:04.000000 flixy2app-0.2/flixy2app.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-10 12:47:04.000000 flixy2app-0.2/flixy2app.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       26 2023-04-10 12:47:04.000000 flixy2app-0.2/flixy2app.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-10 12:47:04.000000 flixy2app-0.2/flixy2app.egg-info/top_level.txt
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 flixy2app-0.2/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-10 12:47:04.079859 flixy2app-0.2/setup.cfg
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      624 2023-04-10 12:46:45.000000 flixy2app-0.2/setup.py
```

### Comparing `flixy2app-0.1/LICENSE` & `flixy2app-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/PKG-INFO` & `flixy2app-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flixy2app
-Version: 0.1
+Version: 0.2
 Summary: A UI-Builder that helps programmers build the front-end without codding it.
 Home-page: https://github.com/SKbarbon/flixy
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flixy2app-0.1/flixy/Demo/demo.py` & `flixy2app-0.2/flixy/Demo/demo.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/PAGE.py` & `flixy2app-0.2/flixy/flixy/PAGE.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/Tools/Haptics.py` & `flixy2app-0.2/flixy/flixy/Tools/Haptics.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/Tools/convert_rgb_to_hex.py` & `flixy2app-0.2/flixy/flixy/Tools/convert_rgb_to_hex.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/Tools/sounds.py` & `flixy2app-0.2/flixy/flixy/Tools/sounds.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/Tools/subscribers/text_subscribe.py` & `flixy2app-0.2/flixy/flixy/Tools/subscribers/text_subscribe.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/__init__.py` & `flixy2app-0.2/flixy/flixy/__init__.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/APPBAR.py` & `flixy2app-0.2/flixy/flixy/controls/APPBAR.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/BUTTON.py` & `flixy2app-0.2/flixy/flixy/controls/BUTTON.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/COLUMN.py` & `flixy2app-0.2/flixy/flixy/controls/COLUMN.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/NAVIGATOR.py` & `flixy2app-0.2/flixy/flixy/controls/NAVIGATOR.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/ROW.py` & `flixy2app-0.2/flixy/flixy/controls/ROW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/SHEET.py` & `flixy2app-0.2/flixy/flixy/controls/SHEET.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/TEXT.py` & `flixy2app-0.2/flixy/flixy/controls/TEXT.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/TEXTFIELD.py` & `flixy2app-0.2/flixy/flixy/controls/TEXTFIELD.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/TEXTVIEW.py` & `flixy2app-0.2/flixy/flixy/controls/TEXTVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/controls/WEBVIEW.py` & `flixy2app-0.2/flixy/flixy/controls/WEBVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/installer.py` & `flixy2app-0.2/flixy/flixy/installer.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/pythonista_ui/VIEW.py` & `flixy2app-0.2/flixy/flixy/pythonista_ui/VIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/pythonista_ui/WKWEBVIEW.py` & `flixy2app-0.2/flixy/flixy/pythonista_ui/WKWEBVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/pythonista_ui/tools/gestures.py` & `flixy2app-0.2/flixy/flixy/pythonista_ui/tools/gestures.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy/flixy/update.py` & `flixy2app-0.2/flixy/flixy/update.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy2app/converter.py` & `flixy2app-0.2/flixy2app/converter.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy2app/generate.py` & `flixy2app-0.2/flixy2app/generate.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.1/flixy2app.egg-info/PKG-INFO` & `flixy2app-0.2/flixy2app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flixy2app
-Version: 0.1
+Version: 0.2
 Summary: A UI-Builder that helps programmers build the front-end without codding it.
 Home-page: https://github.com/SKbarbon/flixy
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flixy2app-0.1/flixy2app.egg-info/SOURCES.txt` & `flixy2app-0.2/flixy2app.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 README.md
 pyproject.toml
 setup.py
 flixy/__init__.py
 flixy/info.txt
 flixy/Demo/__init__.py
 flixy/Demo/demo.py
+flixy/Learn/__init__.py
+flixy/Learn/learn.py
+flixy/Learn/lessons/Text.py
+flixy/Learn/lessons/__init__.py
+flixy/Learn/lessons/app.py
+flixy/Learn/lessons/button.py
+flixy/Learn/lessons/column.py
+flixy/Learn/lessons/navigate.py
+flixy/Learn/lessons/page.py
+flixy/Learn/lessons/row.py
+flixy/Learn/lessons/sheet.py
+flixy/Learn/lessons/textfield.py
+flixy/Learn/lessons/webview.py
 flixy/flixy/APP.py
 flixy/flixy/PAGE.py
 flixy/flixy/__init__.py
 flixy/flixy/installer.py
 flixy/flixy/update.py
 flixy/flixy/Tools/Haptics.py
 flixy/flixy/Tools/__init__.py
```

### Comparing `flixy2app-0.1/setup.py` & `flixy2app-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='flixy2app',
-    version='0.1',
+    version='0.2',
     author='SKbarbon',
     description='A UI-Builder that helps programmers build the front-end without codding it.',
     long_description=long_description,
     url='https://github.com/SKbarbon/flixy',
     install_requires=["flet", "requests", "PyInstaller"],
     packages=find_packages(),
     classifiers=[
```

