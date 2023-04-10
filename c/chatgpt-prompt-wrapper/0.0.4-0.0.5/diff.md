# Comparing `tmp/chatgpt_prompt_wrapper-0.0.4.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.4.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.5.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.4.tar` & `chatgpt_prompt_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,20 @@
--rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.4/LICENSE
--rw-r--r--   0        0        0     8020 2023-04-09 15:52:54.237309 chatgpt_prompt_wrapper-0.0.4/README.md
--rw-r--r--   0        0        0     2668 2023-04-09 15:53:09.174448 chatgpt_prompt_wrapper-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     3422 2023-04-09 15:40:50.061149 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
--rw-r--r--   0        0        0      426 2023-04-09 15:40:56.568943 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      349 2023-04-09 10:56:55.641263 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4076 2023-04-09 15:40:56.570213 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/ask.cpython-311.pyc
--rw-r--r--   0        0        0     2228 2023-04-09 15:36:48.300461 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/ask.cpython-39.pyc
--rw-r--r--   0        0        0     5976 2023-04-09 15:44:36.384736 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/chat.cpython-39.pyc
--rw-r--r--   0        0        0     9910 2023-04-09 15:40:56.572114 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/chatgpt.cpython-311.pyc
--rw-r--r--   0        0        0     6628 2023-04-09 15:44:36.278719 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/chatgpt.cpython-39.pyc
--rw-r--r--   0        0        0     2414 2023-04-09 15:31:06.479272 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/ask.py
--rw-r--r--   0        0        0     6370 2023-04-09 15:44:22.102233 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chat.py
--rw-r--r--   0        0        0     7504 2023-04-09 15:43:30.852390 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
--rw-r--r--   0        0        0     5324 2023-04-09 15:56:41.373142 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__init__.py
--rw-r--r--   0        0        0      374 2023-04-08 12:08:10.316082 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      303 2023-04-09 08:16:02.965964 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1644 2023-04-08 12:08:30.203863 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/commands.cpython-311.pyc
--rw-r--r--   0        0        0     1058 2023-04-09 15:44:36.414978 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/commands.cpython-39.pyc
--rw-r--r--   0        0        0     1217 2023-04-08 12:08:30.204184 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/cost.cpython-311.pyc
--rw-r--r--   0        0        0      642 2023-04-09 08:16:02.966921 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/cost.cpython-39.pyc
--rw-r--r--   0        0        0     1199 2023-04-08 12:08:30.202279 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/init.cpython-311.pyc
--rw-r--r--   0        0        0      688 2023-04-08 12:10:44.880831 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/commands.py
--rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/cost.py
--rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/init.py
--rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0     1490 2023-04-09 08:44:22.264024 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/docstring.py
--rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.5/LICENSE
+-rw-r--r--   0        0        0    11271 2023-04-10 09:44:31.488624 chatgpt_prompt_wrapper-0.0.5/README.md
+-rw-r--r--   0        0        0     2668 2023-04-10 09:45:29.939535 chatgpt_prompt_wrapper-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3626 2023-04-10 09:32:15.650242 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0     2414 2023-04-10 09:24:23.945045 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     6614 2023-04-10 09:44:24.879992 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7504 2023-04-10 09:25:04.924259 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     5525 2023-04-10 09:44:24.883171 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-10 01:24:32.721402 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0    12625 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.5/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.4/LICENSE` & `chatgpt_prompt_wrapper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.4/README.md` & `chatgpt_prompt_wrapper-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -14,44 +14,45 @@
 
 ```
 $ pip install chatgpt-prompt-wrapper
 ```
 
 ## Usage
 
-### Command line interface
+### Command line interface Help
 
 ```
 $ cg help
-usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT]
-          [--show] [--hide] [--multiline] [--no_multiline] [--show_cost]
+usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT] [--show] [--hide] [--multiline]
+          [--no_multiline] [--vi] [--emacs] [--show_cost]
           subcommand [message ...]
 
 positional arguments:
   subcommand            Subcommand to run. Use 'commands' subcommand to list up available subcommands.
   message               Message to send to ChatGPT
 
 optional arguments:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     OpenAI API key.
   -c CONF, --conf CONF  Path to the configuration toml file.
   -m MODEL, --model MODEL
                         ChatGPT Model to use.
   -t MAX_TOKENS, --max_tokens MAX_TOKENS
-                        The maximum number of tokens to generate in the chat completion. Set 0 to use
-                        the max values for the model minus prompt tokens.
+                        The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model
+                        minus prompt tokens.
   -T MIN_MAX_TOKENS, --min_max_tokens MIN_MAX_TOKENS
                         The minimum of max_tokens for the completion when max_tokens = 0.
   -l TOKENS_LIMIT, --tokens_limit TOKENS_LIMIT
-                        The limit of the total tokens of the prompt and the completion. Set 0 to use
-                        the max values for the model.
+                        The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model.
   --show                Show prompt for ask command.
   --hide                Hide prompt for ask command.
   --multiline           Use multiline input for chat command.
   --no_multiline        Use single line input for chat command.
+  --vi                  Use vi mode at chat.
+  --emacs               Use emacs mode at chat.
   --show_cost           Show cost used.
 ```
 
 ```
 $ cg commands
 Available subcommands:
   Reserved commands:
@@ -63,16 +64,40 @@
     version   : Show version.
     help      : Show help.
   User commands:
     test      : Example command to test the OpenAI API.
     ...
 ```
 
+### Ask, Chat
+
+`ask` and `chat` are reserved command to run simple interaction w/o predefined prompt.
+
+`cg ask <message>` will returns the answer from ChatGPT for `message`.
+
+`cg chat` starts a chat.
+
+:memo: In the `chat` mode, all messages in the past including answers from
+ChatGPT will be sent for each time when you send a new message.
+
+The oldest message will be dropped if the number of total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the limit of tokens (`tokens_limit` or the number of max tokens (-1) for the used model).
+
+It means you will send almost the max length after a long conversation.
+Please keep the cost in mind. You may want to set `tokens_limit`.
+
 ### Configuration file
 
+You can define your own subcommand in the configuration files.
+
+A subcommand can be `ask` mode or `chat` mode.
+
+- `ask` mode: Send a predefined prompt and a message from the command line and receive one answer.
+- `chat` mode: Start chat with a predefined prompt if defined.
+  - `chat` mode can be `multiline` mode or single (`no_multiline`) mode.
+
 #### File path
 
 The default path to the configuration file is **$XDG_CONFIG_HOME/cg/config.toml**.
 
 If **$XDG_CONFIG_HOME** is not defined, use **~/.config/cg/config.toml**.
 
 If it does not exist and **~/.cg/config.toml** exists,
@@ -106,14 +131,18 @@
 - `show`: Set `true` to show prompt for non chat command.
 - `hide`: Set `true` to hide prompt for non chat command (default).
 
 The options for chat mode:
 
 - `multiline`: Set `true` to hide prompt for non chat command (default).
 - `no_multiline`: Set `true` to hide prompt for non chat command.
+- `vi`: Set `true` to use vi mode.
+- `emacs`: Set `true` to use emacs mode (default).
+
+You can make a example configuration file by `cg init`.
 
 Here is a example configuration:
 
 ```toml
 [global]
 # Global configuration
 # `global` is special name and not a subcommand
@@ -177,14 +206,81 @@
 
 ![py command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_py.png)
 
 - enjoy_chat
 
 ![chat command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_chat.gif)
 
+## Example usage as a part of an external script
+
+### Git commit by ChatGPT
+
+Prepare the following script with name like `git-c`
+and put it in the directory under the PATH.
+
+```bash
+#!/usr/bin/env bash
+
+if ! type cg >/dev/null 2>&1; then
+  echo "cg command not found. Please install cg command."
+  echo "    $ pip install chatgpt-prompt-wrapper"
+  exit 1
+fi
+
+if [ "$1" = "-a" ];then
+  git add -u
+fi
+
+git hook run --ignore-missing pre-commit
+if [ $? -ne 0 ]; then
+  exit 1
+fi
+
+prompt="
+Please make git commit messages for the following diff output.
+
+Each commit message must be one line starting with one of the following words.
+
+* feat: (new feature for the user, not a new feature for build script)
+* fix: (bug fix for the user, not a fix to a build script)
+* docs: (changes to the documentation)
+* style: (formatting, missing semi colons, etc; no production code change)
+* refactor: (refactoring production code, eg. renaming a variable)
+* test: (adding missing tests, refactoring tests; no production code change)
+* chore: (updating grunt tasks etc; no production code change)
+
+
+### diff
+
+$(git diff --cached)
+"
+
+message="$(cg ask "$prompt")
+
+# feat: (new feature for the user, not a new feature for build script)
+# fix: (bug fix for the user, not a fix to a build script)
+# docs: (changes to the documentation)
+# style: (formatting, missing semi colons, etc; no production code change)
+# refactor: (refactoring production code, eg. renaming a variable)
+# test: (adding missing tests, refactoring tests; no production code change)
+# chore: (updating grunt tasks etc; no production code change)
+#
+# Ref: https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716
+"
+
+git commit --no-verify -e -m "$message"
+```
+
+Now you can use `git c` command.
+
+If any updates are staged, run `git c` and the git opens the editor for the commit
+with commit messages made by ChatGPT.
+
+`-a` option can be used as same as `git commit -a`
+
 ## Development
 
 ### Poetry
 
 Use [Poetry](https://python-poetry.org/) to setup environment.
 
 To install poetry, run:
```

### Comparing `chatgpt_prompt_wrapper-0.0.4/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
```

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import os
 import sys
 from argparse import ArgumentParser, Namespace
 
-non_chatgpt_params = [
-    "subcommand",
-    "message",
-    "conf",
-    "show",
-    "hide",
-    "multiline",
-    "no_multiline",
-    "show_cost",
+direct_chatgpt_params = [
+    "key",
+    "model",
+    "max_tokens",
+    "min_max_tokens",
+    "tokens_limit",
 ]
 
 
 def get_arg_parser() -> ArgumentParser:
     arg_parser = ArgumentParser()
     arg_parser.add_argument(
         "subcommand",
@@ -73,14 +70,24 @@
     )
     arg_parser.add_argument(
         "--no_multiline",
         help="Use single line input for chat command.",
         action="store_true",
     )
     arg_parser.add_argument(
+        "--vi",
+        help="Use vi mode at chat.",
+        action="store_true",
+    )
+    arg_parser.add_argument(
+        "--emacs",
+        help="Use emacs mode at chat.",
+        action="store_true",
+    )
+    arg_parser.add_argument(
         "--show_cost",
         help="Show cost used.",
         action="store_true",
     )
     return arg_parser
```

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/ask.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/ask.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chat.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,36 +16,40 @@
 class Chat(ChatGPT):
     """Chat class for interacting with OpenAI's API.
 
     Parameters
     ----------
     multiline : bool
         Whether to use multiline prompt.
+    vi: bool
+        If true, use the vi keybindings at input prompt (default is emacs key bindings).
     chat_exit_cmd: list[str]
         The command to exit the chat.
     """
 
     multiline: bool = True
+    vi: bool = False
     chat_exit_cmd: list[str] = field(
         default_factory=lambda: ["bye", "bye!", "exit", "quit"]
     )
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        self.make_propt()
+        self.make_prompt()
 
-    def make_propt(self) -> None:
+    def make_prompt(self) -> None:
         if self.multiline:
-            toolbar_view = HTML(
-                f"Send text: <b>[Meta+Enter]</b>, <b>[Esc]</b><b>[Enter]</b>. Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>"
-            )
+            toolbar_text = f"Send text: <b>[Meta+Enter]</b>, <b>[Esc]</b><b>[Enter]</b>. Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>, "
         else:
-            toolbar_view = HTML(
-                f"Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>"
-            )
+            f"Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>,"
+        if self.vi:
+            toolbar_text += "<b>Vi mode</b>."
+        else:
+            toolbar_text += "<b>emacs mode</b>."
+        toolbar_view = HTML(toolbar_text)
 
         def bottom_toolbar() -> HTML:
             return toolbar_view
 
         def prompt_continuation(
             width: int, line_number: int, is_soft_wrap: bool
         ) -> str:
@@ -66,14 +70,15 @@
 
         self.prompt_params = {
             "style": style,
             "multiline": self.multiline,
             "prompt_continuation": prompt_continuation,
             "bottom_toolbar": bottom_toolbar,
             "key_bindings": bindings,
+            "vi_mode": self.vi,
         }
 
     def set_no_line_break_log(self) -> None:
         self.default_terminators = [
             (h, h.terminator)
             for h in self.log.handlers
             if isinstance(h, logging.StreamHandler)
```

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 from argparse import Namespace
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 from .__version__ import __version__
-from .arg_parser import cli_help, non_chatgpt_params, parse_arg
+from .arg_parser import cli_help, direct_chatgpt_params, parse_arg
 from .chatgpt import Ask, Chat, Messages
 from .chatgpt_prompt_wrapper_exception import ChatGPTPromptWrapperError
 from .cmd import commands, cost, init
 from .config import get_config
 from .log_formatter import get_logger
 
 try:
@@ -51,49 +51,53 @@
         config["multiline"] = not config["no_multiline"]
     if args.multiline:
         config["multiline"] = True
     elif args.no_multiline:
         config["multiline"] = False
 
 
+def set_config_vi(config: dict[str, Any], args: Namespace) -> None:
+    if "vi" in config:
+        pass
+    elif "emacs" in config:
+        config["vi"] = not config["emacs"]
+    if args.vi:
+        config["vi"] = True
+    elif args.emacs:
+        config["vi"] = False
+
+
 def get_show_cost(config: dict[str, Any], args: Namespace) -> bool:
     show_cost = False
     show_cost = config["show_cost"] if "show_cost" in config else False
     if args.show_cost:
         show_cost = True
     return show_cost
 
 
 def check_args(
     config: dict[str, Any], args: Namespace
 ) -> tuple[dict[str, Any], Messages, bool, bool]:
     set_config_messages(config, args)
     set_config_show(config, args)
     set_config_multiline(config, args)
+    set_config_vi(config, args)
     show_cost = get_show_cost(config, args)
     chat = config["chat"] if "chat" in config else False
 
     for arg in vars(args):
-        if arg in non_chatgpt_params:
+        if arg not in direct_chatgpt_params:
             continue
         if (param := getattr(args, arg)) is not None:
             config[arg] = param
 
     chatgpt_params = {
         k: v
         for k, v in config.items()
-        if k
-        not in [
-            "messages",
-            "description",
-            "hide",
-            "chat",
-            "no_multi",
-            "show_cost",
-        ]
+        if k in direct_chatgpt_params + ["show", "multiline", "vi"]
     }
     if not chat and not config["messages"]:
         raise ChatGPTPromptWrapperError(
             "This subcommand (ask mode) does not predefined prompt and need input message."
         )
     return chatgpt_params, config["messages"], chat, show_cost
```

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/commands.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/config.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/docstring.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/docstring.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.5/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.4/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -48,44 +48,45 @@
 
 ```
 $ pip install chatgpt-prompt-wrapper
 ```
 
 ## Usage
 
-### Command line interface
+### Command line interface Help
 
 ```
 $ cg help
-usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT]
-          [--show] [--hide] [--multiline] [--no_multiline] [--show_cost]
+usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT] [--show] [--hide] [--multiline]
+          [--no_multiline] [--vi] [--emacs] [--show_cost]
           subcommand [message ...]
 
 positional arguments:
   subcommand            Subcommand to run. Use 'commands' subcommand to list up available subcommands.
   message               Message to send to ChatGPT
 
 optional arguments:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     OpenAI API key.
   -c CONF, --conf CONF  Path to the configuration toml file.
   -m MODEL, --model MODEL
                         ChatGPT Model to use.
   -t MAX_TOKENS, --max_tokens MAX_TOKENS
-                        The maximum number of tokens to generate in the chat completion. Set 0 to use
-                        the max values for the model minus prompt tokens.
+                        The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model
+                        minus prompt tokens.
   -T MIN_MAX_TOKENS, --min_max_tokens MIN_MAX_TOKENS
                         The minimum of max_tokens for the completion when max_tokens = 0.
   -l TOKENS_LIMIT, --tokens_limit TOKENS_LIMIT
-                        The limit of the total tokens of the prompt and the completion. Set 0 to use
-                        the max values for the model.
+                        The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model.
   --show                Show prompt for ask command.
   --hide                Hide prompt for ask command.
   --multiline           Use multiline input for chat command.
   --no_multiline        Use single line input for chat command.
+  --vi                  Use vi mode at chat.
+  --emacs               Use emacs mode at chat.
   --show_cost           Show cost used.
 ```
 
 ```
 $ cg commands
 Available subcommands:
   Reserved commands:
@@ -97,16 +98,40 @@
     version   : Show version.
     help      : Show help.
   User commands:
     test      : Example command to test the OpenAI API.
     ...
 ```
 
+### Ask, Chat
+
+`ask` and `chat` are reserved command to run simple interaction w/o predefined prompt.
+
+`cg ask <message>` will returns the answer from ChatGPT for `message`.
+
+`cg chat` starts a chat.
+
+:memo: In the `chat` mode, all messages in the past including answers from
+ChatGPT will be sent for each time when you send a new message.
+
+The oldest message will be dropped if the number of total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the limit of tokens (`tokens_limit` or the number of max tokens (-1) for the used model).
+
+It means you will send almost the max length after a long conversation.
+Please keep the cost in mind. You may want to set `tokens_limit`.
+
 ### Configuration file
 
+You can define your own subcommand in the configuration files.
+
+A subcommand can be `ask` mode or `chat` mode.
+
+- `ask` mode: Send a predefined prompt and a message from the command line and receive one answer.
+- `chat` mode: Start chat with a predefined prompt if defined.
+  - `chat` mode can be `multiline` mode or single (`no_multiline`) mode.
+
 #### File path
 
 The default path to the configuration file is **$XDG_CONFIG_HOME/cg/config.toml**.
 
 If **$XDG_CONFIG_HOME** is not defined, use **~/.config/cg/config.toml**.
 
 If it does not exist and **~/.cg/config.toml** exists,
@@ -140,14 +165,18 @@
 - `show`: Set `true` to show prompt for non chat command.
 - `hide`: Set `true` to hide prompt for non chat command (default).
 
 The options for chat mode:
 
 - `multiline`: Set `true` to hide prompt for non chat command (default).
 - `no_multiline`: Set `true` to hide prompt for non chat command.
+- `vi`: Set `true` to use vi mode.
+- `emacs`: Set `true` to use emacs mode (default).
+
+You can make a example configuration file by `cg init`.
 
 Here is a example configuration:
 
 ```toml
 [global]
 # Global configuration
 # `global` is special name and not a subcommand
@@ -211,14 +240,81 @@
 
 ![py command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_py.png)
 
 - enjoy_chat
 
 ![chat command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_chat.gif)
 
+## Example usage as a part of an external script
+
+### Git commit by ChatGPT
+
+Prepare the following script with name like `git-c`
+and put it in the directory under the PATH.
+
+```bash
+#!/usr/bin/env bash
+
+if ! type cg >/dev/null 2>&1; then
+  echo "cg command not found. Please install cg command."
+  echo "    $ pip install chatgpt-prompt-wrapper"
+  exit 1
+fi
+
+if [ "$1" = "-a" ];then
+  git add -u
+fi
+
+git hook run --ignore-missing pre-commit
+if [ $? -ne 0 ]; then
+  exit 1
+fi
+
+prompt="
+Please make git commit messages for the following diff output.
+
+Each commit message must be one line starting with one of the following words.
+
+* feat: (new feature for the user, not a new feature for build script)
+* fix: (bug fix for the user, not a fix to a build script)
+* docs: (changes to the documentation)
+* style: (formatting, missing semi colons, etc; no production code change)
+* refactor: (refactoring production code, eg. renaming a variable)
+* test: (adding missing tests, refactoring tests; no production code change)
+* chore: (updating grunt tasks etc; no production code change)
+
+
+### diff
+
+$(git diff --cached)
+"
+
+message="$(cg ask "$prompt")
+
+# feat: (new feature for the user, not a new feature for build script)
+# fix: (bug fix for the user, not a fix to a build script)
+# docs: (changes to the documentation)
+# style: (formatting, missing semi colons, etc; no production code change)
+# refactor: (refactoring production code, eg. renaming a variable)
+# test: (adding missing tests, refactoring tests; no production code change)
+# chore: (updating grunt tasks etc; no production code change)
+#
+# Ref: https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716
+"
+
+git commit --no-verify -e -m "$message"
+```
+
+Now you can use `git c` command.
+
+If any updates are staged, run `git c` and the git opens the editor for the commit
+with commit messages made by ChatGPT.
+
+`-a` option can be used as same as `git commit -a`
+
 ## Development
 
 ### Poetry
 
 Use [Poetry](https://python-poetry.org/) to setup environment.
 
 To install poetry, run:
```

