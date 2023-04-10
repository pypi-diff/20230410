# Comparing `tmp/sessender-0.4.3.tar.gz` & `tmp/sessender-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessender-0.4.3.tar", last modified: Wed Mar 29 11:10:26 2023, max compression
+gzip compressed data, was "sessender-0.4.5.tar", last modified: Mon Apr 10 13:03:09 2023, max compression
```

## Comparing `sessender-0.4.3.tar` & `sessender-0.4.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:10:26.737384 sessender-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-29 11:10:14.000000 sessender-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-29 11:10:26.737384 sessender-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-29 11:10:14.000000 sessender-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:10:26.737384 sessender-0.4.3/sessender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-29 11:10:26.000000 sessender-0.4.3/sessender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-29 11:10:26.000000 sessender-0.4.3/sessender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 11:10:26.000000 sessender-0.4.3/sessender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 11:10:26.000000 sessender-0.4.3/sessender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-29 11:10:14.000000 sessender-0.4.3/sessender.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 11:10:26.737384 sessender-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-29 11:10:14.000000 sessender-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:03:09.867876 sessender-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 13:02:59.000000 sessender-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-10 13:03:09.867876 sessender-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 13:02:59.000000 sessender-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:03:09.867876 sessender-0.4.5/sessender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-10 13:02:59.000000 sessender-0.4.5/sessender.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:03:09.867876 sessender-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 13:02:59.000000 sessender-0.4.5/setup.py
```

### Comparing `sessender-0.4.3/LICENSE` & `sessender-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sessender-0.4.3/PKG-INFO` & `sessender-0.4.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessender
-Version: 0.4.3
+Version: 0.4.5
 Summary: A Python package for sending emails using AWS SES
 Home-page: https://github.com/amitsdalal/sessender
 Author: Amit Dalal
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -36,14 +36,17 @@
 - `SES_PORT`: Your Amazon SES SMTP port.
 - `EMAIL_RECIPIENT`: The recipient email address.
 - `EMAIL_SENDER`: The sender email address.
 
 
 Then, create a `Sessender` object with your credentials:
 
+To send a plain text email, use the send_email method with the message parameter:
+
+
 ```python
 from sessender import SesSender
 
 sender = SesSender()
 
 sender.send_email(
     subject='Hello, world!',
@@ -56,14 +59,31 @@
 ```python
 sender.send_email(
     subject='Hello, world!',
     message='This is a test email from Sessender with an attachment.',
     attachment='/path/to/attachment.txt'
 )
 ```
+To send a html email, use the send_email method with the html_message parameter:
+
+```python
+sender.send_email(
+    subject='Hello, world!',
+    html_message='<h1>This is a test email from Sessender in HTML format.</h1>',
+)
+```
+You can also include attachments with your emails by passing a file path to the attachment parameter:
+
+```python
+sender.send_email(
+    subject='Hello, world!',
+    html_message='This is a test email from Sessender with an attachment.',
+    attachment='/path/to/attachment.txt'
+)
+```
 
 ## Contributing
 If you'd like to contribute to Sessender, please fork the repository and create a pull request. We welcome contributions of all kinds, including bug fixes, new features, and documentation improvements.
 
 # License
 Sessender is licensed under the MIT License. See LICENSE for more information.
```

### Comparing `sessender-0.4.3/README.md` & `sessender-0.4.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 - `SES_PORT`: Your Amazon SES SMTP port.
 - `EMAIL_RECIPIENT`: The recipient email address.
 - `EMAIL_SENDER`: The sender email address.
 
 
 Then, create a `Sessender` object with your credentials:
 
+To send a plain text email, use the send_email method with the message parameter:
+
+
 ```python
 from sessender import SesSender
 
 sender = SesSender()
 
 sender.send_email(
     subject='Hello, world!',
@@ -42,13 +45,30 @@
 ```python
 sender.send_email(
     subject='Hello, world!',
     message='This is a test email from Sessender with an attachment.',
     attachment='/path/to/attachment.txt'
 )
 ```
+To send a html email, use the send_email method with the html_message parameter:
+
+```python
+sender.send_email(
+    subject='Hello, world!',
+    html_message='<h1>This is a test email from Sessender in HTML format.</h1>',
+)
+```
+You can also include attachments with your emails by passing a file path to the attachment parameter:
+
+```python
+sender.send_email(
+    subject='Hello, world!',
+    html_message='This is a test email from Sessender with an attachment.',
+    attachment='/path/to/attachment.txt'
+)
+```
 
 ## Contributing
 If you'd like to contribute to Sessender, please fork the repository and create a pull request. We welcome contributions of all kinds, including bug fixes, new features, and documentation improvements.
 
 # License
 Sessender is licensed under the MIT License. See LICENSE for more information.
```

### Comparing `sessender-0.4.3/sessender.egg-info/PKG-INFO` & `sessender-0.4.5/sessender.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessender
-Version: 0.4.3
+Version: 0.4.5
 Summary: A Python package for sending emails using AWS SES
 Home-page: https://github.com/amitsdalal/sessender
 Author: Amit Dalal
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -36,14 +36,17 @@
 - `SES_PORT`: Your Amazon SES SMTP port.
 - `EMAIL_RECIPIENT`: The recipient email address.
 - `EMAIL_SENDER`: The sender email address.
 
 
 Then, create a `Sessender` object with your credentials:
 
+To send a plain text email, use the send_email method with the message parameter:
+
+
 ```python
 from sessender import SesSender
 
 sender = SesSender()
 
 sender.send_email(
     subject='Hello, world!',
@@ -56,14 +59,31 @@
 ```python
 sender.send_email(
     subject='Hello, world!',
     message='This is a test email from Sessender with an attachment.',
     attachment='/path/to/attachment.txt'
 )
 ```
+To send a html email, use the send_email method with the html_message parameter:
+
+```python
+sender.send_email(
+    subject='Hello, world!',
+    html_message='<h1>This is a test email from Sessender in HTML format.</h1>',
+)
+```
+You can also include attachments with your emails by passing a file path to the attachment parameter:
+
+```python
+sender.send_email(
+    subject='Hello, world!',
+    html_message='This is a test email from Sessender with an attachment.',
+    attachment='/path/to/attachment.txt'
+)
+```
 
 ## Contributing
 If you'd like to contribute to Sessender, please fork the repository and create a pull request. We welcome contributions of all kinds, including bug fixes, new features, and documentation improvements.
 
 # License
 Sessender is licensed under the MIT License. See LICENSE for more information.
```

### Comparing `sessender-0.4.3/sessender.py` & `sessender-0.4.5/sessender.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,27 @@
 
         except Exception as e:
             error_msg = f"Error initializing Sessender:\n{traceback.format_exc()}"
             print(error_msg)
             logging.error(error_msg)
             raise e
 
-    def send_email(self, subject, message, attachment=None):
+    def send_email(self, subject, message=None, html_message=None, attachment=None):
         try:
             # Create a message
             msg = MIMEMultipart()
             msg['From'] = self.sender
             msg['To'] = self.recipient
             msg['Subject'] = subject
-            msg.attach(MIMEText(message))
+
+            # Attach plain text or HTML message
+            if html_message:
+                msg.attach(MIMEText(html_message, 'html'))
+            elif message:
+                msg.attach(MIMEText(message))
 
             # Add attachment to message if specified
             if attachment:
                 with open(attachment, 'rb') as f:
                     part = MIMEApplication(f.read(), Name=os.path.basename(attachment))
                     part['Content-Disposition'] = f'attachment; filename="{os.path.basename(attachment)}"'
                     msg.attach(part)
```

### Comparing `sessender-0.4.3/setup.py` & `sessender-0.4.5/setup.py`

 * *Files identical despite different names*

