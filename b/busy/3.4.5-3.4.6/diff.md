# Comparing `tmp/busy-3.4.5.tar.gz` & `tmp/busy-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-3.4.5.tar", last modified: Mon Apr 10 09:43:27 2023, max compression
+gzip compressed data, was "busy-3.4.6.tar", last modified: Mon Apr 10 09:59:09 2023, max compression
```

## Comparing `busy-3.4.5.tar` & `busy-3.4.6.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.945001 busy-3.4.5/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-30 16:53:52.000000 busy-3.4.5/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)    21954 2023-04-10 09:43:27.944452 busy-3.4.5/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)    21709 2023-04-09 05:42:36.000000 busy-3.4.5/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.892286 busy-3.4.5/busy/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       66 2023-03-30 16:53:52.000000 busy-3.4.5/busy/__main__.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.906083 busy-3.4.5/busy/command/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1872 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/activate_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      825 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/add_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      245 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/base_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     8907 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      279 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/curses_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1643 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/defer_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      981 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/delete_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/drop_and_pop_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1309 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/edit_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1908 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/finish_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      681 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/list_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      212 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/queues_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      254 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/resource_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      950 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/switch_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      196 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/tags_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      476 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/top_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3957 2023-04-10 09:34:40.000000 busy-3.4.5/busy/handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.910328 busy-3.4.5/busy/model/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/model/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1931 2023-04-10 09:34:40.000000 busy-3.4.5/busy/model/item.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2598 2023-03-30 16:53:52.000000 busy-3.4.5/busy/model/task.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.912918 busy-3.4.5/busy/queue/
--rw-r--r--   0 francispotter   (501) staff       (20)      102 2023-04-10 09:34:40.000000 busy-3.4.5/busy/queue/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5099 2023-04-10 09:34:40.000000 busy-3.4.5/busy/queue/queue.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2139 2023-04-10 09:34:40.000000 busy-3.4.5/busy/queue/todo_queue.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.913623 busy-3.4.5/busy/root/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/root/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2297 2023-04-10 09:34:40.000000 busy-3.4.5/busy/root/file_system_root.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2204 2023-03-30 16:53:52.000000 busy-3.4.5/busy/selector.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.915761 busy-3.4.5/busy/ui/
--rw-r--r--   0 francispotter   (501) staff       (20)      133 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     6839 2023-04-10 09:34:40.000000 busy-3.4.5/busy/ui/curses_ui.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1567 2023-04-10 09:34:40.000000 busy-3.4.5/busy/ui/shell_ui.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.917434 busy-3.4.5/busy/ui/tcl_ui/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/tcl_ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      824 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/tcl_ui/edit_task_widget.py
--rw-r--r--   0 francispotter   (501) staff       (20)      701 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/tcl_ui/get_item_widget.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5178 2023-04-10 09:34:40.000000 busy-3.4.5/busy/ui/ui.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.920284 busy-3.4.5/busy/util/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     6682 2023-04-10 09:34:40.000000 busy-3.4.5/busy/util/class_family.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2882 2023-04-10 09:34:40.000000 busy-3.4.5/busy/util/date_util.py
--rw-r--r--   0 francispotter   (501) staff       (20)      217 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/python_version.py
--rw-r--r--   0 francispotter   (501) staff       (20)      973 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/super_wrapper.py
--rw-r--r--   0 francispotter   (501) staff       (20)      131 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/textbox_util.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.894733 busy-3.4.5/busy.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)    21954 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     2195 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       43 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       82 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      596 2023-04-10 09:34:40.000000 busy-3.4.5/pyproject.toml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.925665 busy-3.4.5/sand/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-02-25 16:13:53.000000 busy-3.4.5/sand/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      336 2023-02-23 13:30:28.000000 busy-3.4.5/sand/_dataclass.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-05 00:41:16.000000 busy-3.4.5/sand/_readline_util.py
--rw-r--r--   0 francispotter   (501) staff       (20)      676 2023-02-25 17:04:15.000000 busy-3.4.5/sand/_textpad.py
--rw-r--r--   0 francispotter   (501) staff       (20)      233 2023-03-06 16:05:27.000000 busy-3.4.5/sand/chooser.py
--rw-r--r--   0 francispotter   (501) staff       (20)      282 2023-03-01 14:38:38.000000 busy-3.4.5/sand/rl-io.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-03-01 15:07:59.000000 busy-3.4.5/sand/subprocess.py
--rw-r--r--   0 francispotter   (501) staff       (20)      806 2023-03-02 16:10:26.000000 busy-3.4.5/sand/wrapper.py
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-10 09:43:27.945108 busy-3.4.5/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.926605 busy-3.4.5/test/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/__init__.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.929412 busy-3.4.5/test/data_class_family/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      101 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/atriarch.py
--rw-r--r--   0 francispotter   (501) staff       (20)       76 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/child.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/grandchild.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.930644 busy-3.4.5/test/handler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/handler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1205 2023-03-30 16:53:52.000000 busy-3.4.5/test/handler/test_handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.931659 busy-3.4.5/test/integration/
--rw-r--r--   0 francispotter   (501) staff       (20)      150 2023-04-10 09:34:40.000000 busy-3.4.5/test/integration/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      416 2023-04-10 09:34:40.000000 busy-3.4.5/test/integration/test_integration.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.935738 busy-3.4.5/test/model/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/model/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      433 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_item.py
--rw-r--r--   0 francispotter   (501) staff       (20)      845 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_item_io.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2857 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_queue.py
--rw-r--r--   0 francispotter   (501) staff       (20)      624 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_queue_replace.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1778 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_task.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4056 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_todo_queue.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.937569 busy-3.4.5/test/root/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-10 09:34:40.000000 busy-3.4.5/test/root/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1406 2023-04-10 09:34:40.000000 busy-3.4.5/test/root/test_file.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2547 2023-04-10 09:34:40.000000 busy-3.4.5/test/root/test_file_system_root.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.939223 busy-3.4.5/test/ui/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      357 2023-03-30 16:53:52.000000 busy-3.4.5/test/ui/test_shell_ui.py
--rw-r--r--   0 francispotter   (501) staff       (20)      790 2023-03-30 16:53:52.000000 busy-3.4.5/test/ui/test_ui_terminal_editor.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.943266 busy-3.4.5/test/util/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      797 2023-04-10 09:34:40.000000 busy-3.4.5/test/util/test_class_families.py
--rw-r--r--   0 francispotter   (501) staff       (20)      237 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/test_class_family.py
--rw-r--r--   0 francispotter   (501) staff       (20)      452 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/test_date.py
--rw-r--r--   0 francispotter   (501) staff       (20)      508 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/test_python_version.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:36:08.000000 busy-3.4.5/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.589567 busy-3.4.6/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-30 16:53:52.000000 busy-3.4.6/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)    20450 2023-04-10 09:59:09.589068 busy-3.4.6/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)    20205 2023-04-10 09:55:35.000000 busy-3.4.6/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.530556 busy-3.4.6/busy/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       66 2023-03-30 16:53:52.000000 busy-3.4.6/busy/__main__.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.548988 busy-3.4.6/busy/command/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1872 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/activate_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      825 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/add_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      245 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/base_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     8907 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      279 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/curses_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1643 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/defer_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      981 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/delete_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/drop_and_pop_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1309 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/edit_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1908 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/finish_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      681 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/list_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      212 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/queues_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      254 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/resource_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      950 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/switch_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      196 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/tags_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      476 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/top_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3957 2023-04-10 09:34:40.000000 busy-3.4.6/busy/handler.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.550680 busy-3.4.6/busy/model/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/model/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1931 2023-04-10 09:34:40.000000 busy-3.4.6/busy/model/item.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2598 2023-03-30 16:53:52.000000 busy-3.4.6/busy/model/task.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.552796 busy-3.4.6/busy/queue/
+-rw-r--r--   0 francispotter   (501) staff       (20)      102 2023-04-10 09:34:40.000000 busy-3.4.6/busy/queue/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5099 2023-04-10 09:34:40.000000 busy-3.4.6/busy/queue/queue.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2139 2023-04-10 09:34:40.000000 busy-3.4.6/busy/queue/todo_queue.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.553823 busy-3.4.6/busy/root/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/root/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2297 2023-04-10 09:34:40.000000 busy-3.4.6/busy/root/file_system_root.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2204 2023-03-30 16:53:52.000000 busy-3.4.6/busy/selector.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.556748 busy-3.4.6/busy/ui/
+-rw-r--r--   0 francispotter   (501) staff       (20)      133 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     6839 2023-04-10 09:34:40.000000 busy-3.4.6/busy/ui/curses_ui.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1567 2023-04-10 09:34:40.000000 busy-3.4.6/busy/ui/shell_ui.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.558838 busy-3.4.6/busy/ui/tcl_ui/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/tcl_ui/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      824 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/tcl_ui/edit_task_widget.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      701 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/tcl_ui/get_item_widget.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5178 2023-04-10 09:34:40.000000 busy-3.4.6/busy/ui/ui.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.562565 busy-3.4.6/busy/util/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     6682 2023-04-10 09:34:40.000000 busy-3.4.6/busy/util/class_family.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2882 2023-04-10 09:34:40.000000 busy-3.4.6/busy/util/date_util.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      217 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/python_version.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      973 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/super_wrapper.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      131 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/textbox_util.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.534568 busy-3.4.6/busy.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)    20450 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     2195 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       43 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       82 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      596 2023-04-10 09:34:40.000000 busy-3.4.6/pyproject.toml
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.571382 busy-3.4.6/sand/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-02-25 16:13:53.000000 busy-3.4.6/sand/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      336 2023-02-23 13:30:28.000000 busy-3.4.6/sand/_dataclass.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-05 00:41:16.000000 busy-3.4.6/sand/_readline_util.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      676 2023-02-25 17:04:15.000000 busy-3.4.6/sand/_textpad.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      233 2023-03-06 16:05:27.000000 busy-3.4.6/sand/chooser.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      282 2023-03-01 14:38:38.000000 busy-3.4.6/sand/rl-io.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-03-01 15:07:59.000000 busy-3.4.6/sand/subprocess.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      806 2023-03-02 16:10:26.000000 busy-3.4.6/sand/wrapper.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-10 09:59:09.589730 busy-3.4.6/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.572221 busy-3.4.6/test/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/__init__.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.574121 busy-3.4.6/test/data_class_family/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      101 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/atriarch.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       76 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/child.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/grandchild.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.574885 busy-3.4.6/test/handler/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/handler/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1205 2023-03-30 16:53:52.000000 busy-3.4.6/test/handler/test_handler.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.576635 busy-3.4.6/test/integration/
+-rw-r--r--   0 francispotter   (501) staff       (20)      150 2023-04-10 09:34:40.000000 busy-3.4.6/test/integration/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      416 2023-04-10 09:34:40.000000 busy-3.4.6/test/integration/test_integration.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.581255 busy-3.4.6/test/model/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/model/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      433 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_item.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      845 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_item_io.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2857 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_queue.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      624 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_queue_replace.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1778 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_task.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     4056 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_todo_queue.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.583580 busy-3.4.6/test/root/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-10 09:34:40.000000 busy-3.4.6/test/root/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1406 2023-04-10 09:34:40.000000 busy-3.4.6/test/root/test_file.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2547 2023-04-10 09:34:40.000000 busy-3.4.6/test/root/test_file_system_root.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.585044 busy-3.4.6/test/ui/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/ui/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      357 2023-03-30 16:53:52.000000 busy-3.4.6/test/ui/test_shell_ui.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      790 2023-03-30 16:53:52.000000 busy-3.4.6/test/ui/test_ui_terminal_editor.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.588146 busy-3.4.6/test/util/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      797 2023-04-10 09:34:40.000000 busy-3.4.6/test/util/test_class_families.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      237 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/test_class_family.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      452 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/test_date.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      508 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/test_python_version.py
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:58:56.000000 busy-3.4.6/version
```

### Comparing `busy-3.4.5/LICENSE` & `busy-3.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/PKG-INFO` & `busy-3.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 3.4.5
+Version: 3.4.6
 Summary: Personal time management system
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -30,59 +30,33 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-You'll need a terminal emulator to access a command or shell prompt. Examples include:
+Beginners, see [INSTALLATION.md](INSTALLATION.md).
 
-- iTerm2 or Terminal on MacOS
-- Gnome Terminal or XTerm on Linux
-- CMD on Windows
-- Terminator on all platforms
+Experienced folks, use [pipx](https://pypa.github.io/pipx/) to install Busy.
 
-Busy also requires Python 3.6.5 or later. To check whether you already have the right version of Python on your system, start your terminal emulator and type:
-
-```
-python -V
+```bash
+pipx install busy
 ```
 
-If that doesn't work, try:
+To upgrade:
 
+```bash
+pipx upgrade busy
 ```
-python3 -V
-```
-
-If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Linux). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
-
-Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
-
-From now on, we're going to use `python3` and `pip3` in code snippets, although your system might prefer simply `python` or `pip`. Just edit them.
-
-_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses pyreadline3` to install the things that don't come out of the box with Python on Windows.
-
-_Python developers only_ Busy does require other packages, so feel free to use a venv.
 
-Here's the command to install the latest stable version of Busy itself:
-
-```
-sudo pip3 install busy && pip3 show busy
-```
-
-If you have previously installed Busy, and want to upgrade to the latest version, type:
-
-```
-sudo pip3 install --upgrade busy && pip3 show busy
-```
 
 Overview
 --------
 
-Busy ships with 2 user interfaces, both of them terminal-based and keyboard-driven:
+Busy ships with two user interfaces, both of them terminal-based and keyboard-driven:
 
 - *Shell UI* - A command-line interface (CLI) using shell conventions and called directly from the shell, one command at a time.
 - *Curses UI* - A faster, more visual interface with one-key commands that remains visible the entire time it's being used.
 
 Some commands also use your favorite terminal-based text editor, such as Emacs, vi, or Nano. It's possible to use Busy without a text editor, but functionality is limited.
 
 Busy's core model is a collection of Items, the most interesting of which are Tasks. Items are organized into Queues, which are ordered sets. You work on the top Task in the Queue, and when it's done, that Task gets removed from the Queue to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
```

### Comparing `busy-3.4.5/README.md` & `busy-3.4.6/busy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: busy
+Version: 3.4.6
+Summary: Personal time management system
+Author-email: Francis Potter <busy@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.6.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Busy
 ====
 
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
@@ -20,59 +30,33 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-You'll need a terminal emulator to access a command or shell prompt. Examples include:
-
-- iTerm2 or Terminal on MacOS
-- Gnome Terminal or XTerm on Linux
-- CMD on Windows
-- Terminator on all platforms
-
-Busy also requires Python 3.6.5 or later. To check whether you already have the right version of Python on your system, start your terminal emulator and type:
-
-```
-python -V
-```
+Beginners, see [INSTALLATION.md](INSTALLATION.md).
 
-If that doesn't work, try:
+Experienced folks, use [pipx](https://pypa.github.io/pipx/) to install Busy.
 
+```bash
+pipx install busy
 ```
-python3 -V
-```
-
-If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Linux). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
 
-Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
-
-From now on, we're going to use `python3` and `pip3` in code snippets, although your system might prefer simply `python` or `pip`. Just edit them.
-
-_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses pyreadline3` to install the things that don't come out of the box with Python on Windows.
-
-_Python developers only_ Busy does require other packages, so feel free to use a venv.
-
-Here's the command to install the latest stable version of Busy itself:
+To upgrade:
 
+```bash
+pipx upgrade busy
 ```
-sudo pip3 install busy && pip3 show busy
-```
-
-If you have previously installed Busy, and want to upgrade to the latest version, type:
 
-```
-sudo pip3 install --upgrade busy && pip3 show busy
-```
 
 Overview
 --------
 
-Busy ships with 2 user interfaces, both of them terminal-based and keyboard-driven:
+Busy ships with two user interfaces, both of them terminal-based and keyboard-driven:
 
 - *Shell UI* - A command-line interface (CLI) using shell conventions and called directly from the shell, one command at a time.
 - *Curses UI* - A faster, more visual interface with one-key commands that remains visible the entire time it's being used.
 
 Some commands also use your favorite terminal-based text editor, such as Emacs, vi, or Nano. It's possible to use Busy without a text editor, but functionality is limited.
 
 Busy's core model is a collection of Items, the most interesting of which are Tasks. Items are organized into Queues, which are ordered sets. You work on the top Task in the Queue, and when it's done, that Task gets removed from the Queue to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
```

### Comparing `busy-3.4.5/busy/command/activate_command.py` & `busy-3.4.6/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/add_command.py` & `busy-3.4.6/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/command.py` & `busy-3.4.6/busy/command/command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/defer_command.py` & `busy-3.4.6/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/delete_command.py` & `busy-3.4.6/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/drop_and_pop_command.py` & `busy-3.4.6/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/edit_command.py` & `busy-3.4.6/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/finish_command.py` & `busy-3.4.6/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/list_command.py` & `busy-3.4.6/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/command/switch_command.py` & `busy-3.4.6/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/handler.py` & `busy-3.4.6/busy/handler.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/model/item.py` & `busy-3.4.6/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/model/task.py` & `busy-3.4.6/busy/model/task.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/queue/queue.py` & `busy-3.4.6/busy/queue/queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/queue/todo_queue.py` & `busy-3.4.6/busy/queue/todo_queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/root/file_system_root.py` & `busy-3.4.6/busy/root/file_system_root.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/selector.py` & `busy-3.4.6/busy/selector.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/ui/curses_ui.py` & `busy-3.4.6/busy/ui/curses_ui.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/ui/shell_ui.py` & `busy-3.4.6/busy/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/ui/tcl_ui/edit_task_widget.py` & `busy-3.4.6/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/ui/tcl_ui/get_item_widget.py` & `busy-3.4.6/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/ui/ui.py` & `busy-3.4.6/busy/ui/ui.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/util/class_family.py` & `busy-3.4.6/busy/util/class_family.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/util/date_util.py` & `busy-3.4.6/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy/util/super_wrapper.py` & `busy-3.4.6/busy/util/super_wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/busy.egg-info/PKG-INFO` & `busy-3.4.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: busy
-Version: 3.4.5
-Summary: Personal time management system
-Author-email: Francis Potter <busy@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Busy
 ====
 
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
@@ -30,59 +20,33 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-You'll need a terminal emulator to access a command or shell prompt. Examples include:
-
-- iTerm2 or Terminal on MacOS
-- Gnome Terminal or XTerm on Linux
-- CMD on Windows
-- Terminator on all platforms
-
-Busy also requires Python 3.6.5 or later. To check whether you already have the right version of Python on your system, start your terminal emulator and type:
-
-```
-python -V
-```
+Beginners, see [INSTALLATION.md](INSTALLATION.md).
 
-If that doesn't work, try:
+Experienced folks, use [pipx](https://pypa.github.io/pipx/) to install Busy.
 
+```bash
+pipx install busy
 ```
-python3 -V
-```
-
-If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Linux). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
 
-Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
-
-From now on, we're going to use `python3` and `pip3` in code snippets, although your system might prefer simply `python` or `pip`. Just edit them.
-
-_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses pyreadline3` to install the things that don't come out of the box with Python on Windows.
-
-_Python developers only_ Busy does require other packages, so feel free to use a venv.
-
-Here's the command to install the latest stable version of Busy itself:
+To upgrade:
 
+```bash
+pipx upgrade busy
 ```
-sudo pip3 install busy && pip3 show busy
-```
-
-If you have previously installed Busy, and want to upgrade to the latest version, type:
 
-```
-sudo pip3 install --upgrade busy && pip3 show busy
-```
 
 Overview
 --------
 
-Busy ships with 2 user interfaces, both of them terminal-based and keyboard-driven:
+Busy ships with two user interfaces, both of them terminal-based and keyboard-driven:
 
 - *Shell UI* - A command-line interface (CLI) using shell conventions and called directly from the shell, one command at a time.
 - *Curses UI* - A faster, more visual interface with one-key commands that remains visible the entire time it's being used.
 
 Some commands also use your favorite terminal-based text editor, such as Emacs, vi, or Nano. It's possible to use Busy without a text editor, but functionality is limited.
 
 Busy's core model is a collection of Items, the most interesting of which are Tasks. Items are organized into Queues, which are ordered sets. You work on the top Task in the Queue, and when it's done, that Task gets removed from the Queue to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
```

### Comparing `busy-3.4.5/busy.egg-info/SOURCES.txt` & `busy-3.4.6/busy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/pyproject.toml` & `busy-3.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/sand/_textpad.py` & `busy-3.4.6/sand/_textpad.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/sand/subprocess.py` & `busy-3.4.6/sand/subprocess.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/sand/wrapper.py` & `busy-3.4.6/sand/wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/handler/test_handler.py` & `busy-3.4.6/test/handler/test_handler.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/model/test_item_io.py` & `busy-3.4.6/test/model/test_item_io.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/model/test_queue.py` & `busy-3.4.6/test/model/test_queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/model/test_queue_replace.py` & `busy-3.4.6/test/model/test_queue_replace.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/model/test_task.py` & `busy-3.4.6/test/model/test_task.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/model/test_todo_queue.py` & `busy-3.4.6/test/model/test_todo_queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/root/test_file.py` & `busy-3.4.6/test/root/test_file.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/root/test_file_system_root.py` & `busy-3.4.6/test/root/test_file_system_root.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/ui/test_ui_terminal_editor.py` & `busy-3.4.6/test/ui/test_ui_terminal_editor.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.5/test/util/test_class_families.py` & `busy-3.4.6/test/util/test_class_families.py`

 * *Files identical despite different names*

