# Comparing `tmp/pdm-django-0.5.2.tar.gz` & `tmp/pdm-django-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-django-0.5.2.tar", last modified: Mon Aug  8 20:28:48 2022, max compression
+gzip compressed data, was "pdm-django-1.0.0.tar", last modified: Mon Apr 10 16:35:57 2023, max compression
```

## Comparing `pdm-django-0.5.2.tar` & `pdm-django-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-rw-r--   0 paul      (1000) paul      (1000)     1069 2022-08-08 19:49:48.460456 pdm-django-0.5.2/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)     1415 2022-08-08 20:02:09.502345 pdm-django-0.5.2/README.md
--rw-rw-r--   0 paul      (1000) paul      (1000)        0 2022-08-08 19:49:48.460456 pdm-django-0.5.2/pdm_django/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1856 2022-08-08 20:23:56.223770 pdm-django-0.5.2/pdm_django/main.py
--rw-rw-r--   0 paul      (1000) paul      (1000)      724 2022-08-08 20:24:04.707680 pdm-django-0.5.2/pyproject.toml
--rw-------   0 paul      (1000) paul      (1000)     1704 2022-08-08 20:28:48.520704 pdm-django-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-10 16:25:26.286469 pdm-django-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1415 2023-04-10 16:25:26.286469 pdm-django-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 16:25:26.286469 pdm-django-1.0.0/pdm_django/__init__.py
+-rw-r--r--   0        0        0     1778 2023-04-10 16:28:40.186395 pdm-django-1.0.0/pdm_django/main.py
+-rw-r--r--   0        0        0      808 2023-04-10 16:35:21.046204 pdm-django-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 pdm-django-1.0.0/PKG-INFO
```

### Comparing `pdm-django-0.5.2/LICENSE` & `pdm-django-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-django-0.5.2/README.md` & `pdm-django-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm-django-0.5.2/pdm_django/main.py` & `pdm-django-1.0.0/pdm_django/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 import sys
 
 from pdm.cli.utils import PdmFormatter
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.commands.run import Command as RunCommand
 from pdm.cli.commands.run import TaskRunner
 from pdm.cli.hooks import HookManager
-from pdm.cli.options import skip_option
 from pdm.cli.utils import check_project_file
 
 
 class DjangoRunCommand(RunCommand):
   OPTIONS = []
   COMMAND_PREFIX = []
 
   def add_arguments(self, parser):
-    skip_option.add_to_parser(parser)
     parser.add_argument(
       "-s",
       "--site-packages",
       action="store_true",
       help="Load site-packages from the selected interpreter",
     )
     parser.add_argument(
```

### Comparing `pdm-django-0.5.2/pyproject.toml` & `pdm-django-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-django"
-version = "0.5.2"
+version = "1.0.0"
 description = "pdm shortcuts for Django projects"
 authors = [
     { name = "Paul Bailey", email = "paul@neutron.studio" },
 ]
 dependencies = []
 requires-python = ">=3.7"
 readme = "README.md"
@@ -25,14 +25,15 @@
     "yapf>=0.32.0",
     "toml>=0.10.2",
 ]
 
 [tool.pdm.scripts]
 format = "yapf -rpi -vv ."
 check_format = "yapf -rpd ."
+publish = "pdm publish --username __token__ --password $PDM_PUBLISH_PASSWORD_NSYNC"
 
 [tool.pdm.scripts._]
 env_file = ".env"
 
 [build-system]
 requires = [
     "pdm-pep517",
```

### Comparing `pdm-django-0.5.2/PKG-INFO` & `pdm-django-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-django
-Version: 0.5.2
+Version: 1.0.0
 Summary: pdm shortcuts for Django projects
 License: MIT
 Author-email: Paul Bailey <paul@neutron.studio>
 Requires-Python: >=3.7
 Project-URL: homepage, https://github.com/neutron-sync/pdm-django
 Description-Content-Type: text/markdown
```

