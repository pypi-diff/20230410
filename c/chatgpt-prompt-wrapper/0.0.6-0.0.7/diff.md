# Comparing `tmp/chatgpt_prompt_wrapper-0.0.6.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.6.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.7.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.6.tar` & `chatgpt_prompt_wrapper-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.6/LICENSE
--rw-r--r--   0        0        0    11271 2023-04-10 09:44:31.488624 chatgpt_prompt_wrapper-0.0.6/README.md
--rw-r--r--   0        0        0     2668 2023-04-10 10:54:07.855262 chatgpt_prompt_wrapper-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     3626 2023-04-10 09:32:15.650242 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
--rw-r--r--   0        0        0     2414 2023-04-10 09:24:23.945045 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/ask.py
--rw-r--r--   0        0        0     6661 2023-04-10 10:52:50.078843 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chat.py
--rw-r--r--   0        0        0     7504 2023-04-10 09:25:04.924259 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
--rw-r--r--   0        0        0     5525 2023-04-10 09:44:24.883171 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/__init__.py
--rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/commands.py
--rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/cost.py
--rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/init.py
--rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0     1490 2023-04-10 01:24:32.721402 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/docstring.py
--rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0    12625 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-10 15:06:55.587443 chatgpt_prompt_wrapper-0.0.7/LICENSE
+-rw-r--r--   0        0        0    11848 2023-04-10 15:38:31.427438 chatgpt_prompt_wrapper-0.0.7/README.md
+-rw-r--r--   0        0        0     2668 2023-04-10 15:41:05.027434 chatgpt_prompt_wrapper-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3638 2023-04-10 15:32:05.457427 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      133 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0     2414 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     6661 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7504 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     5836 2023-04-10 15:15:17.007437 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1410 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0    13202 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.7/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.6/LICENSE` & `chatgpt_prompt_wrapper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/README.md` & `chatgpt_prompt_wrapper-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 # chatgpt-prompt-wrapper
 
 [![test](https://github.com/rcmdnk/chatgpt-prompt-wrapper/actions/workflows/test.yml/badge.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/actions/workflows/test.yml)
 [![test coverage](https://img.shields.io/badge/coverage-check%20here-blue.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/tree/coverage)
 
 Python CLI implementation for [ChatGPT](https://openai.com/blog/chatgpt).
 
-## Requirement
+## Requirements
 
 - Python 3.9, 3.10, 3.11
 - Poetry (For development)
 
 ## Installation
 
 ```
 $ pip install chatgpt-prompt-wrapper
 ```
 
+## Preparation
+
+To get an OpenAI API key, go to [Account API Keys - OpenAI API](https://platform.openai.com/account/api-keys).
+
+Set it as the environment variable `OPENAI_API_KEY`.
+
+To load the variable when you start the terminal, write it in **.bashrc** or **.zshrc**.
+
+```
+export OPENAI_API_KEY="sk-..."
+```
+
+Alternatively, pass the key using the '-k' or '--key' argument in the command.
+
 ## Usage
 
-### Command line interface Help
+### Command-line interface Help
 
 ```
 $ cg help
 usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT] [--show] [--hide] [--multiline]
           [--no_multiline] [--vi] [--emacs] [--show_cost]
           subcommand [message ...]
 
@@ -66,66 +80,69 @@
   User commands:
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Ask, Chat
 
-`ask` and `chat` are reserved command to run simple interaction w/o predefined prompt.
+`ask` and `chat` are reserved commands for running simple interaction without a predefined prompt.
 
-`cg ask <message>` will returns the answer from ChatGPT for `message`.
+`cg ask <message>` returns the answer from ChatGPT for `message`.
 
 `cg chat` starts a chat.
 
-:memo: In the `chat` mode, all messages in the past including answers from
-ChatGPT will be sent for each time when you send a new message.
+:memo: In `chat` mode, all messages in the past, including answers from
+ChatGPT, will be sent each time you send a new message.
 
-The oldest message will be dropped if the number of total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the limit of tokens (`tokens_limit` or the number of max tokens (-1) for the used model).
+The oldest message will be dropped when the total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the tokens limit (`tokens_limit` or the number of max tokens (-1) for the used model).
 
 It means you will send almost the max length after a long conversation.
 Please keep the cost in mind. You may want to set `tokens_limit`.
 
 ### Configuration file
 
-You can define your own subcommand in the configuration files.
+You can define your command in the configuration files.
 
-A subcommand can be `ask` mode or `chat` mode.
+A command can be in either `ask` mode or `chat` mode.
 
 - `ask` mode: Send a predefined prompt and a message from the command line and receive one answer.
-- `chat` mode: Start chat with a predefined prompt if defined.
-  - `chat` mode can be `multiline` mode or single (`no_multiline`) mode.
+- `chat` mode: Start a chat with a predefined prompt if defined:
+  - `chat` mode can be in either `multiline` mode or single (`no_multiline`) mode.
 
 #### File path
 
 The default path to the configuration file is **$XDG_CONFIG_HOME/cg/config.toml**.
 
 If **$XDG_CONFIG_HOME** is not defined, use **~/.config/cg/config.toml**.
 
 If it does not exist and **~/.cg/config.toml** exists,
 the existing file is used.
 
 You can change the path by `-c <file>` (`--conf <file>`) option.
 
 #### How to write the configuration file
 
-The configuration file is written in the TOML format.
+The configuration file is written in the [TOML format](https://toml.io/en/).
+
+You can define a command as the top table name.
 
-Subcommand is defined as the top table name.
+`global` is the special table to define global options,
+which are enabled for all commands if the command does not have the corresponding options.
 
 The options for each table can be:
 
 - `description`: Description of the command.
-- `chat`: Set `true` to make the command chat mode (default is ask mode, only one exchange).
-- `show_cost`: Set `true` to show cost at the end of the command.
-- `model`: The model to use. (default: "gpt-3.5-turbo")
-- `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model. (default: 0)
-- `min_max_tokens`: The minimum of max_tokens for the completion when max_tokens = 0. (default: 200)
-- `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model. (default: 0)
+- `chat`: Set `true` to switch to `chat` mode (default is `ask` mode, only one exchange).
+- `show_cost`: Set `true` to show the cost at the end of the command.
+- `model`: The model to use (default: "gpt-3.5-turbo").
+- `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the maximum values for the model. (default: 0)
+- `min_max_tokens`: The minimum of `max_tokens` for the completion when `max_tokens = 0`. (default: 200)
+- `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the maximum values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
-- `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time. (default: 1)
+- `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p at the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
 The options for ask mode:
 
 - `show`: Set `true` to show prompt for non chat command.
```

### Comparing `chatgpt_prompt_wrapper-0.0.6/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
```

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "-k",
         "--key",
         help="OpenAI API key.",
         type=str,
         default=os.environ.get("OPENAI_API_KEY", ""),
     )
     arg_parser.add_argument(
-        "-c", "--conf", help="Path to the configuration toml file.", type=str
+        "-c", "--conf", help="Path to the configuration TOML file.", type=str
     )
     arg_parser.add_argument(
         "-m", "--model", help="ChatGPT Model to use.", type=str
     )
     arg_parser.add_argument(
         "-t",
         "--max_tokens",
@@ -51,40 +51,40 @@
         "-l",
         "--tokens_limit",
         help="The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model.",
         type=int,
     )
     arg_parser.add_argument(
         "--show",
-        help="Show prompt for ask command.",
+        help="Show prompt for `ask` command.",
         action="store_true",
     )
     arg_parser.add_argument(
         "--hide",
-        help="Hide prompt for ask command.",
+        help="Hide prompt for `ask` command.",
         action="store_true",
     )
     arg_parser.add_argument(
         "--multiline",
-        help="Use multiline input for chat command.",
+        help="Use multiline input for `chat` command.",
         action="store_true",
     )
     arg_parser.add_argument(
         "--no_multiline",
-        help="Use single line input for chat command.",
+        help="Use single line input for `chat` command.",
         action="store_true",
     )
     arg_parser.add_argument(
         "--vi",
-        help="Use vi mode at chat.",
+        help="Use vi mode at `chat`.",
         action="store_true",
     )
     arg_parser.add_argument(
         "--emacs",
-        help="Use emacs mode at chat.",
+        help="Use emacs mode at `chat`.",
         action="store_true",
     )
     arg_parser.add_argument(
         "--show_cost",
         help="Show cost used.",
         action="store_true",
     )
```

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/ask.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/ask.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chat.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         log.info(f"\nEstimated cost: ${new_cost:.6f}")
     cost_data = {}
     if cost_file.exists():
         with open(cost_file, "r") as f:
             cost_data = {k: v for k, v in sorted(json.load(f).items())}
     month = datetime.now().strftime("%Y%m")
     cost_data[month] = cost_data.get(month, 0) + new_cost
+    cost_file.parent.mkdir(parents=True, exist_ok=True)
     with open(cost_file, "w") as f:
         json.dump(cost_data, f)
 
 
 def run_chatgpt(
     messages: Messages, params: dict[str, Any], chat: bool
 ) -> float:
@@ -153,21 +154,26 @@
         return
 
     if not args.key:
         raise ChatGPTPromptWrapperError(
             "Set OPEN_AI_API_KEY environment variable or give it by -k (--key) argument."
         )
 
-    if not config_file.is_file():
+    if cmd not in ['ask', 'chat'] and not config_file.is_file():
         raise ChatGPTPromptWrapperError(
-            f"Config file {config_file} does not exist"
+            f"Configuration file {config_file} does not exist"
+            f"`ask` or `cht` subcommand can be used w/o configuration file."
+            f"You prepare the configuration file by `cg init` command."
         )
 
-    with open(config_file, "rb") as f:
-        config = tomllib.load(f)
+    if config_file.is_file():
+        with open(config_file, "rb") as f:
+            config = tomllib.load(f)
+    else:
+        config = {}
 
     if cmd == "commands":
         commands(config, log)
         return
 
     cmds = ["ask", "chat"] + list(config)
     if cmd not in cmds or cmd == "global":
```

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/cmd/commands.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/config.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/docstring.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/docstring.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.6/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -35,28 +35,42 @@
 # chatgpt-prompt-wrapper
 
 [![test](https://github.com/rcmdnk/chatgpt-prompt-wrapper/actions/workflows/test.yml/badge.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/actions/workflows/test.yml)
 [![test coverage](https://img.shields.io/badge/coverage-check%20here-blue.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/tree/coverage)
 
 Python CLI implementation for [ChatGPT](https://openai.com/blog/chatgpt).
 
-## Requirement
+## Requirements
 
 - Python 3.9, 3.10, 3.11
 - Poetry (For development)
 
 ## Installation
 
 ```
 $ pip install chatgpt-prompt-wrapper
 ```
 
+## Preparation
+
+To get an OpenAI API key, go to [Account API Keys - OpenAI API](https://platform.openai.com/account/api-keys).
+
+Set it as the environment variable `OPENAI_API_KEY`.
+
+To load the variable when you start the terminal, write it in **.bashrc** or **.zshrc**.
+
+```
+export OPENAI_API_KEY="sk-..."
+```
+
+Alternatively, pass the key using the '-k' or '--key' argument in the command.
+
 ## Usage
 
-### Command line interface Help
+### Command-line interface Help
 
 ```
 $ cg help
 usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT] [--show] [--hide] [--multiline]
           [--no_multiline] [--vi] [--emacs] [--show_cost]
           subcommand [message ...]
 
@@ -100,66 +114,69 @@
   User commands:
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Ask, Chat
 
-`ask` and `chat` are reserved command to run simple interaction w/o predefined prompt.
+`ask` and `chat` are reserved commands for running simple interaction without a predefined prompt.
 
-`cg ask <message>` will returns the answer from ChatGPT for `message`.
+`cg ask <message>` returns the answer from ChatGPT for `message`.
 
 `cg chat` starts a chat.
 
-:memo: In the `chat` mode, all messages in the past including answers from
-ChatGPT will be sent for each time when you send a new message.
+:memo: In `chat` mode, all messages in the past, including answers from
+ChatGPT, will be sent each time you send a new message.
 
-The oldest message will be dropped if the number of total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the limit of tokens (`tokens_limit` or the number of max tokens (-1) for the used model).
+The oldest message will be dropped when the total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the tokens limit (`tokens_limit` or the number of max tokens (-1) for the used model).
 
 It means you will send almost the max length after a long conversation.
 Please keep the cost in mind. You may want to set `tokens_limit`.
 
 ### Configuration file
 
-You can define your own subcommand in the configuration files.
+You can define your command in the configuration files.
 
-A subcommand can be `ask` mode or `chat` mode.
+A command can be in either `ask` mode or `chat` mode.
 
 - `ask` mode: Send a predefined prompt and a message from the command line and receive one answer.
-- `chat` mode: Start chat with a predefined prompt if defined.
-  - `chat` mode can be `multiline` mode or single (`no_multiline`) mode.
+- `chat` mode: Start a chat with a predefined prompt if defined:
+  - `chat` mode can be in either `multiline` mode or single (`no_multiline`) mode.
 
 #### File path
 
 The default path to the configuration file is **$XDG_CONFIG_HOME/cg/config.toml**.
 
 If **$XDG_CONFIG_HOME** is not defined, use **~/.config/cg/config.toml**.
 
 If it does not exist and **~/.cg/config.toml** exists,
 the existing file is used.
 
 You can change the path by `-c <file>` (`--conf <file>`) option.
 
 #### How to write the configuration file
 
-The configuration file is written in the TOML format.
+The configuration file is written in the [TOML format](https://toml.io/en/).
+
+You can define a command as the top table name.
 
-Subcommand is defined as the top table name.
+`global` is the special table to define global options,
+which are enabled for all commands if the command does not have the corresponding options.
 
 The options for each table can be:
 
 - `description`: Description of the command.
-- `chat`: Set `true` to make the command chat mode (default is ask mode, only one exchange).
-- `show_cost`: Set `true` to show cost at the end of the command.
-- `model`: The model to use. (default: "gpt-3.5-turbo")
-- `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model. (default: 0)
-- `min_max_tokens`: The minimum of max_tokens for the completion when max_tokens = 0. (default: 200)
-- `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model. (default: 0)
+- `chat`: Set `true` to switch to `chat` mode (default is `ask` mode, only one exchange).
+- `show_cost`: Set `true` to show the cost at the end of the command.
+- `model`: The model to use (default: "gpt-3.5-turbo").
+- `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the maximum values for the model. (default: 0)
+- `min_max_tokens`: The minimum of `max_tokens` for the completion when `max_tokens = 0`. (default: 200)
+- `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the maximum values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
-- `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time. (default: 1)
+- `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p at the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
 The options for ask mode:
 
 - `show`: Set `true` to show prompt for non chat command.
```

