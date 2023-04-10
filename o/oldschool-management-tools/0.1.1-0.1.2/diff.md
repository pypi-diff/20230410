# Comparing `tmp/oldschool_management_tools-0.1.1.tar.gz` & `tmp/oldschool_management_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldschool_management_tools-0.1.1.tar", max compression
+gzip compressed data, was "oldschool_management_tools-0.1.2.tar", max compression
```

## Comparing `oldschool_management_tools-0.1.1.tar` & `oldschool_management_tools-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       96 2023-04-10 12:05:51.622779 oldschool_management_tools-0.1.1/oldschool_management_tools/__init__.py
--rw-r--r--   0        0        0     1063 2022-11-05 13:50:02.083491 oldschool_management_tools-0.1.1/oldschool_management_tools/calendar_items/calendar_item.py
--rw-r--r--   0        0        0      565 2023-04-10 12:03:47.257190 oldschool_management_tools-0.1.1/oldschool_management_tools/mgmt_tools_cmd.py
--rw-r--r--   0        0        0     2041 2023-04-10 12:05:13.986985 oldschool_management_tools-0.1.1/oldschool_management_tools/oldschool_management_tools.py
--rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.1/oldschool_management_tools/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.1/oldschool_management_tools/README.md
--rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.1/oldschool_management_tools/special_prompts/special_prompts.py
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.1/oldschool_management_tools/tests/__init__.py
--rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.1/oldschool_management_tools/testy.py
--rw-r--r--   0        0        0      436 2023-04-10 12:20:22.624588 oldschool_management_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.1/README.md
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-04-10 14:00:06.731384 oldschool_management_tools-0.1.2/oldschool_management_tools/__init__.py
+-rw-r--r--   0        0        0     1315 2023-04-10 13:00:12.829587 oldschool_management_tools-0.1.2/oldschool_management_tools/calendar_items/calendar_item.py
+-rw-r--r--   0        0        0      717 2023-04-10 13:59:08.542015 oldschool_management_tools-0.1.2/oldschool_management_tools/mgmt_tools_cmd.py
+-rw-r--r--   0        0        0     4238 2023-04-10 14:01:09.839528 oldschool_management_tools-0.1.2/oldschool_management_tools/oldschool_management_tools.py
+-rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.2/oldschool_management_tools/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.2/oldschool_management_tools/README.md
+-rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.2/oldschool_management_tools/special_prompts/special_prompts.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.2/oldschool_management_tools/tests/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.2/oldschool_management_tools/testy.py
+-rw-r--r--   0        0        0      436 2023-04-10 14:02:10.130419 oldschool_management_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.2/PKG-INFO
```

### Comparing `oldschool_management_tools-0.1.1/oldschool_management_tools/calendar_items/calendar_item.py` & `oldschool_management_tools-0.1.2/oldschool_management_tools/calendar_items/calendar_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from dataclasses import dataclass
-from datetime import time
+from datetime import time, datetime
 from termcolor import cprint
 
 
 def nice_time_str(time_in_zone) -> str:
     return str(time_in_zone)[0:-3]
 
 
 @dataclass
 class CalendarItem:
     name: str
     location: str
     category: str
+    start_datetime: datetime
     start_time: time
+    end_datetime: datetime
     end_time: time
 
     def print(self):
         cprint(f"{nice_time_str(self.start_time)} to {nice_time_str(self.end_time)} - {self.name} - {self.location}", self.category)
 
     @classmethod
     def from_outlook_apt(cls, apt):
+        start_datetime = datetime.fromisoformat(str(apt.StartInStartTimeZone))
         start_time = time.fromisoformat(str(apt.StartInStartTimeZone.time()))
+        end_datetime = datetime.fromisoformat(str(apt.EndInEndTimeZone))
         end_time = time.fromisoformat(str(apt.EndInEndTimeZone.time()))
 
         location = apt.Location
         category = apt.Categories.split(' ')[0].lower()
         match category:
             case '':
                 category = 'blue'
             case 'orange':
                 category = 'yellow'
             case 'purple':
                 category = 'magenta'
-        return CalendarItem(apt.Subject, location, category, start_time, end_time)
+        return CalendarItem(apt.Subject, location, category, start_datetime, start_time, end_datetime, end_time)
```

### Comparing `oldschool_management_tools-0.1.1/oldschool_management_tools/mgmt_tools_cmd.py` & `oldschool_management_tools-0.1.2/oldschool_management_tools/mgmt_tools_cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import cmd
-from oldschool_management_tools.oldschool_management_tools import parse_day, show_day_sched, prompt_day_tasks
+from oldschool_management_tools.oldschool_management_tools import parse_day, show_day_sched, prompt_day_tasks, fill_prep
 
 
 class MgmtToolsCmd(cmd.Cmd):
     intro = "Welcome to Old School Management Tools"
     prompt = "(mgmt) "
 
     def do_prompt_tasks(self, day):
         parsed_day = parse_day(day)
         prompt_day_tasks(parsed_day)
 
     def do_show_sched(self, day):
         parsed_day = parse_day(day)
         show_day_sched(parsed_day)
 
+    def do_fill_prep(self, day):
+        parsed_day = parse_day(day)
+        fill_prep(parsed_day)
+
     def do_die(self, args):
         return True
 
     def do_EOF(self, args):
         return True
 
+
+MgmtToolsCmd().cmdloop()
+exit(0)
```

### Comparing `oldschool_management_tools-0.1.1/oldschool_management_tools/special_prompts/special_prompts.py` & `oldschool_management_tools-0.1.2/oldschool_management_tools/special_prompts/special_prompts.py`

 * *Files identical despite different names*

