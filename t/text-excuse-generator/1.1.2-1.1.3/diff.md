# Comparing `tmp/text_excuse_generator-1.1.2.tar.gz` & `tmp/text_excuse_generator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_excuse_generator-1.1.2.tar", last modified: Mon Apr 10 06:00:26 2023, max compression
+gzip compressed data, was "text_excuse_generator-1.1.3.tar", last modified: Mon Apr 10 07:40:23 2023, max compression
```

## Comparing `text_excuse_generator-1.1.2.tar` & `text_excuse_generator-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 06:00:26.682911 text_excuse_generator-1.1.2/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.2/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 06:00:26.682599 text_excuse_generator-1.1.2/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 06:00:26.682960 text_excuse_generator-1.1.2/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)      989 2023-04-10 06:00:12.000000 text_excuse_generator-1.1.2/setup.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 06:00:26.681310 text_excuse_generator-1.1.2/text_excuse_generator/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.2/text_excuse_generator/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)    10166 2023-04-10 05:50:44.000000 text_excuse_generator-1.1.2/text_excuse_generator/excuse_generator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 06:00:26.682378 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/top_level.txt
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:40:23.865104 text_excuse_generator-1.1.3/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.3/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:40:23.864934 text_excuse_generator-1.1.3/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 07:40:23.865154 text_excuse_generator-1.1.3/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)      986 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:40:23.864050 text_excuse_generator-1.1.3/text_excuse_generator/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.3/text_excuse_generator/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)    10312 2023-04-10 07:37:07.000000 text_excuse_generator-1.1.3/text_excuse_generator/excuse_generator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:40:23.864714 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 07:40:23.000000 text_excuse_generator-1.1.3/text_excuse_generator.egg-info/top_level.txt
```

### Comparing `text_excuse_generator-1.1.2/LICENSE` & `text_excuse_generator-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.2/PKG-INFO` & `text_excuse_generator-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_excuse_generator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,15 +62,15 @@
 
 You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 #### **Sending a Text Message**
 
 If you want to send a text with command line arguments, run:
 ```bash
-python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]
+python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py Me "Your mom" "I'm late to 😈" "Too many wizards around" -s
 ```
 Omit the `[--send_text_flag]` if you don't want to send the text message.
 
@@ -84,15 +84,15 @@
 python3 text_excuse_generator.py -e "AC1234567890" "1234567890" "+15555555555" "sk-1234567890"
 ```
 
 #### **Saving a New Recipient**
 
 If you want to save a new recipient to the system, run:
 ```bash
-python3 text_excuse_generator.py [-a/--add] [name] [phone_number]
+python3 text_excuse_generator.py [-a/--add] [NAME] [PHONE_NUMBER]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py -a "Your mom" +15555555555
 ```
 
 ### Importing as a Module
@@ -208,15 +208,15 @@
 
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`setup_env()`](#setup_env-takes-in) function in the `text_excuse_generator` module.
 
 ### Running
 
 **YOU HAVE TO INSTALL THE DEPENDENCIES & SETUP THE `.env` FILE BEFORE TRYING TO RUN THE PROGRAM!!!**
 
-Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]` in the command line in the source directory.
+Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]` in the command line in the source directory.
 
 More detailed instructions are in the [Uses](#uses) section.
 
 ## Quality Assurance
 All variable, function, class, module, & file names are written in [snake_case](https://en.wikipedia.org/wiki/Snake_case) to make sure everything is consistent, and all `const` variables are written in ALL-CAPS. The code is also quite commented and the variable names are quite verbose, so it should be easy enough to understand what's going on.
 
 If there are any other/better ways to check for quality assurance, please let me know in the [suggestions](https://github.com/Huckdirks/Excuse_Text_Generator/discussions/new?category=suggestions)!
```

### Comparing `text_excuse_generator-1.1.2/setup.py` & `text_excuse_generator-1.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README_PATH = join(dirname(__file__), "docs/README.md")
 
 with open(README_PATH, "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name = "text_excuse_generator",
-    version = "1.1.2",
+	version = '1.1.3',
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it",
     long_description = LONG_DESCRIPTION,
     long_description_content_type = "text/markdown",
     packages = find_packages(),
     install_requires = ["python-dotenv", "twilio", "openai", "phonenumbers"],
```

### Comparing `text_excuse_generator-1.1.2/text_excuse_generator/excuse_generator.py` & `text_excuse_generator-1.1.3/text_excuse_generator/excuse_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         return False
     
     INDEX = lines.index("# Phone Numbers to text\n")
     lines.insert(INDEX + 1, f"{NEW_RECIPIENT.upper()}_PHONE_NUMBER = \"{PHONE_NUMBER}\"\n")
 
     with open("personal_info.env", "w") as file:
         file.writelines(lines)
-        print(f"Added recipient \'{NEW_RECIPIENT}\' with phone number \'{PHONE_NUMBER}\' to .env file!")
 
+    print(f"Added recipient \'{NEW_RECIPIENT}\' with phone number \'{PHONE_NUMBER}\' to .env file!")
     return True
 
 
 # If the -s or --send flag is given, send the text
 def send_twilio_text(TO_PHONE_NUMBER: str, MESSAGE: str) -> None:
     if not isfile(ENV_PATH):
         print(f"Error: \'{ENV_NAME}\' file not set up! Use the -e or --setup_env flag to set up the .env file")
@@ -138,25 +138,25 @@
         EXCUSE = input("Enter the excuse you want to use: ")
 
         send_text_question = input("Do you want to send the text? (y/n): ")
         if send_text_question.lower() == "y" or send_text_question.lower() == "yes":
             SEND_TEXT = True
 
     else:   # Give info on how to use the program if the wrong # of parameters are given
-        print("\nUsage: python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_flag]")
+        print("\nUsage: python3 text_excuse_generator.py [SENDER] [SENDER] [SENDER] [SENDER] [--send_flag]")
         print("\tsender: The person who is sending the text")
         print("\trecipient: The person you want to text (can be saved person or a phone number)")
         print("\tproblem: The \"problem\" you are having")
         print("\texcuse: The excuse you want to use")
         print("\t--send_flag: If you want to send the text, add -s or --send. If you don't want to send the text, omit this flag\n")
         print("Or just run the program with no arguments to be prompted for input")
         print("Put any parameters longer than a single word in quotes, e.g. \"I'm sick\"\n")
-        print("To add a new recipient to the .env file, run python3 text_excuse_generator.py [-a/--add] [recipient] [PHONE_NUMBER]\n\te.g. python3 text_excuse_generator.py -a \"John Doe\" \"+15555555555\"\n")
+        print("To add a new recipient to the .env file, run python3 text_excuse_generator.py [-a/--add] [RECIPIENT] [PHONE_NUMBER]\n\te.g. python3 text_excuse_generator.py -a \"John Doe\" \"+15555555555\"\n")
         print("To setup the .env file, run python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]\n\te.g. python3 text_excuse_generator.py -e \"AC1234567890abcdef1234567890abcdef\" \"1234567890abcdef1234567890abcdef\" \"+15555555555\" \"1234567890abcdef1234567890abcdef\"\n")
-        print("The prompt sent to ChatGPT is: \"Write a text message to [recipient] explaining that you [problem] because [excuse].\"\n")
+        print("The prompt sent to ChatGPT is: \"Write a text message to [RECIPIENT] explaining that you [PROBLEM] because [EXCUSE]. Also start the message by stating this is [USER], and end the message by telling the recipient to text my actual phone number back if you really need me.\"\n")
         return
         
 
     # If the .env file is not set up, or is empty, return   
     if not isfile(ENV_PATH):
         print(f"Error: \'{ENV_NAME}\' file not set up! Use the -e or --setup_env flag to set up the .env file")
         return
```

### Comparing `text_excuse_generator-1.1.2/text_excuse_generator.egg-info/PKG-INFO` & `text_excuse_generator-1.1.3/text_excuse_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-excuse-generator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,15 +62,15 @@
 
 You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 #### **Sending a Text Message**
 
 If you want to send a text with command line arguments, run:
 ```bash
-python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]
+python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py Me "Your mom" "I'm late to 😈" "Too many wizards around" -s
 ```
 Omit the `[--send_text_flag]` if you don't want to send the text message.
 
@@ -84,15 +84,15 @@
 python3 text_excuse_generator.py -e "AC1234567890" "1234567890" "+15555555555" "sk-1234567890"
 ```
 
 #### **Saving a New Recipient**
 
 If you want to save a new recipient to the system, run:
 ```bash
-python3 text_excuse_generator.py [-a/--add] [name] [phone_number]
+python3 text_excuse_generator.py [-a/--add] [NAME] [PHONE_NUMBER]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py -a "Your mom" +15555555555
 ```
 
 ### Importing as a Module
@@ -208,15 +208,15 @@
 
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`setup_env()`](#setup_env-takes-in) function in the `text_excuse_generator` module.
 
 ### Running
 
 **YOU HAVE TO INSTALL THE DEPENDENCIES & SETUP THE `.env` FILE BEFORE TRYING TO RUN THE PROGRAM!!!**
 
-Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]` in the command line in the source directory.
+Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]` in the command line in the source directory.
 
 More detailed instructions are in the [Uses](#uses) section.
 
 ## Quality Assurance
 All variable, function, class, module, & file names are written in [snake_case](https://en.wikipedia.org/wiki/Snake_case) to make sure everything is consistent, and all `const` variables are written in ALL-CAPS. The code is also quite commented and the variable names are quite verbose, so it should be easy enough to understand what's going on.
 
 If there are any other/better ways to check for quality assurance, please let me know in the [suggestions](https://github.com/Huckdirks/Excuse_Text_Generator/discussions/new?category=suggestions)!
```

