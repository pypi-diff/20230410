# Comparing `tmp/text_excuse_generator-1.1.1.tar.gz` & `tmp/text_excuse_generator-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_excuse_generator-1.1.1.tar", last modified: Mon Apr 10 05:25:49 2023, max compression
+gzip compressed data, was "text_excuse_generator-1.1.2.tar", last modified: Mon Apr 10 06:00:26 2023, max compression
```

## Comparing `text_excuse_generator-1.1.1.tar` & `text_excuse_generator-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 05:25:49.168624 text_excuse_generator-1.1.1/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.1/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 05:25:49.168417 text_excuse_generator-1.1.1/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 05:25:49.168671 text_excuse_generator-1.1.1/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)      989 2023-04-10 05:25:14.000000 text_excuse_generator-1.1.1/setup.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 05:25:49.167595 text_excuse_generator-1.1.1/text_excuse_generator/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.1/text_excuse_generator/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)    10439 2023-04-10 05:20:50.000000 text_excuse_generator-1.1.1/text_excuse_generator/excuse_generator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 05:25:49.168196 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/top_level.txt
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 06:00:26.682911 text_excuse_generator-1.1.2/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.2/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 06:00:26.682599 text_excuse_generator-1.1.2/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 06:00:26.682960 text_excuse_generator-1.1.2/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)      989 2023-04-10 06:00:12.000000 text_excuse_generator-1.1.2/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 06:00:26.681310 text_excuse_generator-1.1.2/text_excuse_generator/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.2/text_excuse_generator/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)    10166 2023-04-10 05:50:44.000000 text_excuse_generator-1.1.2/text_excuse_generator/excuse_generator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 06:00:26.682378 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 06:00:26.000000 text_excuse_generator-1.1.2/text_excuse_generator.egg-info/top_level.txt
```

### Comparing `text_excuse_generator-1.1.1/LICENSE` & `text_excuse_generator-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.1/PKG-INFO` & `text_excuse_generator-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_excuse_generator
-Version: 1.1.1
+Version: 1.1.2
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `text_excuse_generator-1.1.1/setup.py` & `text_excuse_generator-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README_PATH = join(dirname(__file__), "docs/README.md")
 
 with open(README_PATH, "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name = "text_excuse_generator",
-    version = "1.1.1",
+    version = "1.1.2",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it",
     long_description = LONG_DESCRIPTION,
     long_description_content_type = "text/markdown",
     packages = find_packages(),
     install_requires = ["python-dotenv", "twilio", "openai", "phonenumbers"],
```

### Comparing `text_excuse_generator-1.1.1/text_excuse_generator/excuse_generator.py` & `text_excuse_generator-1.1.2/text_excuse_generator/excuse_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,82 +84,81 @@
     
     print("Text sent!")
     return
 
 
 # Generate an excuse and text it to a recipient. If no parameters are given, either by being passed in or given via the Command Line, it will prompt the user for input
 def generate_excuse(**kwargs) -> str:
-    #if not user or recipient or problem or excuse:  # If no parameters are given
-    if not kwargs:  # If no parameters are given
-        if len(argv) == 4 or len(argv) == 5 or len(argv) == 6:        # If command line arguments are given, use them
-            if len(argv) == 4 and (argv[1].lower() == "-a" or argv[1].lower() == "--add"):  # If the -a or --add flag is given with correct parameters, and correct # of parameters are passed in
-                add_recipient(argv[2], argv[3])
-                return
-            elif (len(argv) == 6 and (argv[1].lower() == "-e" or argv[1].lower() == "--setup_env")):   # If the -e or --setup_env flag is given with correct parameters, and correct # of parameters are passed in
-                setup_env(argv[2], argv[3], argv[4], argv[5])
-                return
-            
-            # Load command line arguments
-            USER = argv[1]
-            RECIPIENT = argv[2]
-            PROBLEM = argv[3]
-            EXCUSE = argv[4]
-            if len(argv) == 6 and (argv[5].lower() == "-s" or argv[5].lower() == "--send"):
-                SEND_TEXT = True
-            elif len(argv) == 6:
-                print("\nError: Invalid flag given! Use -s or --send to send the text")
-                return
-
-        elif len(argv) == 1:    # If no arguments are given, ask for user input
-            if not isfile(ENV_PATH):  # If the .env file is not set up, ask the user if they want to set it up
-                set_up_env_question = input(f"Error: \'{ENV_NAME}\' file not set up!\nDo you want to set it up now? (y/n): ")
-                if set_up_env_question.lower() == "y" or set_up_env_question.lower() == "yes":
-                    TWILIO_ACCOUNT_SID = input("Enter your Twilio Account SID: ")
-                    TWILIO_AUTH_TOKEN = input("Enter your Twilio Auth Token: ")
-                    TWILIO_PHONE_NUMBER = input("Enter your Twilio Phone Number: ")
-                    OPENAI_API_KEY = input("Enter your OpenAI API Key: ")
-                    if not setup_env(TWILIO_ACCOUNT_SID, TWILIO_AUTH_TOKEN, TWILIO_PHONE_NUMBER, OPENAI_API_KEY):
-                        return
-                else:
-                    print("Error: Cannot generate an EXCUSE without setting up the .env file!")
-                    return
-            
-            USER = input("Enter who is sending the text: ")
-            RECIPIENT = input("Enter who you want to text: ")
-            PROBLEM = input("Enter the fake problem you are having: ")
-            EXCUSE = input("Enter the excuse you want to use: ")
-
-            send_text_question = input("Do you want to send the text? (y/n): ")
-            if send_text_question.lower() == "y" or send_text_question.lower() == "yes":
-                SEND_TEXT = True
-
-        else:   # Give info on how to use the program
-            print("\nUsage: python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_flag]")
-            print("\tsender: The person who is sending the text")
-            print("\trecipient: The person you want to text (can be saved person or a phone number)")
-            print("\tproblem: The \"problem\" you are having")
-            print("\texcuse: The excuse you want to use")
-            print("\t--send_flag: If you want to send the text, add -s or --send. If you don't want to send the text, omit this flag\n")
-            print("Or just run the program with no arguments to be prompted for input")
-            print("Put any parameters longer than a single word in quotes, e.g. \"I'm sick\"\n")
-            print("To add a new recipient to the .env file, run python3 text_excuse_generator.py [-a/--add] [recipient] [PHONE_NUMBER]\n\te.g. python3 text_excuse_generator.py -a \"John Doe\" \"+15555555555\"\n")
-            print("To setup the .env file, run python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]\n\te.g. python3 text_excuse_generator.py -e \"AC1234567890abcdef1234567890abcdef\" \"1234567890abcdef1234567890abcdef\" \"+15555555555\" \"1234567890abcdef1234567890abcdef\"\n")
-            print("The prompt sent to ChatGPT is: \"Write a text message to [recipient] explaining that you [problem] because [excuse].\"\n")
-            return
-        
-    else:   # If parameters are given
+    if kwargs:  # If parameters are passed in
         USER = kwargs["user"]
         RECIPIENT = kwargs["recipient"]
         PROBLEM = kwargs["problem"]
         EXCUSE = kwargs["excuse"]
         if "send_text" in kwargs:
             SEND_TEXT = kwargs["send_text"]
         if not USER or not RECIPIENT or not PROBLEM or not EXCUSE:
             print("Error: All parameters must be given!\nUsage: generate_excuse(user = \"\", recipient = \"\", problem = \"\", excuse = \"\", send_text = True)")
             return
+        
+    elif len(argv) == 4 or len(argv) == 5 or len(argv) == 6:        # If command line arguments are given, use them
+        if len(argv) == 4 and (argv[1].lower() == "-a" or argv[1].lower() == "--add"):  # If the -a or --add flag is given with correct parameters, and correct # of parameters are passed in
+            add_recipient(argv[2], argv[3])
+            return
+        elif (len(argv) == 6 and (argv[1].lower() == "-e" or argv[1].lower() == "--setup_env")):   # If the -e or --setup_env flag is given with correct parameters, and correct # of parameters are passed in
+            setup_env(argv[2], argv[3], argv[4], argv[5])
+            return
+            
+        # Load command line arguments
+        USER = argv[1]
+        RECIPIENT = argv[2]
+        PROBLEM = argv[3]
+        EXCUSE = argv[4]
+        if len(argv) == 6 and (argv[5].lower() == "-s" or argv[5].lower() == "--send"):
+            SEND_TEXT = True
+        elif len(argv) == 6:
+            print("\nError: Invalid flag given! Use -s or --send to send the text")
+            return
+
+    elif len(argv) == 1:    # If no arguments are given, ask for user input
+        if not isfile(ENV_PATH):  # If the .env file is not set up, ask the user if they want to set it up
+            set_up_env_question = input(f"Error: \'{ENV_NAME}\' file not set up!\nDo you want to set it up now? (y/n): ")
+            if set_up_env_question.lower() == "y" or set_up_env_question.lower() == "yes":
+                TWILIO_ACCOUNT_SID = input("Enter your Twilio Account SID: ")
+                TWILIO_AUTH_TOKEN = input("Enter your Twilio Auth Token: ")
+                TWILIO_PHONE_NUMBER = input("Enter your Twilio Phone Number: ")
+                OPENAI_API_KEY = input("Enter your OpenAI API Key: ")
+                if not setup_env(TWILIO_ACCOUNT_SID, TWILIO_AUTH_TOKEN, TWILIO_PHONE_NUMBER, OPENAI_API_KEY):
+                    return
+            else:
+                print("Error: Cannot generate an EXCUSE without setting up the .env file!")
+                return
+            
+        USER = input("Enter who is sending the text: ")
+        RECIPIENT = input("Enter who you want to text: ")
+        PROBLEM = input("Enter the fake problem you are having: ")
+        EXCUSE = input("Enter the excuse you want to use: ")
+
+        send_text_question = input("Do you want to send the text? (y/n): ")
+        if send_text_question.lower() == "y" or send_text_question.lower() == "yes":
+            SEND_TEXT = True
+
+    else:   # Give info on how to use the program if the wrong # of parameters are given
+        print("\nUsage: python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_flag]")
+        print("\tsender: The person who is sending the text")
+        print("\trecipient: The person you want to text (can be saved person or a phone number)")
+        print("\tproblem: The \"problem\" you are having")
+        print("\texcuse: The excuse you want to use")
+        print("\t--send_flag: If you want to send the text, add -s or --send. If you don't want to send the text, omit this flag\n")
+        print("Or just run the program with no arguments to be prompted for input")
+        print("Put any parameters longer than a single word in quotes, e.g. \"I'm sick\"\n")
+        print("To add a new recipient to the .env file, run python3 text_excuse_generator.py [-a/--add] [recipient] [PHONE_NUMBER]\n\te.g. python3 text_excuse_generator.py -a \"John Doe\" \"+15555555555\"\n")
+        print("To setup the .env file, run python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]\n\te.g. python3 text_excuse_generator.py -e \"AC1234567890abcdef1234567890abcdef\" \"1234567890abcdef1234567890abcdef\" \"+15555555555\" \"1234567890abcdef1234567890abcdef\"\n")
+        print("The prompt sent to ChatGPT is: \"Write a text message to [recipient] explaining that you [problem] because [excuse].\"\n")
+        return
+        
 
     # If the .env file is not set up, or is empty, return   
     if not isfile(ENV_PATH):
         print(f"Error: \'{ENV_NAME}\' file not set up! Use the -e or --setup_env flag to set up the .env file")
         return
     
     # Load the .env file
```

### Comparing `text_excuse_generator-1.1.1/text_excuse_generator.egg-info/PKG-INFO` & `text_excuse_generator-1.1.2/text_excuse_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-excuse-generator
-Version: 1.1.1
+Version: 1.1.2
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

