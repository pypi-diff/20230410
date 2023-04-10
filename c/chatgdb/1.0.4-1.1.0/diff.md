# Comparing `tmp/chatgdb-1.0.4.tar.gz` & `tmp/chatgdb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgdb-1.0.4.tar", max compression
+gzip compressed data, was "chatgdb-1.1.0.tar", max compression
```

## Comparing `chatgdb-1.0.4.tar` & `chatgdb-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-03-31 21:54:58.877640 chatgdb-1.0.4/LICENSE
--rw-r--r--   0        0        0     3364 2023-04-08 15:40:59.988687 chatgdb-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-01 22:30:13.298149 chatgdb-1.0.4/chatgdb/__init__.py
--rw-r--r--   0        0        0     1159 2023-04-09 00:04:17.999150 chatgdb-1.0.4/chatgdb/cli.py
--rw-r--r--   0        0        0     5325 2023-04-08 23:18:29.443556 chatgdb-1.0.4/chatgdb/core.py
--rw-r--r--   0        0        0      567 2023-04-09 00:05:26.683568 chatgdb-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 chatgdb-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-10 02:21:45.761529 chatgdb-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3614 2023-04-10 02:21:45.764862 chatgdb-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 01:32:55.050988 chatgdb-1.1.0/chatgdb/__init__.py
+-rw-r--r--   0        0        0     1159 2023-04-10 01:57:51.202881 chatgdb-1.1.0/chatgdb/cli.py
+-rw-r--r--   0        0        0     2068 2023-04-10 02:21:45.764862 chatgdb-1.1.0/chatgdb/gdb.py
+-rw-r--r--   0        0        0     1517 2023-04-10 02:21:45.764862 chatgdb-1.1.0/chatgdb/lldb.py
+-rw-r--r--   0        0        0     4049 2023-04-10 02:21:45.764862 chatgdb-1.1.0/chatgdb/utils.py
+-rw-r--r--   0        0        0      567 2023-04-10 02:21:45.764862 chatgdb-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 chatgdb-1.1.0/PKG-INFO
```

### Comparing `chatgdb-1.0.4/LICENSE` & `chatgdb-1.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 pgosar
+Copyright (c) 2023 Pranay Gosar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `chatgdb-1.0.4/README.md` & `chatgdb-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ChatGDB
-Harness the power of ChatGPT inside the GDB debugger!
+Harness the power of ChatGPT inside the GDB/LLDB debugger!
 
 
-ChatGDB is a tool designed to superpower your debugging experience with GDB, a debugger for compiled languages. Use it to accelerate your debugging workflow by leveraging the power of ChatGPT to assist you while using GDB! 
+ChatGDB is a tool designed to superpower your debugging experience with GDB or LLDB, debuggers for compiled languages. Use it to accelerate your debugging workflow by leveraging the power of ChatGPT to assist you while using GDB/LLDB! 
 
-It allows you to explain in natural language what you want to do, and then automatically execute the relevant command. Optionally, you can ask ChatGPT to explain the command it just ran or even pass in any question for it to answer. Focus on what's important - figuring out that nasty bug instead of chasing down GDB commands at the tip of your tongue.
+It allows you to explain in natural language what you want to do, and then automatically execute the relevant command. Optionally, you can ask ChatGPT to explain the command it just ran or even pass in any question for it to answer. Focus on what's important - figuring out that nasty bug instead of chasing down GDB/LLDB commands at the tip of your tongue.
 
 ![Image](https://lh5.googleusercontent.com/xZMLwWWxavqYjC3fyCIZJ0m-s-f-XEoiOeWGbxRrw3dWoukUoWzJJ4iiBkVO2Vtiyr4K6o0WkTs7B40TapeBPIYwgVRVhDXGVjB4tFYoKH3_nK847nYXl3pISB6dEP6Wp_o0uPlfJOjCrLspm0_VNw)
 
 ## Contents
 
 1. [Installation](#installation-intructions)
 2. [Updating](#updating)
@@ -44,19 +44,23 @@
 
 To update ChatGDB, run the following
 
 ```pip3 install chatgdb --upgrade```
 
 
 ### Usage
-I first recommend editing your ```$HOME/.gdbinit``` to source the main script automatically on startup. Run the following command:
+For GDB usage, I first recommend editing your ```$HOME/.gdbinit``` to source the main script automatically on startup. Run the following command:
 
-```echo "source $(python -m site --user-site)/chatgdb/core.py" > $HOME/.gdbinit```
+```echo "source $(python -m site --user-site)/chatgdb/gdb.py" > $HOME/.gdbinit```
 
-While inside GDB the command chat appended by your query, for example ```chat list all breakpoints that I created```. 
+The same applies for LLDB. Edit your ```$HOME/.lldbinit``` and run the following command:
+
+```echo "command script import $(python -m site --user-site)/chatgdb/lldb.py" > $HOME/.lldbinit```
+
+While inside your debugger, you can run the command chat appended by your query, for example ```chat list all breakpoints that I created```. 
 There is also a command called ```explain``` that you can use with no arguments to explain the previously run command, 
 and optionally, with a query to just ask GPT a question. For example, running ```explain``` directly after running 
 ```break 7``` would prompt the tool to explain how breakpoints work. Running ```explain how input formatting works in gdb``` 
 would prompt it to explain input formatting (see the image at the top).
 
 Run chat help to print out a short tutorial on how to use the tool.
```

### Comparing `chatgdb-1.0.4/chatgdb/cli.py` & `chatgdb-1.1.0/chatgdb/cli.py`

 * *Files identical despite different names*

### Comparing `chatgdb-1.0.4/pyproject.toml` & `chatgdb-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ChatGDB"
-version = "1.0.4"
+version = "1.1.0"
 authors = ["Pranay Gosar <gosarpranay@gmail.com>"]
 description = "Harness the power of ChatGPT directly inside the GDB debugger!"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/pgosar/chatgdb"
 keywords = ["gdb", "debugger", "chatgpt"]
```

### Comparing `chatgdb-1.0.4/PKG-INFO` & `chatgdb-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgdb
-Version: 1.0.4
+Version: 1.1.0
 Summary: Harness the power of ChatGPT directly inside the GDB debugger!
 Home-page: https://github.com/pgosar/chatgdb
 License: MIT
 Keywords: gdb,debugger,chatgpt
 Author: Pranay Gosar
 Author-email: gosarpranay@gmail.com
 Requires-Python: >=3.3,<4.0
@@ -19,20 +19,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Bug Tracker, https://github.com/pgosar/chatgdb/issues
 Project-URL: Repository, https://github.com/pgosar/chatgdb
 Description-Content-Type: text/markdown
 
 # ChatGDB
-Harness the power of ChatGPT inside the GDB debugger!
+Harness the power of ChatGPT inside the GDB/LLDB debugger!
 
 
-ChatGDB is a tool designed to superpower your debugging experience with GDB, a debugger for compiled languages. Use it to accelerate your debugging workflow by leveraging the power of ChatGPT to assist you while using GDB! 
+ChatGDB is a tool designed to superpower your debugging experience with GDB or LLDB, debuggers for compiled languages. Use it to accelerate your debugging workflow by leveraging the power of ChatGPT to assist you while using GDB/LLDB! 
 
-It allows you to explain in natural language what you want to do, and then automatically execute the relevant command. Optionally, you can ask ChatGPT to explain the command it just ran or even pass in any question for it to answer. Focus on what's important - figuring out that nasty bug instead of chasing down GDB commands at the tip of your tongue.
+It allows you to explain in natural language what you want to do, and then automatically execute the relevant command. Optionally, you can ask ChatGPT to explain the command it just ran or even pass in any question for it to answer. Focus on what's important - figuring out that nasty bug instead of chasing down GDB/LLDB commands at the tip of your tongue.
 
 ![Image](https://lh5.googleusercontent.com/xZMLwWWxavqYjC3fyCIZJ0m-s-f-XEoiOeWGbxRrw3dWoukUoWzJJ4iiBkVO2Vtiyr4K6o0WkTs7B40TapeBPIYwgVRVhDXGVjB4tFYoKH3_nK847nYXl3pISB6dEP6Wp_o0uPlfJOjCrLspm0_VNw)
 
 ## Contents
 
 1. [Installation](#installation-intructions)
 2. [Updating](#updating)
@@ -68,19 +68,23 @@
 
 To update ChatGDB, run the following
 
 ```pip3 install chatgdb --upgrade```
 
 
 ### Usage
-I first recommend editing your ```$HOME/.gdbinit``` to source the main script automatically on startup. Run the following command:
+For GDB usage, I first recommend editing your ```$HOME/.gdbinit``` to source the main script automatically on startup. Run the following command:
 
-```echo "source $(python -m site --user-site)/chatgdb/core.py" > $HOME/.gdbinit```
+```echo "source $(python -m site --user-site)/chatgdb/gdb.py" > $HOME/.gdbinit```
 
-While inside GDB the command chat appended by your query, for example ```chat list all breakpoints that I created```. 
+The same applies for LLDB. Edit your ```$HOME/.lldbinit``` and run the following command:
+
+```echo "command script import $(python -m site --user-site)/chatgdb/lldb.py" > $HOME/.lldbinit```
+
+While inside your debugger, you can run the command chat appended by your query, for example ```chat list all breakpoints that I created```. 
 There is also a command called ```explain``` that you can use with no arguments to explain the previously run command, 
 and optionally, with a query to just ask GPT a question. For example, running ```explain``` directly after running 
 ```break 7``` would prompt the tool to explain how breakpoints work. Running ```explain how input formatting works in gdb``` 
 would prompt it to explain input formatting (see the image at the top).
 
 Run chat help to print out a short tutorial on how to use the tool.
```

