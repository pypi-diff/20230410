# Comparing `tmp/oldschool_management_tools-0.0.8.tar.gz` & `tmp/oldschool_management_tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldschool_management_tools-0.0.8.tar", last modified: Mon Nov  7 18:21:38 2022, max compression
+gzip compressed data, was "oldschool_management_tools-0.1.0.tar", max compression
```

## Comparing `oldschool_management_tools-0.0.8.tar` & `oldschool_management_tools-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 18:21:38.144352 oldschool_management_tools-0.0.8/
--rw-rw-rw-   0        0        0      378 2022-11-07 18:21:38.139333 oldschool_management_tools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        4 2022-10-15 13:56:15.000000 oldschool_management_tools-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-11-07 18:21:38.145317 oldschool_management_tools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1245 2022-11-07 18:21:01.000000 oldschool_management_tools-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-07 18:21:38.115185 oldschool_management_tools-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-07 18:21:38.120380 oldschool_management_tools-0.0.8/src/oldschool_management_tools/
-drwxrwxrwx   0        0        0        0 2022-11-07 18:21:38.137338 oldschool_management_tools-0.0.8/src/oldschool_management_tools/calendar_items/
--rw-rw-rw-   0        0        0     1063 2022-11-05 13:50:02.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools/calendar_items/calendar_item.py
--rw-rw-rw-   0        0        0      598 2022-10-23 10:09:16.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools/mgmt_tools_cmd.py
--rw-rw-rw-   0        0        0     1987 2022-11-06 12:32:08.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools/oldschool_management_tools.py
-drwxrwxrwx   0        0        0        0 2022-11-07 18:21:38.138335 oldschool_management_tools-0.0.8/src/oldschool_management_tools/special_prompts/
--rw-rw-rw-   0        0        0      698 2022-11-06 16:58:42.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools/special_prompts/special_prompts.py
-drwxrwxrwx   0        0        0        0 2022-11-07 18:21:38.136341 oldschool_management_tools-0.0.8/src/oldschool_management_tools.egg-info/
--rw-rw-rw-   0        0        0      378 2022-11-07 18:21:38.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2022-11-07 18:21:38.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 18:21:38.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-11-07 18:21:38.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-11-07 18:21:38.000000 oldschool_management_tools-0.0.8/src/oldschool_management_tools.egg-info/top_level.txt
+-rw-r--r--   0        0        0       96 2023-04-10 12:05:51.622779 oldschool_management_tools-0.1.0/oldschool_management_tools/__init__.py
+-rw-r--r--   0        0        0     1063 2022-11-05 13:50:02.083491 oldschool_management_tools-0.1.0/oldschool_management_tools/calendar_items/calendar_item.py
+-rw-r--r--   0        0        0      565 2023-04-10 12:03:47.257190 oldschool_management_tools-0.1.0/oldschool_management_tools/mgmt_tools_cmd.py
+-rw-r--r--   0        0        0     2041 2023-04-10 12:05:13.986985 oldschool_management_tools-0.1.0/oldschool_management_tools/oldschool_management_tools.py
+-rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.0/oldschool_management_tools/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.0/oldschool_management_tools/README.md
+-rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.0/oldschool_management_tools/special_prompts/special_prompts.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.0/oldschool_management_tools/tests/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.0/oldschool_management_tools/testy.py
+-rw-r--r--   0        0        0      440 2023-04-10 12:03:11.141215 oldschool_management_tools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.0/README.md
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.0/PKG-INFO
```

### Comparing `oldschool_management_tools-0.0.8/src/oldschool_management_tools/calendar_items/calendar_item.py` & `oldschool_management_tools-0.1.0/oldschool_management_tools/calendar_items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.0.8/src/oldschool_management_tools/mgmt_tools_cmd.py` & `oldschool_management_tools-0.1.0/oldschool_management_tools/mgmt_tools_cmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cmd
-from oldschool_management_tools import parse_day, show_day_sched, prompt_day_tasks
+from oldschool_management_tools.oldschool_management_tools import parse_day, show_day_sched, prompt_day_tasks
 
 
 class MgmtToolsCmd(cmd.Cmd):
     intro = "Welcome to Old School Management Tools"
     prompt = "(mgmt) "
 
     def do_prompt_tasks(self, day):
@@ -16,10 +16,7 @@
 
     def do_die(self, args):
         return True
 
     def do_EOF(self, args):
         return True
 
-
-if __name__ == "__main__":
-    MgmtToolsCmd().cmdloop()
```

### Comparing `oldschool_management_tools-0.0.8/src/oldschool_management_tools/oldschool_management_tools.py` & `oldschool_management_tools-0.1.0/oldschool_management_tools/oldschool_management_tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timedelta, date, time
 from win32com import client
-from special_prompts.special_prompts import SPECIAL_PROMPTS
+from oldschool_management_tools.special_prompts.special_prompts import SPECIAL_PROMPTS
 from os import system
-from calendar_items.calendar_item import CalendarItem
+from oldschool_management_tools.calendar_items.calendar_item import CalendarItem
 
 # Ideas:
 #  - See allocated time per day
 #  - Plan in breaks
 #  - Draw schedule in hours
 
 # Do the work where it is fast :)
```

### Comparing `oldschool_management_tools-0.0.8/src/oldschool_management_tools/special_prompts/special_prompts.py` & `oldschool_management_tools-0.1.0/oldschool_management_tools/special_prompts/special_prompts.py`

 * *Files identical despite different names*

