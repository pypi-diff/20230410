# Comparing `tmp/ssh-hosts-0.3.1.tar.gz` & `tmp/ssh-hosts-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh-hosts-0.3.1.tar", last modified: Sun Apr  2 09:45:15 2023, max compression
+gzip compressed data, was "ssh-hosts-0.3.2.tar", last modified: Mon Apr 10 17:22:02 2023, max compression
```

## Comparing `ssh-hosts-0.3.1.tar` & `ssh-hosts-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 09:45:15.415234 ssh-hosts-0.3.1/
--rw-rw-rw-   0        0        0     1100 2023-02-02 18:07:15.000000 ssh-hosts-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3022 2023-04-02 09:45:15.414722 ssh-hosts-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2325 2023-04-02 09:32:46.000000 ssh-hosts-0.3.1/README.md
--rw-rw-rw-   0        0        0      858 2023-04-02 09:32:44.000000 ssh-hosts-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-02 09:45:15.416267 ssh-hosts-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-02-02 18:07:15.000000 ssh-hosts-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 09:45:15.382002 ssh-hosts-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-02 09:45:15.407461 ssh-hosts-0.3.1/src/ssh_hosts.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-04-02 09:45:15.000000 ssh-hosts-0.3.1/src/ssh_hosts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-02 09:45:15.000000 ssh-hosts-0.3.1/src/ssh_hosts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 09:45:15.000000 ssh-hosts-0.3.1/src/ssh_hosts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-02 09:45:15.000000 ssh-hosts-0.3.1/src/ssh_hosts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-02 09:45:15.000000 ssh-hosts-0.3.1/src/ssh_hosts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-02 09:45:15.412394 ssh-hosts-0.3.1/src/sshhosts/
--rw-rw-rw-   0        0        0        0 2023-02-02 18:07:15.000000 ssh-hosts-0.3.1/src/sshhosts/__init__.py
--rw-rw-rw-   0        0        0     6985 2023-04-02 09:32:48.000000 ssh-hosts-0.3.1/src/sshhosts/sshhosts.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.158801 ssh-hosts-0.3.2/
+-rw-rw-rw-   0        0        0     1100 2023-02-02 18:07:15.000000 ssh-hosts-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3802 2023-04-10 17:22:02.158801 ssh-hosts-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3084 2023-04-10 17:16:13.000000 ssh-hosts-0.3.2/README.md
+-rw-rw-rw-   0        0        0      858 2023-04-10 17:16:10.000000 ssh-hosts-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 17:22:02.158801 ssh-hosts-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-02-02 18:07:15.000000 ssh-hosts-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.095526 ssh-hosts-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.143171 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/
+-rw-rw-rw-   0        0        0     3802 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.143171 ssh-hosts-0.3.2/src/sshhosts/
+-rw-rw-rw-   0        0        0        0 2023-02-02 18:07:15.000000 ssh-hosts-0.3.2/src/sshhosts/__init__.py
+-rw-rw-rw-   0        0        0     9189 2023-04-10 17:16:17.000000 ssh-hosts-0.3.2/src/sshhosts/sshhosts.py
```

### Comparing `ssh-hosts-0.3.1/LICENSE.txt` & `ssh-hosts-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssh-hosts-0.3.1/PKG-INFO` & `ssh-hosts-0.3.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-hosts
-Version: 0.3.1
+Version: 0.3.2
 Summary: Quickly connect to host entries from your SSH config file
 Author: Christoph Stein
 License: MIT
 Project-URL: homepage, https://gitlab.com/s7one/ssh-hosts
 Project-URL: documentation, https://gitlab.com/s7one/ssh-hosts
 Project-URL: repository, https://gitlab.com/s7one/ssh-hosts
 Keywords: SSH,Hosts,Network
@@ -13,35 +13,69 @@
 Classifier: Environment :: Console
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SSH-Hosts
 
-Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one of them.
+Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one of them. This is handy if you organize a bunch of host entries in your SSH client config like, e.g.:
+
+```
+Host foo
+  Hostname foohost
+  User foouser
+  IdentityFile fookey
+
+Host bar
+  Hostname barhost
+  User baruser
+  IdentityFile barkey
+```
+
+Note: It is also possible to use wildcards in your SSH client config to set values for multiple hosts at once. This script will *not* show these entries, since they cannot be used to connect to a host directly.
 
 ## Installation
 
   * Install from pypi: ```pip install ssh-hosts```
 
   OR
 
   * Download the pip package from GitLab
-  * Install it with pip, e.g. pip install sshhosts-0.3.1-py3-none-any.whl
+  * Install it with pip, e.g. pip install sshhosts-0.3.2-py3-none-any.whl
 
-## Usage
-
-### Basic usage
+## Basic usage
 
 Just run
 ```
 ssh-hosts
 ```
 Running with no arguments will read in your ssh configuration from ```~/.ssh/config``` and list all found host entries. Type the number of an entry to connect to that given host.
 
+## Command line arguments overview
+
+```
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -c CONFIG, --config CONFIG
+                        Path to configuration file
+  -e EXCLUDE, --exclude EXCLUDE
+                        Exclude hosts based on python regular expression
+  -s SSH_COMMAND, --ssh_command SSH_COMMAND
+                        SSH command
+  -l, --loop            Do not exit when ssh session ends, show host list again instead
+  -t, --terminal_tab_mode
+                        Attempt to start ssh session in new tab/window of terminal
+  -o, --sort_host_entries
+                        Sort host entries
+  -r, --reverse_order   Reverse sorting order
+```
+
+## Arguments
+
 ### Path to SSH configuration
 
 ```
 ssh-hosts -c '<path to ssh config>'
 ```
 This will read in the SSH configuration file from the given path instead of ```~/.ssh/config```.
 
@@ -86,30 +120,17 @@
 
 Tries so start ssh connections in new tabs if running in *Windows Terminal*, or in new windows when running in *tmux*.
 
 ```
 ssh-hosts --terminal_tab_mode
 ```
 
-## Command line arguments overview
+You can combine this with ```loop``` mode to keep the list of hosts open on one tab/window of your terminal and quickly launch connections in new tabs/windows.
 
+e.g.
 ```
-optional arguments:
-  -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -c CONFIG, --config CONFIG
-                        Path to configuration file
-  -e EXCLUDE, --exclude EXCLUDE
-                        Exclude hosts based on python regular expression
-  -s SSH_COMMAND, --ssh_command SSH_COMMAND
-                        SSH command
-  -l, --loop            Do not exit when ssh session ends, show host list again instead
-  -t, --terminal_tab_mode
-                        Attempt to start ssh session in new tab/window of terminal
+ssh-hosts --terminal_tab_mode --loop
 ```
-## Examples
-
-
 
 ## Licensing
 
 Licensed under the MIT license, see also LICENSE.txt
```

### Comparing `ssh-hosts-0.3.1/README.md` & `ssh-hosts-0.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,64 @@
 # SSH-Hosts
 
-Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one of them.
+Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one of them. This is handy if you organize a bunch of host entries in your SSH client config like, e.g.:
+
+```
+Host foo
+  Hostname foohost
+  User foouser
+  IdentityFile fookey
+
+Host bar
+  Hostname barhost
+  User baruser
+  IdentityFile barkey
+```
+
+Note: It is also possible to use wildcards in your SSH client config to set values for multiple hosts at once. This script will *not* show these entries, since they cannot be used to connect to a host directly.
 
 ## Installation
 
   * Install from pypi: ```pip install ssh-hosts```
 
   OR
 
   * Download the pip package from GitLab
-  * Install it with pip, e.g. pip install sshhosts-0.3.1-py3-none-any.whl
+  * Install it with pip, e.g. pip install sshhosts-0.3.2-py3-none-any.whl
 
-## Usage
-
-### Basic usage
+## Basic usage
 
 Just run
 ```
 ssh-hosts
 ```
 Running with no arguments will read in your ssh configuration from ```~/.ssh/config``` and list all found host entries. Type the number of an entry to connect to that given host.
 
+## Command line arguments overview
+
+```
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -c CONFIG, --config CONFIG
+                        Path to configuration file
+  -e EXCLUDE, --exclude EXCLUDE
+                        Exclude hosts based on python regular expression
+  -s SSH_COMMAND, --ssh_command SSH_COMMAND
+                        SSH command
+  -l, --loop            Do not exit when ssh session ends, show host list again instead
+  -t, --terminal_tab_mode
+                        Attempt to start ssh session in new tab/window of terminal
+  -o, --sort_host_entries
+                        Sort host entries
+  -r, --reverse_order   Reverse sorting order
+```
+
+## Arguments
+
 ### Path to SSH configuration
 
 ```
 ssh-hosts -c '<path to ssh config>'
 ```
 This will read in the SSH configuration file from the given path instead of ```~/.ssh/config```.
 
@@ -69,30 +103,17 @@
 
 Tries so start ssh connections in new tabs if running in *Windows Terminal*, or in new windows when running in *tmux*.
 
 ```
 ssh-hosts --terminal_tab_mode
 ```
 
-## Command line arguments overview
+You can combine this with ```loop``` mode to keep the list of hosts open on one tab/window of your terminal and quickly launch connections in new tabs/windows.
 
+e.g.
 ```
-optional arguments:
-  -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -c CONFIG, --config CONFIG
-                        Path to configuration file
-  -e EXCLUDE, --exclude EXCLUDE
-                        Exclude hosts based on python regular expression
-  -s SSH_COMMAND, --ssh_command SSH_COMMAND
-                        SSH command
-  -l, --loop            Do not exit when ssh session ends, show host list again instead
-  -t, --terminal_tab_mode
-                        Attempt to start ssh session in new tab/window of terminal
+ssh-hosts --terminal_tab_mode --loop
 ```
-## Examples
-
-
 
 ## Licensing
 
 Licensed under the MIT license, see also LICENSE.txt
```

### Comparing `ssh-hosts-0.3.1/pyproject.toml` & `ssh-hosts-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [project]
 name = "ssh-hosts"
 description = "Quickly connect to host entries from your SSH config file"
 authors = [
     {name = "Christoph Stein" }
 ]
 requires-python = ">=3.9"
-version = "0.3.1"
+version = "0.3.2"
 
 keywords = ["SSH", "Hosts", "Network"]
 readme = "README.md"
 #license = {file = "LICENSE.txt"}
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ssh-hosts-0.3.1/src/ssh_hosts.egg-info/PKG-INFO` & `ssh-hosts-0.3.2/src/ssh_hosts.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-hosts
-Version: 0.3.1
+Version: 0.3.2
 Summary: Quickly connect to host entries from your SSH config file
 Author: Christoph Stein
 License: MIT
 Project-URL: homepage, https://gitlab.com/s7one/ssh-hosts
 Project-URL: documentation, https://gitlab.com/s7one/ssh-hosts
 Project-URL: repository, https://gitlab.com/s7one/ssh-hosts
 Keywords: SSH,Hosts,Network
@@ -13,35 +13,69 @@
 Classifier: Environment :: Console
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SSH-Hosts
 
-Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one of them.
+Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one of them. This is handy if you organize a bunch of host entries in your SSH client config like, e.g.:
+
+```
+Host foo
+  Hostname foohost
+  User foouser
+  IdentityFile fookey
+
+Host bar
+  Hostname barhost
+  User baruser
+  IdentityFile barkey
+```
+
+Note: It is also possible to use wildcards in your SSH client config to set values for multiple hosts at once. This script will *not* show these entries, since they cannot be used to connect to a host directly.
 
 ## Installation
 
   * Install from pypi: ```pip install ssh-hosts```
 
   OR
 
   * Download the pip package from GitLab
-  * Install it with pip, e.g. pip install sshhosts-0.3.1-py3-none-any.whl
+  * Install it with pip, e.g. pip install sshhosts-0.3.2-py3-none-any.whl
 
-## Usage
-
-### Basic usage
+## Basic usage
 
 Just run
 ```
 ssh-hosts
 ```
 Running with no arguments will read in your ssh configuration from ```~/.ssh/config``` and list all found host entries. Type the number of an entry to connect to that given host.
 
+## Command line arguments overview
+
+```
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -c CONFIG, --config CONFIG
+                        Path to configuration file
+  -e EXCLUDE, --exclude EXCLUDE
+                        Exclude hosts based on python regular expression
+  -s SSH_COMMAND, --ssh_command SSH_COMMAND
+                        SSH command
+  -l, --loop            Do not exit when ssh session ends, show host list again instead
+  -t, --terminal_tab_mode
+                        Attempt to start ssh session in new tab/window of terminal
+  -o, --sort_host_entries
+                        Sort host entries
+  -r, --reverse_order   Reverse sorting order
+```
+
+## Arguments
+
 ### Path to SSH configuration
 
 ```
 ssh-hosts -c '<path to ssh config>'
 ```
 This will read in the SSH configuration file from the given path instead of ```~/.ssh/config```.
 
@@ -86,30 +120,17 @@
 
 Tries so start ssh connections in new tabs if running in *Windows Terminal*, or in new windows when running in *tmux*.
 
 ```
 ssh-hosts --terminal_tab_mode
 ```
 
-## Command line arguments overview
+You can combine this with ```loop``` mode to keep the list of hosts open on one tab/window of your terminal and quickly launch connections in new tabs/windows.
 
+e.g.
 ```
-optional arguments:
-  -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -c CONFIG, --config CONFIG
-                        Path to configuration file
-  -e EXCLUDE, --exclude EXCLUDE
-                        Exclude hosts based on python regular expression
-  -s SSH_COMMAND, --ssh_command SSH_COMMAND
-                        SSH command
-  -l, --loop            Do not exit when ssh session ends, show host list again instead
-  -t, --terminal_tab_mode
-                        Attempt to start ssh session in new tab/window of terminal
+ssh-hosts --terminal_tab_mode --loop
 ```
-## Examples
-
-
 
 ## Licensing
 
 Licensed under the MIT license, see also LICENSE.txt
```

### Comparing `ssh-hosts-0.3.1/src/sshhosts/sshhosts.py` & `ssh-hosts-0.3.2/src/sshhosts/sshhosts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,196 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import sys
 from os.path import expanduser
 from os import environ
+import platform
 import subprocess
 import logging
 import argparse
 import re
 
 # ---- Argument parser ----
 def GetVersion() -> str:
-    return "0.3.1"
+    return "0.3.2"
 
 def GetArgParser() -> argparse.ArgumentParser:
     tArgParser = argparse.ArgumentParser(usage="%(prog)s [OPTIONS]",
                                          description="List and connect to host entries from your ssh configuration")
 
     tArgParser.add_argument("-v", "--version", action="version", version = f"{tArgParser.prog} version {GetVersion()}")
     tArgParser.add_argument("-c", "--config", help="Path to configuration file", type=str, default=None, required=False)
     tArgParser.add_argument("-e", "--exclude", help="Exclude hosts based on python regular expression", type=str, default=None, required=False)
     tArgParser.add_argument("-s", "--ssh_command", help="SSH command", type=str, default="ssh", required=False)
     tArgParser.add_argument("-l", "--loop", help="Do not exit when ssh session ends, show host list again instead", action="store_true")
     tArgParser.add_argument("-t", "--terminal_tab_mode", help="Attempt to start ssh session in new tab/window of terminal", action="store_true")
+    tArgParser.add_argument("-o", "--sort_host_entries", help="Sort host entries", action="store_true")
+    tArgParser.add_argument("-r", "--reverse_order", help="Reverse sorting order", action="store_true")
     return tArgParser
 
 # -- Logger setup ---
 def setuplogging():
     # Set application wide debug level and format
     #logging.basicConfig(format='%(asctime)s - %(levelname)s: %(message)s',
     logging.basicConfig(format='%(levelname)s: %(message)s',
                         datefmt='%d.%m.%Y %H:%M:%S',
                         level=logging.INFO)
 
-# -- Read in entries from ssh config file ---
-def CollectFromSSHConfig(Filename: str, RegExp: str, IgnoreCase: bool = False):
-    try:
-        with open(Filename, 'r') as f:
-            Matches = re.findall(RegExp, f.read(), re.MULTILINE | (re.IGNORECASE if IgnoreCase else 0))
-            #logging.debug (f'Searched {Filename} for {RegExp}. Result: {Matches}')
-            return Matches
-    except FileNotFoundError as e:
-        logging.warning(f'File not found: {Filename}')
-        return []
-    except Exception as e:
-        logging.debug(f'Skipping file {Filename}, cause: {str(e)}')
-        return []
-
-def ReadInHosts(InitialConfigfile: str):
+# -- Read in host entries from a SSH client configuration file --
+class SSHConfigHosts:
     HostsRegExp = r'^\s*Host\s+(.+)'
     IncludesRegExp = r'^\s*Include\s+([\w:\/\_\-\"\.\\]+)\s*'
 
-    # Check for includes
-    SSHConfigs = []
-    SSHConfigs.append(InitialConfigfile)
-    IncludedConfigs = CollectFromSSHConfig(InitialConfigfile, IncludesRegExp, True)
-    for i in IncludedConfigs: SSHConfigs.append(i)
-    logging.debug(f'Searching SSH configuration files: {SSHConfigs}')
-
-    # Read in Host entries from all found configuration files
-    AllHosts = []
-    for i in SSHConfigs:
-        Hosts = CollectFromSSHConfig(i, HostsRegExp)
-        for j in Hosts: AllHosts.append(j)
-    logging.debug(f'Host list: {AllHosts}')
-
-    return AllHosts
-
-# -- List hosts and get choice from user ---
-def PickChoice(Hosts):
-    Message = str()
-    for index, item in enumerate(Hosts):
-        Message += f'{index + 1}) {item}\n'
-    Message = Message.replace('"','') # Quotes not needed for display, looks a bit more clean
-
-    try:
-        # User may input more than one number, separated by whitespaces.
-        # Thus: Split string, try to convert every substring into an integer and check
-        # if it is a valid index value. Return a list of valid choices.
-        Input = input(f'\n{Message}Connect to: ')
-        Choices = Input.split()
-        ChoicesChecked = []
-        for i in Choices:
-            try:
-                if 0 < int(i) <= len(Hosts): ChoicesChecked.append(int(i) - 1)
-            except ValueError: pass # Ignore ValueError - those entries will not be added to the ChoicesChecked list because the exception hits before the 'append' happens. No need to take further action here.
-        return ChoicesChecked
-    except KeyboardInterrupt:
-        return []
+    def __init__(self):
+        self.ConfigFilePaths = []
+        self.FilteredHosts = []
+        self.AllHosts = []
+
+    # -- Read in entries from ssh config file ---
+    @staticmethod
+    def CollectFromSSHConfig(Filename: str, RegExp: str, IgnoreCase: bool = False):
+        try:
+            with open(Filename, 'r') as f:
+                Matches = re.findall(RegExp, f.read(), re.MULTILINE | (re.IGNORECASE if IgnoreCase else 0))
+                #logging.debug (f'Searched {Filename} for {RegExp}. Result: {Matches}')
+                return Matches
+        except FileNotFoundError as e:
+            logging.warning(f'File not found: {Filename}')
+            return []
+        except Exception as e:
+            logging.debug(f'Skipping file {Filename}, cause: {str(e)}')
+            return []
+
+    def ReadInHosts(self, InitialConfigfile: str, RegEx = None, SortList = False, ReverseOrder = False):
+        # Check for includes
+        self.ConfigFilePaths = []
+        self.ConfigFilePaths.append(InitialConfigfile)
+        IncludedConfigs = SSHConfigHosts.CollectFromSSHConfig(InitialConfigfile, SSHConfigHosts.IncludesRegExp, IgnoreCase = True)
+        for i in IncludedConfigs: self.ConfigFilePaths.append(i)
+        logging.debug(f'Searching SSH configuration files: {self.ConfigFilePaths}')
+
+        # Read in Host entries from all found configuration files
+        self.AllHosts = []
+        for i in self.ConfigFilePaths:
+            Hosts = SSHConfigHosts.CollectFromSSHConfig(i, SSHConfigHosts.HostsRegExp, IgnoreCase = True)
+            for j in Hosts: self.AllHosts.append(j)
+        logging.debug(f'Host list: {self.AllHosts}')
+
+        # Filter unwanted entries
+        if not self.FilterHosts(RegEx): return False
+
+        # Sort list if requested
+        if SortList: self.SortHosts(ReverseOrder)
+        return True
+
+    # -- Filter hosts --
+    def FilterHosts(self, RegEx = None):
+        self.FilteredHosts = []
+        try:
+            if RegEx: self.FilteredHosts = [i for i in self.AllHosts if not ('*' in i) and not ('?' in i) and not ('!' in i) and not re.fullmatch(RegEx, i)]
+            else:     self.FilteredHosts = [i for i in self.AllHosts if not ('*' in i) and not ('?' in i) and not ('!' in i)]
+        except re.error as e:
+            logging.error(f'Invalid regular expression: {e.msg}')
+            return False
+        return True
+
+    # -- Sort list --
+    def SortHosts(self, ReverseOrder = False):
+        self.FilteredHosts.sort(key = str.lower, reverse = ReverseOrder)
+
+class ConsoleFuncs:
+    def __init__(self):
+        self.Platform = platform.system().lower()
+
+    # -- List strings and get choice from user ---
+    @staticmethod
+    def PickChoice(ChoicesList, Prompt: str = "Choose: "):
+        Message = str()
+        for index, item in enumerate(ChoicesList):
+            Message += f'{index + 1}) {item}\n'
+        Message = Message.replace('"','') # Quotes not needed for display, looks a bit more clean
+
+        try:
+            # User may input more than one number, separated by whitespaces.
+            # Thus: Split string, try to convert every substring into an integer and check
+            # if it is a valid index value. Return a list of valid choices.
+            Input = input(f'\n{Message}{Prompt}')
+            Choices = Input.split()
+            ChoicesChecked = []
+            for i in Choices:
+                try:
+                    if 0 < int(i) <= len(ChoicesList): ChoicesChecked.append(int(i) - 1)
+                except ValueError: pass # Ignore ValueError - those entries will not be added to the ChoicesChecked list because the exception hits before the 'append' happens. No need to take further action here.
+            return ChoicesChecked
+        except KeyboardInterrupt:
+            return []
+
+    # -- Clear console on supported platforms --
+    def Clear(self):
+        if 'windows' in self.Platform: subprocess.run('cls',   shell = True)
+        if 'linux'   in self.Platform: subprocess.run('clear', shell = True)
+        return
 
 # -- Get ssh config from users home directory if no path was supplied ---
 def GetHomeSSHConfigPath():
     return expanduser('~/.ssh/config')
 
-# -- Filter hosts --
-def FilterHosts(Hosts, RegEx = None):
-    try:
-        if RegEx: FilteredHosts = [i for i in Hosts if not i == '*' and not re.fullmatch(RegEx, i)]
-        else:     FilteredHosts = [i for i in Hosts if not i == '*']
-    except re.error as e:
-        logging.error(f'Invalid regular expression: {e.msg}')
-        return None
-    return FilteredHosts
-
 # -- Get commandline to start new ssh connection --
 def CommandLine(SSHCommand: str, Host:str, TerminalTabMode: bool = False):
     # Is it good style to hardcode this stuff here? Probably not. Do I care? Nope.
     Host_no_quotes = Host.replace('"','')
-    if TerminalTabMode and ("WT_SESSION" in environ): return f'wt -w 0 new-tab {SSHCommand} {Host}'
-    if TerminalTabMode and ("TMUX" in environ):       return f'tmux new-window -n "ssh {Host_no_quotes}" {SSHCommand} {Host}'
+    WindowTitle = f'SSH {Host_no_quotes}'
+    if TerminalTabMode and ("WT_SESSION" in environ): return f'wt -w 0 new-tab --title "{WindowTitle}" {SSHCommand} {Host}'
+    if TerminalTabMode and ("TMUX" in environ):       return f'tmux new-window -n "{WindowTitle}" {SSHCommand} {Host}'
     return f'{SSHCommand} {Host}' # no TerminalTabMode or unsupported terminal
 
 # --- main routine ----
 def run_program():
     # setup logging
     setuplogging()
 
     # read in command line arguments
     parser = GetArgParser()
     targs = parser.parse_args()
 
     # Get host entries from configuration file
+    ConfHosts = SSHConfigHosts()
     SSHConfigFile = targs.config if targs.config is not None else GetHomeSSHConfigPath()
     logging.info(f'Reading host entries from {SSHConfigFile}')
-    Hosts = ReadInHosts(SSHConfigFile)
-    logging.debug(f'Hosts: {Hosts}')
-    if len(Hosts) == 0:
-        logging.info('No host entries found')
-        return 0
 
-    # Filter unwanted items
-    FilteredHosts = FilterHosts(Hosts, targs.exclude)
-    if not FilteredHosts:
-        logging.info('No hosts, exit.')
+    if not ConfHosts.ReadInHosts(SSHConfigFile,
+                                 targs.exclude,
+                                 targs.sort_host_entries,
+                                 targs.reverse_order):
+        logging.error('Error reading in host entries, exit.')
+        return 1
+    if len(ConfHosts.FilteredHosts) == 0:
+        logging.info("No hosts, exit.")
         return 0
 
     # Let user choose a host and start ssh connection
+    Console = ConsoleFuncs()
     while True:
-        Choice = PickChoice(FilteredHosts)
+        Choice = Console.PickChoice(ConfHosts.FilteredHosts, 'Connect to: ')
         if not Choice:  # Abort right away if list of choices is empty
             logging.info('Abort')
             return 0
         for i in Choice: # loop through list of chosen host indices, and run the ssh command for each one
-            logging.info(f'Connecting to "{FilteredHosts[i]}"')
+            logging.info(f'Connecting to "{ConfHosts.FilteredHosts[i]}"')
             try:
                 Completed = subprocess.run(CommandLine(targs.ssh_command,
-                                                       FilteredHosts[i],
+                                                       ConfHosts.FilteredHosts[i],
                                                        targs.terminal_tab_mode),
                                            shell = True)
                 logging.info(f'"{Completed.args}" returned "{Completed.returncode}"')
-                if (not targs.loop) and (len(Choice) == 1): return Completed.returncode # When not in loop mode and only 1 choice was give: return exit code of the ssh session
+                if (not targs.loop) and (len(Choice) == 1):
+                    return Completed.returncode # When not in loop mode and only 1 choice was give: return exit code of the ssh session
+                if targs.loop and targs.terminal_tab_mode:
+                    Console.Clear() # When running in terminal tab mode AND loop mode: Clear the console after launching new tabs/windows, looks more clean
             except KeyboardInterrupt:
                 logging.info('Canceled by user')
                 return 0
-        if not targs.loop: return 0 # When in 'loop' mode: do not return, display list again and pick next choice
+        if not targs.loop:
+            return 0 # When in 'loop' mode: do not return, display list again and pick next choice
 
 if __name__ == '__main__':
     sys.exit(run_program())
```

