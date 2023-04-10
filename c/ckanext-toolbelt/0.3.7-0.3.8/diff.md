# Comparing `tmp/ckanext-toolbelt-0.3.7.tar.gz` & `tmp/ckanext-toolbelt-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-toolbelt-0.3.7.tar", last modified: Fri Apr  7 06:22:12 2023, max compression
+gzip compressed data, was "ckanext-toolbelt-0.3.8.tar", last modified: Mon Apr 10 08:49:36 2023, max compression
```

## Comparing `ckanext-toolbelt-0.3.7.tar` & `ckanext-toolbelt-0.3.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.116515 ckanext-toolbelt-0.3.7/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      215 2023-04-07 06:21:56.000000 ckanext-toolbelt-0.3.7/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6287 2023-04-07 06:22:12.126515 ckanext-toolbelt-0.3.7/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5640 2023-04-02 17:12:40.000000 ckanext-toolbelt-0.3.7/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.086515 ckanext-toolbelt-0.3.7/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.086515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.086515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      233 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1406 2023-04-02 14:43:43.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/_shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.086515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/ckan/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      143 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/ckan/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1291 2023-03-11 04:59:51.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/ckan/db.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1383 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/ckan/search_index.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/dev.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      368 2023-04-03 09:57:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2097 2023-04-05 17:25:28.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1380 2023-04-02 14:43:43.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_gh_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1826 2023-04-02 17:06:54.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_readme.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2393 2023-04-03 08:34:54.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_template.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      652 2023-04-01 15:00:10.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      463 2023-04-02 12:00:10.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/action_release-please.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1968 2023-04-01 12:17:07.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/action_test.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      832 2023-04-05 17:27:19.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/config_gulp-sass.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1671 2023-04-05 17:19:20.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       91 2023-04-03 08:36:25.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/config_pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-04-02 12:33:30.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/template_black.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      207 2023-04-03 08:52:49.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/template_commitizen.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2023-04-03 15:36:15.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/template_isort.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2325 2023-04-02 12:34:17.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/template_pyright.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2023-04-02 12:33:54.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/template_pytest.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       36 2023-04-02 12:33:40.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/template_ruff.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      115 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/decorators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/magic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2652 2023-04-02 13:26:50.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/magic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1091 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/cascade_organization_updates.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_scroll/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-03-06 13:24:19.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      328 2023-03-11 04:59:51.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_scroll/templates/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      150 2023-03-06 13:25:14.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_sqlalchemy/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1397 2023-04-03 09:47:05.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11435 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/group_changes.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4153 2023-04-02 13:28:30.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/group_composite.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1835 2023-04-03 09:46:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/safe_upload.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.076515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.076515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/group/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3034 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      562 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.076515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      721 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.096515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1112 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1231 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      103 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      234 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.106515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      185 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.106515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/plugins/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2689 2023-04-02 13:28:30.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      163 2023-03-11 04:59:51.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/test_decorators.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      141 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/test_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.106515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/types/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      326 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/types/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.116515 ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      629 2023-04-03 09:43:17.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2948 2023-04-03 09:46:37.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/cache.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1041 2023-04-03 10:13:16.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/collector.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3164 2023-04-03 09:34:41.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5048 2023-03-11 08:19:19.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/hierarchy.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      651 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/structures.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-07 06:22:12.116515 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6287 2023-04-07 06:22:12.000000 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3007 2023-04-07 06:22:12.000000 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-07 06:22:12.000000 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      919 2023-04-07 06:22:12.000000 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-07 06:22:12.000000 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       33 2023-04-07 06:22:12.000000 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-07 06:22:12.000000 ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3120 2023-04-03 15:38:38.000000 ckanext-toolbelt-0.3.7/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.3.7/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2526 2023-04-07 06:22:12.126515 ckanext-toolbelt-0.3.7/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      260 2023-04-03 08:37:38.000000 ckanext-toolbelt-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/search_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_gh_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_gulp-sass.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_black.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_commitizen.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_isort.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_pyright.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_pytest.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/magic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/cascade_organization_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/safe_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/setup.py
```

### Comparing `ckanext-toolbelt-0.3.7/LICENSE` & `ckanext-toolbelt-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/PKG-INFO` & `ckanext-toolbelt-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.3.7
+Version: 0.3.8
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.3.7/README.md` & `ckanext-toolbelt-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/_shared.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/_shared.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/ckan/db.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/db.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/ckan/search_index.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/search_index.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/dev.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_config.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_gh_action.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_gh_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_readme.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_readme.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/make_template.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_template.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/action_test.yaml` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_test.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/config_gulp-sass.js` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_gulp-sass.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
 const destDir = resolve(assetsDir, "css");
 
 const build = () =>
     src(resolve(srcDir, "$PLUGIN.scss"))
     .pipe(if_(isDev, sourcemaps.init()))
     .pipe(sass({
         outputStyle: "compressed"
-    }))
+    }).on('error', sass.logError))
     .pipe(if_(isDev, sourcemaps.write()))
     .pipe(dest(destDir))
     .pipe(touch());
 
 const watchStyles = () =>
     watch(resolve(srcDir, "*.scss"), {
         ignoreInitial: false
```

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/config_pre-commit.yaml` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/cli/templates/template_pyright.toml` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_pyright.toml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/magic/__init__.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/magic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,14 @@
 import ckan.plugins.toolkit as tk
 
 log = logging.getLogger(__name__)
 
 
 def conjure_fast_group_activities():
     log.info("ieiunium sicut ventus")
-    if tk.check_ckan_version("2.10"):
-        log.error("This spell works only for CKAN v2.9")
-        return
 
     def ___group_activity_perfomance_patch(group_id, include_hidden_activity=False):
         import ckan.model as model
 
         group = model.Group.get(group_id)
         if not group:
             # Return a query with no results.
@@ -49,15 +46,18 @@
         )
 
         if not include_hidden_activity:
             group_activity = _filter_activitites_from_users(group_activity)  # noqa
             member_activity = _filter_activitites_from_users(member_activity)  # noqa
         return _activities_union_all(group_activity, member_activity)  # noqa
 
-    from ckan.model.activity import _group_activity_query
+    if tk.check_ckan_version("2.10"):
+        from ckanext.activity.model.activity import _group_activity_query
+    else:
+        from ckan.model.activity import _group_activity_query
 
     _group_activity_query.__code__ = ___group_activity_perfomance_patch.__code__
 
 
 def transfigure_xloaded_file(func):
     """Proces a file before uploading it to datastore.
```

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/cascade_organization_updates.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/group_changes.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_changes.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/group_composite.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_composite.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/safe_upload.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/safe_upload.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/__init__.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/cache.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/collector.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/collector.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/fs.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/hierarchy.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext/toolbelt/utils/structures.py` & `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/PKG-INFO` & `ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.3.7
+Version: 0.3.8
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/SOURCES.txt` & `ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/ckanext_toolbelt.egg-info/entry_points.txt` & `ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/pyproject.toml` & `ckanext-toolbelt-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.7/setup.cfg` & `ckanext-toolbelt-0.3.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-toolbelt
-version = 0.3.7
+version = 0.3.8
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-toolbelt
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

