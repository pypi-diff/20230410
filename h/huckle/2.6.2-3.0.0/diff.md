# Comparing `tmp/huckle-2.6.2.tar.gz` & `tmp/huckle-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huckle-2.6.2.tar", last modified: Sat Nov  5 18:37:33 2022, max compression
+gzip compressed data, was "huckle-3.0.0.tar", last modified: Sun Apr  9 23:11:31 2023, max compression
```

## Comparing `huckle-2.6.2.tar` & `huckle-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-11-05 18:37:33.752328 huckle-2.6.2/
--rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-2.6.2/LICENSE.txt
--rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-2.6.2/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     7963 2022-11-05 18:37:33.752405 huckle-2.6.2/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     7104 2022-11-05 18:37:00.000000 huckle-2.6.2/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-11-05 18:37:33.751254 huckle-2.6.2/huckle/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-2.6.2/huckle/__init__.py
--rwxr-x---   0 jeff       (501) staff       (20)      308 2022-03-20 22:23:06.000000 huckle-2.6.2/huckle/__main__.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     5057 2022-10-29 17:56:09.000000 huckle-2.6.2/huckle/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-11-05 18:37:33.752157 huckle-2.6.2/huckle/data/
--rwxr-x---   0 jeff       (501) staff       (20)     1865 2022-03-20 22:23:06.000000 huckle-2.6.2/huckle/data/huckle.1
--rwxr-xr-x   0 jeff       (501) staff       (20)    10129 2022-10-29 17:56:09.000000 huckle-2.6.2/huckle/hclinav.py
--rwxr-x---   0 jeff       (501) staff       (20)     2589 2022-03-20 22:23:06.000000 huckle-2.6.2/huckle/huckle.py
--rwxr-x---   0 jeff       (501) staff       (20)      858 2022-03-20 22:23:06.000000 huckle-2.6.2/huckle/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      248 2022-11-05 18:26:58.000000 huckle-2.6.2/huckle/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-11-05 18:37:33.752003 huckle-2.6.2/huckle.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     7963 2022-11-05 18:37:33.000000 huckle-2.6.2/huckle.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      381 2022-11-05 18:37:33.000000 huckle-2.6.2/huckle.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2022-11-05 18:37:33.000000 huckle-2.6.2/huckle.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       48 2022-11-05 18:37:33.000000 huckle-2.6.2/huckle.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       84 2022-11-05 18:37:33.000000 huckle-2.6.2/huckle.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        7 2022-11-05 18:37:33.000000 huckle-2.6.2/huckle.egg-info/top_level.txt
--rwxr-x---   0 jeff       (501) staff       (20)       67 2022-11-05 18:37:33.752623 huckle-2.6.2/setup.cfg
--rwxr-x---   0 jeff       (501) staff       (20)     2745 2022-11-05 18:37:26.000000 huckle-2.6.2/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.079616 huckle-3.0.0/
+-rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.0.0/LICENSE.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.0.0/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-04-09 23:11:31.079683 huckle-3.0.0/PKG-INFO
+-rwx------   0 jeff       (501) staff       (20)     7575 2023-04-09 22:47:09.000000 huckle-3.0.0/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.078526 huckle-3.0.0/huckle/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.0.0/huckle/__init__.py
+-rwxr-x---   0 jeff       (501) staff       (20)      308 2022-03-20 22:23:06.000000 huckle-3.0.0/huckle/__main__.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     4501 2023-04-09 22:30:29.000000 huckle-3.0.0/huckle/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.079514 huckle-3.0.0/huckle/data/
+-rwxr-x---   0 jeff       (501) staff       (20)     2352 2023-04-09 22:53:51.000000 huckle-3.0.0/huckle/data/huckle.1
+-rwxr-xr-x   0 jeff       (501) staff       (20)    10129 2022-10-29 17:56:09.000000 huckle-3.0.0/huckle/hclinav.py
+-rwxr-x---   0 jeff       (501) staff       (20)     2842 2023-04-09 22:16:07.000000 huckle-3.0.0/huckle/huckle.py
+-rwxr-x---   0 jeff       (501) staff       (20)      858 2022-03-20 22:23:06.000000 huckle-3.0.0/huckle/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      248 2023-04-09 19:06:38.000000 huckle-3.0.0/huckle/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.079401 huckle-3.0.0/huckle.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      381 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       48 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       84 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        7 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/top_level.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       67 2023-04-09 23:11:31.079889 huckle-3.0.0/setup.cfg
+-rwxr-x---   0 jeff       (501) staff       (20)     3314 2023-04-09 22:54:19.000000 huckle-3.0.0/setup.py
```

### Comparing `huckle-2.6.2/LICENSE.txt` & `huckle-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `huckle-2.6.2/PKG-INFO` & `huckle-3.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,9 @@
-Metadata-Version: 2.1
-Name: huckle
-Version: 2.6.2
-Summary: A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
-Home-page: https://github.com/cometaj2/huckle
-Author: Jeff Michaud
-Author-email: cometaj2@comcast.net
-License: MIT
-Keywords: cli client hypermedia rest generic development
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE.txt
-
-Huckle (hypermedia unified CLI... with a kick) |build status|_ |pypi|_ 
-======================================================================
+Huckle (hypermedia unified CLI... with a kick) |pyver|_ |build status|_ |pypi|_ 
+===============================================================================
 
 Huckle is a CLI that can act as an impostor for any CLI expressed via hypertext
 command line interface (HCLI) semantics.
 
 ----
 
 Huckle provides a way for developers to interact with, or script around, any API that exposes HCLI
@@ -51,30 +30,36 @@
 [3] http://alps.io
 
 [4] https://groups.google.com/forum/#!forum/huck-hypermedia-unified-cli-with-a-kick
 
 Install Python, pip and huckle
 ------------------------------
 
-Huckle requires bash with access to man pages, Python and pip
-
-  - Install a supported version of Python for your system
+Huckle requires bash with access to man pages, Python and pip. Install a supported version of Python for your system.
 
 Install huckle via Python's pip:
 
-  - pip install huckle
+.. code-block:: console
+
+    pip install huckle
 
 Basic usage
 -----------
 
+huckle env
+
+    This provides a sample environment configuration for your PATH environment variable. This can be permanently configured
+    for your environment by adding the command 'eval $(huckle env) in your shell startup configuration
+    (e.g. .bashrc, .bash_profile, .profile)
+
 huckle cli install \<url>
 
     This attempts to auto create and configure a CLI name if provided with the root URL of an HCLI API.
-    If successful, the CLI can be invoked by name, after restarting the terminal. huckle attempts to update
-    the PATH under .bash_profile and .bashrc to account for login and non-login terminal use.
+    If successful, the CLI can be invoked by name, after updating the path (see 'huckle env'). You can permanently enable
+    HCLI entrypoint scripts by adding 'eval $(huckle env) to your a ~/.bashrc, ~/.bash_profile, or ~/.profile.
     
     Note that an existing configuration file is left alone if the command is run multiple times 
     for the same CLI.
 
     An example HCLI that can be used with Huckle is available on hcli.io:
         - `<http://hcli.io/hcli/cli/jsonf?command=jsonf>`_ (HCLI root)  
         - `<http://hcli.io/hal/#/hcli/cli/jsonf?command=jsonf>`_ (HAL Browser navigation)
@@ -211,7 +196,9 @@
 
 - Disgraceful handling when a cli is invoked when the associated HCLI service is down
   
 .. |build status| image:: https://circleci.com/gh/cometaj2/huckle.svg?style=shield
 .. _build status: https://circleci.com/gh/cometaj2/huckle
 .. |pypi| image:: https://badge.fury.io/py/huckle.svg
 .. _pypi: https://badge.fury.io/py/huckle
+.. |pyver| image:: https://img.shields.io/pypi/pyversions/huckle.svg
+.. _pyver: https://pypi.python.org/pypi/huckle
```

### Comparing `huckle-2.6.2/README.rst` & `huckle-3.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,30 @@
-Huckle (hypermedia unified CLI... with a kick) |build status|_ |pypi|_ 
-======================================================================
+Metadata-Version: 2.1
+Name: huckle
+Version: 3.0.0
+Summary: A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
+Home-page: https://github.com/cometaj2/huckle
+Author: Jeff Michaud
+Author-email: cometaj2@comcast.net
+License: MIT
+Keywords: cli client hypermedia rest generic development
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+Huckle (hypermedia unified CLI... with a kick) |pyver|_ |build status|_ |pypi|_ 
+===============================================================================
 
 Huckle is a CLI that can act as an impostor for any CLI expressed via hypertext
 command line interface (HCLI) semantics.
 
 ----
 
 Huckle provides a way for developers to interact with, or script around, any API that exposes HCLI
@@ -30,30 +51,36 @@
 [3] http://alps.io
 
 [4] https://groups.google.com/forum/#!forum/huck-hypermedia-unified-cli-with-a-kick
 
 Install Python, pip and huckle
 ------------------------------
 
-Huckle requires bash with access to man pages, Python and pip
-
-  - Install a supported version of Python for your system
+Huckle requires bash with access to man pages, Python and pip. Install a supported version of Python for your system.
 
 Install huckle via Python's pip:
 
-  - pip install huckle
+.. code-block:: console
+
+    pip install huckle
 
 Basic usage
 -----------
 
+huckle env
+
+    This provides a sample environment configuration for your PATH environment variable. This can be permanently configured
+    for your environment by adding the command 'eval $(huckle env) in your shell startup configuration
+    (e.g. .bashrc, .bash_profile, .profile)
+
 huckle cli install \<url>
 
     This attempts to auto create and configure a CLI name if provided with the root URL of an HCLI API.
-    If successful, the CLI can be invoked by name, after restarting the terminal. huckle attempts to update
-    the PATH under .bash_profile and .bashrc to account for login and non-login terminal use.
+    If successful, the CLI can be invoked by name, after updating the path (see 'huckle env'). You can permanently enable
+    HCLI entrypoint scripts by adding 'eval $(huckle env) to your a ~/.bashrc, ~/.bash_profile, or ~/.profile.
     
     Note that an existing configuration file is left alone if the command is run multiple times 
     for the same CLI.
 
     An example HCLI that can be used with Huckle is available on hcli.io:
         - `<http://hcli.io/hcli/cli/jsonf?command=jsonf>`_ (HCLI root)  
         - `<http://hcli.io/hal/#/hcli/cli/jsonf?command=jsonf>`_ (HAL Browser navigation)
@@ -190,7 +217,9 @@
 
 - Disgraceful handling when a cli is invoked when the associated HCLI service is down
   
 .. |build status| image:: https://circleci.com/gh/cometaj2/huckle.svg?style=shield
 .. _build status: https://circleci.com/gh/cometaj2/huckle
 .. |pypi| image:: https://badge.fury.io/py/huckle.svg
 .. _pypi: https://badge.fury.io/py/huckle
+.. |pyver| image:: https://img.shields.io/pypi/pyversions/huckle.svg
+.. _pyver: https://pypi.python.org/pypi/huckle
```

### Comparing `huckle-2.6.2/huckle/config.py` & `huckle-3.0.0/huckle/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -68,28 +68,14 @@
     else:
         raise Exception("huckle: the configuration for " + cli + " already exists. leaving the existing configuration untouched.")
 
     hutils.create_folder(cli_manpage_path + "/huckle." + cli)
 
 # sets up an alias for a cli so that it can be called directly by name (instead of calling it via the explicit huckle call) 
 def alias_cli(cli):
-    if not is_configured(dot_bash_profile, dot_huckle_scripts):
-        f = open(dot_bash_profile, "a+")
-        f.write("\n")
-        f.write("# we make sure the huckle entrypoint scripts can be located\n")
-        f.write("export PATH=$PATH:" + dot_huckle_scripts)
-        f.close
-
-    if not is_configured(dot_bashrc, dot_huckle_scripts):
-        f = open(dot_bashrc, "a+")
-        f.write("\n")
-        f.write("# we make sure the huckle entrypoint scripts can be located\n")
-        f.write("export PATH=$PATH:" + dot_huckle_scripts)
-        f.close
-
     if not os.path.exists(dot_huckle_scripts + "/" + cli):
         g = open(dot_huckle_scripts + "/" + cli, "a+")
         os.chmod(dot_huckle_scripts + "/" + cli, 0o700)
         g.write("#!/bin/bash\n")
         g.write("huckle cli run " + cli + " $@")
         g.close
```

### Comparing `huckle-2.6.2/huckle/data/huckle.1` & `huckle-3.0.0/huckle/data/huckle.1`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,36 @@
 .I <parameter>
 ]
 .SH DESCRIPTION
 .B huckle
 is a generic CLI that can be used with any API that abides by
 the standard version 1.0 hypertext command line interface (HCLI) semantics.
 
-A terminal restart is required after the creation of the very first CLI alias. CLI aliases created thereafter are immediately usable.
+CLI aliases are directly invoked by name provided the HCLI entry scripts are locatable in your shell PATH.
+See 'huckle env' for details to make your environment configuration more permanent.
 
 .SH COMMANDS
+.IP "env"
+This outputs the HCLI entry scripts path to export to enable direct HCLI execution by name (i.e. <cliname>. Equivalent to huckle cli run <cliname>).
+
+"eval $(huckle env)" can be setup in ~/.bashrc, ~/.bash_profile or ~/.profile to ensure the path is always loaded on shell start.
 .IP "cli install <url>"
 This attempts to install/auto configure a CLI if provided with the root URL of an HCLI API. If successful, the CLI
-can be invoked by name, and its configuration is located under ~/.huckle/etc/<cliname>/config.
+can be invoked by name.
+
+Its entry script is located under ~/.huckle/bin/<cliname>.
+Its configuration is located under ~/.huckle/etc/<cliname>/config.
 
 Note that an existing configuration file is left alone if the command is run multiple times
 for the same CLI.
 .IP "cli rm <cliname>"
 Removes an installed CLI.
 .IP "cli run <cliname>"
 Used to invoke a CLI by name, the details of which are otherwise left to API implementers. This is equivalent to invoking
-<cliname> directly after CLI installation.
+<cliname> directly after CLI installation and after exporting the huckle env path (see "huckle env").
 .IP "cli ls"
 Lists all the installed CLIs.
 .IP "cli config <cliname>"
 Lists the configuration options of an installed CLI.
 .IP "<cliname> ..."
 The <cliname> alias created for brevity, via huckle cli install.
 .IP "<cliname> ... help"
@@ -42,15 +50,15 @@
 .SH OPTIONS
 .IP --version
 .B huckle
 version and the version of it's dependencies.
 .SH EXAMPLE
 huckle cli install https://hcli.io/hcli/cli/jsonf?command=jsonf
 
-huckle cli run jsonf (equivalent to simply invoking "jsonf" after a successful cli installation and a terminal restart)
+huckle cli run jsonf (equivalent to simply invoking "jsonf" in the shell after a successful cli installation and setup via 'eval $(huckle env)')
 
 huckle cli ls
 
 huckle cli config jsonf
 
 huckle cli rm jsonf
```

### Comparing `huckle-2.6.2/huckle/hclinav.py` & `huckle-3.0.0/huckle/hclinav.py`

 * *Files identical despite different names*

### Comparing `huckle-2.6.2/huckle/huckle.py` & `huckle-3.0.0/huckle/huckle.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,14 +69,20 @@
             huckle_help()
 
     elif len(sys.argv) == 2:
 
         if sys.argv[1] == "--version":
             show_dependencies() 
 
+        elif sys.argv[1] == "env":
+            print("export PATH=$PATH:" + config.dot_huckle_scripts)
+            print("")
+            print("# To point your shell to huckle's HCLI entrypoint scripts, run:")
+            print("# eval $(huckle env)")
+
         elif sys.argv[1] == "help":
             hclinav.display_man_page(config.huckle_manpage_path)
             sys.exit(0)
 
         else:
             huckle_help()
```

### Comparing `huckle-2.6.2/huckle/hutils.py` & `huckle-3.0.0/huckle/hutils.py`

 * *Files identical despite different names*

### Comparing `huckle-2.6.2/huckle.egg-info/PKG-INFO` & `huckle-3.0.0/huckle.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 2.6.2
+Version: 3.0.0
 Summary: A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-Huckle (hypermedia unified CLI... with a kick) |build status|_ |pypi|_ 
-======================================================================
+Huckle (hypermedia unified CLI... with a kick) |pyver|_ |build status|_ |pypi|_ 
+===============================================================================
 
 Huckle is a CLI that can act as an impostor for any CLI expressed via hypertext
 command line interface (HCLI) semantics.
 
 ----
 
 Huckle provides a way for developers to interact with, or script around, any API that exposes HCLI
@@ -51,30 +51,36 @@
 [3] http://alps.io
 
 [4] https://groups.google.com/forum/#!forum/huck-hypermedia-unified-cli-with-a-kick
 
 Install Python, pip and huckle
 ------------------------------
 
-Huckle requires bash with access to man pages, Python and pip
-
-  - Install a supported version of Python for your system
+Huckle requires bash with access to man pages, Python and pip. Install a supported version of Python for your system.
 
 Install huckle via Python's pip:
 
-  - pip install huckle
+.. code-block:: console
+
+    pip install huckle
 
 Basic usage
 -----------
 
+huckle env
+
+    This provides a sample environment configuration for your PATH environment variable. This can be permanently configured
+    for your environment by adding the command 'eval $(huckle env) in your shell startup configuration
+    (e.g. .bashrc, .bash_profile, .profile)
+
 huckle cli install \<url>
 
     This attempts to auto create and configure a CLI name if provided with the root URL of an HCLI API.
-    If successful, the CLI can be invoked by name, after restarting the terminal. huckle attempts to update
-    the PATH under .bash_profile and .bashrc to account for login and non-login terminal use.
+    If successful, the CLI can be invoked by name, after updating the path (see 'huckle env'). You can permanently enable
+    HCLI entrypoint scripts by adding 'eval $(huckle env) to your a ~/.bashrc, ~/.bash_profile, or ~/.profile.
     
     Note that an existing configuration file is left alone if the command is run multiple times 
     for the same CLI.
 
     An example HCLI that can be used with Huckle is available on hcli.io:
         - `<http://hcli.io/hcli/cli/jsonf?command=jsonf>`_ (HCLI root)  
         - `<http://hcli.io/hal/#/hcli/cli/jsonf?command=jsonf>`_ (HAL Browser navigation)
@@ -211,7 +217,9 @@
 
 - Disgraceful handling when a cli is invoked when the associated HCLI service is down
   
 .. |build status| image:: https://circleci.com/gh/cometaj2/huckle.svg?style=shield
 .. _build status: https://circleci.com/gh/cometaj2/huckle
 .. |pypi| image:: https://badge.fury.io/py/huckle.svg
 .. _pypi: https://badge.fury.io/py/huckle
+.. |pyver| image:: https://img.shields.io/pypi/pyversions/huckle.svg
+.. _pyver: https://pypi.python.org/pypi/huckle
```

### Comparing `huckle-2.6.2/setup.py` & `huckle-3.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,32 @@
 
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 from huckle import package
 from huckle import hutils
 
+if sys.argv[-1] == 'dry-run':
+    branch = subprocess.check_output('git rev-parse --abbrev-ref HEAD', shell=True).strip().decode("utf-8")
+    if branch != "master":
+        sys.exit("dry-run from a branch other than master is disallowed.")
+    os.system("rm -rf huckle.egg-info")
+    os.system("rm -rf build")
+    os.system("rm -rf dist")
+    os.system("python setup.py sdist --dry-run")
+    os.system("python setup.py bdist_wheel --dry-run")
+    os.system("twine check dist/*")
+    sys.exit()
+
 if sys.argv[-1] == 'publish':
     branch = subprocess.check_output('git rev-parse --abbrev-ref HEAD', shell=True).strip()
     if branch.decode('ASCII') != "master":
         sys.exit("publishing from a branch other than master is disallowed.")
+    os.system("rm -rf huckle.egg-info")
+    os.system("rm -rf build")
     os.system("rm -rf dist")
     os.system("python setup.py sdist")
     os.system("python setup.py bdist_wheel")
     os.system("twine upload dist/* -r pypi")
     os.system("git tag -a %s -m 'version %s'" % ("huckle-" + package.__version__, "huckle-" + package.__version__))
     os.system("git push")
     os.system("git push --tags")
@@ -36,30 +50,30 @@
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='huckle',
     version=package.__version__,
     description='A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.',
+    long_description_content_type="text/x-rst",    
     long_description=long_description,
     url='https://github.com/cometaj2/huckle',
     author='Jeff Michaud',
     author_email='cometaj2@comcast.net',
     license='MIT',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     keywords='cli client hypermedia rest generic development',
     packages=find_packages(exclude=['__pycache__', 'tests']),
     install_requires=[package.dependencies[0],
                       package.dependencies[1],
                       package.dependencies[2],
                       package.dependencies[3]],
```

