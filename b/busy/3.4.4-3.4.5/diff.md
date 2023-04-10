# Comparing `tmp/busy-3.4.4.tar.gz` & `tmp/busy-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-3.4.4.tar", last modified: Fri Apr  7 05:38:03 2023, max compression
+gzip compressed data, was "busy-3.4.5.tar", last modified: Mon Apr 10 09:43:27 2023, max compression
```

## Comparing `busy-3.4.4.tar` & `busy-3.4.5.tar`

### file list

```diff
@@ -1,109 +1,108 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.959057 busy-3.4.4/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-30 16:53:52.000000 busy-3.4.4/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)    21828 2023-04-07 05:38:03.958393 busy-3.4.4/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)    21583 2023-04-07 05:33:57.000000 busy-3.4.4/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.894292 busy-3.4.4/busy/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/busy/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       66 2023-03-30 16:53:52.000000 busy-3.4.4/busy/__main__.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.916758 busy-3.4.4/busy/command/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1872 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/activate_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      825 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/add_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      245 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/base_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     8907 2023-04-07 05:33:57.000000 busy-3.4.4/busy/command/command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      279 2023-04-07 05:33:57.000000 busy-3.4.4/busy/command/curses_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1643 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/defer_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      981 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/delete_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-04-07 05:33:57.000000 busy-3.4.4/busy/command/drop_and_pop_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1309 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/edit_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1908 2023-04-07 05:33:57.000000 busy-3.4.4/busy/command/finish_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      681 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/list_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      212 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/queues_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      254 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/resource_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      950 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/switch_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      196 2023-03-30 16:53:52.000000 busy-3.4.4/busy/command/tags_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      476 2023-04-07 05:33:57.000000 busy-3.4.4/busy/command/top_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3957 2023-04-07 05:33:57.000000 busy-3.4.4/busy/handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.918684 busy-3.4.4/busy/model/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/busy/model/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1931 2023-04-07 05:33:57.000000 busy-3.4.4/busy/model/item.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2598 2023-03-30 16:53:52.000000 busy-3.4.4/busy/model/task.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.920899 busy-3.4.4/busy/queue/
--rw-r--r--   0 francispotter   (501) staff       (20)      102 2023-04-07 05:33:57.000000 busy-3.4.4/busy/queue/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5099 2023-04-07 05:33:57.000000 busy-3.4.4/busy/queue/queue.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2139 2023-04-07 05:33:57.000000 busy-3.4.4/busy/queue/todo_queue.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.921930 busy-3.4.4/busy/root/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/busy/root/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2297 2023-04-07 05:33:57.000000 busy-3.4.4/busy/root/file_system_root.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2204 2023-03-30 16:53:52.000000 busy-3.4.4/busy/selector.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.924320 busy-3.4.4/busy/ui/
--rw-r--r--   0 francispotter   (501) staff       (20)      133 2023-03-30 16:53:52.000000 busy-3.4.4/busy/ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     6839 2023-04-07 05:33:57.000000 busy-3.4.4/busy/ui/curses_ui.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1573 2023-04-07 05:33:57.000000 busy-3.4.4/busy/ui/shell_ui.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.926408 busy-3.4.4/busy/ui/tcl_ui/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/busy/ui/tcl_ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      824 2023-03-30 16:53:52.000000 busy-3.4.4/busy/ui/tcl_ui/edit_task_widget.py
--rw-r--r--   0 francispotter   (501) staff       (20)      701 2023-03-30 16:53:52.000000 busy-3.4.4/busy/ui/tcl_ui/get_item_widget.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5178 2023-04-07 05:33:57.000000 busy-3.4.4/busy/ui/ui.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.933233 busy-3.4.4/busy/util/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/busy/util/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     6682 2023-04-07 05:33:57.000000 busy-3.4.4/busy/util/class_family.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2882 2023-04-07 05:33:57.000000 busy-3.4.4/busy/util/date_util.py
--rw-r--r--   0 francispotter   (501) staff       (20)      217 2023-03-30 16:53:52.000000 busy-3.4.4/busy/util/python_version.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1231 2023-04-06 23:39:24.000000 busy-3.4.4/busy/util/readline_util.py
--rw-r--r--   0 francispotter   (501) staff       (20)      973 2023-03-30 16:53:52.000000 busy-3.4.4/busy/util/super_wrapper.py
--rw-r--r--   0 francispotter   (501) staff       (20)      131 2023-03-30 16:53:52.000000 busy-3.4.4/busy/util/textbox_util.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.900142 busy-3.4.4/busy.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)    21828 2023-04-07 05:38:03.000000 busy-3.4.4/busy.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     2222 2023-04-07 05:38:03.000000 busy-3.4.4/busy.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-07 05:38:03.000000 busy-3.4.4/busy.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       43 2023-04-07 05:38:03.000000 busy-3.4.4/busy.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       20 2023-04-07 05:38:03.000000 busy-3.4.4/busy.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-07 05:38:03.000000 busy-3.4.4/busy.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      524 2023-04-07 05:33:57.000000 busy-3.4.4/pyproject.toml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.938458 busy-3.4.4/sand/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-02-25 16:13:53.000000 busy-3.4.4/sand/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      336 2023-02-23 13:30:28.000000 busy-3.4.4/sand/_dataclass.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-05 00:41:16.000000 busy-3.4.4/sand/_readline_util.py
--rw-r--r--   0 francispotter   (501) staff       (20)      676 2023-02-25 17:04:15.000000 busy-3.4.4/sand/_textpad.py
--rw-r--r--   0 francispotter   (501) staff       (20)      233 2023-03-06 16:05:27.000000 busy-3.4.4/sand/chooser.py
--rw-r--r--   0 francispotter   (501) staff       (20)      282 2023-03-01 14:38:38.000000 busy-3.4.4/sand/rl-io.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-03-01 15:07:59.000000 busy-3.4.4/sand/subprocess.py
--rw-r--r--   0 francispotter   (501) staff       (20)      806 2023-03-02 16:10:26.000000 busy-3.4.4/sand/wrapper.py
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-07 05:38:03.959158 busy-3.4.4/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.939166 busy-3.4.4/test/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/test/__init__.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.941154 busy-3.4.4/test/data_class_family/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/test/data_class_family/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      101 2023-03-30 16:53:52.000000 busy-3.4.4/test/data_class_family/atriarch.py
--rw-r--r--   0 francispotter   (501) staff       (20)       76 2023-03-30 16:53:52.000000 busy-3.4.4/test/data_class_family/child.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-03-30 16:53:52.000000 busy-3.4.4/test/data_class_family/grandchild.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.942087 busy-3.4.4/test/handler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/test/handler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1205 2023-03-30 16:53:52.000000 busy-3.4.4/test/handler/test_handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.943506 busy-3.4.4/test/integration/
--rw-r--r--   0 francispotter   (501) staff       (20)      150 2023-04-07 05:33:57.000000 busy-3.4.4/test/integration/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      416 2023-04-07 05:33:57.000000 busy-3.4.4/test/integration/test_integration.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.948709 busy-3.4.4/test/model/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/test/model/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      433 2023-04-07 05:33:57.000000 busy-3.4.4/test/model/test_item.py
--rw-r--r--   0 francispotter   (501) staff       (20)      845 2023-04-07 05:33:57.000000 busy-3.4.4/test/model/test_item_io.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2857 2023-04-07 05:33:57.000000 busy-3.4.4/test/model/test_queue.py
--rw-r--r--   0 francispotter   (501) staff       (20)      624 2023-04-07 05:33:57.000000 busy-3.4.4/test/model/test_queue_replace.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1778 2023-04-07 05:33:57.000000 busy-3.4.4/test/model/test_task.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4056 2023-04-07 05:33:57.000000 busy-3.4.4/test/model/test_todo_queue.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.952426 busy-3.4.4/test/root/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-07 05:33:57.000000 busy-3.4.4/test/root/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1406 2023-04-07 05:33:57.000000 busy-3.4.4/test/root/test_file.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2529 2023-04-07 05:33:57.000000 busy-3.4.4/test/root/test_file_system_root.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.954250 busy-3.4.4/test/ui/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/test/ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      357 2023-03-30 16:53:52.000000 busy-3.4.4/test/ui/test_shell_ui.py
--rw-r--r--   0 francispotter   (501) staff       (20)      790 2023-03-30 16:53:52.000000 busy-3.4.4/test/ui/test_ui_terminal_editor.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-07 05:38:03.957495 busy-3.4.4/test/util/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.4/test/util/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      797 2023-04-07 05:33:57.000000 busy-3.4.4/test/util/test_class_families.py
--rw-r--r--   0 francispotter   (501) staff       (20)      237 2023-03-30 16:53:52.000000 busy-3.4.4/test/util/test_class_family.py
--rw-r--r--   0 francispotter   (501) staff       (20)      452 2023-03-30 16:53:52.000000 busy-3.4.4/test/util/test_date.py
--rw-r--r--   0 francispotter   (501) staff       (20)      508 2023-03-30 16:53:52.000000 busy-3.4.4/test/util/test_python_version.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-07 05:35:23.000000 busy-3.4.4/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.945001 busy-3.4.5/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-30 16:53:52.000000 busy-3.4.5/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)    21954 2023-04-10 09:43:27.944452 busy-3.4.5/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)    21709 2023-04-09 05:42:36.000000 busy-3.4.5/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.892286 busy-3.4.5/busy/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       66 2023-03-30 16:53:52.000000 busy-3.4.5/busy/__main__.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.906083 busy-3.4.5/busy/command/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1872 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/activate_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      825 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/add_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      245 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/base_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     8907 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      279 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/curses_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1643 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/defer_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      981 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/delete_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/drop_and_pop_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1309 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/edit_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1908 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/finish_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      681 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/list_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      212 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/queues_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      254 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/resource_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      950 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/switch_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      196 2023-03-30 16:53:52.000000 busy-3.4.5/busy/command/tags_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      476 2023-04-10 09:34:40.000000 busy-3.4.5/busy/command/top_command.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3957 2023-04-10 09:34:40.000000 busy-3.4.5/busy/handler.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.910328 busy-3.4.5/busy/model/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/model/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1931 2023-04-10 09:34:40.000000 busy-3.4.5/busy/model/item.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2598 2023-03-30 16:53:52.000000 busy-3.4.5/busy/model/task.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.912918 busy-3.4.5/busy/queue/
+-rw-r--r--   0 francispotter   (501) staff       (20)      102 2023-04-10 09:34:40.000000 busy-3.4.5/busy/queue/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5099 2023-04-10 09:34:40.000000 busy-3.4.5/busy/queue/queue.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2139 2023-04-10 09:34:40.000000 busy-3.4.5/busy/queue/todo_queue.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.913623 busy-3.4.5/busy/root/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/root/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2297 2023-04-10 09:34:40.000000 busy-3.4.5/busy/root/file_system_root.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2204 2023-03-30 16:53:52.000000 busy-3.4.5/busy/selector.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.915761 busy-3.4.5/busy/ui/
+-rw-r--r--   0 francispotter   (501) staff       (20)      133 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     6839 2023-04-10 09:34:40.000000 busy-3.4.5/busy/ui/curses_ui.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1567 2023-04-10 09:34:40.000000 busy-3.4.5/busy/ui/shell_ui.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.917434 busy-3.4.5/busy/ui/tcl_ui/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/tcl_ui/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      824 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/tcl_ui/edit_task_widget.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      701 2023-03-30 16:53:52.000000 busy-3.4.5/busy/ui/tcl_ui/get_item_widget.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5178 2023-04-10 09:34:40.000000 busy-3.4.5/busy/ui/ui.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.920284 busy-3.4.5/busy/util/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     6682 2023-04-10 09:34:40.000000 busy-3.4.5/busy/util/class_family.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2882 2023-04-10 09:34:40.000000 busy-3.4.5/busy/util/date_util.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      217 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/python_version.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      973 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/super_wrapper.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      131 2023-03-30 16:53:52.000000 busy-3.4.5/busy/util/textbox_util.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.894733 busy-3.4.5/busy.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)    21954 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     2195 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       43 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       82 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:43:27.000000 busy-3.4.5/busy.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      596 2023-04-10 09:34:40.000000 busy-3.4.5/pyproject.toml
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.925665 busy-3.4.5/sand/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-02-25 16:13:53.000000 busy-3.4.5/sand/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      336 2023-02-23 13:30:28.000000 busy-3.4.5/sand/_dataclass.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-05 00:41:16.000000 busy-3.4.5/sand/_readline_util.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      676 2023-02-25 17:04:15.000000 busy-3.4.5/sand/_textpad.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      233 2023-03-06 16:05:27.000000 busy-3.4.5/sand/chooser.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      282 2023-03-01 14:38:38.000000 busy-3.4.5/sand/rl-io.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-03-01 15:07:59.000000 busy-3.4.5/sand/subprocess.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      806 2023-03-02 16:10:26.000000 busy-3.4.5/sand/wrapper.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-10 09:43:27.945108 busy-3.4.5/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.926605 busy-3.4.5/test/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/__init__.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.929412 busy-3.4.5/test/data_class_family/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      101 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/atriarch.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       76 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/child.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-03-30 16:53:52.000000 busy-3.4.5/test/data_class_family/grandchild.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.930644 busy-3.4.5/test/handler/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/handler/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1205 2023-03-30 16:53:52.000000 busy-3.4.5/test/handler/test_handler.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.931659 busy-3.4.5/test/integration/
+-rw-r--r--   0 francispotter   (501) staff       (20)      150 2023-04-10 09:34:40.000000 busy-3.4.5/test/integration/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      416 2023-04-10 09:34:40.000000 busy-3.4.5/test/integration/test_integration.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.935738 busy-3.4.5/test/model/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/model/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      433 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_item.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      845 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_item_io.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2857 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_queue.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      624 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_queue_replace.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1778 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_task.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     4056 2023-04-10 09:34:40.000000 busy-3.4.5/test/model/test_todo_queue.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.937569 busy-3.4.5/test/root/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-10 09:34:40.000000 busy-3.4.5/test/root/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1406 2023-04-10 09:34:40.000000 busy-3.4.5/test/root/test_file.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2547 2023-04-10 09:34:40.000000 busy-3.4.5/test/root/test_file_system_root.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.939223 busy-3.4.5/test/ui/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/ui/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      357 2023-03-30 16:53:52.000000 busy-3.4.5/test/ui/test_shell_ui.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      790 2023-03-30 16:53:52.000000 busy-3.4.5/test/ui/test_ui_terminal_editor.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:43:27.943266 busy-3.4.5/test/util/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      797 2023-04-10 09:34:40.000000 busy-3.4.5/test/util/test_class_families.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      237 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/test_class_family.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      452 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/test_date.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      508 2023-03-30 16:53:52.000000 busy-3.4.5/test/util/test_python_version.py
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:36:08.000000 busy-3.4.5/version
```

### Comparing `busy-3.4.4/LICENSE` & `busy-3.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/PKG-INFO` & `busy-3.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 3.4.4
+Version: 3.4.5
 Summary: Personal time management system
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -55,15 +55,15 @@
 
 If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Linux). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
 
 Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
 
 From now on, we're going to use `python3` and `pip3` in code snippets, although your system might prefer simply `python` or `pip`. Just edit them.
 
-_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses` to install curses.
+_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses pyreadline3` to install the things that don't come out of the box with Python on Windows.
 
 _Python developers only_ Busy does require other packages, so feel free to use a venv.
 
 Here's the command to install the latest stable version of Busy itself:
 
 ```
 sudo pip3 install busy && pip3 show busy
@@ -91,18 +91,18 @@
 
 Using the Shell UI
 ------------------
 
 To get started, add some Tasks to your default Queue.
 
 ```
-busy add "Take a shower"
-busy add "Do the laundry"
-busy add "Phone mom"
-busy add "Donate to the Busy project"
+busy add --description "Take a shower"
+busy add --description "Do the laundry"
+busy add --description "Phone mom"
+busy add --description "Donate to the Busy project"
 ```
 
 Then, when you're ready to start your day, ask Busy what to do first:
 
 ```
 busy top
 ```
```

### Comparing `busy-3.4.4/README.md` & `busy-3.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Linux). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
 
 Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
 
 From now on, we're going to use `python3` and `pip3` in code snippets, although your system might prefer simply `python` or `pip`. Just edit them.
 
-_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses` to install curses.
+_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses pyreadline3` to install the things that don't come out of the box with Python on Windows.
 
 _Python developers only_ Busy does require other packages, so feel free to use a venv.
 
 Here's the command to install the latest stable version of Busy itself:
 
 ```
 sudo pip3 install busy && pip3 show busy
@@ -81,18 +81,18 @@
 
 Using the Shell UI
 ------------------
 
 To get started, add some Tasks to your default Queue.
 
 ```
-busy add "Take a shower"
-busy add "Do the laundry"
-busy add "Phone mom"
-busy add "Donate to the Busy project"
+busy add --description "Take a shower"
+busy add --description "Do the laundry"
+busy add --description "Phone mom"
+busy add --description "Donate to the Busy project"
 ```
 
 Then, when you're ready to start your day, ask Busy what to do first:
 
 ```
 busy top
 ```
```

### Comparing `busy-3.4.4/busy/command/activate_command.py` & `busy-3.4.5/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/add_command.py` & `busy-3.4.5/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/command.py` & `busy-3.4.5/busy/command/command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/defer_command.py` & `busy-3.4.5/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/delete_command.py` & `busy-3.4.5/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/drop_and_pop_command.py` & `busy-3.4.5/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/edit_command.py` & `busy-3.4.5/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/finish_command.py` & `busy-3.4.5/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/list_command.py` & `busy-3.4.5/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/command/switch_command.py` & `busy-3.4.5/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/handler.py` & `busy-3.4.5/busy/handler.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/model/item.py` & `busy-3.4.5/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/model/task.py` & `busy-3.4.5/busy/model/task.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/queue/queue.py` & `busy-3.4.5/busy/queue/queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/queue/todo_queue.py` & `busy-3.4.5/busy/queue/todo_queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/root/file_system_root.py` & `busy-3.4.5/busy/root/file_system_root.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/selector.py` & `busy-3.4.5/busy/selector.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/ui/curses_ui.py` & `busy-3.4.5/busy/ui/curses_ui.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/ui/shell_ui.py` & `busy-3.4.5/busy/ui/shell_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 #
 # The code for argparse lives at https://github.com/python/cpython/blob/main/Lib/argparse.py
 
 
 from argparse import ArgumentParser
 from io import StringIO
 
+from wizlib.rlinput import rlinput
+
 from busy.ui.ui import TerminalUI
-from busy.util.readline_util import rlinput
 from busy.ui.ui import UserCancelError
 from busy.ui.ui import Prompt
 
 
 class ShellUI(TerminalUI):
 
     name = "shell"
@@ -21,19 +22,19 @@
     def output(self, intro=""):
         """Print some regular output"""
         if intro:
             print(intro)
 
     def get_string(self, intro, default=""):
         prompt = Prompt(intro=intro)
-        return rlinput(intro=self._prompt_string(prompt), default=default)
+        return rlinput(prompt=self._prompt_string(prompt), default=default)
 
     def get_option(self, chooser):
         """Get a choice from the user"""
-        key = rlinput(intro=self._prompt_string(chooser))
+        key = rlinput(prompt=self._prompt_string(chooser))
         return chooser.choice_by_key(key)
     
     def _prompt_string(self, prompt):
         result = ""
         if prompt.intro:
             result += prompt.intro + " "
         if prompt.default:
```

### Comparing `busy-3.4.4/busy/ui/tcl_ui/edit_task_widget.py` & `busy-3.4.5/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/ui/tcl_ui/get_item_widget.py` & `busy-3.4.5/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/ui/ui.py` & `busy-3.4.5/busy/ui/ui.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/util/class_family.py` & `busy-3.4.5/busy/util/class_family.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/util/date_util.py` & `busy-3.4.5/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy/util/super_wrapper.py` & `busy-3.4.5/busy/util/super_wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/busy.egg-info/PKG-INFO` & `busy-3.4.5/busy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 3.4.4
+Version: 3.4.5
 Summary: Personal time management system
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -55,15 +55,15 @@
 
 If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Linux). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
 
 Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
 
 From now on, we're going to use `python3` and `pip3` in code snippets, although your system might prefer simply `python` or `pip`. Just edit them.
 
-_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses` to install curses.
+_Windows only_ Install Python from the Microsoft store, but then use `pip install windows-curses pyreadline3` to install the things that don't come out of the box with Python on Windows.
 
 _Python developers only_ Busy does require other packages, so feel free to use a venv.
 
 Here's the command to install the latest stable version of Busy itself:
 
 ```
 sudo pip3 install busy && pip3 show busy
@@ -91,18 +91,18 @@
 
 Using the Shell UI
 ------------------
 
 To get started, add some Tasks to your default Queue.
 
 ```
-busy add "Take a shower"
-busy add "Do the laundry"
-busy add "Phone mom"
-busy add "Donate to the Busy project"
+busy add --description "Take a shower"
+busy add --description "Do the laundry"
+busy add --description "Phone mom"
+busy add --description "Donate to the Busy project"
 ```
 
 Then, when you're ready to start your day, ask Busy what to do first:
 
 ```
 busy top
 ```
```

### Comparing `busy-3.4.4/busy.egg-info/SOURCES.txt` & `busy-3.4.5/busy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 busy/ui/tcl_ui/__init__.py
 busy/ui/tcl_ui/edit_task_widget.py
 busy/ui/tcl_ui/get_item_widget.py
 busy/util/__init__.py
 busy/util/class_family.py
 busy/util/date_util.py
 busy/util/python_version.py
-busy/util/readline_util.py
 busy/util/super_wrapper.py
 busy/util/textbox_util.py
 sand/__init__.py
 sand/_dataclass.py
 sand/_readline_util.py
 sand/_textpad.py
 sand/chooser.py
```

### Comparing `busy-3.4.4/pyproject.toml` & `busy-3.4.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     {name = "Francis Potter", email = "busy@steampunkwizard.ca"}
 ]
 description = "Personal time management system"
 readme = "README.md"
 requires-python = ">=3.6.5"
 license = {text = "MIT"}
 dependencies = [
-    "platformdirs >=3.2.0"
+    "platformdirs >=3.2.0",
+    "wizlib >=0.2.2",
+    "windows-curses; platform_system=='Windows'"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.package-dir]
 busy = "busy"
 
 [project.scripts]
```

### Comparing `busy-3.4.4/sand/_textpad.py` & `busy-3.4.5/sand/_textpad.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/sand/subprocess.py` & `busy-3.4.5/sand/subprocess.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/sand/wrapper.py` & `busy-3.4.5/sand/wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/handler/test_handler.py` & `busy-3.4.5/test/handler/test_handler.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/model/test_item_io.py` & `busy-3.4.5/test/model/test_item_io.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/model/test_queue.py` & `busy-3.4.5/test/model/test_queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/model/test_queue_replace.py` & `busy-3.4.5/test/model/test_queue_replace.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/model/test_task.py` & `busy-3.4.5/test/model/test_task.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/model/test_todo_queue.py` & `busy-3.4.5/test/model/test_todo_queue.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/root/test_file.py` & `busy-3.4.5/test/root/test_file.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/root/test_file_system_root.py` & `busy-3.4.5/test/root/test_file_system_root.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,23 @@
             with mock.patch.dict('os.environ', {'BUSY_ROOT': td}):
                 sd1 = FileSystemRoot()
                 sd1.get_queue('p').add('a')
                 sd1.save()
                 f = Path(td) / 'p.txt'
                 self.assertEqual(f.read_text(), 'a\n')
 
-    def test_user_root(self):
-        with TemporaryDirectory() as td:
-            with mock.patch.dict('os.environ', clear=True):
-                with mock.patch('pathlib.Path.home', lambda: Path(td)):
-                    sd1 = FileSystemRoot()
-                    sd1.get_queue('w').add('a')
-                    sd1.save()
-                    f = Path(td) / '.busy' / 'w.txt'
-                    self.assertEqual(f.read_text(), 'a\n')
+    # def test_user_root(self):
+    #     with TemporaryDirectory() as td:
+    #         with mock.patch.dict('os.environ', clear=True):
+    #             with mock.patch('pathlib.Path.home', lambda: Path(td)):
+    #                 sd1 = FileSystemRoot()
+    #                 sd1.get_queue('w').add('a')
+    #                 sd1.save()
+    #                 f = Path(td) / '.busy' / 'w.txt'
+    #                 self.assertEqual(f.read_text(), 'a\n')
 
     def test_list_queues(self):
         with TemporaryDirectory() as td:
             r = FileSystemRoot(Path(td))
             q1 = r.get_queue('a')
             q1.add('a')
             q2 = r.get_queue('b')
```

### Comparing `busy-3.4.4/test/ui/test_ui_terminal_editor.py` & `busy-3.4.5/test/ui/test_ui_terminal_editor.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.4/test/util/test_class_families.py` & `busy-3.4.5/test/util/test_class_families.py`

 * *Files identical despite different names*

