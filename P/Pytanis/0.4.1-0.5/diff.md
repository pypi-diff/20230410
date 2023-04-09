# Comparing `tmp/pytanis-0.4.1.tar.gz` & `tmp/pytanis-0.5.tar.gz`

## Comparing `pytanis-0.4.1.tar` & `pytanis-0.5.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pytanis-0.4.1/.flake8
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pytanis-0.4.1/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytanis-0.4.1/.linkcheckerrc
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pytanis-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 pytanis-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 pytanis-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 pytanis-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/authors.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/changelog.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/contributing.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/index.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/license.md
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/favicon.svg
--rw-r--r--   0        0        0   363926 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/gsheet_proposal_selection.png
--rw-r--r--   0        0        0   259341 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/gsheet_schedule.png
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/icon.svg
--rw-r--r--   0        0        0    35049 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/logo.svg
--rw-r--r--   0        0        0    54963 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/logo_banner.png
--rw-r--r--   0        0        0    34834 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/logo_banner.svg
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/pillars_black.svg
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/assets/images/pillars_white.svg
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/scripts/gen_ref_nav.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/scripts/set_release_version.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/snippets/links.txt
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/tasks/cfp.md
--rw-r--r--   0        0        0    10623 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/tasks/review.md
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/tasks/schedule.md
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/tasks/selection.md
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/usage/gsheet.md
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/usage/installation.md
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/usage/mail.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pytanis-0.4.1/docs/usage/pretalx.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/.gitignore
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/template.ipynb
--rw-r--r--   0        0        0    14471 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/10_reviewer-assignment_v1.ipynb
--rw-r--r--   0        0        0    15592 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/20_mail_to_reviewers_v1.ipynb
--rw-r--r--   0        0        0    14782 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/30_selection_v1.ipynb
--rw-r--r--   0        0        0   175339 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image_v1.ipynb
--rw-r--r--   0        0        0   163229 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/50_scheduling_v1.ipynb
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image/README.md
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image/Roboto-Regular.ttf
--rw-r--r--   0        0        0    45037 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image/template.png
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image/output/README.md
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/_version.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/config.py
--rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/google.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/highs.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/review.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/utils.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/helpdesk/__init__.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/helpdesk/client.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/helpdesk/mail.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/helpdesk/types.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/pretalx/__init__.py
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/pretalx/client.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/pretalx/types.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 pytanis-0.4.1/src/pytanis/pretalx/utils.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pytanis-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytanis-0.4.1/tests/test_config.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pytanis-0.4.1/tests/cfgs/client_secret.json
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pytanis-0.4.1/tests/cfgs/config.toml
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pytanis-0.4.1/tests/helpdesk/test_mail.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pytanis-0.4.1/tests/pretalx/test_client.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pytanis-0.4.1/.gitignore
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pytanis-0.4.1/AUTHORS.md
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pytanis-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 pytanis-0.4.1/README.md
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 pytanis-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    11787 2020-02-02 00:00:00.000000 pytanis-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pytanis-0.5/.flake8
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pytanis-0.5/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytanis-0.5/.linkcheckerrc
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pytanis-0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 pytanis-0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 pytanis-0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 pytanis-0.5/mkdocs.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pytanis-0.5/docs/authors.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytanis-0.5/docs/changelog.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pytanis-0.5/docs/contributing.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 pytanis-0.5/docs/index.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pytanis-0.5/docs/license.md
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/favicon.svg
+-rw-r--r--   0        0        0   363926 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/gsheet_proposal_selection.png
+-rw-r--r--   0        0        0   259341 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/gsheet_schedule.png
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/icon.svg
+-rw-r--r--   0        0        0    35049 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0    54963 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/logo_banner.png
+-rw-r--r--   0        0        0    34834 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/logo_banner.svg
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/pillars_black.svg
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pytanis-0.5/docs/assets/images/pillars_white.svg
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pytanis-0.5/docs/scripts/gen_ref_nav.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pytanis-0.5/docs/scripts/set_release_version.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 pytanis-0.5/docs/snippets/links.txt
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pytanis-0.5/docs/tasks/cfp.md
+-rw-r--r--   0        0        0    10623 2020-02-02 00:00:00.000000 pytanis-0.5/docs/tasks/review.md
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pytanis-0.5/docs/tasks/schedule.md
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 pytanis-0.5/docs/tasks/selection.md
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 pytanis-0.5/docs/usage/gsheet.md
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pytanis-0.5/docs/usage/installation.md
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 pytanis-0.5/docs/usage/mail.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pytanis-0.5/docs/usage/pretalx.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/.gitignore
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/template.ipynb
+-rw-r--r--   0        0        0    14471 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/10_reviewer-assignment_v1.ipynb
+-rw-r--r--   0        0        0    15592 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/20_mail_to_reviewers_v1.ipynb
+-rw-r--r--   0        0        0    14782 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/30_selection_v1.ipynb
+-rw-r--r--   0        0        0   175339 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image_v1.ipynb
+-rw-r--r--   0        0        0   163229 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/50_scheduling_v1.ipynb
+-rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/60_agenda_export_v1.ipynb
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image/README.md
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    45037 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image/template.png
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image/output/README.md
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/_version.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/config.py
+-rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/google.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/highs.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/review.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/utils.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/helpdesk/__init__.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/helpdesk/client.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/helpdesk/mail.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/helpdesk/types.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/pretalx/__init__.py
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/pretalx/client.py
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/pretalx/types.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 pytanis-0.5/src/pytanis/pretalx/utils.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pytanis-0.5/tests/conftest.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytanis-0.5/tests/test_config.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pytanis-0.5/tests/cfgs/client_secret.json
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pytanis-0.5/tests/cfgs/config.toml
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pytanis-0.5/tests/helpdesk/test_mail.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pytanis-0.5/tests/pretalx/test_client.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pytanis-0.5/.gitignore
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pytanis-0.5/AUTHORS.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pytanis-0.5/LICENSE.txt
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 pytanis-0.5/README.md
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 pytanis-0.5/pyproject.toml
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 pytanis-0.5/PKG-INFO
```

### Comparing `pytanis-0.4.1/.pre-commit-config.yaml` & `pytanis-0.5/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=auto']  # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
 
 # If you want to avoid flake8 errors due to unused vars or imports:
 - repo: https://github.com/PyCQA/autoflake
-  rev: v2.0.1
+  rev: v2.0.2
   hooks:
   - id: autoflake
     args: [
       --in-place,
       --remove-all-unused-imports,
       --remove-unused-variables,
     ]
```

### Comparing `pytanis-0.4.1/CHANGELOG.md` & `pytanis-0.5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## Version 0.5 (2023-04-10)
+
+- Change the start/end time of a slot to a datetime
+
 ## Version 0.4.1 (2023-03-25)
 
 - Additional documentation about the CfP and some minor fixes
 
 ## Version 0.4 (2023-03-10)
 
 - More functionality regarding the proposal selection process like `mark_rows`
```

### Comparing `pytanis-0.4.1/CONTRIBUTING.md` & `pytanis-0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/mkdocs.yml` & `pytanis-0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/index.md` & `pytanis-0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/favicon.svg` & `pytanis-0.5/docs/assets/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/gsheet_proposal_selection.png` & `pytanis-0.5/docs/assets/images/gsheet_proposal_selection.png`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/gsheet_schedule.png` & `pytanis-0.5/docs/assets/images/gsheet_schedule.png`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/icon.svg` & `pytanis-0.5/docs/assets/images/icon.svg`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/logo.svg` & `pytanis-0.5/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/logo_banner.png` & `pytanis-0.5/docs/assets/images/logo_banner.png`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/logo_banner.svg` & `pytanis-0.5/docs/assets/images/logo_banner.svg`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/pillars_black.svg` & `pytanis-0.5/docs/assets/images/pillars_black.svg`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/assets/images/pillars_white.svg` & `pytanis-0.5/docs/assets/images/pillars_white.svg`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/scripts/gen_ref_nav.py` & `pytanis-0.5/docs/scripts/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/scripts/set_release_version.py` & `pytanis-0.5/docs/scripts/set_release_version.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/snippets/links.txt` & `pytanis-0.5/docs/snippets/links.txt`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/tasks/cfp.md` & `pytanis-0.5/docs/tasks/cfp.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/tasks/review.md` & `pytanis-0.5/docs/tasks/review.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/tasks/schedule.md` & `pytanis-0.5/docs/tasks/schedule.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/tasks/selection.md` & `pytanis-0.5/docs/tasks/selection.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/usage/gsheet.md` & `pytanis-0.5/docs/usage/gsheet.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/usage/installation.md` & `pytanis-0.5/docs/usage/installation.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/usage/mail.md` & `pytanis-0.5/docs/usage/mail.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/docs/usage/pretalx.md` & `pytanis-0.5/docs/usage/pretalx.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/notebooks/template.ipynb` & `pytanis-0.5/notebooks/template.ipynb`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/10_reviewer-assignment_v1.ipynb` & `pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/10_reviewer-assignment_v1.ipynb`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/20_mail_to_reviewers_v1.ipynb` & `pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/20_mail_to_reviewers_v1.ipynb`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/30_selection_v1.ipynb` & `pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/30_selection_v1.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.10.9'}}"}*

```diff
@@ -525,15 +525,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.9"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image_v1.ipynb` & `pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image_v1.ipynb`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/50_scheduling_v1.ipynb` & `pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/50_scheduling_v1.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.10.9'}}"}*

```diff
@@ -1529,15 +1529,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.9"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image/Roboto-Regular.ttf` & `pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/notebooks/pyconde-pydata-berlin-2023/40_talk_image/template.png` & `pytanis-0.5/notebooks/pyconde-pydata-berlin-2023/40_talk_image/template.png`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/__init__.py` & `pytanis-0.5/src/pytanis/__init__.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/config.py` & `pytanis-0.5/src/pytanis/config.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/google.py` & `pytanis-0.5/src/pytanis/google.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/highs.py` & `pytanis-0.5/src/pytanis/highs.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/review.py` & `pytanis-0.5/src/pytanis/review.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/utils.py` & `pytanis-0.5/src/pytanis/utils.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/helpdesk/client.py` & `pytanis-0.5/src/pytanis/helpdesk/client.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/helpdesk/mail.py` & `pytanis-0.5/src/pytanis/helpdesk/mail.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/helpdesk/types.py` & `pytanis-0.5/src/pytanis/helpdesk/types.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/pretalx/client.py` & `pytanis-0.5/src/pytanis/pretalx/client.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/src/pytanis/pretalx/types.py` & `pytanis-0.5/src/pytanis/pretalx/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,16 @@
 class Speaker(SubmissionSpeaker):
     submissions: List[str]  # submission codes
     availabilities: Optional[List[SpeakerAvailability]]  # maybe needs organizer permissions?
     answers: Optional[List[Answer]]  # maybe needs organizer permissions?
 
 
 class Slot(BaseModel):
-    # ToDo: Check the datatypes here again, not mentioned in the API
-    start: str
-    end: str
+    start: datetime
+    end: datetime
     room: MultiLingualStr
     room_id: int
 
 
 class Resource(BaseModel):
     resource: str
     description: str
```

### Comparing `pytanis-0.4.1/src/pytanis/pretalx/utils.py` & `pytanis-0.5/src/pytanis/pretalx/utils.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/tests/conftest.py` & `pytanis-0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/tests/helpdesk/test_mail.py` & `pytanis-0.5/tests/helpdesk/test_mail.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/tests/pretalx/test_client.py` & `pytanis-0.5/tests/pretalx/test_client.py`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/.gitignore` & `pytanis-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/LICENSE.txt` & `pytanis-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/README.md` & `pytanis-0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/pyproject.toml` & `pytanis-0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytanis-0.4.1/PKG-INFO` & `pytanis-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytanis
-Version: 0.4.1
+Version: 0.5
 Summary: Utilities for the program organization of conferences using Pretalx
 Project-URL: Documentation, https://florianwilhelm.info/pytanis/
 Project-URL: Sponsor, https://github.com/sponsors/FlorianWilhelm
 Project-URL: Tracker, https://github.com/FlorianWilhelm/pytanis/issues
 Project-URL: Source, https://github.com/FlorianWilhelm/pytanis
 Author-email: Florian Wilhelm <Florian.Wilhelm@gmail.com>
 License-Expression: MIT
```

