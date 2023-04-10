# Comparing `tmp/oldschool_management_tools-0.1.2.tar.gz` & `tmp/oldschool_management_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldschool_management_tools-0.1.2.tar", max compression
+gzip compressed data, was "oldschool_management_tools-0.1.3.tar", max compression
```

## Comparing `oldschool_management_tools-0.1.2.tar` & `oldschool_management_tools-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       70 2023-04-10 14:00:06.731384 oldschool_management_tools-0.1.2/oldschool_management_tools/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-10 13:00:12.829587 oldschool_management_tools-0.1.2/oldschool_management_tools/calendar_items/calendar_item.py
--rw-r--r--   0        0        0      717 2023-04-10 13:59:08.542015 oldschool_management_tools-0.1.2/oldschool_management_tools/mgmt_tools_cmd.py
--rw-r--r--   0        0        0     4238 2023-04-10 14:01:09.839528 oldschool_management_tools-0.1.2/oldschool_management_tools/oldschool_management_tools.py
--rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.2/oldschool_management_tools/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.2/oldschool_management_tools/README.md
--rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.2/oldschool_management_tools/special_prompts/special_prompts.py
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.2/oldschool_management_tools/tests/__init__.py
--rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.2/oldschool_management_tools/testy.py
--rw-r--r--   0        0        0      436 2023-04-10 14:02:10.130419 oldschool_management_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.2/README.md
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-04-10 14:00:06.731384 oldschool_management_tools-0.1.3/oldschool_management_tools/__init__.py
+-rw-r--r--   0        0        0     1315 2023-04-10 13:00:12.829587 oldschool_management_tools-0.1.3/oldschool_management_tools/calendar_items/calendar_item.py
+-rw-r--r--   0        0        0      889 2023-04-10 14:31:53.992235 oldschool_management_tools-0.1.3/oldschool_management_tools/mgmt_tools_cmd.py
+-rw-r--r--   0        0        0     4804 2023-04-10 14:52:09.479176 oldschool_management_tools-0.1.3/oldschool_management_tools/oldschool_management_tools.py
+-rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.3/oldschool_management_tools/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.3/oldschool_management_tools/README.md
+-rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.3/oldschool_management_tools/special_prompts/special_prompts.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.3/oldschool_management_tools/tests/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.3/oldschool_management_tools/testy.py
+-rw-r--r--   0        0        0      436 2023-04-10 14:52:14.977522 oldschool_management_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.3/PKG-INFO
```

### Comparing `oldschool_management_tools-0.1.2/oldschool_management_tools/calendar_items/calendar_item.py` & `oldschool_management_tools-0.1.3/oldschool_management_tools/calendar_items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.2/oldschool_management_tools/mgmt_tools_cmd.py` & `oldschool_management_tools-0.1.3/oldschool_management_tools/mgmt_tools_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import cmd
-from oldschool_management_tools.oldschool_management_tools import parse_day, show_day_sched, prompt_day_tasks, fill_prep
+from oldschool_management_tools.oldschool_management_tools import parse_day, show_day_sched, prompt_day_tasks, fill_prep, wipe_prep
+
 
 
 class MgmtToolsCmd(cmd.Cmd):
     intro = "Welcome to Old School Management Tools"
     prompt = "(mgmt) "
 
     def do_prompt_tasks(self, day):
@@ -14,16 +15,24 @@
         parsed_day = parse_day(day)
         show_day_sched(parsed_day)
 
     def do_fill_prep(self, day):
         parsed_day = parse_day(day)
         fill_prep(parsed_day)
 
+    def do_wipe_prep(self, day):
+        parsed_day = parse_day(day)
+        wipe_prep(parsed_day)
+
     def do_die(self, args):
         return True
 
+
+    def do_exit(self, args):
+        return True
+
     def do_EOF(self, args):
         return True
 
 
 MgmtToolsCmd().cmdloop()
 exit(0)
```

### Comparing `oldschool_management_tools-0.1.2/oldschool_management_tools/oldschool_management_tools.py` & `oldschool_management_tools-0.1.3/oldschool_management_tools/oldschool_management_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 def start_of_day(day: date) -> datetime:
     return datetime.combine(day, time())
 
 
 def parse_day(day) -> datetime:
     match day:
-        case "today":
+        case None | '' | "today":
             return start_of_day(date.today())
         case "tomorrow":
             return start_of_day(date.today()) + timedelta(days=1)
         case d if day.isnumeric():
             return start_of_day(date.today()) + timedelta(days=int(d))
         case _:
             raise ValueError(f"Bad day [{day}]")
@@ -102,14 +102,32 @@
                                          prep_slot.start_datetime, prep_slot.start_datetime.time(),
                                          prep_slot.end_datetime, prep_slot.end_datetime.time()))
         last_apt_end_time = apt.end_datetime
 
     [add_apt(cal, apt) for apt in new_apts]
 
 
+def wipe_prep(parsed_day=datetime.today()):
+    cal = get_day_cal(parsed_day)
+    cal_item_num = 0
+    try:
+        while cal.Count > cal_item_num + 1:
+            appt = cal[cal_item_num]
+            cal_item = CalendarItem.from_outlook_apt(appt)
+
+            if cal_item.category == "yellow" and cal_item.name.startswith("Prep"):
+                appt.Delete()
+                cal = get_day_cal(parsed_day)
+            else:
+                cal_item_num = cal_item_num + 1
+    except IndexError:
+        # Probably fine
+        pass
+
+
 def add_apt(cal: win32com.client.CDispatch, apt: CalendarItem):
     outlook = client.Dispatch('Outlook.Application')
     apt.print()
     appt = outlook.CreateItem(1)
     appt.Start = str(apt.start_datetime)[0:-6]
     appt.Subject = apt.name
     appt.Categories = apt.category + " Category"
```

### Comparing `oldschool_management_tools-0.1.2/oldschool_management_tools/special_prompts/special_prompts.py` & `oldschool_management_tools-0.1.3/oldschool_management_tools/special_prompts/special_prompts.py`

 * *Files identical despite different names*

