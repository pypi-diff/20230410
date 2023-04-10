# Comparing `tmp/chatgpt_prompt_wrapper-0.0.5.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.5.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.6.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.5.tar` & `chatgpt_prompt_wrapper-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.5/LICENSE
--rw-r--r--   0        0        0    11271 2023-04-10 09:44:31.488624 chatgpt_prompt_wrapper-0.0.5/README.md
--rw-r--r--   0        0        0     2668 2023-04-10 09:45:29.939535 chatgpt_prompt_wrapper-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     3626 2023-04-10 09:32:15.650242 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
--rw-r--r--   0        0        0     2414 2023-04-10 09:24:23.945045 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/ask.py
--rw-r--r--   0        0        0     6614 2023-04-10 09:44:24.879992 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chat.py
--rw-r--r--   0        0        0     7504 2023-04-10 09:25:04.924259 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
--rw-r--r--   0        0        0     5525 2023-04-10 09:44:24.883171 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/__init__.py
--rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/commands.py
--rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/cost.py
--rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/init.py
--rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0     1490 2023-04-10 01:24:32.721402 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/docstring.py
--rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0    12625 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.6/LICENSE
+-rw-r--r--   0        0        0    11271 2023-04-10 09:44:31.488624 chatgpt_prompt_wrapper-0.0.6/README.md
+-rw-r--r--   0        0        0     2668 2023-04-10 10:54:07.855262 chatgpt_prompt_wrapper-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3626 2023-04-10 09:32:15.650242 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0     2414 2023-04-10 09:24:23.945045 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     6661 2023-04-10 10:52:50.078843 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7504 2023-04-10 09:25:04.924259 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     5525 2023-04-10 09:44:24.883171 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-10 01:24:32.721402 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0    12625 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.6/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.5/LICENSE` & `chatgpt_prompt_wrapper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/README.md` & `chatgpt_prompt_wrapper-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
```

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/ask.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/ask.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chat.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
         super().__post_init__()
         self.make_prompt()
 
     def make_prompt(self) -> None:
         if self.multiline:
             toolbar_text = f"Send text: <b>[Meta+Enter]</b>, <b>[Esc]</b><b>[Enter]</b>. Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>, "
         else:
-            f"Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>,"
+            toolbar_text = (
+                f"Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>,"
+            )
         if self.vi:
             toolbar_text += "<b>Vi mode</b>."
         else:
             toolbar_text += "<b>emacs mode</b>."
         toolbar_view = HTML(toolbar_text)
 
         def bottom_toolbar() -> HTML:
```

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/commands.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/config.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/docstring.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/docstring.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.5/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
```

