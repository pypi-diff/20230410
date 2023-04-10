# Comparing `tmp/text_excuse_generator-1.1.0.tar.gz` & `tmp/text_excuse_generator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_excuse_generator-1.1.0.tar", last modified: Mon Apr 10 04:49:51 2023, max compression
+gzip compressed data, was "text_excuse_generator-1.1.1.tar", last modified: Mon Apr 10 05:25:49 2023, max compression
```

## Comparing `text_excuse_generator-1.1.0.tar` & `text_excuse_generator-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 04:49:51.842603 text_excuse_generator-1.1.0/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.0/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 04:49:51.842408 text_excuse_generator-1.1.0/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 04:49:51.842650 text_excuse_generator-1.1.0/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)      989 2023-04-10 04:48:55.000000 text_excuse_generator-1.1.0/setup.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 04:49:51.840640 text_excuse_generator-1.1.0/text_excuse_generator/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.0/text_excuse_generator/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)    10426 2023-04-10 04:26:02.000000 text_excuse_generator-1.1.0/text_excuse_generator/excuse_generator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 04:49:51.842176 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 04:49:51.000000 text_excuse_generator-1.1.0/text_excuse_generator.egg-info/top_level.txt
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 05:25:49.168624 text_excuse_generator-1.1.1/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.1/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 05:25:49.168417 text_excuse_generator-1.1.1/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 05:25:49.168671 text_excuse_generator-1.1.1/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)      989 2023-04-10 05:25:14.000000 text_excuse_generator-1.1.1/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 05:25:49.167595 text_excuse_generator-1.1.1/text_excuse_generator/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.1/text_excuse_generator/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)    10439 2023-04-10 05:20:50.000000 text_excuse_generator-1.1.1/text_excuse_generator/excuse_generator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 05:25:49.168196 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 05:25:49.000000 text_excuse_generator-1.1.1/text_excuse_generator.egg-info/top_level.txt
```

### Comparing `text_excuse_generator-1.1.0/LICENSE` & `text_excuse_generator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.0/PKG-INFO` & `text_excuse_generator-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_excuse_generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `text_excuse_generator-1.1.0/setup.py` & `text_excuse_generator-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README_PATH = join(dirname(__file__), "docs/README.md")
 
 with open(README_PATH, "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name = "text_excuse_generator",
-    version = "1.1.0",
+    version = "1.1.1",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it",
     long_description = LONG_DESCRIPTION,
     long_description_content_type = "text/markdown",
     packages = find_packages(),
     install_requires = ["python-dotenv", "twilio", "openai", "phonenumbers"],
```

### Comparing `text_excuse_generator-1.1.0/text_excuse_generator/excuse_generator.py` & `text_excuse_generator-1.1.1/text_excuse_generator/excuse_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # Constants
 ENV_NAME = "personal_info.env"  # CHANGE THIS TO YOUR ENVIRONMENT NAME (.env file)
 ENV_PATH = join(dirname(__file__), ENV_NAME)
 
 
 # Set up .env file
 def setup_env(TWILIO_ACCOUNT_SID: str, TWILIO_AUTH_TOKEN: str, TWILIO_PHONE_NUMBER: str, OPENAI_API_KEY: str) -> bool:
-    print(ENV_PATH)
     # Check if .env file exists and not empty
     if isfile(ENV_PATH):
         print(f"Error: \'{ENV_NAME}\' file already set up!")
         return False
     
     if not is_valid_number(parse(TWILIO_PHONE_NUMBER)):
         print("Error: Invalid phone number!")
@@ -170,24 +169,24 @@
     if (RECIPIENT[0] == '+' and RECIPIENT[1:].isnumeric()) and is_valid_number(parse(RECIPIENT)):   # Check if RECIPIENT is a phone number
         to_phone_number = RECIPIENT
     elif SEND_TEXT:
         RECIPIENT_FORMATTED = RECIPIENT.replace(" ", "_")
         to_phone_number = getenv(f"{RECIPIENT_FORMATTED.upper()}_PHONE_NUMBER")
         if to_phone_number == None: # If the recipient is not in the .env file
             print(f"\nError: No phone number found for recipient \'{RECIPIENT}\' in .env file!")
-            if len(argv) != 1:  # If not in user input mode, exit, else ask if they want to add the recipient
+            if len(argv) != 1 or not len(kwargs) == 0:  # If not in user input mode, exit, else ask if they want to add the recipient
                 return
             
             # Ask if they want to add the recipient
             ADD_RECIPIENT_QUESTION = input("Do you want to add this recipient to the .env file? (y/n): ")
-            if not ADD_RECIPIENT_QUESTION.lower() == "y" or not ADD_RECIPIENT_QUESTION.lower() == "yes":
-                return
-            
-            to_phone_number = input("Enter the phone number of the recipient: ")
-            if not add_recipient(RECIPIENT, to_phone_number):   # If the recipient could not be added
+            if ADD_RECIPIENT_QUESTION.lower() == "y" or ADD_RECIPIENT_QUESTION.lower() == "yes":
+                to_phone_number = input("Enter the phone number of the recipient: ")
+                if not add_recipient(RECIPIENT, to_phone_number):   # If the recipient could not be added
+                    return
+            else:
                 return
 
     # Create the message (AI Time!)
     CHATGPT_CONTEXT = f"Write a text message to {RECIPIENT} explaining that you {PROBLEM} because {EXCUSE}. Also start the message by stating this is {USER}, and end the message by telling the recipient to text my actual phone number back if you really need me."
     print("\nCreating message...\n")
 
     # OpenAI API
```

### Comparing `text_excuse_generator-1.1.0/text_excuse_generator.egg-info/PKG-INFO` & `text_excuse_generator-1.1.1/text_excuse_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-excuse-generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

