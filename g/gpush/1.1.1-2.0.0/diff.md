# Comparing `tmp/gpush-1.1.1.tar.gz` & `tmp/gpush-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-1.1.1.tar", last modified: Sun Apr  9 20:20:02 2023, max compression
+gzip compressed data, was "gpush-2.0.0.tar", last modified: Mon Apr 10 19:25:55 2023, max compression
```

## Comparing `gpush-1.1.1.tar` & `gpush-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 20:20:02.354586 gpush-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1156 2023-04-09 20:20:02.354586 gpush-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1066 2023-04-09 20:19:59.000000 gpush-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 20:20:02.354586 gpush-1.1.1/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1156 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1802 2023-04-09 20:19:59.000000 gpush-1.1.1/gpush.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-09 20:19:59.000000 gpush-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 20:20:02.354586 gpush-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      343 2023-04-09 20:19:59.000000 gpush-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:25:55.128754 gpush-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-10 19:25:51.000000 gpush-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-10 19:25:55.128754 gpush-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-10 19:25:51.000000 gpush-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-04-10 19:25:51.000000 gpush-2.0.0/gpush
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:25:55.128754 gpush-2.0.0/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-10 19:25:51.000000 gpush-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 19:25:55.128754 gpush-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-10 19:25:52.000000 gpush-2.0.0/setup.py
```

### Comparing `gpush-1.1.1/PKG-INFO` & `gpush-2.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-Metadata-Version: 2.1
-Name: gpush
-Version: 1.1.1
-Description-Content-Type: text/markdown
-
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
 
 # Installation
 
 This package is available for installation via pypi
 
 ```
 pip3 install gpush
 ```
 
-# Configuration
+# Usage
 
-To start using gpush, run the following (update as required if you do not use zsh)
+When running gpush in a git directory, use `gpush` to replace your standard `git commit && git push` commands. `gpush` will ask three questions to determine detail about your commit and generate a conventionally formatted git commit message.
 
-```
-echo "alias gpush=\"python3 -m gpush\"" >> ~/.zshrc
-```
+!["gpush_demo"](docs/gpush_demo.gif)
 
-To start using straight away, source your file
+# Local development
+
+To develop locally, execute the pip3 installation in the local directory:
 
 ```
-source ~/.zshrc
+pip3 install .
 ```
 
-# Usage
+Alternatively, create an alias in your zshrc file (Use appropriate profile file if you do not use zsh)
 
-When running gpush in a git directory, use `gpush` to replace your standard `git commit && git push` commands. `gpush` will ask three questions to determine detail about your commit and generate a conventionally formatted git commit message.
+echo "alias gpush=\"python3 /path/to/git/gpush/gpush\"" >> ~/.zshrc
+To start using straight away, source your file
 
-!["gpush_demo"](docs/gpush_demo.gif)
+source ~/.zshrc
 
 # python-semantic-release
 
 `gpush` generates commit messages that are compliant with [python-semantic-release](https://python-semantic-release.readthedocs.io/en/latest/). See example in the [GitHub Repository](https://github.com/tjtharrison/gpush/blob/main/.github/workflows/semver.yaml)
```

### Comparing `gpush-1.1.1/gpush.egg-info/PKG-INFO` & `gpush-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: gpush
-Version: 1.1.1
+Version: 2.0.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
 
 # Installation
 
 This package is available for installation via pypi
 
 ```
 pip3 install gpush
 ```
 
-# Configuration
+# Usage
 
-To start using gpush, run the following (update as required if you do not use zsh)
+When running gpush in a git directory, use `gpush` to replace your standard `git commit && git push` commands. `gpush` will ask three questions to determine detail about your commit and generate a conventionally formatted git commit message.
 
-```
-echo "alias gpush=\"python3 -m gpush\"" >> ~/.zshrc
-```
+!["gpush_demo"](docs/gpush_demo.gif)
 
-To start using straight away, source your file
+# Local development
+
+To develop locally, execute the pip3 installation in the local directory:
 
 ```
-source ~/.zshrc
+pip3 install .
 ```
 
-# Usage
+Alternatively, create an alias in your zshrc file (Use appropriate profile file if you do not use zsh)
 
-When running gpush in a git directory, use `gpush` to replace your standard `git commit && git push` commands. `gpush` will ask three questions to determine detail about your commit and generate a conventionally formatted git commit message.
+echo "alias gpush=\"python3 /path/to/git/gpush/gpush\"" >> ~/.zshrc
+To start using straight away, source your file
 
-!["gpush_demo"](docs/gpush_demo.gif)
+source ~/.zshrc
 
 # python-semantic-release
 
 `gpush` generates commit messages that are compliant with [python-semantic-release](https://python-semantic-release.readthedocs.io/en/latest/). See example in the [GitHub Repository](https://github.com/tjtharrison/gpush/blob/main/.github/workflows/semver.yaml)
```

### Comparing `gpush-1.1.1/gpush.py` & `gpush-2.0.0/gpush`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 """
 Python script to handle git commit and push to standardise commit messages using conventional commit
 messages.
 
 Usage: gpush
 """
```

