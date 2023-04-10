# Comparing `tmp/shell_gpt-0.8.7.tar.gz` & `tmp/shell_gpt-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_gpt-0.8.7.tar", last modified: Mon Apr 10 10:10:10 2023, max compression
+gzip compressed data, was "shell_gpt-0.8.8.tar", last modified: Mon Apr 10 15:05:44 2023, max compression
```

## Comparing `shell_gpt-0.8.7.tar` & `shell_gpt-0.8.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.242655 shell_gpt-0.8.7/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.7/LICENSE
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15413 2023-04-10 10:10:10.242432 shell_gpt-0.8.7/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15065 2023-04-09 21:48:47.000000 shell_gpt-0.8.7/README.md
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-10 10:10:10.242696 shell_gpt-0.8.7/setup.cfg
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-09 21:48:47.000000 shell_gpt-0.8.7/setup.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.240763 shell_gpt-0.8.7/sgpt/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      451 2023-04-09 21:20:27.000000 shell_gpt-0.8.7/sgpt/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.7/sgpt/__main__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4398 2023-04-09 19:35:59.000000 shell_gpt-0.8.7/sgpt/app.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.7/sgpt/cache.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3069 2023-04-09 19:35:59.000000 shell_gpt-0.8.7/sgpt/client.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2857 2023-04-09 21:52:14.000000 shell_gpt-0.8.7/sgpt/config.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.241465 shell_gpt-0.8.7/sgpt/handlers/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.7/sgpt/handlers/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.7/sgpt/handlers/chat_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.7/sgpt/handlers/default_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1195 2023-04-09 21:48:13.000000 shell_gpt-0.8.7/sgpt/handlers/handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.7/sgpt/handlers/repl_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.7/sgpt/make_prompt.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1877 2023-04-09 19:35:59.000000 shell_gpt-0.8.7/sgpt/utils.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 10:10:10.242240 shell_gpt-0.8.7/shell_gpt.egg-info/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15413 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/entry_points.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/requires.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-10 10:10:10.000000 shell_gpt-0.8.7/shell_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.428330 shell_gpt-0.8.8/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.8/LICENSE
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    16334 2023-04-10 15:05:44.428164 shell_gpt-0.8.8/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15986 2023-04-10 14:38:44.000000 shell_gpt-0.8.8/README.md
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-10 15:05:44.428375 shell_gpt-0.8.8/setup.cfg
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-10 14:38:44.000000 shell_gpt-0.8.8/setup.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.426005 shell_gpt-0.8.8/sgpt/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      451 2023-04-10 10:35:51.000000 shell_gpt-0.8.8/sgpt/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.8/sgpt/__main__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4674 2023-04-10 13:41:05.000000 shell_gpt-0.8.8/sgpt/app.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.8/sgpt/cache.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3069 2023-04-09 19:35:59.000000 shell_gpt-0.8.8/sgpt/client.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2857 2023-04-10 10:35:51.000000 shell_gpt-0.8.8/sgpt/config.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.427143 shell_gpt-0.8.8/sgpt/handlers/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.8/sgpt/handlers/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.8/sgpt/handlers/chat_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.8/sgpt/handlers/default_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1195 2023-04-10 10:35:51.000000 shell_gpt-0.8.8/sgpt/handlers/handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.8/sgpt/handlers/repl_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.8/sgpt/make_prompt.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1877 2023-04-09 19:35:59.000000 shell_gpt-0.8.8/sgpt/utils.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.427982 shell_gpt-0.8.8/shell_gpt.egg-info/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    16334 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/requires.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/top_level.txt
```

### Comparing `shell_gpt-0.8.7/LICENSE` & `shell_gpt-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/PKG-INFO` & `shell_gpt-0.8.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.8.7
+Version: 0.8.8
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shell GPT
-A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.7
+pip install shell-gpt==0.8.8
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
 ### Simple queries
 We can use it as normal search engine, asking about anything:
 ```shell
 sgpt "nginx default config file location"
 # -> The default configuration file for Nginx is located at /etc/nginx/nginx.conf.
 ```
 ```shell
-sgpt "docker show all local images"
-# -> You can view all locally available Docker images by running: `docker images`
-```
-```shell
 sgpt "mass of sun"
 # -> = 1.99 × 10^30 kg
 ```
-### Conversion
-Convert various units and measurements without having to search for the conversion formula or use a separate conversion website. You can convert units such as time, distance, weight, temperature, and more.
 ```shell
 sgpt "1 hour and 30 minutes to seconds"
 # -> 5,400 seconds
 ```
+### Summarization and analyzing
+ShellGPT accepts prompt from both stdin and command line argument, you choose the most convenient input method for your preferences. Whether you prefer piping input through the terminal or specifying it directly as arguments, `sgpt` got you covered. This versatile feature is particularly useful when you need to pass file content or pipe output from other commands to the GPT models for summarization or analysis. For example, you can easily generate a git commit message based on a diff:
 ```shell
-sgpt "1 kilometer to miles"
-# -> 1 kilometer is equal to 0.62137 miles.
+git diff | sgpt "Generate git commit message, my changes"
+# -> Commit message: Implement Model enum and get_edited_prompt()
 ```
+You can analyze logs from various sources by passing them using stdin or command line arguments, along with a user-friendly prompt. This enables you to quickly identify errors and get suggestions for possible solutions:
+```shell
+docker logs -n 20 container_name | sgpt "check logs, find errors, provide possible solutions"
+# ...
+```
+This powerful feature simplifies the process of managing and understanding data from different sources, making it easier for you to focus on what really matters: improving your projects and applications.
+
 ### Shell commands
 Have you ever found yourself forgetting common shell commands, such as `chmod`, and needing to look up the syntax online? With `--shell` or shortcut `-s` option, you can quickly find and execute the commands you need right in the terminal.
 ```shell
 sgpt --shell "make all files in current directory read only"
 # -> chmod 444 *
 # -> Execute shell command? [y/N]: y
 # ...
@@ -63,48 +66,35 @@
 # -> sudo softwareupdate -i -a
 ```
 The same prompt, when used on Ubuntu, will generate a different suggestion:
 ```shell
 sgpt -s "update my system"
 # -> sudo apt update && sudo apt upgrade -y
 ```
-
 Let's try some docker containers:
 ```shell
 sgpt -s "start nginx using docker, forward 443 and 80 port, mount current folder with index.html"
 # -> docker run -d -p 443:443 -p 80:80 -v $(pwd):/usr/share/nginx/html nginx
 # -> Execute shell command? [y/N]: y
 # ...
 ```
-Also, we can provide some parameters name in our prompt, for example, passing output file name to ffmpeg:
+We can still use pipes to pass input to `sgpt` and get shell commands as output:
 ```shell
-sgpt -s "slow down video twice using ffmpeg, input video name \"input.mp4\" output video name \"output.mp4\""
-# -> ffmpeg -i input.mp4 -filter:v "setpts=2.0*PTS" output.mp4
-# -> Execute shell command? [y/N]: y
-# ...
-```
+cat data.json | sgpt -s "curl localhost with provided json"
+# -> curl -X POST -H "Content-Type: application/json" -d '{"a": 1, "b": 2, "c": 3}' http://localhost
+````
 We can apply additional shell magic in our prompt, in this example passing file names to ffmpeg:
 ```shell
 ls
 # -> 1.mp4 2.mp4 3.mp4
 sgpt -s "using ffmpeg combine multiple videos into one without audio. Video file names: $(ls -m)"
 # -> ffmpeg -i 1.mp4 -i 2.mp4 -i 3.mp4 -filter_complex "[0:v] [1:v] [2:v] concat=n=3:v=1 [v]" -map "[v]" out.mp4
 # -> Execute shell command? [y/N]: y
 # ...
 ```
-Since ChatGPT can also do summarization and analyzing of input text, we can ask it to generate commit message:
-```shell
-sgpt "Generate git commit message, my changes: $(git diff)"
-# -> Commit message: Implement Model enum and get_edited_prompt() func, add temperature, top_p and editor args for OpenAI request.
-```
-Or ask it to find error in logs and provide more details:
-```shell
-sgpt "check these logs, find errors, and explain what the error is about: ${docker logs -n 20 container_name}"
-# ...
-```
 ### Generating code
 With `--code` parameters we can query only code as output, for example:
 ```shell
 sgpt --code "Solve classic fizz buzz problem using Python"
 ```
 ```python
 for i in range(1, 101):
@@ -125,34 +115,57 @@
 # 2
 # Fizz
 # 4
 # Buzz
 # Fizz
 # ...
 ```
+We can also use pipes to pass input to `sgpt`:
+```shell
+cat fizz_buzz.py | python -m sgpt --code "Generate comments for each line of my code"
+```
+```python
+# Loop through numbers 1 to 100
+for i in range(1, 101):
+    # Check if number is divisible by both 3 and 5
+    if i % 3 == 0 and i % 5 == 0:
+        # Print "FizzBuzz" if number is divisible by both 3 and 5
+        print("FizzBuzz")
+    # Check if number is divisible by 3
+    elif i % 3 == 0:
+        # Print "Fizz" if number is divisible by 3
+        print("Fizz")
+    # Check if number is divisible by 5
+    elif i % 5 == 0:
+        # Print "Buzz" if number is divisible by 5
+        print("Buzz")
+    # If number is not divisible by 3 or 5, print the number itself
+    else:
+        print(i)
+```
 
 ### Chat
 To start a chat session, use the `--chat` option followed by a unique session name and a prompt. You can also use "temp" as a session name to start a temporary chat session.
 ```shell
 sgpt --chat number "please remember my favorite number: 4"
 # -> I will remember that your favorite number is 4.
 sgpt --chat number "what would be my favorite number + 4?"
 # -> Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
-You can also use chat sessions to iteratively improve ChatGPT's suggestions by providing additional clues.
+You can also use chat sessions to iteratively improve GPT suggestions by providing additional clues.
 ```shell
 sgpt --chat python_requst --code "make an example request to localhost using Python"
 ```
 ```python
 import requests
 
 response = requests.get('http://localhost')
 print(response.text)
 ```
-Asking ChatGPT to add a cache to our request.
+Asking AI to add a cache to our request.
 ```shell
 sgpt --chat python_request --code "add caching"
 ```
 ```python
 import requests
 from cachecontrol import CacheControl
 
@@ -236,15 +249,15 @@
 Control cache using `--cache` (default) and `--no-cache` options. This caching applies for all `sgpt` requests to OpenAI API:
 ```shell
 sgpt "what are the colors of a rainbow"
 # -> The colors of a rainbow are red, orange, yellow, green, blue, indigo, and violet.
 ```
 Next time, same exact query will get results from local cache instantly. Note that `sgpt "what are the colors of a rainbow" --temperature 0.5` will make a new request, since we didn't provide `--temperature` (same applies to `--top-probability`) on previous request.
 
-This is just some examples of what we can do using ChatGPT model, I'm sure you will find it useful for your specific use cases.
+This is just some examples of what we can do using OpenAI GPT models, I'm sure you will find it useful for your specific use cases.
 
 ### Runtime configuration file
 You can setup some parameters in runtime configuration file `~/.config/shell_gpt/.sgptrc`:
 ```text
 # API key, also it is possible to define OPENAI_API_KEY env.
 OPENAI_API_KEY=your_api_key
 # OpenAI host, useful if you would like to use proxy.
```

### Comparing `shell_gpt-0.8.7/README.md` & `shell_gpt-0.8.8/shell_gpt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,61 @@
+Metadata-Version: 2.1
+Name: shell-gpt
+Version: 0.8.8
+Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
+Home-page: https://github.com/ther1d/shell_gpt
+Author: Farkhod Sadykov
+Author-email: farkhod@sadykov.dev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Shell GPT
-A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.7
+pip install shell-gpt==0.8.8
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
 ### Simple queries
 We can use it as normal search engine, asking about anything:
 ```shell
 sgpt "nginx default config file location"
 # -> The default configuration file for Nginx is located at /etc/nginx/nginx.conf.
 ```
 ```shell
-sgpt "docker show all local images"
-# -> You can view all locally available Docker images by running: `docker images`
-```
-```shell
 sgpt "mass of sun"
 # -> = 1.99 × 10^30 kg
 ```
-### Conversion
-Convert various units and measurements without having to search for the conversion formula or use a separate conversion website. You can convert units such as time, distance, weight, temperature, and more.
 ```shell
 sgpt "1 hour and 30 minutes to seconds"
 # -> 5,400 seconds
 ```
+### Summarization and analyzing
+ShellGPT accepts prompt from both stdin and command line argument, you choose the most convenient input method for your preferences. Whether you prefer piping input through the terminal or specifying it directly as arguments, `sgpt` got you covered. This versatile feature is particularly useful when you need to pass file content or pipe output from other commands to the GPT models for summarization or analysis. For example, you can easily generate a git commit message based on a diff:
+```shell
+git diff | sgpt "Generate git commit message, my changes"
+# -> Commit message: Implement Model enum and get_edited_prompt()
+```
+You can analyze logs from various sources by passing them using stdin or command line arguments, along with a user-friendly prompt. This enables you to quickly identify errors and get suggestions for possible solutions:
 ```shell
-sgpt "1 kilometer to miles"
-# -> 1 kilometer is equal to 0.62137 miles.
+docker logs -n 20 container_name | sgpt "check logs, find errors, provide possible solutions"
+# ...
 ```
+This powerful feature simplifies the process of managing and understanding data from different sources, making it easier for you to focus on what really matters: improving your projects and applications.
+
 ### Shell commands
 Have you ever found yourself forgetting common shell commands, such as `chmod`, and needing to look up the syntax online? With `--shell` or shortcut `-s` option, you can quickly find and execute the commands you need right in the terminal.
 ```shell
 sgpt --shell "make all files in current directory read only"
 # -> chmod 444 *
 # -> Execute shell command? [y/N]: y
 # ...
@@ -53,48 +66,35 @@
 # -> sudo softwareupdate -i -a
 ```
 The same prompt, when used on Ubuntu, will generate a different suggestion:
 ```shell
 sgpt -s "update my system"
 # -> sudo apt update && sudo apt upgrade -y
 ```
-
 Let's try some docker containers:
 ```shell
 sgpt -s "start nginx using docker, forward 443 and 80 port, mount current folder with index.html"
 # -> docker run -d -p 443:443 -p 80:80 -v $(pwd):/usr/share/nginx/html nginx
 # -> Execute shell command? [y/N]: y
 # ...
 ```
-Also, we can provide some parameters name in our prompt, for example, passing output file name to ffmpeg:
+We can still use pipes to pass input to `sgpt` and get shell commands as output:
 ```shell
-sgpt -s "slow down video twice using ffmpeg, input video name \"input.mp4\" output video name \"output.mp4\""
-# -> ffmpeg -i input.mp4 -filter:v "setpts=2.0*PTS" output.mp4
-# -> Execute shell command? [y/N]: y
-# ...
-```
+cat data.json | sgpt -s "curl localhost with provided json"
+# -> curl -X POST -H "Content-Type: application/json" -d '{"a": 1, "b": 2, "c": 3}' http://localhost
+````
 We can apply additional shell magic in our prompt, in this example passing file names to ffmpeg:
 ```shell
 ls
 # -> 1.mp4 2.mp4 3.mp4
 sgpt -s "using ffmpeg combine multiple videos into one without audio. Video file names: $(ls -m)"
 # -> ffmpeg -i 1.mp4 -i 2.mp4 -i 3.mp4 -filter_complex "[0:v] [1:v] [2:v] concat=n=3:v=1 [v]" -map "[v]" out.mp4
 # -> Execute shell command? [y/N]: y
 # ...
 ```
-Since ChatGPT can also do summarization and analyzing of input text, we can ask it to generate commit message:
-```shell
-sgpt "Generate git commit message, my changes: $(git diff)"
-# -> Commit message: Implement Model enum and get_edited_prompt() func, add temperature, top_p and editor args for OpenAI request.
-```
-Or ask it to find error in logs and provide more details:
-```shell
-sgpt "check these logs, find errors, and explain what the error is about: ${docker logs -n 20 container_name}"
-# ...
-```
 ### Generating code
 With `--code` parameters we can query only code as output, for example:
 ```shell
 sgpt --code "Solve classic fizz buzz problem using Python"
 ```
 ```python
 for i in range(1, 101):
@@ -115,34 +115,57 @@
 # 2
 # Fizz
 # 4
 # Buzz
 # Fizz
 # ...
 ```
+We can also use pipes to pass input to `sgpt`:
+```shell
+cat fizz_buzz.py | python -m sgpt --code "Generate comments for each line of my code"
+```
+```python
+# Loop through numbers 1 to 100
+for i in range(1, 101):
+    # Check if number is divisible by both 3 and 5
+    if i % 3 == 0 and i % 5 == 0:
+        # Print "FizzBuzz" if number is divisible by both 3 and 5
+        print("FizzBuzz")
+    # Check if number is divisible by 3
+    elif i % 3 == 0:
+        # Print "Fizz" if number is divisible by 3
+        print("Fizz")
+    # Check if number is divisible by 5
+    elif i % 5 == 0:
+        # Print "Buzz" if number is divisible by 5
+        print("Buzz")
+    # If number is not divisible by 3 or 5, print the number itself
+    else:
+        print(i)
+```
 
 ### Chat
 To start a chat session, use the `--chat` option followed by a unique session name and a prompt. You can also use "temp" as a session name to start a temporary chat session.
 ```shell
 sgpt --chat number "please remember my favorite number: 4"
 # -> I will remember that your favorite number is 4.
 sgpt --chat number "what would be my favorite number + 4?"
 # -> Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
-You can also use chat sessions to iteratively improve ChatGPT's suggestions by providing additional clues.
+You can also use chat sessions to iteratively improve GPT suggestions by providing additional clues.
 ```shell
 sgpt --chat python_requst --code "make an example request to localhost using Python"
 ```
 ```python
 import requests
 
 response = requests.get('http://localhost')
 print(response.text)
 ```
-Asking ChatGPT to add a cache to our request.
+Asking AI to add a cache to our request.
 ```shell
 sgpt --chat python_request --code "add caching"
 ```
 ```python
 import requests
 from cachecontrol import CacheControl
 
@@ -226,15 +249,15 @@
 Control cache using `--cache` (default) and `--no-cache` options. This caching applies for all `sgpt` requests to OpenAI API:
 ```shell
 sgpt "what are the colors of a rainbow"
 # -> The colors of a rainbow are red, orange, yellow, green, blue, indigo, and violet.
 ```
 Next time, same exact query will get results from local cache instantly. Note that `sgpt "what are the colors of a rainbow" --temperature 0.5` will make a new request, since we didn't provide `--temperature` (same applies to `--top-probability`) on previous request.
 
-This is just some examples of what we can do using ChatGPT model, I'm sure you will find it useful for your specific use cases.
+This is just some examples of what we can do using OpenAI GPT models, I'm sure you will find it useful for your specific use cases.
 
 ### Runtime configuration file
 You can setup some parameters in runtime configuration file `~/.config/shell_gpt/.sgptrc`:
 ```text
 # API key, also it is possible to define OPENAI_API_KEY env.
 OPENAI_API_KEY=your_api_key
 # OpenAI host, useful if you would like to use proxy.
```

### Comparing `shell_gpt-0.8.7/setup.py` & `shell_gpt-0.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # pylint: disable=consider-using-with
 setup(
     name="shell_gpt",
-    version="0.8.7",
+    version="0.8.8",
     packages=find_packages(),
     install_requires=[
         "typer~=0.7.0",
         "requests~=2.28.2",
         "rich==13.3.1",
         "distro~=1.8.0",
     ],
```

### Comparing `shell_gpt-0.8.7/sgpt/app.py` & `shell_gpt-0.8.8/sgpt/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 as the command line interface. It supports different modes of output including
 shell commands and code, and allows users to specify the desired OpenAI model
 and length and other options of the output. Additionally, it supports executing
 shell commands directly from the interface.
 
 API Key is stored locally for easy use in future runs.
 """
-
+import sys
 
 # To allow users to use arrow keys in the REPL.
 import readline  # pylint: disable=unused-import
 
 import typer
 
 # Click is part of typer.
@@ -83,23 +83,31 @@
     list_chat: bool = typer.Option(  # pylint: disable=W0613
         False,
         help="List all existing chat ids.",
         callback=ChatHandler.list_ids,
         rich_help_panel="Chat Options",
     ),
 ) -> None:
+    stdin_passed = not sys.stdin.isatty()
+
+    if stdin_passed and not repl:
+        prompt = sys.stdin.read() + (prompt or "")
+
     if not prompt and not editor and not repl:
         raise MissingParameter(param_hint="PROMPT", param_type="string")
 
     if shell and code:
         raise BadArgumentUsage("--shell and --code options cannot be used together.")
 
     if chat and repl:
         raise BadArgumentUsage("--chat and --repl options cannot be used together.")
 
+    if editor and stdin_passed:
+        raise BadArgumentUsage("--editor option cannot be used with stdin input.")
+
     if editor:
         prompt = get_edited_prompt()
 
     api_host = config.get("OPENAI_API_HOST")
     api_key = config.get("OPENAI_API_KEY")
     client = OpenAIClient(api_host, api_key)
 
@@ -128,15 +136,15 @@
             prompt,
             model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             caching=cache,
         )
 
-    if shell and typer.confirm("Execute shell command?"):
+    if shell and not stdin_passed and typer.confirm("Execute shell command?"):
         run_command(full_completion)
 
 
 def entry_point() -> None:
     # Python package entry point defined in setup.py
     typer.run(main)
```

### Comparing `shell_gpt-0.8.7/sgpt/cache.py` & `shell_gpt-0.8.8/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/client.py` & `shell_gpt-0.8.8/sgpt/client.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/config.py` & `shell_gpt-0.8.8/sgpt/config.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/handlers/chat_handler.py` & `shell_gpt-0.8.8/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/handlers/default_handler.py` & `shell_gpt-0.8.8/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/handlers/handler.py` & `shell_gpt-0.8.8/sgpt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/handlers/repl_handler.py` & `shell_gpt-0.8.8/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/make_prompt.py` & `shell_gpt-0.8.8/sgpt/make_prompt.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/sgpt/utils.py` & `shell_gpt-0.8.8/sgpt/utils.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.7/shell_gpt.egg-info/PKG-INFO` & `shell_gpt-0.8.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,51 @@
-Metadata-Version: 2.1
-Name: shell-gpt
-Version: 0.8.7
-Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
-Home-page: https://github.com/ther1d/shell_gpt
-Author: Farkhod Sadykov
-Author-email: farkhod@sadykov.dev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shell GPT
-A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.7
+pip install shell-gpt==0.8.8
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
 ### Simple queries
 We can use it as normal search engine, asking about anything:
 ```shell
 sgpt "nginx default config file location"
 # -> The default configuration file for Nginx is located at /etc/nginx/nginx.conf.
 ```
 ```shell
-sgpt "docker show all local images"
-# -> You can view all locally available Docker images by running: `docker images`
-```
-```shell
 sgpt "mass of sun"
 # -> = 1.99 × 10^30 kg
 ```
-### Conversion
-Convert various units and measurements without having to search for the conversion formula or use a separate conversion website. You can convert units such as time, distance, weight, temperature, and more.
 ```shell
 sgpt "1 hour and 30 minutes to seconds"
 # -> 5,400 seconds
 ```
+### Summarization and analyzing
+ShellGPT accepts prompt from both stdin and command line argument, you choose the most convenient input method for your preferences. Whether you prefer piping input through the terminal or specifying it directly as arguments, `sgpt` got you covered. This versatile feature is particularly useful when you need to pass file content or pipe output from other commands to the GPT models for summarization or analysis. For example, you can easily generate a git commit message based on a diff:
+```shell
+git diff | sgpt "Generate git commit message, my changes"
+# -> Commit message: Implement Model enum and get_edited_prompt()
+```
+You can analyze logs from various sources by passing them using stdin or command line arguments, along with a user-friendly prompt. This enables you to quickly identify errors and get suggestions for possible solutions:
 ```shell
-sgpt "1 kilometer to miles"
-# -> 1 kilometer is equal to 0.62137 miles.
+docker logs -n 20 container_name | sgpt "check logs, find errors, provide possible solutions"
+# ...
 ```
+This powerful feature simplifies the process of managing and understanding data from different sources, making it easier for you to focus on what really matters: improving your projects and applications.
+
 ### Shell commands
 Have you ever found yourself forgetting common shell commands, such as `chmod`, and needing to look up the syntax online? With `--shell` or shortcut `-s` option, you can quickly find and execute the commands you need right in the terminal.
 ```shell
 sgpt --shell "make all files in current directory read only"
 # -> chmod 444 *
 # -> Execute shell command? [y/N]: y
 # ...
@@ -63,48 +56,35 @@
 # -> sudo softwareupdate -i -a
 ```
 The same prompt, when used on Ubuntu, will generate a different suggestion:
 ```shell
 sgpt -s "update my system"
 # -> sudo apt update && sudo apt upgrade -y
 ```
-
 Let's try some docker containers:
 ```shell
 sgpt -s "start nginx using docker, forward 443 and 80 port, mount current folder with index.html"
 # -> docker run -d -p 443:443 -p 80:80 -v $(pwd):/usr/share/nginx/html nginx
 # -> Execute shell command? [y/N]: y
 # ...
 ```
-Also, we can provide some parameters name in our prompt, for example, passing output file name to ffmpeg:
+We can still use pipes to pass input to `sgpt` and get shell commands as output:
 ```shell
-sgpt -s "slow down video twice using ffmpeg, input video name \"input.mp4\" output video name \"output.mp4\""
-# -> ffmpeg -i input.mp4 -filter:v "setpts=2.0*PTS" output.mp4
-# -> Execute shell command? [y/N]: y
-# ...
-```
+cat data.json | sgpt -s "curl localhost with provided json"
+# -> curl -X POST -H "Content-Type: application/json" -d '{"a": 1, "b": 2, "c": 3}' http://localhost
+````
 We can apply additional shell magic in our prompt, in this example passing file names to ffmpeg:
 ```shell
 ls
 # -> 1.mp4 2.mp4 3.mp4
 sgpt -s "using ffmpeg combine multiple videos into one without audio. Video file names: $(ls -m)"
 # -> ffmpeg -i 1.mp4 -i 2.mp4 -i 3.mp4 -filter_complex "[0:v] [1:v] [2:v] concat=n=3:v=1 [v]" -map "[v]" out.mp4
 # -> Execute shell command? [y/N]: y
 # ...
 ```
-Since ChatGPT can also do summarization and analyzing of input text, we can ask it to generate commit message:
-```shell
-sgpt "Generate git commit message, my changes: $(git diff)"
-# -> Commit message: Implement Model enum and get_edited_prompt() func, add temperature, top_p and editor args for OpenAI request.
-```
-Or ask it to find error in logs and provide more details:
-```shell
-sgpt "check these logs, find errors, and explain what the error is about: ${docker logs -n 20 container_name}"
-# ...
-```
 ### Generating code
 With `--code` parameters we can query only code as output, for example:
 ```shell
 sgpt --code "Solve classic fizz buzz problem using Python"
 ```
 ```python
 for i in range(1, 101):
@@ -125,34 +105,57 @@
 # 2
 # Fizz
 # 4
 # Buzz
 # Fizz
 # ...
 ```
+We can also use pipes to pass input to `sgpt`:
+```shell
+cat fizz_buzz.py | python -m sgpt --code "Generate comments for each line of my code"
+```
+```python
+# Loop through numbers 1 to 100
+for i in range(1, 101):
+    # Check if number is divisible by both 3 and 5
+    if i % 3 == 0 and i % 5 == 0:
+        # Print "FizzBuzz" if number is divisible by both 3 and 5
+        print("FizzBuzz")
+    # Check if number is divisible by 3
+    elif i % 3 == 0:
+        # Print "Fizz" if number is divisible by 3
+        print("Fizz")
+    # Check if number is divisible by 5
+    elif i % 5 == 0:
+        # Print "Buzz" if number is divisible by 5
+        print("Buzz")
+    # If number is not divisible by 3 or 5, print the number itself
+    else:
+        print(i)
+```
 
 ### Chat
 To start a chat session, use the `--chat` option followed by a unique session name and a prompt. You can also use "temp" as a session name to start a temporary chat session.
 ```shell
 sgpt --chat number "please remember my favorite number: 4"
 # -> I will remember that your favorite number is 4.
 sgpt --chat number "what would be my favorite number + 4?"
 # -> Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
-You can also use chat sessions to iteratively improve ChatGPT's suggestions by providing additional clues.
+You can also use chat sessions to iteratively improve GPT suggestions by providing additional clues.
 ```shell
 sgpt --chat python_requst --code "make an example request to localhost using Python"
 ```
 ```python
 import requests
 
 response = requests.get('http://localhost')
 print(response.text)
 ```
-Asking ChatGPT to add a cache to our request.
+Asking AI to add a cache to our request.
 ```shell
 sgpt --chat python_request --code "add caching"
 ```
 ```python
 import requests
 from cachecontrol import CacheControl
 
@@ -236,15 +239,15 @@
 Control cache using `--cache` (default) and `--no-cache` options. This caching applies for all `sgpt` requests to OpenAI API:
 ```shell
 sgpt "what are the colors of a rainbow"
 # -> The colors of a rainbow are red, orange, yellow, green, blue, indigo, and violet.
 ```
 Next time, same exact query will get results from local cache instantly. Note that `sgpt "what are the colors of a rainbow" --temperature 0.5` will make a new request, since we didn't provide `--temperature` (same applies to `--top-probability`) on previous request.
 
-This is just some examples of what we can do using ChatGPT model, I'm sure you will find it useful for your specific use cases.
+This is just some examples of what we can do using OpenAI GPT models, I'm sure you will find it useful for your specific use cases.
 
 ### Runtime configuration file
 You can setup some parameters in runtime configuration file `~/.config/shell_gpt/.sgptrc`:
 ```text
 # API key, also it is possible to define OPENAI_API_KEY env.
 OPENAI_API_KEY=your_api_key
 # OpenAI host, useful if you would like to use proxy.
```

