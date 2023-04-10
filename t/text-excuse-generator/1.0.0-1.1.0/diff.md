# Comparing `tmp/text_excuse_generator-1.0.0.tar.gz` & `tmp/text_excuse_generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_excuse_generator-1.0.0.tar", last modified: Mon Apr 10 03:05:31 2023, max compression
+gzip compressed data, was "text_excuse_generator-1.1.0.tar", last modified: Mon Apr 10 04:49:51 2023, max compression
```

## Comparing `text_excuse_generator-1.0.0.tar` & `text_excuse_generator-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 03:05:31.234566 text_excuse_generator-1.0.0/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.0.0/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    10814 2023-04-10 03:05:31.234356 text_excuse_generator-1.0.0/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 03:05:31.234612 text_excuse_generator-1.0.0/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)      989 2023-04-10 02:52:03.000000 text_excuse_generator-1.0.0/setup.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 03:05:31.233539 text_excuse_generator-1.0.0/text_excuse_generator/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:00:20.000000 text_excuse_generator-1.0.0/text_excuse_generator/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)     9827 2023-04-09 22:07:10.000000 text_excuse_generator-1.0.0/text_excuse_generator/text_excuse_generator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 03:05:31.234158 text_excuse_generator-1.0.0/text_excuse_generator.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    10814 2023-04-10 03:05:31.000000 text_excuse_generator-1.0.0/text_excuse_generator.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      321 2023-04-10 03:05:31.000000 text_excuse_generator-1.0.0/text_excuse_generator.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 03:05:31.000000 text_excuse_generator-1.0.0/text_excuse_generator.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 03:05:31.000000 text_excuse_generator-1.0.0/text_excuse_generator.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 03:05:31.000000 text_excuse_generator-1.0.0/text_excuse_generator.egg-info/top_level.txt
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 04:49:51.842603 text_excuse_generator-1.1.0/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.0/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 04:49:51.842408 text_excuse_generator-1.1.0/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 04:49:51.842650 text_excuse_generator-1.1.0/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)      989 2023-04-10 04:48:55.000000 text_excuse_generator-1.1.0/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 04:49:51.840640 text_excuse_generator-1.1.0/text_excuse_generator/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.0/text_excuse_generator/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)    10426 2023-04-10 04:26:02.000000 text_excuse_generator-1.1.0/text_excuse_generator/excuse_generator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 04:49:51.842176 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/top_level.txt
```

### Comparing `text_excuse_generator-1.0.0/LICENSE` & `text_excuse_generator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.0.0/PKG-INFO` & `text_excuse_generator-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_excuse_generator
-Version: 1.0.0
+Version: 1.1.0
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 - [Uses](#uses)
     - [Running from Command Line](#running-from-command-line)
     - [Running with Command Line Arguments](#running-with-command-line-arguments)
         - [Sending a Text Message](#sending-a-text-message)
         - [Setting Up .env File](#setting-up-env-file)
         - [Saving a New Recipient](#saving-a-new-recipient)
     - [Importing as a Module](#importing-as-a-module)
+        - [Installing with pip](#installing-with-pip)
         - [`generate_excuse()`](#generate_excuse-takes-in)
         - [`setup_env()`](#setup_env-takes-in)
         - [`add_recipient()`](#add_recipient-takes-in)
         - [`send_twilio_text()`](#send_twilio_text-takes-in)
 - [Running](#running)
     - [Dependencies](#dependencies)
     - [Setting Up .env File](#setting-up-env-file-1)
@@ -45,23 +46,25 @@
 
 There are three main ways to interact with the program: by running it normally, by running it with command line arguments, or by importing it into another python file.
 
 Note: `[recipient]` can be a name or a case sensitive phone number: e.g. `Huck` or `+15555555555`. You must also set up your .env file (more details in [Dependencies](#setting-up-env-file)).
 
 ### Running from Command Line
 
+I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. You can run it by typing:
 ```bash
 python3 text_excuse_generator.py
 ```
+If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 When you run the program normally, it will ask you for the sender, recipient, problem, and excuse, and if you want to send the text message. It will then generate a text message, and send it to the recipient if chosen. If you input a name into recipient that isn't saved to the system yet when sending a text, it will ask you if you want to save it to the system. If you choose to save it, it will ask you for the phone number, and then save it to the system. You can also just use a phone number for the recipient field, and it will send the text to that number.
 
 ### Running with Command Line Arguments
 
-You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses.
+You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 #### **Sending a Text Message**
 
 If you want to send a text with command line arguments, run:
 ```bash
 python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]
 ```
@@ -92,30 +95,42 @@
 python3 text_excuse_generator.py -a "Your mom" +15555555555
 ```
 
 ### Importing as a Module
 
 You can also import the program as a module into another python file. The `text_excuse_generator` module has  four functions: `generate_excuse()`, `setup_env()`, `add_recipient()`, & `send_twilio_text()`.
 
+#### Installing with pip
+
+Simply run:
+```bash
+pip install text-excuse-generator
+```
+To import the module into your python file, put this at the top of your file:
+```python
+from text_excuse_generator.excuse_generator import *
+```
+Or you can import the individual functions.
+
 #### `generate_excuse()` takes in:
 ```python
 generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> str
 ```
 `generate_excuse()` returns a string of the text message that was generated.
 
 If you want to generate a text message, call the function like this:
 
 ```python
 generate_excuse("user", "recipient", "problem", "excuse", True)
 ```
 e.g.
 ```python
-generate_excuse("me", "your mom", "I'm late to 😈", "Too many wizards around", True)
+generate_excuse(user = "me", recipient = "your mom", problem = "I'm late to 😈", excuse = "Too many wizards around", send_text = True)
 ```
-Omit the `[--send_text_flag]` if you don't want to send the text message.
+Make sure to put the fields before the variables when calling the function. Omit the `[--send_text_flag]` if you don't want to send the text message.
 
 #### `setup_env()` takes in:
 ```python
 setup_env(TWILIO_ACCOUNT_SID: str, TWILIO_AUTH_TOKEN: str, TWILIO_PHONE_NUMBER: str, OPENAI_API_KEY: str) -> bool
 ```
 If you want to set up your .env file, call `setup_env()` like this:
 ```python
@@ -171,16 +186,26 @@
 
 And this information from OpenAI:
 - OpenAI API Key
 
 And then [set up the `.env` file](#setting-up-env-file-1) with this information.
 #### Install
 
+##### For Command Line Use
+
 Double click [`dependencies`](../dependencies), or run `bash `[`dependencies`](../dependencies) or `./`[`dependencies`](../dependencies) in the root directory or to install the python dependencies. You must have [pip](https://pip.pypa.io/en/stable/installation/) installed to download the new dependencies. Also, you'll need to install [python](https://www.python.org/downloads/) yourself if you haven't already.
 
+##### For Importing as a Module
+
+If you just run:
+```bash
+pip install text-excuse-generator
+```
+The dependencies will be installed automatically, along with the rest of the module!
+
 **[List of Dependencies](DEPENDENCIES.md)**
 
 ### Setting Up .env File
 
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`setup_env()`](#setup_env-takes-in) function in the `text_excuse_generator` module.
 
 ### Running
```

### Comparing `text_excuse_generator-1.0.0/setup.py` & `text_excuse_generator-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README_PATH = join(dirname(__file__), "docs/README.md")
 
 with open(README_PATH, "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name = "text_excuse_generator",
-    version = "1.0.0",
+    version = "1.1.0",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it",
     long_description = LONG_DESCRIPTION,
     long_description_content_type = "text/markdown",
     packages = find_packages(),
     install_requires = ["python-dotenv", "twilio", "openai", "phonenumbers"],
```

### Comparing `text_excuse_generator-1.0.0/text_excuse_generator/text_excuse_generator.py` & `text_excuse_generator-1.1.0/text_excuse_generator/excuse_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,72 +6,73 @@
 
 # Python Libraries
 from os import getenv
 from os.path import dirname, join, isfile
 from sys import argv
 
 # Constants
-ENV_NAME = "personal_info"  # CHANGE THIS TO YOUR ENVIRONMENT NAME (.env file)
-ENV_PATH = join(dirname(__file__), f"{ENV_NAME}.env")
+ENV_NAME = "personal_info.env"  # CHANGE THIS TO YOUR ENVIRONMENT NAME (.env file)
+ENV_PATH = join(dirname(__file__), ENV_NAME)
 
 
 # Set up .env file
 def setup_env(TWILIO_ACCOUNT_SID: str, TWILIO_AUTH_TOKEN: str, TWILIO_PHONE_NUMBER: str, OPENAI_API_KEY: str) -> bool:
+    print(ENV_PATH)
     # Check if .env file exists and not empty
-    if isfile(f"{ENV_NAME}.env"):
-        print(f"Error: \'{ENV_NAME}.env\' file already set up!")
+    if isfile(ENV_PATH):
+        print(f"Error: \'{ENV_NAME}\' file already set up!")
         return False
     
     if not is_valid_number(parse(TWILIO_PHONE_NUMBER)):
         print("Error: Invalid phone number!")
         return False
 
     # Set up the .env file
-    lines = ["# Twilio API\n", f"TWILIO_ACCOUNT_SID = {TWILIO_ACCOUNT_SID}\n", f"TWILIO_AUTH_TOKEN = {TWILIO_AUTH_TOKEN}\n", f"TWILIO_PHONE_NUMBER = {TWILIO_PHONE_NUMBER}\n", "\n", "# OpenAI API\n", f"OPENAI_API_KEY = {OPENAI_API_KEY}\n", "\n", "# Phone Numbers to text\n"]
+    LINES = ["# Twilio API\n", f"TWILIO_ACCOUNT_SID = {TWILIO_ACCOUNT_SID}\n", f"TWILIO_AUTH_TOKEN = {TWILIO_AUTH_TOKEN}\n", f"TWILIO_PHONE_NUMBER = {TWILIO_PHONE_NUMBER}\n", "\n", "# OpenAI API\n", f"OPENAI_API_KEY = {OPENAI_API_KEY}\n", "\n", "# Phone Numbers to text\n"]
 
     # Write to the .env file
-    with open(f"{ENV_NAME}.env", "w") as file:
-        file.writelines(lines)
+    with open(ENV_PATH, "w") as file:
+        file.writelines(LINES)
 
-    print(f"Set up \'{ENV_NAME}.env\' file!")
+    print(f"Set up \'{ENV_NAME}\' file!")
     return True
 
 
 # Save a phone number to the .env file
 def add_recipient(RECIPIENT: str, PHONE_NUMBER: str) -> bool:
     if not is_valid_number(parse(PHONE_NUMBER)):
         print("Error: Invalid phone number!")
         return False
     
     # Replace spaces with underscores for formatting
     NEW_RECIPIENT = RECIPIENT.replace(" ", "_")
     lines = []
     
     # Add a new user to the .env file
-    with open(f"{ENV_NAME}.env", "r") as file:
+    with open(f"{ENV_NAME}", "r") as file:
         lines = file.readlines()
 
     if f"{NEW_RECIPIENT.upper()}_PHONE_NUMBER" in lines:
         print(f"Error: Recipient \'{NEW_RECIPIENT}\' already exists in .env file! Manually edit the .env file if you want to change the phone number.")
         return False
     
-    index = lines.index("# Phone Numbers to text\n")
-    lines.insert(index + 1, f"{NEW_RECIPIENT.upper()}_PHONE_NUMBER = \"{PHONE_NUMBER}\"\n")
+    INDEX = lines.index("# Phone Numbers to text\n")
+    lines.insert(INDEX + 1, f"{NEW_RECIPIENT.upper()}_PHONE_NUMBER = \"{PHONE_NUMBER}\"\n")
 
     with open("personal_info.env", "w") as file:
         file.writelines(lines)
         print(f"Added recipient \'{NEW_RECIPIENT}\' with phone number \'{PHONE_NUMBER}\' to .env file!")
 
     return True
 
 
 # If the -s or --send flag is given, send the text
 def send_twilio_text(TO_PHONE_NUMBER: str, MESSAGE: str) -> None:
     if not isfile(ENV_PATH):
-        print(f"Error: \'{ENV_NAME}.env\' file not set up! Use the -e or --setup_env flag to set up the .env file")
+        print(f"Error: \'{ENV_NAME}\' file not set up! Use the -e or --setup_env flag to set up the .env file")
         return
     
     # Load the .env file
     load_dotenv(ENV_PATH)
 
     print("Sending text...")
     # Twilio API
@@ -83,113 +84,127 @@
     )
     
     print("Text sent!")
     return
 
 
 # Generate an excuse and text it to a recipient. If no parameters are given, either by being passed in or given via the Command Line, it will prompt the user for input
-def generate_excuse(user: str = "", recipient: str = "", problem: str = "", excuse: str = "", send_text: bool = False) -> str:
-    if not user or recipient or problem or excuse:  # If no parameters are given
+def generate_excuse(**kwargs) -> str:
+    #if not user or recipient or problem or excuse:  # If no parameters are given
+    if not kwargs:  # If no parameters are given
         if len(argv) == 4 or len(argv) == 5 or len(argv) == 6:        # If command line arguments are given, use them
             if len(argv) == 4 and (argv[1].lower() == "-a" or argv[1].lower() == "--add"):  # If the -a or --add flag is given with correct parameters, and correct # of parameters are passed in
                 add_recipient(argv[2], argv[3])
                 return
             elif (len(argv) == 6 and (argv[1].lower() == "-e" or argv[1].lower() == "--setup_env")):   # If the -e or --setup_env flag is given with correct parameters, and correct # of parameters are passed in
                 setup_env(argv[2], argv[3], argv[4], argv[5])
                 return
             
             # Load command line arguments
-            user = argv[1]
-            recipient = argv[2]
-            problem = argv[3]
-            excuse = argv[4]
+            USER = argv[1]
+            RECIPIENT = argv[2]
+            PROBLEM = argv[3]
+            EXCUSE = argv[4]
             if len(argv) == 6 and (argv[5].lower() == "-s" or argv[5].lower() == "--send"):
-                send_text = True
+                SEND_TEXT = True
             elif len(argv) == 6:
                 print("\nError: Invalid flag given! Use -s or --send to send the text")
                 return
 
         elif len(argv) == 1:    # If no arguments are given, ask for user input
             if not isfile(ENV_PATH):  # If the .env file is not set up, ask the user if they want to set it up
-                set_up_env_question = input(f"Error: \'{ENV_NAME}.env\' file not set up!\nDo you want to set it up now? (y/n): ")
-                if not set_up_env_question.lower() == "y" or not set_up_env_question.lower() == "yes":
+                set_up_env_question = input(f"Error: \'{ENV_NAME}\' file not set up!\nDo you want to set it up now? (y/n): ")
+                if set_up_env_question.lower() == "y" or set_up_env_question.lower() == "yes":
+                    TWILIO_ACCOUNT_SID = input("Enter your Twilio Account SID: ")
+                    TWILIO_AUTH_TOKEN = input("Enter your Twilio Auth Token: ")
+                    TWILIO_PHONE_NUMBER = input("Enter your Twilio Phone Number: ")
+                    OPENAI_API_KEY = input("Enter your OpenAI API Key: ")
+                    if not setup_env(TWILIO_ACCOUNT_SID, TWILIO_AUTH_TOKEN, TWILIO_PHONE_NUMBER, OPENAI_API_KEY):
+                        return
+                else:
+                    print("Error: Cannot generate an EXCUSE without setting up the .env file!")
                     return
-                
-                TWILIO_ACCOUNT_SID = input("Enter your Twilio Account SID: ")
-                TWILIO_AUTH_TOKEN = input("Enter your Twilio Auth Token: ")
-                TWILIO_PHONE_NUMBER = input("Enter your Twilio Phone Number: ")
-                OPENAI_API_KEY = input("Enter your OpenAI API Key: ")
-                setup_env(TWILIO_ACCOUNT_SID, TWILIO_AUTH_TOKEN, TWILIO_PHONE_NUMBER, OPENAI_API_KEY)
             
-            user = input("Enter who is sending the text: ")
-            recipient = input("Enter who you want to text: ")
-            problem = input("Enter the fake problem you are having: ")
-            excuse = input("Enter the excuse you want to use: ")
+            USER = input("Enter who is sending the text: ")
+            RECIPIENT = input("Enter who you want to text: ")
+            PROBLEM = input("Enter the fake problem you are having: ")
+            EXCUSE = input("Enter the excuse you want to use: ")
 
             send_text_question = input("Do you want to send the text? (y/n): ")
             if send_text_question.lower() == "y" or send_text_question.lower() == "yes":
-                send_text = True
+                SEND_TEXT = True
 
         else:   # Give info on how to use the program
             print("\nUsage: python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_flag]")
             print("\tsender: The person who is sending the text")
             print("\trecipient: The person you want to text (can be saved person or a phone number)")
             print("\tproblem: The \"problem\" you are having")
             print("\texcuse: The excuse you want to use")
             print("\t--send_flag: If you want to send the text, add -s or --send. If you don't want to send the text, omit this flag\n")
             print("Or just run the program with no arguments to be prompted for input")
             print("Put any parameters longer than a single word in quotes, e.g. \"I'm sick\"\n")
             print("To add a new recipient to the .env file, run python3 text_excuse_generator.py [-a/--add] [recipient] [PHONE_NUMBER]\n\te.g. python3 text_excuse_generator.py -a \"John Doe\" \"+15555555555\"\n")
             print("To setup the .env file, run python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]\n\te.g. python3 text_excuse_generator.py -e \"AC1234567890abcdef1234567890abcdef\" \"1234567890abcdef1234567890abcdef\" \"+15555555555\" \"1234567890abcdef1234567890abcdef\"\n")
             print("The prompt sent to ChatGPT is: \"Write a text message to [recipient] explaining that you [problem] because [excuse].\"\n")
             return
+        
+    else:   # If parameters are given
+        USER = kwargs["user"]
+        RECIPIENT = kwargs["recipient"]
+        PROBLEM = kwargs["problem"]
+        EXCUSE = kwargs["excuse"]
+        if "send_text" in kwargs:
+            SEND_TEXT = kwargs["send_text"]
+        if not USER or not RECIPIENT or not PROBLEM or not EXCUSE:
+            print("Error: All parameters must be given!\nUsage: generate_excuse(user = \"\", recipient = \"\", problem = \"\", excuse = \"\", send_text = True)")
+            return
 
     # If the .env file is not set up, or is empty, return   
     if not isfile(ENV_PATH):
-        print(f"Error: \'{ENV_NAME}.env\' file not set up! Use the -e or --setup_env flag to set up the .env file")
+        print(f"Error: \'{ENV_NAME}\' file not set up! Use the -e or --setup_env flag to set up the .env file")
         return
     
     # Load the .env file
     load_dotenv(ENV_PATH)
 
     to_phone_number = ""
-    if (recipient[0] == '+' and recipient[1:].isnumeric()) and is_valid_number(parse(recipient)):   # Check if recipient is a phone number
-        to_phone_number = recipient
-    elif send_text:
-        RECIPIENT_FORMATTED = recipient.replace(" ", "_")
+    if (RECIPIENT[0] == '+' and RECIPIENT[1:].isnumeric()) and is_valid_number(parse(RECIPIENT)):   # Check if RECIPIENT is a phone number
+        to_phone_number = RECIPIENT
+    elif SEND_TEXT:
+        RECIPIENT_FORMATTED = RECIPIENT.replace(" ", "_")
         to_phone_number = getenv(f"{RECIPIENT_FORMATTED.upper()}_PHONE_NUMBER")
         if to_phone_number == None: # If the recipient is not in the .env file
-            print(f"\nError: No phone number found for recipient \'{recipient}\' in .env file!")
+            print(f"\nError: No phone number found for recipient \'{RECIPIENT}\' in .env file!")
             if len(argv) != 1:  # If not in user input mode, exit, else ask if they want to add the recipient
                 return
             
             # Ask if they want to add the recipient
             ADD_RECIPIENT_QUESTION = input("Do you want to add this recipient to the .env file? (y/n): ")
             if not ADD_RECIPIENT_QUESTION.lower() == "y" or not ADD_RECIPIENT_QUESTION.lower() == "yes":
                 return
             
             to_phone_number = input("Enter the phone number of the recipient: ")
-            if not add_recipient(recipient, to_phone_number):   # If the recipient could not be added
+            if not add_recipient(RECIPIENT, to_phone_number):   # If the recipient could not be added
                 return
 
     # Create the message (AI Time!)
-    CHATGPT_CONTEXT = f"Write a text message to {recipient} explaining that you {problem} because {excuse}. Also start the message by stating this is {user}, and end the message by telling the recipient to text my actual phone number back if you really need me."
+    CHATGPT_CONTEXT = f"Write a text message to {RECIPIENT} explaining that you {PROBLEM} because {EXCUSE}. Also start the message by stating this is {USER}, and end the message by telling the recipient to text my actual phone number back if you really need me."
     print("\nCreating message...\n")
 
     # OpenAI API
     openai.api_key = getenv("OPENAI_API_KEY")
     AI_QUERY = openai.ChatCompletion.create(
         model = "gpt-3.5-turbo",
         messages = [{"role": "user", "content": CHATGPT_CONTEXT}]
     )
 
     AI_RESPONSE = AI_QUERY.choices[0].message.content
     print(f"Chat GPT's Response:\n{AI_RESPONSE}\n")
 
-    if send_text:   # If the -s or --send flag is given, send the text
+    if SEND_TEXT:   # If the -s or --send flag is given, send the text
         send_twilio_text(to_phone_number, AI_RESPONSE)
 
     return AI_RESPONSE
 
 
 if __name__ == "__main__":
     generate_excuse()
```

### Comparing `text_excuse_generator-1.0.0/text_excuse_generator.egg-info/PKG-INFO` & `text_excuse_generator-1.1.0/text_excuse_generator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-excuse-generator
-Version: 1.0.0
+Version: 1.1.0
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 - [Uses](#uses)
     - [Running from Command Line](#running-from-command-line)
     - [Running with Command Line Arguments](#running-with-command-line-arguments)
         - [Sending a Text Message](#sending-a-text-message)
         - [Setting Up .env File](#setting-up-env-file)
         - [Saving a New Recipient](#saving-a-new-recipient)
     - [Importing as a Module](#importing-as-a-module)
+        - [Installing with pip](#installing-with-pip)
         - [`generate_excuse()`](#generate_excuse-takes-in)
         - [`setup_env()`](#setup_env-takes-in)
         - [`add_recipient()`](#add_recipient-takes-in)
         - [`send_twilio_text()`](#send_twilio_text-takes-in)
 - [Running](#running)
     - [Dependencies](#dependencies)
     - [Setting Up .env File](#setting-up-env-file-1)
@@ -45,23 +46,25 @@
 
 There are three main ways to interact with the program: by running it normally, by running it with command line arguments, or by importing it into another python file.
 
 Note: `[recipient]` can be a name or a case sensitive phone number: e.g. `Huck` or `+15555555555`. You must also set up your .env file (more details in [Dependencies](#setting-up-env-file)).
 
 ### Running from Command Line
 
+I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. You can run it by typing:
 ```bash
 python3 text_excuse_generator.py
 ```
+If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 When you run the program normally, it will ask you for the sender, recipient, problem, and excuse, and if you want to send the text message. It will then generate a text message, and send it to the recipient if chosen. If you input a name into recipient that isn't saved to the system yet when sending a text, it will ask you if you want to save it to the system. If you choose to save it, it will ask you for the phone number, and then save it to the system. You can also just use a phone number for the recipient field, and it will send the text to that number.
 
 ### Running with Command Line Arguments
 
-You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses.
+You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 #### **Sending a Text Message**
 
 If you want to send a text with command line arguments, run:
 ```bash
 python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]
 ```
@@ -92,30 +95,42 @@
 python3 text_excuse_generator.py -a "Your mom" +15555555555
 ```
 
 ### Importing as a Module
 
 You can also import the program as a module into another python file. The `text_excuse_generator` module has  four functions: `generate_excuse()`, `setup_env()`, `add_recipient()`, & `send_twilio_text()`.
 
+#### Installing with pip
+
+Simply run:
+```bash
+pip install text-excuse-generator
+```
+To import the module into your python file, put this at the top of your file:
+```python
+from text_excuse_generator.excuse_generator import *
+```
+Or you can import the individual functions.
+
 #### `generate_excuse()` takes in:
 ```python
 generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> str
 ```
 `generate_excuse()` returns a string of the text message that was generated.
 
 If you want to generate a text message, call the function like this:
 
 ```python
 generate_excuse("user", "recipient", "problem", "excuse", True)
 ```
 e.g.
 ```python
-generate_excuse("me", "your mom", "I'm late to 😈", "Too many wizards around", True)
+generate_excuse(user = "me", recipient = "your mom", problem = "I'm late to 😈", excuse = "Too many wizards around", send_text = True)
 ```
-Omit the `[--send_text_flag]` if you don't want to send the text message.
+Make sure to put the fields before the variables when calling the function. Omit the `[--send_text_flag]` if you don't want to send the text message.
 
 #### `setup_env()` takes in:
 ```python
 setup_env(TWILIO_ACCOUNT_SID: str, TWILIO_AUTH_TOKEN: str, TWILIO_PHONE_NUMBER: str, OPENAI_API_KEY: str) -> bool
 ```
 If you want to set up your .env file, call `setup_env()` like this:
 ```python
@@ -171,16 +186,26 @@
 
 And this information from OpenAI:
 - OpenAI API Key
 
 And then [set up the `.env` file](#setting-up-env-file-1) with this information.
 #### Install
 
+##### For Command Line Use
+
 Double click [`dependencies`](../dependencies), or run `bash `[`dependencies`](../dependencies) or `./`[`dependencies`](../dependencies) in the root directory or to install the python dependencies. You must have [pip](https://pip.pypa.io/en/stable/installation/) installed to download the new dependencies. Also, you'll need to install [python](https://www.python.org/downloads/) yourself if you haven't already.
 
+##### For Importing as a Module
+
+If you just run:
+```bash
+pip install text-excuse-generator
+```
+The dependencies will be installed automatically, along with the rest of the module!
+
 **[List of Dependencies](DEPENDENCIES.md)**
 
 ### Setting Up .env File
 
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`setup_env()`](#setup_env-takes-in) function in the `text_excuse_generator` module.
 
 ### Running
```

