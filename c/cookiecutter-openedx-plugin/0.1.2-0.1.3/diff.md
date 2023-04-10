# Comparing `tmp/cookiecutter-openedx-plugin-0.1.2.tar.gz` & `tmp/cookiecutter-openedx-plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-openedx-plugin-0.1.2.tar", last modified: Sun Apr  9 15:08:52 2023, max compression
+gzip compressed data, was "cookiecutter-openedx-plugin-0.1.3.tar", last modified: Mon Apr 10 18:09:16 2023, max compression
```

## Comparing `cookiecutter-openedx-plugin-0.1.2.tar` & `cookiecutter-openedx-plugin-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:08:52.223916 cookiecutter-openedx-plugin-0.1.2/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.2/LICENSE.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)     7077 2023-04-09 15:08:52.223774 cookiecutter-openedx-plugin-0.1.2/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5284 2023-04-09 15:06:33.000000 cookiecutter-openedx-plugin-0.1.2/README.md
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:08:52.221031 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     7077 2023-04-09 15:08:52.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)      814 2023-04-09 15:08:52.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-09 15:08:52.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-09 15:08:52.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/entry_points.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-09 15:08:52.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/not-zip-safe
--rw-r--r--   0 mcdaniel   (501) staff       (20)      107 2023-04-09 15:08:52.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       20 2023-04-09 15:08:52.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:08:52.222202 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 00:24:18.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     6347 2023-04-08 19:11:42.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/apps.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:08:52.222438 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/badges/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:13.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/badges/__init__.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:08:52.222864 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/badges/backends/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:07.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/badges/backends/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     6862 2023-04-08 13:52:53.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/badges/backends/badgr_boto3.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:08:52.223469 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/settings/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/settings/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)      887 2023-04-08 14:05:20.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/settings/common.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)      166 2023-04-08 14:14:37.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/settings/production.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    16571 2023-04-08 19:02:36.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/signals.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2498 2023-04-08 00:19:59.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/utils.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4800 2023-04-08 14:09:07.000000 cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/waffle.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2707 2023-04-09 15:05:52.000000 cookiecutter-openedx-plugin-0.1.2/pyproject.toml
--rw-r--r--   0 mcdaniel   (501) staff       (20)       38 2023-04-09 15:08:52.223957 cookiecutter-openedx-plugin-0.1.2/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4458 2023-04-08 00:43:51.000000 cookiecutter-openedx-plugin-0.1.2/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-10 18:09:16.110787 cookiecutter-openedx-plugin-0.1.3/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.3/LICENSE.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     7075 2023-04-10 18:09:16.110645 cookiecutter-openedx-plugin-0.1.3/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5282 2023-04-10 18:08:43.000000 cookiecutter-openedx-plugin-0.1.3/README.md
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-10 18:09:16.107702 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     7075 2023-04-10 18:09:16.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      842 2023-04-10 18:09:16.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-10 18:09:16.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-10 18:09:16.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-10 18:09:15.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      107 2023-04-10 18:09:16.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       20 2023-04-10 18:09:16.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-10 18:09:16.109161 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 00:24:18.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     6347 2023-04-08 19:11:42.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/apps.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-10 18:09:16.109374 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/badges/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:13.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/badges/__init__.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-10 18:09:16.109776 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/badges/backends/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:07.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/badges/backends/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     6862 2023-04-08 13:52:53.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/badges/backends/badgr_boto3.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-10 18:09:16.110344 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/settings/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/settings/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      887 2023-04-08 14:05:20.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/settings/common.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      166 2023-04-08 14:14:37.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/settings/production.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    16571 2023-04-08 19:02:36.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/signals.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       94 2023-04-10 18:04:26.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/urls.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2498 2023-04-08 00:19:59.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/utils.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4800 2023-04-08 14:09:07.000000 cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/waffle.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2707 2023-04-10 18:05:11.000000 cookiecutter-openedx-plugin-0.1.3/pyproject.toml
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       38 2023-04-10 18:09:16.110826 cookiecutter-openedx-plugin-0.1.3/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4458 2023-04-08 00:43:51.000000 cookiecutter-openedx-plugin-0.1.3/setup.py
```

### Comparing `cookiecutter-openedx-plugin-0.1.2/LICENSE.txt` & `cookiecutter-openedx-plugin-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.2/PKG-INFO` & `cookiecutter-openedx-plugin-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-openedx-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: An open edx plugin that implements customizations for deployment to Kubernetes
 Home-page: https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Download-URL: https://github.com/cookiecutter-openedx/cookiecutter-openedx-devops.git
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 License: AGPLv3
 Project-URL: Homepage, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
@@ -55,15 +55,15 @@
 
 See [Installing extra xblocks and requirements](https://docs.tutor.overhang.io/configuration.html)
 
 ```bash
 tutor config save       # to ensure that tutor's root folder system has been created
 
 # OPTION 1: install as a PyPi package
-echo "cookiecutter-openedx-plugin>=0.1.2" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+echo "cookiecutter-openedx-plugin>=0.1.3" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 
 # OPTION 2: install as an editable requirement
 echo "-e git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 
 cat "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 tutor images build openedx
 tutor local quickstart
@@ -74,15 +74,15 @@
 Add the following to your [Cookiecutter Github Actions Build workflow](https://github.com/cookiecutter-openedx/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/.github/workflows/build-openedx.yml)
 
 ```yaml
       - name: Add cookiecutter-openedx-plugin
         uses: openedx-actions/tutor-plugin-build-openedx-add-requirement
         with:
           pip-package: cookiecutter-openedx-plugin
-          pip-package-version: ">=0.1.2"
+          pip-package-version: "0.1.3"
 ```
 
 ### Documentation
 
 Documentation is available here: [Documentation](https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin)
 
 ### Support
@@ -91,19 +91,19 @@
 
 ### Contributing
 
 We welcome contributions! cookiecutter-openedx-plugin is part of the [cookiecutter-openedx](https://github.com/cookiecutter-openedx) project. Pull requests are welcome in all repos belonging to this organization. You can also contact [Lawrence McDaniel](https://lawrencemcdaniel.com/contact) directly.
 
 ### Getting Started With Local development
 
-* Use the same virtual environment that you use for edx-platform
-* Ensure that your Python interpreter to 3.8x
-* install black: <https://pypi.org/project/black/>
-* install flake8: <https://flake8.pycqa.org/en/latest/>
-* install flake8-coding: <https://pypi.org/project/flake8-coding/>
+- Use the same virtual environment that you use for edx-platform
+- Ensure that your Python interpreter to 3.8x
+- install black: <https://pypi.org/project/black/>
+- install flake8: <https://flake8.pycqa.org/en/latest/>
+- install flake8-coding: <https://pypi.org/project/flake8-coding/>
 
 ```bash
 # Run these from within your edx-platform virtual environment
 python3 -m venv venv
 source venv/bin/activate
 
 cd /path/to/edx-platform
@@ -117,21 +117,21 @@
 
 pip install pre-commit black flake8
 pre-commit install
 ```
 
 #### Local development good practices
 
-* run `black` on modified code before committing.
-* run `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`
-* run `flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics`
-* run `pre-commit run --all-files` before pushing. see: <https://pre-commit.com/>
+- run `black` on modified code before committing.
+- run `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`
+- run `flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics`
+- run `pre-commit run --all-files` before pushing. see: <https://pre-commit.com/>
 
 #### edx-platform dependencies
 
 To avoid freaky version conflicts in prod it's a good idea to install all of the edx-platform requirements to your local dev virtual environment.
 
-* requirements/edx/base.txt
-* requirements/edx/develop.txt,
-* requirements/edx/testing.txt
+- requirements/edx/base.txt
+- requirements/edx/develop.txt,
+- requirements/edx/testing.txt
 
 At a minimum this will give you the full benefit of your IDE's linter.
```

### Comparing `cookiecutter-openedx-plugin-0.1.2/README.md` & `cookiecutter-openedx-plugin-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 See [Installing extra xblocks and requirements](https://docs.tutor.overhang.io/configuration.html)
 
 ```bash
 tutor config save       # to ensure that tutor's root folder system has been created
 
 # OPTION 1: install as a PyPi package
-echo "cookiecutter-openedx-plugin>=0.1.2" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+echo "cookiecutter-openedx-plugin>=0.1.3" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 
 # OPTION 2: install as an editable requirement
 echo "-e git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 
 cat "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 tutor images build openedx
 tutor local quickstart
@@ -38,15 +38,15 @@
 Add the following to your [Cookiecutter Github Actions Build workflow](https://github.com/cookiecutter-openedx/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/.github/workflows/build-openedx.yml)
 
 ```yaml
       - name: Add cookiecutter-openedx-plugin
         uses: openedx-actions/tutor-plugin-build-openedx-add-requirement
         with:
           pip-package: cookiecutter-openedx-plugin
-          pip-package-version: ">=0.1.2"
+          pip-package-version: "0.1.3"
 ```
 
 ### Documentation
 
 Documentation is available here: [Documentation](https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin)
 
 ### Support
@@ -55,19 +55,19 @@
 
 ### Contributing
 
 We welcome contributions! cookiecutter-openedx-plugin is part of the [cookiecutter-openedx](https://github.com/cookiecutter-openedx) project. Pull requests are welcome in all repos belonging to this organization. You can also contact [Lawrence McDaniel](https://lawrencemcdaniel.com/contact) directly.
 
 ### Getting Started With Local development
 
-* Use the same virtual environment that you use for edx-platform
-* Ensure that your Python interpreter to 3.8x
-* install black: <https://pypi.org/project/black/>
-* install flake8: <https://flake8.pycqa.org/en/latest/>
-* install flake8-coding: <https://pypi.org/project/flake8-coding/>
+- Use the same virtual environment that you use for edx-platform
+- Ensure that your Python interpreter to 3.8x
+- install black: <https://pypi.org/project/black/>
+- install flake8: <https://flake8.pycqa.org/en/latest/>
+- install flake8-coding: <https://pypi.org/project/flake8-coding/>
 
 ```bash
 # Run these from within your edx-platform virtual environment
 python3 -m venv venv
 source venv/bin/activate
 
 cd /path/to/edx-platform
@@ -81,21 +81,21 @@
 
 pip install pre-commit black flake8
 pre-commit install
 ```
 
 #### Local development good practices
 
-* run `black` on modified code before committing.
-* run `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`
-* run `flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics`
-* run `pre-commit run --all-files` before pushing. see: <https://pre-commit.com/>
+- run `black` on modified code before committing.
+- run `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`
+- run `flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics`
+- run `pre-commit run --all-files` before pushing. see: <https://pre-commit.com/>
 
 #### edx-platform dependencies
 
 To avoid freaky version conflicts in prod it's a good idea to install all of the edx-platform requirements to your local dev virtual environment.
 
-* requirements/edx/base.txt
-* requirements/edx/develop.txt,
-* requirements/edx/testing.txt
+- requirements/edx/base.txt
+- requirements/edx/develop.txt,
+- requirements/edx/testing.txt
 
 At a minimum this will give you the full benefit of your IDE's linter.
```

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/PKG-INFO` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-openedx-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: An open edx plugin that implements customizations for deployment to Kubernetes
 Home-page: https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Download-URL: https://github.com/cookiecutter-openedx/cookiecutter-openedx-devops.git
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 License: AGPLv3
 Project-URL: Homepage, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
@@ -55,15 +55,15 @@
 
 See [Installing extra xblocks and requirements](https://docs.tutor.overhang.io/configuration.html)
 
 ```bash
 tutor config save       # to ensure that tutor's root folder system has been created
 
 # OPTION 1: install as a PyPi package
-echo "cookiecutter-openedx-plugin>=0.1.2" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+echo "cookiecutter-openedx-plugin>=0.1.3" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 
 # OPTION 2: install as an editable requirement
 echo "-e git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 
 cat "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 tutor images build openedx
 tutor local quickstart
@@ -74,15 +74,15 @@
 Add the following to your [Cookiecutter Github Actions Build workflow](https://github.com/cookiecutter-openedx/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/.github/workflows/build-openedx.yml)
 
 ```yaml
       - name: Add cookiecutter-openedx-plugin
         uses: openedx-actions/tutor-plugin-build-openedx-add-requirement
         with:
           pip-package: cookiecutter-openedx-plugin
-          pip-package-version: ">=0.1.2"
+          pip-package-version: "0.1.3"
 ```
 
 ### Documentation
 
 Documentation is available here: [Documentation](https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin)
 
 ### Support
@@ -91,19 +91,19 @@
 
 ### Contributing
 
 We welcome contributions! cookiecutter-openedx-plugin is part of the [cookiecutter-openedx](https://github.com/cookiecutter-openedx) project. Pull requests are welcome in all repos belonging to this organization. You can also contact [Lawrence McDaniel](https://lawrencemcdaniel.com/contact) directly.
 
 ### Getting Started With Local development
 
-* Use the same virtual environment that you use for edx-platform
-* Ensure that your Python interpreter to 3.8x
-* install black: <https://pypi.org/project/black/>
-* install flake8: <https://flake8.pycqa.org/en/latest/>
-* install flake8-coding: <https://pypi.org/project/flake8-coding/>
+- Use the same virtual environment that you use for edx-platform
+- Ensure that your Python interpreter to 3.8x
+- install black: <https://pypi.org/project/black/>
+- install flake8: <https://flake8.pycqa.org/en/latest/>
+- install flake8-coding: <https://pypi.org/project/flake8-coding/>
 
 ```bash
 # Run these from within your edx-platform virtual environment
 python3 -m venv venv
 source venv/bin/activate
 
 cd /path/to/edx-platform
@@ -117,21 +117,21 @@
 
 pip install pre-commit black flake8
 pre-commit install
 ```
 
 #### Local development good practices
 
-* run `black` on modified code before committing.
-* run `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`
-* run `flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics`
-* run `pre-commit run --all-files` before pushing. see: <https://pre-commit.com/>
+- run `black` on modified code before committing.
+- run `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`
+- run `flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics`
+- run `pre-commit run --all-files` before pushing. see: <https://pre-commit.com/>
 
 #### edx-platform dependencies
 
 To avoid freaky version conflicts in prod it's a good idea to install all of the edx-platform requirements to your local dev virtual environment.
 
-* requirements/edx/base.txt
-* requirements/edx/develop.txt,
-* requirements/edx/testing.txt
+- requirements/edx/base.txt
+- requirements/edx/develop.txt,
+- requirements/edx/testing.txt
 
 At a minimum this will give you the full benefit of your IDE's linter.
```

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_openedx_plugin.egg-info/SOURCES.txt` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_openedx_plugin.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 cookiecutter_openedx_plugin.egg-info/entry_points.txt
 cookiecutter_openedx_plugin.egg-info/not-zip-safe
 cookiecutter_openedx_plugin.egg-info/requires.txt
 cookiecutter_openedx_plugin.egg-info/top_level.txt
 cookiecutter_plugin/__init__.py
 cookiecutter_plugin/apps.py
 cookiecutter_plugin/signals.py
+cookiecutter_plugin/urls.py
 cookiecutter_plugin/utils.py
 cookiecutter_plugin/waffle.py
 cookiecutter_plugin/badges/__init__.py
 cookiecutter_plugin/badges/backends/__init__.py
 cookiecutter_plugin/badges/backends/badgr_boto3.py
 cookiecutter_plugin/settings/__init__.py
 cookiecutter_plugin/settings/common.py
```

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/apps.py` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/apps.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/badges/backends/badgr_boto3.py` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/badges/backends/badgr_boto3.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/settings/common.py` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/settings/common.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/signals.py` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/signals.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/utils.py` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.2/cookiecutter_plugin/waffle.py` & `cookiecutter-openedx-plugin-0.1.3/cookiecutter_plugin/waffle.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.2/pyproject.toml` & `cookiecutter-openedx-plugin-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 #------------------------------------------------------------------------------
 # PyPi meta data
 #------------------------------------------------------------------------------
 [project]
 name = "cookiecutter-openedx-plugin"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Lawrence McDaniel", email="lpm0073@gmail.com" }
 ]
 description = "An open edx plugin that implements customizations for deployment to Kubernetes"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cookiecutter-openedx-plugin-0.1.2/setup.py` & `cookiecutter-openedx-plugin-0.1.3/setup.py`

 * *Files identical despite different names*

