# Comparing `tmp/sysdweb-1.1.4.tar.gz` & `tmp/sysdweb-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysdweb-1.1.4.tar", last modified: Tue May 17 08:12:39 2022, max compression
+gzip compressed data, was "sysdweb-1.1.5.tar", last modified: Mon Apr 10 11:50:36 2023, max compression
```

## Comparing `sysdweb-1.1.4.tar` & `sysdweb-1.1.5.tar`

### file list

```diff
@@ -1,43 +1,35 @@
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.889915 sysdweb-1.1.4/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    35141 2018-04-16 14:00:34.000000 sysdweb-1.1.4/LICENSE
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)      156 2018-04-16 14:00:34.000000 sysdweb-1.1.4/MANIFEST.in
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     3866 2022-05-17 08:12:39.889915 sysdweb-1.1.4/PKG-INFO
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     2884 2022-05-09 11:30:58.000000 sysdweb-1.1.4/README.md
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)       56 2018-04-16 14:00:34.000000 sysdweb-1.1.4/requirements.txt
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)       38 2022-05-17 08:12:39.889915 sysdweb-1.1.4/setup.cfg
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     2055 2019-03-13 12:11:28.000000 sysdweb-1.1.4/setup.py
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.876581 sysdweb-1.1.4/sysdweb/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)      441 2022-05-17 08:06:17.000000 sysdweb-1.1.4/sysdweb/__init__.py
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     3697 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/config.py
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     2006 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/main.py
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     6300 2022-05-17 08:04:31.000000 sysdweb-1.1.4/sysdweb/server.py
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     2765 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/systemd.py
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.873247 sysdweb-1.1.4/sysdweb/templates/
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.873247 sysdweb-1.1.4/sysdweb/templates/static/
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.879914 sysdweb-1.1.4/sysdweb/templates/static/css/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    23409 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/css/bootstrap-theme.min.css
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)   121200 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/css/bootstrap.min.css
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)      315 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/css/sysdweb.css
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.886581 sysdweb-1.1.4/sysdweb/templates/static/fonts/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    20127 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)   108738 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    45404 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    23424 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    18028 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.886581 sysdweb-1.1.4/sysdweb/templates/static/img/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)   370070 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/img/favicon.ico
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    18861 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/img/favicon.png
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.889915 sysdweb-1.1.4/sysdweb/templates/static/js/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)    37045 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/js/bootstrap.min.js
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)      902 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/static/js/sysdweb.js
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.889915 sysdweb-1.1.4/sysdweb/templates/views/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     4421 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/views/index.tpl
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     1332 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb/templates/views/journal.tpl
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     1451 2018-04-16 14:00:34.000000 sysdweb-1.1.4/sysdweb.conf
-drwxr-xr-x   0 ogarcia   (1000) ogarcia   (1000)        0 2022-05-17 08:12:39.879914 sysdweb-1.1.4/sysdweb.egg-info/
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     3866 2022-05-17 08:12:39.000000 sysdweb-1.1.4/sysdweb.egg-info/PKG-INFO
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)     1047 2022-05-17 08:12:39.000000 sysdweb-1.1.4/sysdweb.egg-info/SOURCES.txt
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)        1 2022-05-17 08:12:39.000000 sysdweb-1.1.4/sysdweb.egg-info/dependency_links.txt
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)       47 2022-05-17 08:12:39.000000 sysdweb-1.1.4/sysdweb.egg-info/entry_points.txt
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)       54 2022-05-17 08:12:39.000000 sysdweb-1.1.4/sysdweb.egg-info/requires.txt
--rw-r--r--   0 ogarcia   (1000) ogarcia   (1000)        8 2022-05-17 08:12:39.000000 sysdweb-1.1.4/sysdweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.735920 sysdweb-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-10 11:50:25.000000 sysdweb-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44302 2023-04-10 11:50:36.735920 sysdweb-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-10 11:50:25.000000 sysdweb-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-10 11:50:25.000000 sysdweb-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:50:36.735920 sysdweb-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.731920 sysdweb-1.1.5/sysdweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/systemd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.727920 sysdweb-1.1.5/sysdweb/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.727920 sysdweb-1.1.5/sysdweb/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.731920 sysdweb-1.1.5/sysdweb/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   522639 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/css/sysdweb.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.731920 sysdweb-1.1.5/sysdweb/templates/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   370070 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/img/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.735920 sysdweb-1.1.5/sysdweb/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80420 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   333078 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/static/js/sysdweb.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.735920 sysdweb-1.1.5/sysdweb/templates/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/views/index.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-10 11:50:25.000000 sysdweb-1.1.5/sysdweb/templates/views/journal.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:50:36.731920 sysdweb-1.1.5/sysdweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44302 2023-04-10 11:50:36.000000 sysdweb-1.1.5/sysdweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-10 11:50:36.000000 sysdweb-1.1.5/sysdweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:50:36.000000 sysdweb-1.1.5/sysdweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 11:50:36.000000 sysdweb-1.1.5/sysdweb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-10 11:50:36.000000 sysdweb-1.1.5/sysdweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 11:50:36.000000 sysdweb-1.1.5/sysdweb.egg-info/top_level.txt
```

### Comparing `sysdweb-1.1.4/LICENSE` & `sysdweb-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sysdweb-1.1.4/README.md` & `sysdweb-1.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 ### From source
 
 ```sh
 git clone https://github.com/ogarcia/sysdweb.git
 virtualenv3 ./sysdweb-venv
 source ./sysdweb-venv/bin/activate
 cd sysdweb
-pip install -r requirements.txt
-python setup.py install
+pip install .
 ```
 
 ### From pypi
 
 ```sh
 virtualenv3 ./sysdweb-venv
 source ./sysdweb-venv/bin/activate
@@ -41,15 +40,15 @@
 
 Once you have configured sysdweb, simply run.
 
 ```
 sysdweb
 ```
 
-By default sysdweb listen in 10080 port to 127.0.0.1, you can change listen
+By default sysdweb listen in 10088 port to 127.0.0.1, you can change listen
 port and address with `-p` and `-l` or via environment variables.
 
 ```sh
 sysdweb -p 9080 -l 0.0.0.0
 ```
 
 Current config environment variables are the following.
@@ -109,21 +108,21 @@
 By default `/api/v1/<service>/journal` returns 100 tail lines of journal
 file of `<service>` unit. You can specify the number of lines by this way.
 
 ```
 /api/v1/<service>/journal/200
 ```
 
-In the example defined above all valid enpoins are.
+In the example defined above all valid endpoints are.
 
 ```
-http://127.0.0.1:10080/api/v1/ngx/start
-http://127.0.0.1:10080/api/v1/ngx/stop
-http://127.0.0.1:10080/api/v1/ngx/restart
-http://127.0.0.1:10080/api/v1/ngx/reload
-http://127.0.0.1:10080/api/v1/ngx/reloadorrestart
-http://127.0.0.1:10080/api/v1/ngx/status
-http://127.0.0.1:10080/api/v1/ngx/journal
-http://127.0.0.1:10080/api/v1/ngx/journal/<number>
+http://127.0.0.1:10088/api/v1/ngx/start
+http://127.0.0.1:10088/api/v1/ngx/stop
+http://127.0.0.1:10088/api/v1/ngx/restart
+http://127.0.0.1:10088/api/v1/ngx/reload
+http://127.0.0.1:10088/api/v1/ngx/reloadorrestart
+http://127.0.0.1:10088/api/v1/ngx/status
+http://127.0.0.1:10088/api/v1/ngx/journal
+http://127.0.0.1:10088/api/v1/ngx/journal/<number>
 ```
 
 [1]: https://aur.archlinux.org/packages/sysdweb/
```

### Comparing `sysdweb-1.1.4/sysdweb/config.py` & `sysdweb-1.1.5/sysdweb/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,98 @@
-#! /usr/bin/env python
-# -*- coding: utf-8 -*-
 # vim:fenc=utf-8
 #
-# Copyright © 2016-2018 Óscar García Amor <ogarcia@connectical.com>
+# Copyright © 2016-2023 Óscar García Amor <ogarcia@connectical.com>
 #
 # Distributed under terms of the GNU GPLv3 license.
 
 import configparser
 import grp
 import logging
 import os
 import pwd
 
-def checkConfig(file=None):
+CONFIG_FILE_NAME = 'sysdweb.conf'
+LOCAL_CONFIG_FILE = os.path.join('.', CONFIG_FILE_NAME)
+SYSTEM_CONFIG_FILE = os.path.join('/etc', CONFIG_FILE_NAME)
+
+logger = logging.getLogger(__name__)
+
+def _get_config_file():
+    xdg_config_home = os.environ.get('XDG_CONFIG_HOME', os.path.join(os.path.expanduser('~'), '.config'))
+    logger.debug(f'XDG_CONFIG_HOME: \'{xdg_config_home}\'.')
+    user_config_file = os.path.join(xdg_config_home, 'sysdweb', CONFIG_FILE_NAME)
+    logger.debug(f'User config file: \'{user_config_file}\'.')
+    for config_file in [LOCAL_CONFIG_FILE, user_config_file, SYSTEM_CONFIG_FILE]:
+        if os.access(config_file, os.R_OK):
+            logger.debug(f'Config file found: \'{config_file}\'.')
+            return config_file
+    raise SystemExit('No config file found.')
+
+def configure(config, config_file=None):
     """
     Parse config and discards errors
     """
-    logger = logging.getLogger('sysdweb.checkConfig')
-    if file != None:
-        if os.access(file, os.R_OK):
-            config_file = [file]
-        else:
-            raise SystemExit('Cannot read config file \'{}\'.'.format(file))
+    if config_file is None:
+        # Try to get one of default config locations
+        config_file = _get_config_file()
     else:
-        config_files = [ './sysdweb.conf',
-                os.path.join(os.path.expanduser('~'), '.config/sysdweb/sysdweb.conf'),
-                '/etc/sysdweb.conf' ]
-        # Try to load one of config locations
-        config_file = [file for file in config_files if os.access(file, os.R_OK)]
-        if config_file == []:
-            raise SystemExit('No config file found.')
-    logger.info('Using config file \'{}\'.'.format(config_file[0]))
+        if not os.access(config_file, os.R_OK):
+            raise SystemExit(f'Cannot read config file \'{config_file}\'.')
+    logger.info(f'Using config file \'{config_file}\'.')
 
-    config = configparser.ConfigParser()
     try:
-        config.read(config_file[0])
-    except Exception as e:
-        err = 'sysdweb config file is corrupted.\n{0}'.format(e)
-        raise SystemExit(err)
+        config.read(config_file)
+    except Exception as err:
+        raise SystemExit(f'sysdweb config file is corrupted.\n{err}')
 
     # Configure valid users
-    if config.get('DEFAULT', 'scope', fallback='system') == 'system':
+    scope = config.get('DEFAULT', 'scope', fallback='system')
+    if scope == 'system':
         # Get a full list of users
         users = config.get('DEFAULT', 'users', fallback=None)
         groups = config.get('DEFAULT', 'groups', fallback=None)
-
-        if users:
-            users = [user.strip() for user in users.split(',')]
-        else:
-            users = []
-
-        if groups:
-            groups = [group.strip() for group in groups.split(',')]
+        users = [] if users is None else list(map(lambda u: u.strip(), users.split(',')))
+        if groups is not None:
+            groups = map(lambda g: g.strip(), groups.split(','))
             # Obtain usenames from groups
             for group in groups:
                 try:
                     users.extend(grp.getgrnam(group)[3])
                 except KeyError:
-                    logger.warning('Group \'{}\' not found in database, skipped.'.format(group))
-
+                    logger.warning(f'Group \'{group}\' not found in database, skipped.')
         # If left any user in list send to main process
-        if users:
+        if users == []:
+            logger.debug('Running in system mode, ALL system users are valid.')
+        else:
             users = list(set(users)) # Remove duplicates
             users.sort() # Sort alphabetically
             logger.debug('Running in system mode, valid users \'{}\'.'.format(', '.join(users)))
             config.set('DEFAULT', 'users', ','.join(users))
-        else:
-            logger.debug('Running in system mode, ALL system users are valid.')
-    else:
+    elif scope == 'user':
         # Only current user can log in
         user = pwd.getpwuid(os.getuid())[0]
-        logger.debug('Running in user mode, valid user \'{}\'.'.format(user))
+        logger.info(f'Running in user mode, valid user \'{user}\'.')
         config.set('DEFAULT', 'users', user)
+    else:
+        raise SystemExit(f'Invalid scope \'{scope}\', must be \'system\' or \'user\'.')
 
     # Read all sections to check if are correctly configurated
     for section in config.sections():
-        if not config.get(section, 'title', fallback=None):
+        if config.get(section, 'title', fallback=None) is None:
             config.remove_section(section)
-            logger.warning('Removed invalid section without title \'{}\' from config.'.format(section))
+            logger.warning(f'Removed invalid section without title \'{section}\' from config.')
         else:
-            if not config.get(section, 'unit', fallback=None):
+            unit = config.get(section, 'unit', fallback=None)
+            if unit is None:
                 config.remove_section(section)
-                logger.warning('Removed invalid section without unit \'{}\' from config.'.format(section))
+                logger.warning(f'Removed invalid section without unit \'{section}\' from config.')
             else:
-                unit = config.get(section, 'unit')
                 if not '.service' in unit:
-                    unit = '{}.service'.format(unit)
+                    unit = f'{unit}.service'
                     config.set(section, 'unit', unit)
-                logger.debug('Configured section \'{}\' for unit \'{}\''.format(section, unit))
+                logger.debug(f'Configured section \'{section}\' for unit \'{unit}\'.')
 
     # If after check all sections no valid sections remain, exit with error
     if len(config.sections()) < 1:
         raise SystemExit('Error in config. No valid sections found.')
 
-    return config
+config = configparser.ConfigParser()
```

### Comparing `sysdweb-1.1.4/sysdweb/main.py` & `sysdweb-1.1.5/sysdweb/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-#! /usr/bin/env python
-# -*- coding: utf-8 -*-
 # vim:fenc=utf-8
 #
-# Copyright © 2016-2018 Óscar García Amor <ogarcia@connectical.com>
+# Copyright © 2016-2023 Óscar García Amor <ogarcia@connectical.com>
 #
 # Distributed under terms of the GNU GPLv3 license.
 
 from sysdweb.server import start
 
 import argparse
 import logging
@@ -32,15 +30,15 @@
             1: logging.INFO,
             2: logging.DEBUG }
 
     # Create argument parser to get config via arguments
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config', metavar='value', default=config, help='custom configuration file path')
     parser.add_argument('-l', '--listen', metavar='value', default=host, help='listen address (host or ip), default: 127.0.0.1')
-    parser.add_argument('-p', '--port', metavar='value', default=port, help='listen port, default: 10080')
+    parser.add_argument('-p', '--port', metavar='value', default=port, help='listen port, default: 10088')
     parser.add_argument('-v', '--verbose', action='count', default=0, help='be verbose (add more v to increase verbosity)')
     args = parser.parse_args()
 
     # Maximum loglevel is 3 if user sends more vvv we ignore it
     args.verbose = 2 if args.verbose >= 2 else args.verbose
 
     # Set loglevel via argument or environment (untouched warning by default)
```

### Comparing `sysdweb-1.1.4/sysdweb/server.py` & `sysdweb-1.1.5/sysdweb/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-#! /usr/bin/env python
-# -*- coding: utf-8 -*-
 # vim:fenc=utf-8
 #
-# Copyright © 2016-2018 Óscar García Amor <ogarcia@connectical.com>
+# Copyright © 2016-2023 Óscar García Amor <ogarcia@connectical.com>
 #
 # Distributed under terms of the GNU GPLv3 license.
 
 from bottle import abort, auth_basic, response, route, hook, run, static_file, template, TEMPLATE_PATH
 from pam import pam
 from socket import gethostname
-from sysdweb.config import checkConfig
+from sysdweb.config import config, configure
 from sysdweb.systemd import systemdBus, Journal
 
 import os
 
 # Search for template path
 template_paths = [ os.path.join(os.path.abspath(os.path.dirname(__file__)), 'templates'),
         '/usr/share/sysdweb/templates']
@@ -83,37 +81,37 @@
             return {'journal': 'not-found'}
         try:
             lines = int(lines)
         except Exception as e:
             response.status = 500
             return {'msg': '{}'.format(e)}
         unit = config.get(service, 'unit')
-        journal = Journal(unit)
+        journal = Journal(unit, True) if config.get('DEFAULT', 'scope', fallback='system') == 'user' else Journal(unit)
         return {'journal': journal.get_tail(lines)}
     else:
         response.status = 400
         return {'msg': 'Sorry, but \'{}\' is not defined in config.'.format(service)}
 
 @route('/')
 @auth_basic(login)
 def get_main():
     services = []
     for service in config.sections():
         service_status = get_service_action(service, 'status')
         if service_status['status'] == 'not-found':
-            cls = 'active'
+            cls = 'light'
         elif service_status['status'] == 'inactive' or service_status['status'] == 'failed':
             cls = 'danger'
         elif service_status['status'] == 'active':
             cls = 'success'
         else:
             cls = 'warning'
-        disabled_start = True if cls == 'active' or cls == 'success' else False
-        disabled_stop = True if cls == 'active' or cls == 'danger' else False
-        disabled_restart = True if cls == 'active' or cls == 'danger' else False
+        disabled_start = True if cls == 'light' or cls == 'success' else False
+        disabled_stop = True if cls == 'light' or cls == 'danger' else False
+        disabled_restart = True if cls == 'light' or cls == 'danger' else False
         services.append({'class': cls,
             'disabled_start': disabled_start,
             'disabled_stop': disabled_stop,
             'disabled_restart': disabled_restart,
             'title': config.get(service, 'title'),
             'service': service})
     return template('index', hostname=gethostname(), services=services)
@@ -136,32 +134,26 @@
     return static_file('favicon.ico', root=os.path.join(static_path, 'img'))
 
 @route('/css/<file>')
 @auth_basic(login)
 def get_css(file):
     return static_file(file, root=os.path.join(static_path, 'css'))
 
-@route('/fonts/<file>')
-@auth_basic(login)
-def get_fonts(file):
-    return static_file(file, root=os.path.join(static_path, 'fonts'))
-
 @route('/img/<file>')
 @auth_basic(login)
 def get_img(file):
     return static_file(file, root=os.path.join(static_path, 'img'))
 
 @route('/js/<file>')
 @auth_basic(login)
 def get_js(file):
     return static_file(file, root=os.path.join(static_path, 'js'))
 
 def start(config_file, host, port):
     # Check config
-    global config
-    config = checkConfig(config_file)
+    configure(config, config_file)
 
-    if host == None: host = config.get('DEFAULT', 'host', fallback='127.0.0.1')
-    if port == None: port = config.get('DEFAULT', 'port', fallback='10080')
+    if host is None: host = config.get('DEFAULT', 'host', fallback='127.0.0.1')
+    if port is None: port = config.get('DEFAULT', 'port', fallback='10088')
 
     # Run webserver
     run(host=host, port=port)
```

### Comparing `sysdweb-1.1.4/sysdweb/systemd.py` & `sysdweb-1.1.5/sysdweb/systemd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-#! /usr/bin/env python
-# -*- coding: utf-8 -*-
 # vim:fenc=utf-8
 #
-# Copyright © 2016-2018 Óscar García Amor <ogarcia@connectical.com>
+# Copyright © 2016-2023 Óscar García Amor <ogarcia@connectical.com>
 #
 # Distributed under terms of the GNU GPLv3 license.
 
 from dbus import SystemBus, SessionBus, Interface, exceptions
 from systemd import journal
 
 DBUS_INTERFACE = 'org.freedesktop.DBus.Properties'
@@ -65,17 +63,18 @@
         try:
             self.manager.ReloadOrRestartUnit(unit, 'replace')
             return True
         except exceptions.DBusException:
             return False
 
 class Journal(object):
-    def __init__(self, unit):
+    def __init__(self, unit, user=False):
         self.reader = journal.Reader()
-        self.reader.add_match(_SYSTEMD_UNIT=unit)
+        match = f'_SYSTEMD_USER_UNIT={unit}' if user else f'_SYSTEMD_UNIT={unit}'
+        self.reader.add_match(match)
 
     def get_tail(self, lines):
         self.reader.seek_tail()
         self.reader.get_previous(lines)
         journal_lines = ['{__REALTIME_TIMESTAMP} {MESSAGE}'.format(**value) for value in self.reader]
         self.reader.close()
         return journal_lines
```

### Comparing `sysdweb-1.1.4/sysdweb/templates/static/img/favicon.ico` & `sysdweb-1.1.5/sysdweb/templates/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `sysdweb-1.1.4/sysdweb/templates/static/img/favicon.png` & `sysdweb-1.1.5/sysdweb/templates/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `sysdweb-1.1.4/sysdweb.egg-info/SOURCES.txt` & `sysdweb-1.1.5/sysdweb.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 LICENSE
-MANIFEST.in
 README.md
-requirements.txt
-setup.py
-sysdweb.conf
+pyproject.toml
 sysdweb/__init__.py
 sysdweb/config.py
 sysdweb/main.py
 sysdweb/server.py
 sysdweb/systemd.py
 sysdweb.egg-info/PKG-INFO
 sysdweb.egg-info/SOURCES.txt
 sysdweb.egg-info/dependency_links.txt
 sysdweb.egg-info/entry_points.txt
 sysdweb.egg-info/requires.txt
 sysdweb.egg-info/top_level.txt
-sysdweb/templates/static/css/bootstrap-theme.min.css
 sysdweb/templates/static/css/bootstrap.min.css
+sysdweb/templates/static/css/bootstrap.min.css.map
 sysdweb/templates/static/css/sysdweb.css
-sysdweb/templates/static/fonts/glyphicons-halflings-regular.eot
-sysdweb/templates/static/fonts/glyphicons-halflings-regular.svg
-sysdweb/templates/static/fonts/glyphicons-halflings-regular.ttf
-sysdweb/templates/static/fonts/glyphicons-halflings-regular.woff
-sysdweb/templates/static/fonts/glyphicons-halflings-regular.woff2
 sysdweb/templates/static/img/favicon.ico
 sysdweb/templates/static/img/favicon.png
-sysdweb/templates/static/js/bootstrap.min.js
+sysdweb/templates/static/js/bootstrap.bundle.min.js
+sysdweb/templates/static/js/bootstrap.bundle.min.js.map
 sysdweb/templates/static/js/sysdweb.js
 sysdweb/templates/views/index.tpl
 sysdweb/templates/views/journal.tpl
```

