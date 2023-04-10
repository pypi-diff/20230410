# Comparing `tmp/chatgpt4-cli-1.4.7.tar.gz` & `tmp/chatgpt4-cli-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.4.7.tar", last modified: Sat Apr  8 13:19:37 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.4.8.tar", last modified: Mon Apr 10 11:02:18 2023, max compression
```

## Comparing `chatgpt4-cli-1.4.7.tar` & `chatgpt4-cli-1.4.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 13:19:37.521268 chatgpt4-cli-1.4.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 13:19:37.517935 chatgpt4-cli-1.4.7/GPTCLI/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-08 12:55:50.000000 chatgpt4-cli-1.4.7/GPTCLI/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.7/GPTCLI/__main__.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-04-08 11:50:58.000000 chatgpt4-cli-1.4.7/GPTCLI/addons.py
--rw-r--r--   0 root         (0) root         (0)     7281 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.7/GPTCLI/emage.py
--rwxr-xr-x   0 root         (0) root         (0)    27153 2023-04-08 13:04:13.000000 chatgpt4-cli-1.4.7/GPTCLI/gptcli.py
--rw-r--r--   0 root         (0) root         (0)     5759 2023-04-08 11:57:02.000000 chatgpt4-cli-1.4.7/GPTCLI/helper.py
--rw-r--r--   0 root         (0) root         (0)     5638 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.7/GPTCLI/image.py
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-06 14:49:38.000000 chatgpt4-cli-1.4.7/GPTCLI/test.py
--rw-r--r--   0 root         (0) root         (0)    15283 2023-04-08 13:19:37.521268 chatgpt4-cli-1.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12054 2023-04-08 13:18:26.000000 chatgpt4-cli-1.4.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 13:19:37.521268 chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15283 2023-04-08 13:19:36.000000 chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2023-04-08 13:19:36.000000 chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 13:19:36.000000 chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-04-08 13:19:36.000000 chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-08 13:19:36.000000 chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-08 13:19:36.000000 chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 13:19:37.521268 chatgpt4-cli-1.4.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1297 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27403 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/setup.py
```

### Comparing `chatgpt4-cli-1.4.7/GPTCLI/emage.py` & `chatgpt4-cli-1.4.8/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.7/GPTCLI/gptcli.py` & `chatgpt4-cli-1.4.8/GPTCLI/gptcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,14 +284,19 @@
             action="store_true",
         )
         parser.add_argument(
             "--update",
             help="Download latest prompts - [awesome-chatgpt-prompts]",
             action="store_true",
         )
+        parser.add_argument(
+            "--sudo",
+            help="Run commands against system with sudo privileges",
+            action="store_true",
+        )
         return parser.parse_args()
 
     def main(self):
         return self.get_args()
 
 
 config_h = config_handler()
@@ -305,15 +310,15 @@
 from .emage import emager
 from re import sub
 from datetime import datetime
 from os import system, remove, path, environ, makedirs
 from threading import Thread as thr
 from appdirs import AppDirs
 from rich.markdown import Markdown
-from .addons import file_parser
+from .addons import file_parser, system_control
 
 app_dir = AppDirs(
     "smartwa",
     "gpt-cli",
 ).user_data_dir
 
 first_time_run = False
@@ -530,25 +535,25 @@
         " ".join(args.settings) if isinstance(args.settings, list) else args.settings
     )
     prompt = time_now_format(prompt_disp)
     config_handler = config_handler()
     color_dict = config_handler.color_dict
     bcolor_dict = config_handler.bcolor_dict
     interactive = local_interactor()
-    parser = lambda self,line:file_parser(line).parse()
+    parser = lambda self, line: file_parser(line).parse()
 
     def apply_color(self):
         print(
             self.bcolor_dict[args.background_color] + self.color_dict[args.input_color]
         )
 
-    def prompt_is_error_free(self,prompt,resp=True) -> bool:
+    def prompt_is_error_free(self, prompt, resp=True) -> bool:
         """Checks if prompt contains [sorry]"""
-        if isinstance(prompt,list):
-            if len(prompt)>=2 and prompt[0:2]==["I'm","sorry"]:
+        if isinstance(prompt, list):
+            if len(prompt) >= 2 and prompt[0:2] == ["I'm", "sorry"]:
                 resp = False
         else:
             if prompt.startswith("I'm sorry"):
                 resp = False
         return resp
 
     def default(self, raw, return_fb=False):
@@ -556,27 +561,27 @@
         run_against_system = False
         if not raw:
             return
         # out = lambda b: print(self.color_dict[args.output_color] + b + Fore.RESET)
         if raw[0:2] == "./":
             system((raw[2:]).strip())
         else:
-            if '--system' in raw:
+            if "--system" in raw:
                 run_against_system = True
-                raw=raw.replace('--system','')
+                raw = raw.replace("--system", "")
             args.message = raw
             print(self.color_dict[args.output_color], end="")
             rp = gpt3.main()
             if rp[0]:
                 feedback = sub("\n\n", "\n", rp[1], 1)
                 if return_fb:
                     return feedback.strip()
                 record_keeper.main(feedback)
                 if run_against_system:
-                    system(feedback.strip())
+                    system_control(feedback).execute(args.sudo)
 
             else:
                 logging.error(str(rp[1]))
             print(Fore.RESET)
         self.do__prompt(self.prompt_disp)
 
     def do_txt2img(self, line):
@@ -601,15 +606,15 @@
                     record_keeper.main(rp["url"])
 
         else:
             print("")
             if not description:
                 logging.error("Failed to generate description.")
         self.do__prompt(self.prompt_disp)
-                
+
     def do_img(self, line):
         line = self.parser(line)
         if not line:
             return
         """Text-to-Image handler"""
         print(self.color_dict[args.output_color], end="\r")
         resp = imager(line.split(" ")).main()
@@ -734,15 +739,15 @@
 
     def do__help(self, line):
         from .helper import help
 
         print(help)
         self.do__prompt(self.prompt_disp)
 
-    def do__exit(self,line):
+    def do__exit(self, line):
         return True
 
 
 def get_api_key() -> str:
     """Gets API from Key_path or args.key"""
     if any([args.key, environ.get("OPENAI_API_KEY")]):
         return args.key or environ.get("OPENAI_API_KEY")
@@ -795,57 +800,62 @@
             if not args.zero_show:
                 show_role()
             return True
         except KeyError:
             logging.warning(error_msg)
     else:
         logging.warning(error_msg)
-    del prompt_dict,keys
+    del prompt_dict, keys
 
 
 def main():
     global chatbot, gpt4, record_keeper
     args.disable_stream = True if args.markdown else args.disable_stream
     record_keeper = tracker(args.output)
     args.api_key = get_api_key()
     predefined_prompt_used = intro_train()
     openai.api_key = args.api_key
     try:
         if args.gpt in ("4"):
             from revChatGPT.V3 import Chatbot
-            
+
             gpt4 = True
             chatbot = Chatbot(
                 api_key=args.api_key,
-                engine=args.model if args.model in config_h.v4models else "gpt-3.5-turbo",
+                engine=args.model
+                if args.model in config_h.v4models
+                else "gpt-3.5-turbo",
                 # timeout=args.timeout, #Available as from revChatGPT>=4.0.6.1
                 proxy=args.proxy,  #
                 max_tokens=args.max_tokens,
                 temperature=args.temperature,
                 presence_penalty=args.presence_frequency,
                 frequency_penalty=args.frequency_penalty,
                 reply_count=args.reply_count,
                 system_prompt=args.system_prompt
                 if args.system_prompt is str
                 else " ".join(args.system_prompt),
-                )
+            )
         else:
             gpt4 = False
             from revChatGPT.V0 import Chatbot
+
             chatbot = Chatbot(api_key=args.api_key, engine=args.model, proxy=args.proxy)
     except Exception as e:
         exit(logging.critical(getExc(e)))
-        
+
     try:
         if args.new_record and path.isfile(args.output):
             remove(args.output)
         run = main_gpt()
         if args.message:
             run.default(
-                " ".join(args.message) if args.message is list else args.message
+                " ".join(run.parser(args.message))
+                if args.message is list
+                else args.message
             )
         run.cmdloop()
     except (KeyboardInterrupt, EOFError):
         exit(logging.info("Stopping program"))
     except Exception as e:
         print(getExc(e))
```

### Comparing `chatgpt4-cli-1.4.7/GPTCLI/helper.py` & `chatgpt4-cli-1.4.8/GPTCLI/helper.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.7/GPTCLI/image.py` & `chatgpt4-cli-1.4.8/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.7/PKG-INFO` & `chatgpt4-cli-1.4.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,329 +1,329 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.4.7
+Version: 1.4.8
 Summary: Terminal for ChatGPT
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Description: <h1 align="center">gpt-cli</h1>
-        <p align="center">
-        <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-        <a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.7&color=green&logo=pypi" alt="Pypi"/>
-        <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
-        <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
-        </p>
-        
-        CLI tool for interacting with [ChatGPT](https://openai.com). 
-        > Chat and generate images.
-        
-        ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
-        
-        ## [Independencies](requirements.txt)
-        
-        * [Openai](https://github.com/openai/openai-python)
-        * [Numpy](https://github.com/numpy/numpy)
-        * [Colorama](https://github.com/tartley/colorama)
-        * [revChatGPT](https://github.com/acheong08/ChatGPT)
-        
-        ### Features
-        
-        - Chat with ChatGPT conversationally.
-        - Stream or Non-stream responses
-        - Maintain record of the chats
-        - Generate Images - Based on your prompt or ChatGPT generated description
-        - Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-        - Fully customizable Commandline Interface
-        - Interact with system commands on the fly
-        
-        ### Prerequisites
-        
-        - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
-        
-        ## Installation
-        
-        Either of the following ways will get you ready.
-        
-        1. Using pip
-        - From pypi
-        
-        ```sh
-        $ sudo pip install chatgpt4-cli
-        ```
-        
-        - Installing from source
-         
-         ```sh
-         $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
-         ```
-        
-        2. Cloning locally and install
-        
-        ```sh
-        $ git clone https://github.com/Simatwa/gpt-cli.git
-        $ cd gpt-cli
-        $ sudo python3 setup.py install
-         #or
-        $ python3 setup.py install
-        ```
-        
-        ## Usage 
-        
-        - Make OPENAI_API_KEY an environment variable.
-        
-        `$ export OPENAI_API_KEY=<openai-api-key>`
-        
-        After that you can launch the script with or without a prompt
-        
-        > For instance :
-        ```sh 
-            #Without a prompt
-           $ gpt-cli 
-            # With a prompt 
-           $ gpt-cli Write a conversation between Sun and Pluto.`
-        ```
-        
-        - Parsing OPENAI_API_KEY as one of the arguments
-        
-        Run `$ gpt-cli -k <gpt-api-key> <Your query>` at the terminal.
-        
-        > For instance :
-        
-        ```sh
-        $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP?
-        ```
-        
-        The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) can be parsed to the script through the following ways:
-        
-        - Specifying the role - (*case-sensitive*)
-        
-            e.g `$ gpt-cli UX/UI Developer`
-        
-        - Specifying the index of the prompt:
-        
-            e.g `$ gpt-cli 29`
-        
-        Run `$ gpt-cli --dump show` to view the act,prompt and their **indexes**
-        
-        You can as well generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-        
-        1. EdgeGPT 
-        
-        ```sh
-        $ gpt-cli-emage --cookie-file <path> <Your prompt>
-        ```  
-        - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the cookies.
-        
-        2. ChatGPT 
-        
-        ```sh
-          # Make OPENAI_API_KEY environment variable
-          $ gpt-cli-image <Your Prompt>
-        ```
-        
-        For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`.
-        
-        ## Highlight
-        <details>
-        <summary>
-        <table>
-        <thead>
-        <tr><th style="text-align: right;">  No.</th><th>Command          </th><th>Action                                     </th></tr>
-        </thead>
-        <tbody>
-        <tr><td style="text-align: right;">    0</td><td>./{command}      </td><td>Run command against system                 </td></tr>
-        <tr><td style="text-align: right;">    1</td><td>img              </td><td>Generate image ChatGPT based on prompt     </td></tr>
-        <tr><td style="text-align: right;">    2</td><td>emg              </td><td>Generate image with EdgeGPT based on prompt</td></tr>
-        <tr><td style="text-align: right;">    3</td><td>txt2img          </td><td>Generate image based on GPT description    </td></tr>
-        <tr><td style="text-align: right;">    4</td><td>_font_color      </td><td>Modify font-color                          </td></tr>
-        <tr><td style="text-align: right;">    5</td><td>_background_color</td><td>Modify background_color                    </td></tr>
-        <tr><td style="text-align: right;">    6</td><td>_prompt          </td><td>Modify terminal prompt                     </td></tr>
-        <tr><td style="text-align: right;">    7</td><td>_save            </td><td>Save current configurations to `.json` file</td></tr>
-        <tr><td style="text-align: right;">    8</td><td>_load            </td><td>Load configurations from file              </td></tr>
-        <tr><td style="text-align: right;">    9</td><td>_rollback        </td><td>Rollback Chat by {n} times                 </td></tr>
-        <tr><td style="text-align: right;">   10</td><td>_reset           </td><td>Reset current chat and start new           </td></tr>
-        <tr><td style="text-align: right;">   11</td><td>_help            </td><td>Show this help info                        </td></tr>
-        <tr><td style="text-align: right;">   12</td><td>{Any Other}      </td><td>Chat with ChatGPT                          </td></tr>
-        </tbody>
-        </table>
-        </summary>
-        
-        1.img : Text-to-Image converter - ChatGPT
-         - e.g ```img Toddler cartoon coding in Python```
-        
-        2.emg : Text-to-Image converter - EdgeGPT
-         - e.g ```emg Toddler cartoon coding in Python```
-        
-        3.txt2img : Generate image based on GPT description
-         - e.g ```txt2img Describe phenotype anatomy of ancient dinosaurs```
-        
-        4._font_color : modifies font-color
-         - e.g ```font_color input red```
-        
-        5._background_color : modifies background_color
-         - e.g ```background_color cyan```
-        
-        6._prompt : Modify CMD prompt
-         - e.g ```prompt ┌─[Smartwa@ChatGPT4]─(%H:%M:%S)```
-        
-        7._load : Load configurations from the json file
-         - e.g ```load DAN.json```
-        
-        8._save : Save the current Chat Configurations
-         - e.g ```save DAN.json```
-        
-        9._rollback : Rollback the Chat by the {n} time(s)
-         - e.g ```_rollback 2```
-        
-        10._reset : Reset current chat and start new
-         - e.g ```_reset Chat as if you are a 10 year old child```
-        
-        11._help : Show this help info
-        
-        * Use double `./` *(fullstop and forward slash)* to interact with **system commands**
-          e.g './ifconfig'
-        </details>
-        
-        <details>
-        <summary>
-        
-          For more info run `gpt-cli -h`.
-        
-          </summary>
-        
-        ```
-        usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
-                       [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
-                       [-kp path] [-ic [cyan|green|yellow|red]]
-                       [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
-                       [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
-                       [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
-                       [-fp path] [-o path] [-pp prefix] [-rp prefix]
-                       [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path]
-                       [--disable-stream] [--new-record] [--disable-recording]
-                       [--zero-show] [--markdown] [--update]
-                       [message ...]
-        
-        Interact with ChatGPT at the terminal
-        
-        positional arguments:
-          message               Message to be send.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v, --version         show program's version number and exit
-          -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k
-                                ChatGPT model to be used
-          -t [0.1-1], --temperature [0.1-1]
-                                Charge of the generated text's randomness
-          -mt [1-7000], --max-tokens [1-7000]
-                                Maximum number of tokens to be generated upon
-                                completion
-          -tp [0.1-1], --top-p [0.1-1]
-                                Sampling threshold during inference time
-          -f [0.1-2], --frequency-penalty [0.1-2]
-                                Chances of word being repeated
-          -p [0.1-2], --presence-frequency [0.1-2]
-                                Chances of topic being repeated
-          -k KEY, --key KEY     OPENAI-API-KEY
-          -kp path, --key-path path
-                                Path to text-file containing GPT-api key
-          -ic [cyan|green|yellow|red], --input-color [cyan|green|yellow|red]
-                                Font color for inputs
-          -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red]
-                                Font color for outputs
-          -bc [blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
-                                Console's background-color
-          -pc [cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red]
-                                Prompt's display color
-          --prompt [SETTINGS ...]
-                                Customizes the prompt display
-          -tm value, --timeout value
-                                Request timeout while making request - (Soon)
-          -pr PROXY, --proxy PROXY
-                                Pivot request through this proxy
-          -rc value, --reply-count value
-                                Number of responses to be received
-          -g 1,4, --gpt 1,4     ChatGPT version to be used
-          -sp [text ...], --system-prompt [text ...]
-                                Text to train ChatGPT at the start
-          -fp path, --file-path path
-                                Path to .csv file containing role and prompt -
-                                [act,prompt]
-          -o path, --output path
-                                Filepath for saving the chats - default
-                                [/home/smartwa/git/gpt-cli/.chatgpt-history.txt]
-          -pp prefix, --prompt-prefix prefix
-                                Text to append before saving each prompt - default
-                                [>>timestamp]
-          -rp prefix, --response-prefix prefix
-                                Text to append before saving each response - default
-                                [None]
-          -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm}
-                                Stdout [keys,values]; Save all prompts in json format
-                                to a file
-          -dl symbol, --delimiter symbol
-                                Delimeter for the .CSV file - [act,prompt]
-          -cf path, --cookie-file path
-                                Path to Bing's cookies - for Edge Image Generation
-          --disable-stream      Specifies not to stream responses from ChatGPT
-          --new-record          Override previous chats under the filepath
-          --disable-recording   Disable saving prompts and responses
-          --zero-show           Specifies not to stdout prompt of the act parsed
-          --markdown            Stdout responses in markdown-format - disables
-                                streaming
-          --update              Download latest prompts - [awesome-chatgpt-prompts]
-        
-        ```
-        
-          </details>
-        
-        > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
-        
-        > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
-        
-        
-        ## Motive
-        
-        <details>
-        <summary>
-        Love for `Terminal` ❤️
-        </summary>
-        As a `terminal guy` I used to find it uncomfortable to keep shifting from one window to next in order to access ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/Simatwa/gpt-cli)
-        </details>
-        
-        ## Contributions
-        
-        - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
-        
-        ### ToDo
-        
-        - [x] Use dialogue
-        - [x] Issue prompt from a file
-        - [ ] Busy bar
-        
-          > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
-        
-        ## Acknowledgements
-        
-        1. [remo7777](https://github.com/remo7777/T-Header)
-        
-        2. [acheong08](https://github.com/acheong08/ChatGPT)
-        
-        3. [f](https://github.com/f/awesome-chatgpt-prompts)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">gpt-cli</h1>
+<p align="center">
+<a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.8&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
+<a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
+</p>
+
+CLI tool for interacting with [ChatGPT](https://openai.com). 
+> Chat and generate images.
+
+![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
+
+## [Independencies](requirements.txt)
+
+* [Openai](https://github.com/openai/openai-python)
+* [Numpy](https://github.com/numpy/numpy)
+* [Colorama](https://github.com/tartley/colorama)
+* [revChatGPT](https://github.com/acheong08/ChatGPT)
+
+### Features
+
+- Chat with ChatGPT conversationally.
+- Stream or Non-stream responses
+- Maintain record of the chats
+- Generate Images - Based on your prompt or ChatGPT generated description
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- Fully customizable Commandline Interface
+- Interact with system commands on the fly
+
+### Prerequisites
+
+- [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
+
+## Installation
+
+Either of the following ways will get you ready.
+
+1. Using pip
+- From pypi
+
+```sh
+$ sudo pip install chatgpt4-cli
+```
+
+- Installing from source
+ 
+ ```sh
+ $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
+ ```
+
+2. Cloning locally and install
+
+```sh
+$ git clone https://github.com/Simatwa/gpt-cli.git
+$ cd gpt-cli
+$ sudo python3 setup.py install
+ #or
+$ python3 setup.py install
+```
+
+## Usage 
+
+- Make OPENAI_API_KEY an environment variable.
+
+`$ export OPENAI_API_KEY=<openai-api-key>`
+
+After that you can launch the script with or without a prompt
+
+> For instance :
+```sh 
+    #Without a prompt
+   $ gpt-cli 
+    # With a prompt 
+   $ gpt-cli Write a conversation between Sun and Pluto.`
+```
+
+- Parsing OPENAI_API_KEY as one of the arguments
+
+Run `$ gpt-cli -k <openai-api-key> <Your query>` at the terminal.
+
+> For instance :
+
+```sh
+$ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP?
+```
+
+The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) can be parsed to the script through the following ways:
+
+- Specifying the role - (*case-sensitive*)
+
+    e.g `$ gpt-cli UX/UI Developer`
+
+- Specifying the index of the prompt:
+
+    e.g `$ gpt-cli 29`
+
+Run `$ gpt-cli --dump show` to view the act,prompt and their **indexes**
+
+You can as well generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+
+1. EdgeGPT 
+
+```sh
+$ gpt-cli-emage --cookie-file <path> <Your prompt>
+```  
+- Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the cookies.
+
+2. ChatGPT 
+
+```sh
+  # Make OPENAI_API_KEY environment variable
+  $ gpt-cli-image <Your Prompt>
+```
+
+For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`.
+
+## Highlight
+<details>
+<summary>
+<table>
+<thead>
+<tr><th style="text-align: right;">  No.</th><th>Command          </th><th>Action                                     </th></tr>
+</thead>
+<tbody>
+<tr><td style="text-align: right;">    0</td><td>./{command}      </td><td>Run command against system                 </td></tr>
+<tr><td style="text-align: right;">    1</td><td>img              </td><td>Generate image ChatGPT based on prompt     </td></tr>
+<tr><td style="text-align: right;">    2</td><td>emg              </td><td>Generate image with EdgeGPT based on prompt</td></tr>
+<tr><td style="text-align: right;">    3</td><td>txt2img          </td><td>Generate image based on GPT description    </td></tr>
+<tr><td style="text-align: right;">    4</td><td>_font_color      </td><td>Modify font-color                          </td></tr>
+<tr><td style="text-align: right;">    5</td><td>_background_color</td><td>Modify background_color                    </td></tr>
+<tr><td style="text-align: right;">    6</td><td>_prompt          </td><td>Modify terminal prompt                     </td></tr>
+<tr><td style="text-align: right;">    7</td><td>_save            </td><td>Save current configurations to `.json` file</td></tr>
+<tr><td style="text-align: right;">    8</td><td>_load            </td><td>Load configurations from file              </td></tr>
+<tr><td style="text-align: right;">    9</td><td>_rollback        </td><td>Rollback Chat by {n} times                 </td></tr>
+<tr><td style="text-align: right;">   10</td><td>_reset           </td><td>Reset current chat and start new           </td></tr>
+<tr><td style="text-align: right;">   11</td><td>_help            </td><td>Show this help info                        </td></tr>
+<tr><td style="text-align: right;">   12</td><td>{Any Other}      </td><td>Chat with ChatGPT                          </td></tr>
+</tbody>
+</table>
+</summary>
+
+1.img : Text-to-Image converter - ChatGPT
+ - e.g ```img Toddler cartoon coding in Python```
+
+2.emg : Text-to-Image converter - EdgeGPT
+ - e.g ```emg Toddler cartoon coding in Python```
+
+3.txt2img : Generate image based on GPT description
+ - e.g ```txt2img Describe phenotype anatomy of ancient dinosaurs```
+
+4._font_color : modifies font-color
+ - e.g ```font_color input red```
+
+5._background_color : modifies background_color
+ - e.g ```background_color cyan```
+
+6._prompt : Modify CMD prompt
+ - e.g ```prompt ┌─[Smartwa@ChatGPT4]─(%H:%M:%S)```
+
+7._load : Load configurations from the json file
+ - e.g ```load DAN.json```
+
+8._save : Save the current Chat Configurations
+ - e.g ```save DAN.json```
+
+9._rollback : Rollback the Chat by the {n} time(s)
+ - e.g ```_rollback 2```
+
+10._reset : Reset current chat and start new
+ - e.g ```_reset Chat as if you are a 10 year old child```
+
+11._help : Show this help info
+
+* Use double `./` *(fullstop and forward slash)* to interact with **system commands**
+  e.g './ifconfig'
+</details>
+
+<details>
+<summary>
+
+  For more info run `gpt-cli -h`.
+
+  </summary>
+
+```
+usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
+               [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
+               [-kp path] [-ic [cyan|green|yellow|red]]
+               [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
+               [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
+               [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
+               [-fp path] [-o path] [-pp prefix] [-rp prefix]
+               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path]
+               [--disable-stream] [--new-record] [--disable-recording]
+               [--zero-show] [--markdown] [--update]
+               [message ...]
+
+Interact with ChatGPT at the terminal
+
+positional arguments:
+  message               Message to be send.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k
+                        ChatGPT model to be used
+  -t [0.1-1], --temperature [0.1-1]
+                        Charge of the generated text's randomness
+  -mt [1-7000], --max-tokens [1-7000]
+                        Maximum number of tokens to be generated upon
+                        completion
+  -tp [0.1-1], --top-p [0.1-1]
+                        Sampling threshold during inference time
+  -f [0.1-2], --frequency-penalty [0.1-2]
+                        Chances of word being repeated
+  -p [0.1-2], --presence-frequency [0.1-2]
+                        Chances of topic being repeated
+  -k KEY, --key KEY     OPENAI-API-KEY
+  -kp path, --key-path path
+                        Path to text-file containing GPT-api key
+  -ic [cyan|green|yellow|red], --input-color [cyan|green|yellow|red]
+                        Font color for inputs
+  -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red]
+                        Font color for outputs
+  -bc [blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
+                        Console's background-color
+  -pc [cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red]
+                        Prompt's display color
+  --prompt [SETTINGS ...]
+                        Customizes the prompt display
+  -tm value, --timeout value
+                        Request timeout while making request - (Soon)
+  -pr PROXY, --proxy PROXY
+                        Pivot request through this proxy
+  -rc value, --reply-count value
+                        Number of responses to be received
+  -g 1,4, --gpt 1,4     ChatGPT version to be used
+  -sp [text ...], --system-prompt [text ...]
+                        Text to train ChatGPT at the start
+  -fp path, --file-path path
+                        Path to .csv file containing role and prompt -
+                        [act,prompt]
+  -o path, --output path
+                        Filepath for saving the chats - default
+                        [/home/smartwa/git/gpt-cli/.chatgpt-history.txt]
+  -pp prefix, --prompt-prefix prefix
+                        Text to append before saving each prompt - default
+                        [>>timestamp]
+  -rp prefix, --response-prefix prefix
+                        Text to append before saving each response - default
+                        [None]
+  -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm}
+                        Stdout [keys,values]; Save all prompts in json format
+                        to a file
+  -dl symbol, --delimiter symbol
+                        Delimeter for the .CSV file - [act,prompt]
+  -cf path, --cookie-file path
+                        Path to Bing's cookies - for Edge Image Generation
+  --disable-stream      Specifies not to stream responses from ChatGPT
+  --new-record          Override previous chats under the filepath
+  --disable-recording   Disable saving prompts and responses
+  --zero-show           Specifies not to stdout prompt of the act parsed
+  --markdown            Stdout responses in markdown-format - disables
+                        streaming
+  --update              Download latest prompts - [awesome-chatgpt-prompts]
+
+```
+
+  </details>
+
+> **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
+
+> **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
+
+
+## Motive
+
+<details>
+<summary>
+Love for `Terminal` ❤️
+</summary>
+As a `terminal guy` I used to find it uncomfortable to keep shifting from one window to next in order to access ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/Simatwa/gpt-cli)
+</details>
+
+## Contributions
+
+- Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
+
+### ToDo
+
+- [x] Use dialogue
+- [x] Issue prompt from a file
+- [ ] Busy bar
+
+  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
+
+## Acknowledgements
+
+1. [remo7777](https://github.com/remo7777/T-Header)
+
+2. [acheong08](https://github.com/acheong08/ChatGPT)
+
+3. [f](https://github.com/f/awesome-chatgpt-prompts)
```

#### html2text {}

```diff
@@ -1,12 +1,17 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.7 Summary: Terminal for
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.8 Summary: Terminal for
 ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Description:
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense) Classifier:
+Intended Audience :: Developers Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
 generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
 assets/Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https:
 //github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
@@ -119,13 +124,7 @@
 github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/
 gpt-cli/issues) without any **guideline** or submitting a [pull request](https:
 //github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue
 prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://github.com/
 Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
 (https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
 acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
-Platform: UNKNOWN Classifier: License :: OSI Approved :: The Unlicense
-(Unlicense) Classifier: Intended Audience :: Developers Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown
```

### Comparing `chatgpt4-cli-1.4.7/README.md` & `chatgpt4-cli-1.4.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.7&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.8&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -77,15 +77,15 @@
    $ gpt-cli 
     # With a prompt 
    $ gpt-cli Write a conversation between Sun and Pluto.`
 ```
 
 - Parsing OPENAI_API_KEY as one of the arguments
 
-Run `$ gpt-cli -k <gpt-api-key> <Your query>` at the terminal.
+Run `$ gpt-cli -k <openai-api-key> <Your query>` at the terminal.
 
 > For instance :
 
 ```sh
 $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP?
 ```
```

### Comparing `chatgpt4-cli-1.4.7/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,329 +1,329 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.4.7
+Version: 1.4.8
 Summary: Terminal for ChatGPT
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Description: <h1 align="center">gpt-cli</h1>
-        <p align="center">
-        <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-        <a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.7&color=green&logo=pypi" alt="Pypi"/>
-        <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
-        <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
-        <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
-        </p>
-        
-        CLI tool for interacting with [ChatGPT](https://openai.com). 
-        > Chat and generate images.
-        
-        ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
-        
-        ## [Independencies](requirements.txt)
-        
-        * [Openai](https://github.com/openai/openai-python)
-        * [Numpy](https://github.com/numpy/numpy)
-        * [Colorama](https://github.com/tartley/colorama)
-        * [revChatGPT](https://github.com/acheong08/ChatGPT)
-        
-        ### Features
-        
-        - Chat with ChatGPT conversationally.
-        - Stream or Non-stream responses
-        - Maintain record of the chats
-        - Generate Images - Based on your prompt or ChatGPT generated description
-        - Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-        - Fully customizable Commandline Interface
-        - Interact with system commands on the fly
-        
-        ### Prerequisites
-        
-        - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
-        
-        ## Installation
-        
-        Either of the following ways will get you ready.
-        
-        1. Using pip
-        - From pypi
-        
-        ```sh
-        $ sudo pip install chatgpt4-cli
-        ```
-        
-        - Installing from source
-         
-         ```sh
-         $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
-         ```
-        
-        2. Cloning locally and install
-        
-        ```sh
-        $ git clone https://github.com/Simatwa/gpt-cli.git
-        $ cd gpt-cli
-        $ sudo python3 setup.py install
-         #or
-        $ python3 setup.py install
-        ```
-        
-        ## Usage 
-        
-        - Make OPENAI_API_KEY an environment variable.
-        
-        `$ export OPENAI_API_KEY=<openai-api-key>`
-        
-        After that you can launch the script with or without a prompt
-        
-        > For instance :
-        ```sh 
-            #Without a prompt
-           $ gpt-cli 
-            # With a prompt 
-           $ gpt-cli Write a conversation between Sun and Pluto.`
-        ```
-        
-        - Parsing OPENAI_API_KEY as one of the arguments
-        
-        Run `$ gpt-cli -k <gpt-api-key> <Your query>` at the terminal.
-        
-        > For instance :
-        
-        ```sh
-        $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP?
-        ```
-        
-        The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) can be parsed to the script through the following ways:
-        
-        - Specifying the role - (*case-sensitive*)
-        
-            e.g `$ gpt-cli UX/UI Developer`
-        
-        - Specifying the index of the prompt:
-        
-            e.g `$ gpt-cli 29`
-        
-        Run `$ gpt-cli --dump show` to view the act,prompt and their **indexes**
-        
-        You can as well generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-        
-        1. EdgeGPT 
-        
-        ```sh
-        $ gpt-cli-emage --cookie-file <path> <Your prompt>
-        ```  
-        - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the cookies.
-        
-        2. ChatGPT 
-        
-        ```sh
-          # Make OPENAI_API_KEY environment variable
-          $ gpt-cli-image <Your Prompt>
-        ```
-        
-        For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`.
-        
-        ## Highlight
-        <details>
-        <summary>
-        <table>
-        <thead>
-        <tr><th style="text-align: right;">  No.</th><th>Command          </th><th>Action                                     </th></tr>
-        </thead>
-        <tbody>
-        <tr><td style="text-align: right;">    0</td><td>./{command}      </td><td>Run command against system                 </td></tr>
-        <tr><td style="text-align: right;">    1</td><td>img              </td><td>Generate image ChatGPT based on prompt     </td></tr>
-        <tr><td style="text-align: right;">    2</td><td>emg              </td><td>Generate image with EdgeGPT based on prompt</td></tr>
-        <tr><td style="text-align: right;">    3</td><td>txt2img          </td><td>Generate image based on GPT description    </td></tr>
-        <tr><td style="text-align: right;">    4</td><td>_font_color      </td><td>Modify font-color                          </td></tr>
-        <tr><td style="text-align: right;">    5</td><td>_background_color</td><td>Modify background_color                    </td></tr>
-        <tr><td style="text-align: right;">    6</td><td>_prompt          </td><td>Modify terminal prompt                     </td></tr>
-        <tr><td style="text-align: right;">    7</td><td>_save            </td><td>Save current configurations to `.json` file</td></tr>
-        <tr><td style="text-align: right;">    8</td><td>_load            </td><td>Load configurations from file              </td></tr>
-        <tr><td style="text-align: right;">    9</td><td>_rollback        </td><td>Rollback Chat by {n} times                 </td></tr>
-        <tr><td style="text-align: right;">   10</td><td>_reset           </td><td>Reset current chat and start new           </td></tr>
-        <tr><td style="text-align: right;">   11</td><td>_help            </td><td>Show this help info                        </td></tr>
-        <tr><td style="text-align: right;">   12</td><td>{Any Other}      </td><td>Chat with ChatGPT                          </td></tr>
-        </tbody>
-        </table>
-        </summary>
-        
-        1.img : Text-to-Image converter - ChatGPT
-         - e.g ```img Toddler cartoon coding in Python```
-        
-        2.emg : Text-to-Image converter - EdgeGPT
-         - e.g ```emg Toddler cartoon coding in Python```
-        
-        3.txt2img : Generate image based on GPT description
-         - e.g ```txt2img Describe phenotype anatomy of ancient dinosaurs```
-        
-        4._font_color : modifies font-color
-         - e.g ```font_color input red```
-        
-        5._background_color : modifies background_color
-         - e.g ```background_color cyan```
-        
-        6._prompt : Modify CMD prompt
-         - e.g ```prompt ┌─[Smartwa@ChatGPT4]─(%H:%M:%S)```
-        
-        7._load : Load configurations from the json file
-         - e.g ```load DAN.json```
-        
-        8._save : Save the current Chat Configurations
-         - e.g ```save DAN.json```
-        
-        9._rollback : Rollback the Chat by the {n} time(s)
-         - e.g ```_rollback 2```
-        
-        10._reset : Reset current chat and start new
-         - e.g ```_reset Chat as if you are a 10 year old child```
-        
-        11._help : Show this help info
-        
-        * Use double `./` *(fullstop and forward slash)* to interact with **system commands**
-          e.g './ifconfig'
-        </details>
-        
-        <details>
-        <summary>
-        
-          For more info run `gpt-cli -h`.
-        
-          </summary>
-        
-        ```
-        usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
-                       [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
-                       [-kp path] [-ic [cyan|green|yellow|red]]
-                       [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
-                       [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
-                       [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
-                       [-fp path] [-o path] [-pp prefix] [-rp prefix]
-                       [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path]
-                       [--disable-stream] [--new-record] [--disable-recording]
-                       [--zero-show] [--markdown] [--update]
-                       [message ...]
-        
-        Interact with ChatGPT at the terminal
-        
-        positional arguments:
-          message               Message to be send.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v, --version         show program's version number and exit
-          -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k
-                                ChatGPT model to be used
-          -t [0.1-1], --temperature [0.1-1]
-                                Charge of the generated text's randomness
-          -mt [1-7000], --max-tokens [1-7000]
-                                Maximum number of tokens to be generated upon
-                                completion
-          -tp [0.1-1], --top-p [0.1-1]
-                                Sampling threshold during inference time
-          -f [0.1-2], --frequency-penalty [0.1-2]
-                                Chances of word being repeated
-          -p [0.1-2], --presence-frequency [0.1-2]
-                                Chances of topic being repeated
-          -k KEY, --key KEY     OPENAI-API-KEY
-          -kp path, --key-path path
-                                Path to text-file containing GPT-api key
-          -ic [cyan|green|yellow|red], --input-color [cyan|green|yellow|red]
-                                Font color for inputs
-          -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red]
-                                Font color for outputs
-          -bc [blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
-                                Console's background-color
-          -pc [cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red]
-                                Prompt's display color
-          --prompt [SETTINGS ...]
-                                Customizes the prompt display
-          -tm value, --timeout value
-                                Request timeout while making request - (Soon)
-          -pr PROXY, --proxy PROXY
-                                Pivot request through this proxy
-          -rc value, --reply-count value
-                                Number of responses to be received
-          -g 1,4, --gpt 1,4     ChatGPT version to be used
-          -sp [text ...], --system-prompt [text ...]
-                                Text to train ChatGPT at the start
-          -fp path, --file-path path
-                                Path to .csv file containing role and prompt -
-                                [act,prompt]
-          -o path, --output path
-                                Filepath for saving the chats - default
-                                [/home/smartwa/git/gpt-cli/.chatgpt-history.txt]
-          -pp prefix, --prompt-prefix prefix
-                                Text to append before saving each prompt - default
-                                [>>timestamp]
-          -rp prefix, --response-prefix prefix
-                                Text to append before saving each response - default
-                                [None]
-          -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm}
-                                Stdout [keys,values]; Save all prompts in json format
-                                to a file
-          -dl symbol, --delimiter symbol
-                                Delimeter for the .CSV file - [act,prompt]
-          -cf path, --cookie-file path
-                                Path to Bing's cookies - for Edge Image Generation
-          --disable-stream      Specifies not to stream responses from ChatGPT
-          --new-record          Override previous chats under the filepath
-          --disable-recording   Disable saving prompts and responses
-          --zero-show           Specifies not to stdout prompt of the act parsed
-          --markdown            Stdout responses in markdown-format - disables
-                                streaming
-          --update              Download latest prompts - [awesome-chatgpt-prompts]
-        
-        ```
-        
-          </details>
-        
-        > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
-        
-        > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
-        
-        
-        ## Motive
-        
-        <details>
-        <summary>
-        Love for `Terminal` ❤️
-        </summary>
-        As a `terminal guy` I used to find it uncomfortable to keep shifting from one window to next in order to access ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/Simatwa/gpt-cli)
-        </details>
-        
-        ## Contributions
-        
-        - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
-        
-        ### ToDo
-        
-        - [x] Use dialogue
-        - [x] Issue prompt from a file
-        - [ ] Busy bar
-        
-          > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
-        
-        ## Acknowledgements
-        
-        1. [remo7777](https://github.com/remo7777/T-Header)
-        
-        2. [acheong08](https://github.com/acheong08/ChatGPT)
-        
-        3. [f](https://github.com/f/awesome-chatgpt-prompts)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">gpt-cli</h1>
+<p align="center">
+<a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.8&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
+<a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
+<a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
+</p>
+
+CLI tool for interacting with [ChatGPT](https://openai.com). 
+> Chat and generate images.
+
+![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
+
+## [Independencies](requirements.txt)
+
+* [Openai](https://github.com/openai/openai-python)
+* [Numpy](https://github.com/numpy/numpy)
+* [Colorama](https://github.com/tartley/colorama)
+* [revChatGPT](https://github.com/acheong08/ChatGPT)
+
+### Features
+
+- Chat with ChatGPT conversationally.
+- Stream or Non-stream responses
+- Maintain record of the chats
+- Generate Images - Based on your prompt or ChatGPT generated description
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily
+- Fully customizable Commandline Interface
+- Interact with system commands on the fly
+
+### Prerequisites
+
+- [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
+
+## Installation
+
+Either of the following ways will get you ready.
+
+1. Using pip
+- From pypi
+
+```sh
+$ sudo pip install chatgpt4-cli
+```
+
+- Installing from source
+ 
+ ```sh
+ $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
+ ```
+
+2. Cloning locally and install
+
+```sh
+$ git clone https://github.com/Simatwa/gpt-cli.git
+$ cd gpt-cli
+$ sudo python3 setup.py install
+ #or
+$ python3 setup.py install
+```
+
+## Usage 
+
+- Make OPENAI_API_KEY an environment variable.
+
+`$ export OPENAI_API_KEY=<openai-api-key>`
+
+After that you can launch the script with or without a prompt
+
+> For instance :
+```sh 
+    #Without a prompt
+   $ gpt-cli 
+    # With a prompt 
+   $ gpt-cli Write a conversation between Sun and Pluto.`
+```
+
+- Parsing OPENAI_API_KEY as one of the arguments
+
+Run `$ gpt-cli -k <openai-api-key> <Your query>` at the terminal.
+
+> For instance :
+
+```sh
+$ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP?
+```
+
+The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) can be parsed to the script through the following ways:
+
+- Specifying the role - (*case-sensitive*)
+
+    e.g `$ gpt-cli UX/UI Developer`
+
+- Specifying the index of the prompt:
+
+    e.g `$ gpt-cli 29`
+
+Run `$ gpt-cli --dump show` to view the act,prompt and their **indexes**
+
+You can as well generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+
+1. EdgeGPT 
+
+```sh
+$ gpt-cli-emage --cookie-file <path> <Your prompt>
+```  
+- Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the cookies.
+
+2. ChatGPT 
+
+```sh
+  # Make OPENAI_API_KEY environment variable
+  $ gpt-cli-image <Your Prompt>
+```
+
+For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`.
+
+## Highlight
+<details>
+<summary>
+<table>
+<thead>
+<tr><th style="text-align: right;">  No.</th><th>Command          </th><th>Action                                     </th></tr>
+</thead>
+<tbody>
+<tr><td style="text-align: right;">    0</td><td>./{command}      </td><td>Run command against system                 </td></tr>
+<tr><td style="text-align: right;">    1</td><td>img              </td><td>Generate image ChatGPT based on prompt     </td></tr>
+<tr><td style="text-align: right;">    2</td><td>emg              </td><td>Generate image with EdgeGPT based on prompt</td></tr>
+<tr><td style="text-align: right;">    3</td><td>txt2img          </td><td>Generate image based on GPT description    </td></tr>
+<tr><td style="text-align: right;">    4</td><td>_font_color      </td><td>Modify font-color                          </td></tr>
+<tr><td style="text-align: right;">    5</td><td>_background_color</td><td>Modify background_color                    </td></tr>
+<tr><td style="text-align: right;">    6</td><td>_prompt          </td><td>Modify terminal prompt                     </td></tr>
+<tr><td style="text-align: right;">    7</td><td>_save            </td><td>Save current configurations to `.json` file</td></tr>
+<tr><td style="text-align: right;">    8</td><td>_load            </td><td>Load configurations from file              </td></tr>
+<tr><td style="text-align: right;">    9</td><td>_rollback        </td><td>Rollback Chat by {n} times                 </td></tr>
+<tr><td style="text-align: right;">   10</td><td>_reset           </td><td>Reset current chat and start new           </td></tr>
+<tr><td style="text-align: right;">   11</td><td>_help            </td><td>Show this help info                        </td></tr>
+<tr><td style="text-align: right;">   12</td><td>{Any Other}      </td><td>Chat with ChatGPT                          </td></tr>
+</tbody>
+</table>
+</summary>
+
+1.img : Text-to-Image converter - ChatGPT
+ - e.g ```img Toddler cartoon coding in Python```
+
+2.emg : Text-to-Image converter - EdgeGPT
+ - e.g ```emg Toddler cartoon coding in Python```
+
+3.txt2img : Generate image based on GPT description
+ - e.g ```txt2img Describe phenotype anatomy of ancient dinosaurs```
+
+4._font_color : modifies font-color
+ - e.g ```font_color input red```
+
+5._background_color : modifies background_color
+ - e.g ```background_color cyan```
+
+6._prompt : Modify CMD prompt
+ - e.g ```prompt ┌─[Smartwa@ChatGPT4]─(%H:%M:%S)```
+
+7._load : Load configurations from the json file
+ - e.g ```load DAN.json```
+
+8._save : Save the current Chat Configurations
+ - e.g ```save DAN.json```
+
+9._rollback : Rollback the Chat by the {n} time(s)
+ - e.g ```_rollback 2```
+
+10._reset : Reset current chat and start new
+ - e.g ```_reset Chat as if you are a 10 year old child```
+
+11._help : Show this help info
+
+* Use double `./` *(fullstop and forward slash)* to interact with **system commands**
+  e.g './ifconfig'
+</details>
+
+<details>
+<summary>
+
+  For more info run `gpt-cli -h`.
+
+  </summary>
+
+```
+usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
+               [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
+               [-kp path] [-ic [cyan|green|yellow|red]]
+               [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
+               [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
+               [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
+               [-fp path] [-o path] [-pp prefix] [-rp prefix]
+               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path]
+               [--disable-stream] [--new-record] [--disable-recording]
+               [--zero-show] [--markdown] [--update]
+               [message ...]
+
+Interact with ChatGPT at the terminal
+
+positional arguments:
+  message               Message to be send.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k
+                        ChatGPT model to be used
+  -t [0.1-1], --temperature [0.1-1]
+                        Charge of the generated text's randomness
+  -mt [1-7000], --max-tokens [1-7000]
+                        Maximum number of tokens to be generated upon
+                        completion
+  -tp [0.1-1], --top-p [0.1-1]
+                        Sampling threshold during inference time
+  -f [0.1-2], --frequency-penalty [0.1-2]
+                        Chances of word being repeated
+  -p [0.1-2], --presence-frequency [0.1-2]
+                        Chances of topic being repeated
+  -k KEY, --key KEY     OPENAI-API-KEY
+  -kp path, --key-path path
+                        Path to text-file containing GPT-api key
+  -ic [cyan|green|yellow|red], --input-color [cyan|green|yellow|red]
+                        Font color for inputs
+  -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red]
+                        Font color for outputs
+  -bc [blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
+                        Console's background-color
+  -pc [cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red]
+                        Prompt's display color
+  --prompt [SETTINGS ...]
+                        Customizes the prompt display
+  -tm value, --timeout value
+                        Request timeout while making request - (Soon)
+  -pr PROXY, --proxy PROXY
+                        Pivot request through this proxy
+  -rc value, --reply-count value
+                        Number of responses to be received
+  -g 1,4, --gpt 1,4     ChatGPT version to be used
+  -sp [text ...], --system-prompt [text ...]
+                        Text to train ChatGPT at the start
+  -fp path, --file-path path
+                        Path to .csv file containing role and prompt -
+                        [act,prompt]
+  -o path, --output path
+                        Filepath for saving the chats - default
+                        [/home/smartwa/git/gpt-cli/.chatgpt-history.txt]
+  -pp prefix, --prompt-prefix prefix
+                        Text to append before saving each prompt - default
+                        [>>timestamp]
+  -rp prefix, --response-prefix prefix
+                        Text to append before saving each response - default
+                        [None]
+  -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm}
+                        Stdout [keys,values]; Save all prompts in json format
+                        to a file
+  -dl symbol, --delimiter symbol
+                        Delimeter for the .CSV file - [act,prompt]
+  -cf path, --cookie-file path
+                        Path to Bing's cookies - for Edge Image Generation
+  --disable-stream      Specifies not to stream responses from ChatGPT
+  --new-record          Override previous chats under the filepath
+  --disable-recording   Disable saving prompts and responses
+  --zero-show           Specifies not to stdout prompt of the act parsed
+  --markdown            Stdout responses in markdown-format - disables
+                        streaming
+  --update              Download latest prompts - [awesome-chatgpt-prompts]
+
+```
+
+  </details>
+
+> **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
+
+> **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
+
+
+## Motive
+
+<details>
+<summary>
+Love for `Terminal` ❤️
+</summary>
+As a `terminal guy` I used to find it uncomfortable to keep shifting from one window to next in order to access ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/Simatwa/gpt-cli)
+</details>
+
+## Contributions
+
+- Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
+
+### ToDo
+
+- [x] Use dialogue
+- [x] Issue prompt from a file
+- [ ] Busy bar
+
+  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
+
+## Acknowledgements
+
+1. [remo7777](https://github.com/remo7777/T-Header)
+
+2. [acheong08](https://github.com/acheong08/ChatGPT)
+
+3. [f](https://github.com/f/awesome-chatgpt-prompts)
```

#### html2text {}

```diff
@@ -1,12 +1,17 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.7 Summary: Terminal for
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.8 Summary: Terminal for
 ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Description:
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense) Classifier:
+Intended Audience :: Developers Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
 generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
 assets/Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https:
 //github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
@@ -119,13 +124,7 @@
 github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/
 gpt-cli/issues) without any **guideline** or submitting a [pull request](https:
 //github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue
 prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://github.com/
 Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
 (https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
 acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
-Platform: UNKNOWN Classifier: License :: OSI Approved :: The Unlicense
-(Unlicense) Classifier: Intended Audience :: Developers Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown
```

### Comparing `chatgpt4-cli-1.4.7/setup.py` & `chatgpt4-cli-1.4.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from setuptools import setup
-from GPTCLI import __version__,__author__,__repo__
-
-def get_file(fnm:str,lst:bool=False):
-    with open(fnm) as fh:
-        if lst:
-            return fh.readlines()
-        return fh.read()
+from GPTCLI import __version__, __author__, __repo__
 
 setup(
     name="chatgpt4-cli",
     packages=["GPTCLI"],
     version=__version__,
     license="MIT",
     author=__author__,
     maintainer=__author__,
     author_email="smartwacaleb@gmail.com",
     description="Terminal for ChatGPT",
     url=__repo__,
     project_urls={"Bug Report": f"{__repo__}/issues/new"},
-    install_requires=get_file('requirements.txt',True),
-    long_description=get_file('README.md'),
+    install_requires=[
+        "numpy>=1.23.4",
+        "colorama>=0.4.6",
+        "openai>=0.26.4",
+        "revChatGPT==4.0.6",
+        "appdirs>=1.4.4",
+        "requests>=2.28.2",
+        "tabulate>=0.9.0",
+    ],
+    long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     entry_points={
-        'console_scripts':[
-            ('gpt-cli = GPTCLI.gptcli:main'),
-            ('gpt-cli-image = GPTCLI.image:main'),
-            ('gpt-cli-emage = GPTCLI.emage:main'),
+        "console_scripts": [
+            ("gpt-cli = GPTCLI.gptcli:main"),
+            ("gpt-cli-image = GPTCLI.image:main"),
+            ("gpt-cli-emage = GPTCLI.emage:main"),
         ]
-    }
-)
+    },
+)
```

