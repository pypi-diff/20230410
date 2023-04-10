# Comparing `tmp/cabinet-2023.3.6.2.tar.gz` & `tmp/cabinet-2023.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.3.6.2.tar", last modified: Tue Mar  7 04:59:38 2023, max compression
+gzip compressed data, was "cabinet-2023.4.9.1.tar", last modified: Mon Apr 10 04:09:49 2023, max compression
```

## Comparing `cabinet-2023.3.6.2.tar` & `cabinet-2023.4.9.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-07 04:59:38.683715 cabinet-2023.3.6.2/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.3.6.2/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4387 2023-03-07 04:59:38.683715 cabinet-2023.3.6.2/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4036 2023-03-06 05:56:28.000000 cabinet-2023.3.6.2/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.3.6.2/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      758 2023-03-07 04:59:38.683715 cabinet-2023.3.6.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-07 04:59:38.679715 cabinet-2023.3.6.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-07 04:59:38.683715 cabinet-2023.3.6.2/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-03-06 04:32:37.000000 cabinet-2023.3.6.2/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       68 2023-03-06 05:51:35.000000 cabinet-2023.3.6.2/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    12971 2023-03-06 06:55:55.000000 cabinet-2023.3.6.2/src/cabinet/cabinet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2533 2023-03-06 06:26:37.000000 cabinet-2023.3.6.2/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-07 04:59:38.683715 cabinet-2023.3.6.2/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4387 2023-03-07 04:59:38.000000 cabinet-2023.3.6.2/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      311 2023-03-07 04:59:38.000000 cabinet-2023.3.6.2/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-03-07 04:59:38.000000 cabinet-2023.3.6.2/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       49 2023-03-07 04:59:38.000000 cabinet-2023.3.6.2/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-03-07 04:59:38.000000 cabinet-2023.3.6.2/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.4.9.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4014 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.4.9.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    20802 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2737 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2023.3.6.2/LICENSE` & `cabinet-2023.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.3.6.2/PKG-INFO` & `cabinet-2023.4.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.3.6.2
+Version: 2023.4.9.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabinet
-A Python library to easily read and write settings in JSON files across repos. Supports email and event logging.
+A Python library to easily store data across multiple projects in one or more JSON files.
+
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
-- Send/receive mail using `cabinet.mail`
+- Send/receive mail using `cabinet.Cabinet().mail()`
 
 ## Structure
 
 - Data is stored in a `settings.json` file in the location of your choice
-- Logs are written to `/path/to/cabinet/log` by default
+- Logs are written to `{/path/to/cabinet}/log/LOG_DAILY_YYYY-MM-DD` by default
+  - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
   cabinet config
 ```
 
 ## Configuration
 
-- To choose where `settings.json` is stored, use `cabinet config` and follow the prompts.
-
-- To choose where logs will be stored, edit `settings.json` and set `path -> log` to the full path to the log folder. (in other words, `{"path": "log": "/path/to/folder"}`)
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit
+### edit() shortcuts
 - see example below to enable something like `cabinet edit shopping` from the terminal
-  - or `cabinet.edit("shopping")`, rather than `cabinet.edit("/home/{username}/path/to/shopping.md")`
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
@@ -80,17 +81,19 @@
 ```
 
 ## Examples
 
 ### `set`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-cabinet.set("employee", "Tyler", "salary", 7.25)
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
 
 ```
 {
     "employee": {
@@ -100,37 +103,40 @@
     }
 }
 ```
 
 ### `get`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
 
-print(cabinet.get("employee", "Tyler", "salary")) # given example settings.json above
+cab = Cabinet()
+
+print(cab.get("employee", "Tyler", "salary"))
 ```
 
 ```
 > python3 test.py
 > 7.25
 ```
 
 ### `edit`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file
-# assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
-cabinet.edit("shopping")
+cab.edit("shopping")
 
 # or you can edit a file directly...
-cabinet.edit("/path/to/shopping.md")
+cab.edit("/path/to/shopping.md")
 ```
 
 ### `mail`
 
 ```
 
 from cabinet import mail
@@ -139,30 +145,32 @@
 
 ```
 
 ### `log`
 
 ```
 
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-# writes to a file named LOG_DAILY YYYY-MM-DD in the default log folder (or cabinet.get('path', 'log')) inside a YYYY-MM-DD folder
+# writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
-cabinet.log("Connection timed out") # defaults to 'info' if no level is set
-cabinet.log("This function hit a breakpoint", level="debug")
-cabinet.log("Looks like the server is on fire", level="critical")
-cabinet.log("This is fine", level="info")
+cab.log("Connection timed out") # defaults to 'info' if no level is set
+cab.log("This function hit a breakpoint", level="debug")
+cab.log("Looks like the server is on fire", level="critical")
+cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cabinet.log("30", logName="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cabinet.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 ## Dependencies
```

### Comparing `cabinet-2023.3.6.2/README.md` & `cabinet-2023.4.9.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # cabinet
-A Python library to easily read and write settings in JSON files across repos. Supports email and event logging.
+A Python library to easily store data across multiple projects in one or more JSON files.
+
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
-- Send/receive mail using `cabinet.mail`
+- Send/receive mail using `cabinet.Cabinet().mail()`
 
 ## Structure
 
 - Data is stored in a `settings.json` file in the location of your choice
-- Logs are written to `/path/to/cabinet/log` by default
+- Logs are written to `{/path/to/cabinet}/log/LOG_DAILY_YYYY-MM-DD` by default
+  - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
   cabinet config
 ```
 
 ## Configuration
 
-- To choose where `settings.json` is stored, use `cabinet config` and follow the prompts.
-
-- To choose where logs will be stored, edit `settings.json` and set `path -> log` to the full path to the log folder. (in other words, `{"path": "log": "/path/to/folder"}`)
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit
+### edit() shortcuts
 - see example below to enable something like `cabinet edit shopping` from the terminal
-  - or `cabinet.edit("shopping")`, rather than `cabinet.edit("/home/{username}/path/to/shopping.md")`
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
@@ -68,17 +69,19 @@
 ```
 
 ## Examples
 
 ### `set`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-cabinet.set("employee", "Tyler", "salary", 7.25)
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
 
 ```
 {
     "employee": {
@@ -88,37 +91,40 @@
     }
 }
 ```
 
 ### `get`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
 
-print(cabinet.get("employee", "Tyler", "salary")) # given example settings.json above
+cab = Cabinet()
+
+print(cab.get("employee", "Tyler", "salary"))
 ```
 
 ```
 > python3 test.py
 > 7.25
 ```
 
 ### `edit`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file
-# assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
-cabinet.edit("shopping")
+cab.edit("shopping")
 
 # or you can edit a file directly...
-cabinet.edit("/path/to/shopping.md")
+cab.edit("/path/to/shopping.md")
 ```
 
 ### `mail`
 
 ```
 
 from cabinet import mail
@@ -127,30 +133,32 @@
 
 ```
 
 ### `log`
 
 ```
 
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-# writes to a file named LOG_DAILY YYYY-MM-DD in the default log folder (or cabinet.get('path', 'log')) inside a YYYY-MM-DD folder
+# writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
-cabinet.log("Connection timed out") # defaults to 'info' if no level is set
-cabinet.log("This function hit a breakpoint", level="debug")
-cabinet.log("Looks like the server is on fire", level="critical")
-cabinet.log("This is fine", level="info")
+cab.log("Connection timed out") # defaults to 'info' if no level is set
+cab.log("This function hit a breakpoint", level="debug")
+cab.log("Looks like the server is on fire", level="critical")
+cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cabinet.log("30", logName="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cabinet.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 ## Dependencies
```

### Comparing `cabinet-2023.3.6.2/setup.cfg` & `cabinet-2023.4.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.03.06.2
+version = 2023.04.09.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls = 
@@ -22,13 +22,13 @@
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
-	cabinet = cabinet.cabinet:main
+	cabinet = cabinet:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cabinet-2023.3.6.2/src/cabinet/mail.py` & `cabinet-2023.4.9.1/src/cabinet/mail.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,68 @@
 """
-cabinet mail
+Cabinet Mail
 
-enables quick email sendind checking
+Provides functionality for sending email using SMTP and MIMEText.
+Does not support Gmail.
+
+A throwaway email is highly recommended.
 """
+
 import smtplib
-import imaplib
+from typing import List
 from urllib.parse import unquote
 import sys
 import pwd
 import os
-import traceback
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
 userDir = pwd.getpwuid(os.getuid())[0]
 
-# Parameters
-port = cabinet.get("email", "port")
-smtp_server = cabinet.get("email", "smtp_server")
-imap_server = cabinet.get("email", "imap_server")
-username = cabinet.get("email", "from")
-password = cabinet.get("email", "from_pw")
+# parameters
+port = cab.get("email", "port")
+smtp_server = cab.get("email", "smtp_server")
+imap_server = cab.get("email", "imap_server")
+username = cab.get("email", "from")
+password = cab.get("email", "from_pw")
 
 
-def send(subject, body, signature='', to_addr=cabinet.get("email", "to") or [], from_name=cabinet.get("email", "from_name") or "Raspberry Pi", logging_enabled=True, is_quiet=False):
+def send(subject: str, body: str, signature: str = '', to_addr: List[str] = None,
+         from_name: str = None, logging_enabled: bool = True, is_quiet: bool = False) -> None:
     """
-    Sends email from the given account; see README for restrictions!
+    Sends an email with the given subject and body to the specified recipients.
+
+    Args:
+    - subject (str): The subject of the email.
+    - body (str): The body of the email.
+    - signature (str): The signature to include at the end of the email.
+    - to_addr (List): A list of email addresses to send the email to.
+    - from_name (str, optional): The name to appear in the "From" field of the email.
+        Reads from settings.json -> email -> from_name if unset.
+        If this is unset, defaults to `Raspberry Pi`
+    - logging_enabled (bool, optional): Whether to log the email send event.
+        Defaults to True.
+    - is_quiet: Whether to suppress log output.
+        Defaults to False.
+
     Gmail will almost certainly not work.
     """
-    from_name = from_name + f" <{username}>"
+
+    from_name = (cab.get("email", "from_name") or "Raspberry Pi") + f" <{username}>"
     signature = signature or f"<br><br>Thanks,<br>{from_name}"
 
-    if len(to_addr) == 0:
-        cabinet.log("cabinet -> email -> to is unset", level="error")
-        return
+    if to_addr is None:
+        to_addr = cab.get("email", "to")
+
+        if to_addr is None:
+            cab.log("cabinet -> email -> to is unset", level="error")
+            return
 
     # Parse
     body += unquote(signature)
     message = MIMEMultipart()
     message["Subject"] = unquote(subject)
     message["From"] = from_name
     message["To"] = (', ').join(to_addr)
@@ -48,39 +72,17 @@
     server = smtplib.SMTP_SSL(smtp_server, port)
 
     try:
         server.login(username, password)
         server.send_message(message)
 
         if logging_enabled:
-            cabinet.log(
+            cab.log(
                 f"Sent Email to {message['To']} as {message['From']}: {subject}", is_quiet=is_quiet)
 
     except smtplib.SMTPAuthenticationError as err:
-        cabinet.log(
-            f"Could not log into {username}; set this with cabinet.\n\n{err}", level="error")
-
-def check():
-    """
-    Returns raw, possibly-encoded emails from the Inbox of the Gmail account described above
-    """
-    try:
-        mail = imaplib.IMAP4_SSL(imap_server)
-        mail.login(username, password)
-        mail.select('inbox')
-
-        data = mail.search(None, 'ALL')
-        mail_ids = data[1]
-        id_list = mail_ids[0].split()
-        latest_email_id = str(int(id_list[-1]))
-
-        return mail.fetch(latest_email_id, '(RFC822)')
-
-    except Exception as e:
-        traceback.print_exc()
-        cabinet.log(
-            f"Ran into a problem checking mail:{str(e).strip()}", level="error")
-
+        cab.log(
+            f"Could not log into {username}; set this with Cabinet.\n\n{err}", level="error")
 
 if __name__ == "__main__":
     if len(sys.argv) == 1:
         print("sys.argv usage: send <subject>, <body>")
```

### Comparing `cabinet-2023.3.6.2/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.3.6.2
+Version: 2023.4.9.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabinet
-A Python library to easily read and write settings in JSON files across repos. Supports email and event logging.
+A Python library to easily store data across multiple projects in one or more JSON files.
+
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
-- Send/receive mail using `cabinet.mail`
+- Send/receive mail using `cabinet.Cabinet().mail()`
 
 ## Structure
 
 - Data is stored in a `settings.json` file in the location of your choice
-- Logs are written to `/path/to/cabinet/log` by default
+- Logs are written to `{/path/to/cabinet}/log/LOG_DAILY_YYYY-MM-DD` by default
+  - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
   cabinet config
 ```
 
 ## Configuration
 
-- To choose where `settings.json` is stored, use `cabinet config` and follow the prompts.
-
-- To choose where logs will be stored, edit `settings.json` and set `path -> log` to the full path to the log folder. (in other words, `{"path": "log": "/path/to/folder"}`)
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit
+### edit() shortcuts
 - see example below to enable something like `cabinet edit shopping` from the terminal
-  - or `cabinet.edit("shopping")`, rather than `cabinet.edit("/home/{username}/path/to/shopping.md")`
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
@@ -80,17 +81,19 @@
 ```
 
 ## Examples
 
 ### `set`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-cabinet.set("employee", "Tyler", "salary", 7.25)
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
 
 ```
 {
     "employee": {
@@ -100,37 +103,40 @@
     }
 }
 ```
 
 ### `get`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
 
-print(cabinet.get("employee", "Tyler", "salary")) # given example settings.json above
+cab = Cabinet()
+
+print(cab.get("employee", "Tyler", "salary"))
 ```
 
 ```
 > python3 test.py
 > 7.25
 ```
 
 ### `edit`
 
 ```
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file
-# assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
-cabinet.edit("shopping")
+cab.edit("shopping")
 
 # or you can edit a file directly...
-cabinet.edit("/path/to/shopping.md")
+cab.edit("/path/to/shopping.md")
 ```
 
 ### `mail`
 
 ```
 
 from cabinet import mail
@@ -139,30 +145,32 @@
 
 ```
 
 ### `log`
 
 ```
 
-from cabinet import cabinet
+from cabinet import Cabinet
+
+cab = Cabinet()
 
-# writes to a file named LOG_DAILY YYYY-MM-DD in the default log folder (or cabinet.get('path', 'log')) inside a YYYY-MM-DD folder
+# writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
-cabinet.log("Connection timed out") # defaults to 'info' if no level is set
-cabinet.log("This function hit a breakpoint", level="debug")
-cabinet.log("Looks like the server is on fire", level="critical")
-cabinet.log("This is fine", level="info")
+cab.log("Connection timed out") # defaults to 'info' if no level is set
+cab.log("This function hit a breakpoint", level="debug")
+cab.log("Looks like the server is on fire", level="critical")
+cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cabinet.log("30", logName="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cabinet.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 ## Dependencies
```

