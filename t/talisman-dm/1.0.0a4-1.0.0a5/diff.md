# Comparing `tmp/talisman-dm-1.0.0a4.tar.gz` & `tmp/talisman-dm-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/talisman-dm-1.0.0a4.tar", last modified: Mon Mar 27 11:08:58 2023, max compression
+gzip compressed data, was "dist/talisman-dm-1.0.0a5.tar", last modified: Mon Apr 10 10:58:44 2023, max compression
```

## Comparing `talisman-dm-1.0.0a4.tar` & `talisman-dm-1.0.0a5.tar`

### file list

```diff
@@ -1,135 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/
--rw-r--r--   0 root         (0) root         (0)      778 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/README.md
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/talisman_dm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/talisman_dm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3897 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/talisman_dm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/talisman_dm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/talisman_dm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/talisman_dm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/content.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     2500 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/document.py
--rw-rw-rw-   0 root         (0) root         (0)     7660 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/fact.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/span.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/datamodel/tree.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/abstract/json_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8895 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/datamodel/directive/
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/directive/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/directive/create_account.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/directive/create_concept.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/directive/create_platform.py
--rw-rw-rw-   0 root         (0) root         (0)    12077 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/datamodel/fact/
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/fact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/fact/concept.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/fact/property.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/fact/relation.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/fact/value.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/span.py
--rw-rw-rw-   0 root         (0) root         (0)     3881 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/datamodel/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/base.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/fact.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/link.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4583 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     2909 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/identifiable.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/mention.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/directives/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/directives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/directives/account.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/directives/concept.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/directives/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6472 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/_container.py
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    10091 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     7193 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/_structure.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4793 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/document/_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/facts/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/facts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/facts/concept.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/facts/links.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/facts/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/facts/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/links/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/links/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/mentions/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/mentions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/mentions/image.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/mentions/node.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/mentions/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/base64.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/structure.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/text.py
--rw-rw-rw-   0 root         (0) root         (0)     1606 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/directives.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/document.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/facts.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/links.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/mentions.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/future/json_schema/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/json_schema/content/
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/content/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/content/markup.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/content/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/content/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/json_schema/directive/
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/directive/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/directive/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/directive/create_account.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/directive/create_concept.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/directive/create_platform.py
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/directive/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3502 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 11:08:58.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/common.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/concept.py
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/property.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/relation.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2023-03-27 11:08:50.000000 talisman-dm-1.0.0a4/tdm/json_schema/fact/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/link.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4576 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/identifiable.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6465 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1825 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    10015 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7193 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/links.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/links/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/links/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/directives.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/facts.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/links.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/mentions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_facts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3593 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/metadata.py
```

### Comparing `talisman-dm-1.0.0a4/PKG-INFO` & `talisman-dm-1.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a4/setup.py` & `talisman-dm-1.0.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/talisman_dm.egg-info/PKG-INFO` & `talisman-dm-1.0.0a5/talisman_dm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a4/talisman_dm.egg-info/SOURCES.txt` & `talisman-dm-1.0.0a5/talisman_dm.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,106 +3,75 @@
 setup.py
 talisman_dm.egg-info/PKG-INFO
 talisman_dm.egg-info/SOURCES.txt
 talisman_dm.egg-info/dependency_links.txt
 talisman_dm.egg-info/requires.txt
 talisman_dm.egg-info/top_level.txt
 tdm/__init__.py
+tdm/helper.py
+tdm/legacy.py
+tdm/model.py
 tdm/abstract/__init__.py
-tdm/abstract/json_schema.py
 tdm/abstract/datamodel/__init__.py
-tdm/abstract/datamodel/content.py
+tdm/abstract/datamodel/base.py
 tdm/abstract/datamodel/directive.py
 tdm/abstract/datamodel/document.py
 tdm/abstract/datamodel/fact.py
-tdm/abstract/datamodel/span.py
-tdm/abstract/datamodel/tree.py
+tdm/abstract/datamodel/link.py
+tdm/abstract/datamodel/mention.py
+tdm/abstract/datamodel/node.py
+tdm/abstract/json_schema/__init__.py
+tdm/abstract/json_schema/composite.py
+tdm/abstract/json_schema/decorator.py
+tdm/abstract/json_schema/model.py
+tdm/abstract/json_schema/serializers/__init__.py
+tdm/abstract/json_schema/serializers/abstract.py
+tdm/abstract/json_schema/serializers/identifiable.py
+tdm/abstract/json_schema/serializers/mention.py
+tdm/abstract/json_schema/serializers/metadata.py
+tdm/abstract/json_schema/serializers/serializers.py
 tdm/datamodel/__init__.py
-tdm/datamodel/content.py
-tdm/datamodel/document.py
-tdm/datamodel/span.py
-tdm/datamodel/tree.py
-tdm/datamodel/directive/__init__.py
-tdm/datamodel/directive/create_account.py
-tdm/datamodel/directive/create_concept.py
-tdm/datamodel/directive/create_platform.py
-tdm/datamodel/fact/__init__.py
-tdm/datamodel/fact/concept.py
-tdm/datamodel/fact/property.py
-tdm/datamodel/fact/relation.py
-tdm/datamodel/fact/value.py
-tdm/future/__init__.py
-tdm/future/helper.py
-tdm/future/abstract/__init__.py
-tdm/future/abstract/datamodel/__init__.py
-tdm/future/abstract/datamodel/base.py
-tdm/future/abstract/datamodel/directive.py
-tdm/future/abstract/datamodel/document.py
-tdm/future/abstract/datamodel/fact.py
-tdm/future/abstract/datamodel/link.py
-tdm/future/abstract/datamodel/mention.py
-tdm/future/abstract/datamodel/node.py
-tdm/future/abstract/json_schema/__init__.py
-tdm/future/abstract/json_schema/composite.py
-tdm/future/abstract/json_schema/decorator.py
-tdm/future/abstract/json_schema/model.py
-tdm/future/abstract/json_schema/serializers/__init__.py
-tdm/future/abstract/json_schema/serializers/abstract.py
-tdm/future/abstract/json_schema/serializers/identifiable.py
-tdm/future/abstract/json_schema/serializers/mention.py
-tdm/future/abstract/json_schema/serializers/metadata.py
-tdm/future/abstract/json_schema/serializers/serializers.py
-tdm/future/datamodel/__init__.py
-tdm/future/datamodel/directives/__init__.py
-tdm/future/datamodel/directives/account.py
-tdm/future/datamodel/directives/concept.py
-tdm/future/datamodel/directives/platform.py
-tdm/future/datamodel/document/__init__.py
-tdm/future/datamodel/document/_base.py
-tdm/future/datamodel/document/_container.py
-tdm/future/datamodel/document/_factory.py
-tdm/future/datamodel/document/_impl.py
-tdm/future/datamodel/document/_structure.py
-tdm/future/datamodel/document/_types.py
-tdm/future/datamodel/document/_view.py
-tdm/future/datamodel/facts/__init__.py
-tdm/future/datamodel/facts/concept.py
-tdm/future/datamodel/facts/links.py
-tdm/future/datamodel/facts/mention.py
-tdm/future/datamodel/facts/value.py
-tdm/future/datamodel/links/__init__.py
-tdm/future/datamodel/links/reference.py
-tdm/future/datamodel/mentions/__init__.py
-tdm/future/datamodel/mentions/image.py
-tdm/future/datamodel/mentions/node.py
-tdm/future/datamodel/mentions/text.py
-tdm/future/datamodel/nodes/__init__.py
-tdm/future/datamodel/nodes/base64.py
-tdm/future/datamodel/nodes/file.py
-tdm/future/datamodel/nodes/structure.py
-tdm/future/datamodel/nodes/text.py
-tdm/future/json_schema/__init__.py
-tdm/future/json_schema/directives.py
-tdm/future/json_schema/document.py
-tdm/future/json_schema/facts.py
-tdm/future/json_schema/links.py
-tdm/future/json_schema/mentions.py
-tdm/future/json_schema/nodes.py
+tdm/datamodel/directives/__init__.py
+tdm/datamodel/directives/account.py
+tdm/datamodel/directives/concept.py
+tdm/datamodel/directives/platform.py
+tdm/datamodel/document/__init__.py
+tdm/datamodel/document/_base.py
+tdm/datamodel/document/_container.py
+tdm/datamodel/document/_factory.py
+tdm/datamodel/document/_impl.py
+tdm/datamodel/document/_structure.py
+tdm/datamodel/document/_types.py
+tdm/datamodel/document/_view.py
+tdm/datamodel/facts/__init__.py
+tdm/datamodel/facts/concept.py
+tdm/datamodel/facts/links.py
+tdm/datamodel/facts/mention.py
+tdm/datamodel/facts/value.py
+tdm/datamodel/links/__init__.py
+tdm/datamodel/links/reference.py
+tdm/datamodel/mentions/__init__.py
+tdm/datamodel/mentions/image.py
+tdm/datamodel/mentions/node.py
+tdm/datamodel/mentions/text.py
+tdm/datamodel/nodes/__init__.py
+tdm/datamodel/nodes/base64.py
+tdm/datamodel/nodes/file.py
+tdm/datamodel/nodes/structure.py
+tdm/datamodel/nodes/text.py
 tdm/json_schema/__init__.py
-tdm/json_schema/document.py
-tdm/json_schema/content/__init__.py
-tdm/json_schema/content/markup.py
-tdm/json_schema/content/metadata.py
-tdm/json_schema/content/node.py
-tdm/json_schema/directive/__init__.py
-tdm/json_schema/directive/abstract.py
-tdm/json_schema/directive/create_account.py
-tdm/json_schema/directive/create_concept.py
-tdm/json_schema/directive/create_platform.py
-tdm/json_schema/directive/factory.py
-tdm/json_schema/fact/__init__.py
-tdm/json_schema/fact/common.py
-tdm/json_schema/fact/concept.py
-tdm/json_schema/fact/factory.py
-tdm/json_schema/fact/property.py
-tdm/json_schema/fact/relation.py
-tdm/json_schema/fact/value.py
+tdm/json_schema/directives.py
+tdm/json_schema/facts.py
+tdm/json_schema/links.py
+tdm/json_schema/mentions.py
+tdm/json_schema/nodes.py
+tdm/v0/__init__.py
+tdm/v0/json_schema/__init__.py
+tdm/v0/json_schema/content.py
+tdm/v0/json_schema/directive.py
+tdm/v0/json_schema/document.py
+tdm/v0/json_schema/fact.py
+tdm/v0/json_schema/metadata.py
+tdm/v0/json_schema/convert/__init__.py
+tdm/v0/json_schema/convert/_facts.py
+tdm/v0/json_schema/convert/_metadata.py
+tdm/v0/json_schema/convert/_nodes.py
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/__init__.py` & `talisman-dm-1.0.0a5/tdm/abstract/datamodel/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/base.py` & `talisman-dm-1.0.0a5/tdm/abstract/datamodel/base.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/document.py` & `talisman-dm-1.0.0a5/tdm/abstract/datamodel/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     @abstractmethod
     def without_facts(self: _TD, facts: Iterable[Union[str, AbstractFact]], *, cascade: bool = False) -> _TD:
         pass
 
     @property
     @abstractmethod
-    def directives(self) -> Dict[Type[AbstractDirective], AbstractDirective]:
+    def directives(self) -> Dict[Type[AbstractDirective], Iterable[AbstractDirective]]:
         pass
 
     @abstractmethod
     def with_directives(self: _TD, directives: Iterable[AbstractDirective], *, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/fact.py` & `talisman-dm-1.0.0a5/tdm/abstract/datamodel/fact.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/datamodel/node.py` & `talisman-dm-1.0.0a5/tdm/abstract/datamodel/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass, field
 from typing import Generic, Set, TypeVar
 
 from frozendict import frozendict
 
-from tdm.future.helper import generics_mapping
+from tdm.helper import generics_mapping
 from .base import Identifiable
 
 
 @dataclass(frozen=True)
 class BaseNodeMetadata:
     hidden: bool = False
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/composite.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/composite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod
 from collections import defaultdict
 from typing import Callable, Dict, Generic, Iterable, List, Tuple, Type, TypeVar, Union
 
 from pydantic import BaseModel, Field, create_model
 from typing_extensions import Annotated, Self
 
-from tdm.future.abstract.datamodel import AbstractNode
+from tdm.abstract.datamodel import AbstractNode
 from .model import ElementModel, create_model_for_type
 
 _ElementType = TypeVar('_ElementType')
 _DATA = TypeVar('_DATA')
 
 
 class AbstractLabeledModel(Generic[_ElementType]):
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/decorator.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, TypeVar
 
-from tdm.future.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, AbstractNodeMention
+from tdm.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, AbstractNodeMention
 from .composite import ModelsGenerator
 
 _MODELS_GENERATORS = {
     AbstractDirective: ModelsGenerator(AbstractDirective),
     AbstractFact: ModelsGenerator(AbstractFact),
     AbstractNodeLink: ModelsGenerator(AbstractNodeLink),
     AbstractNodeMention: ModelsGenerator(AbstractNodeMention, include_label=True),
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/model.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 from dataclasses import fields
 from typing import Any, Dict, Generic, Optional, Type, TypeVar
 
 from pydantic import BaseModel, Extra, create_model, root_validator
 from typing_extensions import Literal, Self
 
-from tdm.future.helper import cache_result, generics_mapping, is_subclass
+from tdm.helper import cache_result, generics_mapping, is_subclass
 from .serializers import AbstractElementModel, AbstractElementSerializer, BaseSerializers
 
 _Element = TypeVar('_Element')
 
 
 # hackish root validator solution as normal validators are not called for skipped required fields
 def set_type_if_none(cls, values):
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/__init__.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/abstract.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/identifiable.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/identifiable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Type, TypeVar
 
-from tdm.future.abstract.datamodel import EnsureIdentifiable
+from tdm.abstract.datamodel import EnsureIdentifiable
 from .abstract import AbstractElementSerializer
 
 _Identifiable = TypeVar('_Identifiable', bound=EnsureIdentifiable)
 
 
 class IdSerializer(AbstractElementSerializer[_Identifiable, str]):
     def __init__(self, type_: Type[_Identifiable]):
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/mention.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/mention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Type
 
-from tdm.future.abstract.datamodel import AbstractNodeMention
+from tdm.abstract.datamodel import AbstractNodeMention
 from .abstract import AbstractElementModel, AbstractModelSerializer
 
 
 class NodeMentionSerializer(AbstractModelSerializer[AbstractNodeMention]):
     def serialize(self, element: AbstractNodeMention) -> AbstractElementModel[AbstractNodeMention]:
-        from tdm.future.json_schema.mentions import serialize_mention
+        from tdm.json_schema.mentions import serialize_mention
         return serialize_mention(element)
 
     def field_type(self, element_type: Type[AbstractNodeMention]) -> Type[AbstractElementModel[AbstractNodeMention]]:
-        from tdm.future.json_schema.mentions import MENTION_MODELS
+        from tdm.json_schema.mentions import MENTION_MODELS
         return MENTION_MODELS[element_type]
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/metadata.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 
-from tdm.future.abstract.datamodel import BaseNodeMetadata
+from tdm.abstract.datamodel import BaseNodeMetadata
 from .abstract import AbstractElementModel, AbstractModelSerializer
 
 
 class NodeMetadataSerializer(AbstractModelSerializer[BaseNodeMetadata]):
     def serialize(self, element: BaseNodeMetadata) -> AbstractElementModel[BaseNodeMetadata]:
         return self.field_type(type(element)).serialize(element)
 
     def field_type(self, element_type: Type[BaseNodeMetadata]) -> Type[AbstractElementModel[BaseNodeMetadata]]:
-        from tdm.future.abstract.json_schema.model import create_model_for_type
+        from tdm.abstract.json_schema.model import create_model_for_type
         return create_model_for_type(element_type)  # actually it is cached
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/abstract/json_schema/serializers/serializers.py` & `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tdm.future.abstract.datamodel import AbstractFact, AbstractNode, AbstractNodeMention, BaseNodeMetadata
+from tdm.abstract.datamodel import AbstractFact, AbstractNode, AbstractNodeMention, BaseNodeMetadata
 from .identifiable import IdSerializer
 from .mention import NodeMentionSerializer
 from .metadata import NodeMetadataSerializer
 
 
 def build_serializers():
     result = {
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/directives/concept.py` & `talisman-dm-1.0.0a5/tdm/datamodel/directives/concept.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 from frozendict import frozendict
 
-from tdm.future.abstract.datamodel import AbstractDirective, Identifiable
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractDirective, Identifiable
+from tdm.abstract.json_schema import generate_model
 
 
 @dataclass(frozen=True)
 class _CreateConceptDirective(AbstractDirective):
     name: str
     concept_type: str
     filters: Tuple[dict, ...]
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/document/_base.py` & `talisman-dm-1.0.0a5/tdm/datamodel/document/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 from typing import Dict, Iterable, Set, Tuple, Type, TypeVar, Union
 
-from tdm.future.abstract.datamodel import EnsureIdentifiable
+from tdm.abstract.datamodel import EnsureIdentifiable
 from ._container import TypedIdsContainer
 from ._types import get_base_type
 from ._view import AbstractView, object_view
 
 _TD = TypeVar('_TD', bound='BaseImpl')
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/document/_container.py` & `talisman-dm-1.0.0a5/tdm/datamodel/document/_container.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/document/_factory.py` & `talisman-dm-1.0.0a5/tdm/datamodel/document/_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import uuid
-from typing import Dict, Iterable, Optional, Tuple
+from typing import Any, Dict, Iterable, Optional, Tuple
 
-from tdm.abstract.datamodel.document import DocumentMetadata
-from tdm.future.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink
-from tdm.future.abstract.datamodel.document import AbstractDocumentFactory, TalismanDocument
+from tdm.abstract.datamodel import AbstractDirective, AbstractDocumentFactory, AbstractFact, AbstractNode, AbstractNodeLink, \
+    TalismanDocument
 from ._container import TypedIdsContainer
 from ._impl import TalismanDocumentImpl
 from ._structure import NodesStructure
 
 
 class TalismanDocumentFactory(AbstractDocumentFactory):
 
@@ -29,15 +28,15 @@
             self,
             content: Iterable[AbstractNode] = (),
             structure: Dict[str, Tuple[str, ...]] = None,
             root: Optional[str] = None,
             node_links: Iterable[AbstractNodeLink] = (),
             facts: Iterable[AbstractFact] = (),
             directives: Iterable[AbstractDirective] = (),
-            metadata: Optional[DocumentMetadata] = None,
+            metadata: Optional[Dict[str, Any]] = None,
             *, id_: Optional[str] = None
     ) -> TalismanDocument:
         doc: TalismanDocumentImpl = self.create_document(id_=id_)
         doc = doc.with_elements((*content, *node_links, *facts, *directives)) \
             .with_links(structure) \
             .with_main_root(root) \
             .with_metadata(metadata)
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/document/_impl.py` & `talisman-dm-1.0.0a5/tdm/datamodel/document/_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from copy import deepcopy
 from functools import wraps
 from typing import Any, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union
 
-from tdm.abstract.datamodel.document import DocumentMetadata
-from tdm.future.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, EnsureIdentifiable, \
-    TalismanDocument
+from tdm.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, EnsureIdentifiable, TalismanDocument
 from ._base import BaseImpl
 from ._container import TypedIdsContainer
 from ._structure import NodesStructure
 from ._view import AbstractView, restore_object
 
 _TD = TypeVar('_TD', bound='TalismanDocumentImpl')
 _D = TypeVar('_D', bound=EnsureIdentifiable)
@@ -32,15 +30,15 @@
 
     def __init__(
             self,
             id2view: Dict[str, Union[EnsureIdentifiable, AbstractView]],
             dependencies: Dict[str, Set[Tuple[str, Type[EnsureIdentifiable]]]],
             containers: Dict[Type[EnsureIdentifiable], TypedIdsContainer],
             structure: NodesStructure,
-            metadata: Optional[DocumentMetadata],  # should be removed in future
+            metadata: Optional[Dict[str, Any]],  # should be removed in future
             *, id_: str):
         super().__init__(id2view, dependencies, containers)
         self._id = id_
         self._structure = structure
 
         self._metadata = deepcopy(metadata)  # should be removed in future
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/document/_structure.py` & `talisman-dm-1.0.0a5/tdm/datamodel/document/_structure.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/document/_types.py` & `talisman-dm-1.0.0a5/tdm/datamodel/document/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Type, Union
 
-from tdm.future.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, EnsureIdentifiable
+from tdm.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, EnsureIdentifiable
 
 _BASE_TYPES = {AbstractNode, AbstractNodeLink, AbstractFact, AbstractDirective}
 
 _CACHE: Dict[Type[EnsureIdentifiable], Type[EnsureIdentifiable]] = {}
 
 
 def get_base_type(element: Union[EnsureIdentifiable, Type[EnsureIdentifiable]]) -> Type[EnsureIdentifiable]:
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/document/_view.py` & `talisman-dm-1.0.0a5/tdm/datamodel/document/_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod
 from dataclasses import dataclass, fields, is_dataclass, make_dataclass
 from typing import Callable, Dict, Generic, Set, Tuple, Type, TypeVar, Union
 
-from tdm.future.abstract.datamodel import EnsureIdentifiable
-from tdm.future.helper import generics_mapping, is_subclass
+from tdm.abstract.datamodel import EnsureIdentifiable
+from tdm.helper import generics_mapping, is_subclass
 
 _T = TypeVar('_T', bound=EnsureIdentifiable)
 
 
 @dataclass(frozen=True)
 class AbstractView(Generic[_T]):
     __depends_on__: Set[str]
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/facts/concept.py` & `talisman-dm-1.0.0a5/tdm/datamodel/facts/concept.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Sequence, Set, Tuple, Union
 
-from tdm.future.abstract.datamodel import AbstractFact, Identifiable
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractFact, Identifiable
+from tdm.abstract.json_schema import generate_model
 
 
 @dataclass(frozen=True)
 class _ConceptFact(AbstractFact):  # not an error as id argument is kw only
     type_id: str
     value: Union[str, Tuple[str, ...]] = tuple()
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/facts/links.py` & `talisman-dm-1.0.0a5/tdm/datamodel/facts/links.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Union
 
-from tdm.future.abstract.datamodel import AbstractLinkFact, Identifiable
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractLinkFact, Identifiable
+from tdm.abstract.json_schema import generate_model
 from .concept import ConceptFact
 from .value import AtomValueFact, CompositeValueFact
 
 
 @generate_model(label='relation')
 @dataclass(frozen=True)
 class RelationFact(Identifiable, AbstractLinkFact[ConceptFact, ConceptFact]):
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/facts/mention.py` & `talisman-dm-1.0.0a5/tdm/datamodel/facts/mention.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Set
 
-from tdm.future.abstract.datamodel import AbstractFact, AbstractNodeMention, Identifiable
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractFact, AbstractNodeMention, Identifiable
+from tdm.abstract.json_schema import generate_model
 from .value import AtomValueFact
 
 
 @dataclass(frozen=True)
 class _MentionFact(AbstractFact):
     mention: AbstractNodeMention
     value: AtomValueFact
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/facts/value.py` & `talisman-dm-1.0.0a5/tdm/datamodel/facts/value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Sequence, Set, Tuple, Union
 
 from frozendict import frozendict
 
-from tdm.future.abstract.datamodel import AbstractFact, Identifiable
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractFact, Identifiable
+from tdm.abstract.json_schema import generate_model
 
 
 @dataclass(frozen=True)
 class _AtomValueFact(AbstractFact):
     type_id: str
     value: Union[dict, Tuple[dict, ...]] = tuple()
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/links/reference.py` & `talisman-dm-1.0.0a5/tdm/datamodel/links/reference.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 
-from tdm.future.abstract.datamodel import AbstractNodeLink, AbstractNodeMention, Identifiable
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractNodeLink, AbstractNodeMention, Identifiable
+from tdm.abstract.json_schema import generate_model
 
 
 @generate_model(label='same')
 @dataclass(frozen=True)
 class SameNodeLink(Identifiable, AbstractNodeLink[AbstractNodeMention, AbstractNodeMention]):
     pass
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/mentions/image.py` & `talisman-dm-1.0.0a5/tdm/datamodel/mentions/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
-from tdm.future.abstract.datamodel import AbstractNodeMention
-from tdm.future.abstract.json_schema import generate_model
-from tdm.future.datamodel.nodes import ImageNode
+from tdm.abstract.datamodel import AbstractNodeMention
+from tdm.abstract.json_schema import generate_model
+from tdm.datamodel.nodes import ImageNode
 
 
 @generate_model
 @dataclass(frozen=True)
 class ImageNodeMention(AbstractNodeMention):
     node: ImageNode
     top: int
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/__init__.py` & `talisman-dm-1.0.0a5/tdm/datamodel/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/file.py` & `talisman-dm-1.0.0a5/tdm/datamodel/nodes/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from tdm.future.abstract.datamodel import AbstractContentNode, BaseNodeMetadata
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractContentNode, BaseNodeMetadata
+from tdm.abstract.json_schema import generate_model
 
 
 @dataclass(frozen=True)
 class FileNodeMetadata(BaseNodeMetadata):
     name: Optional[str] = None
     size: Optional[int] = None
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/structure.py` & `talisman-dm-1.0.0a5/tdm/datamodel/nodes/structure.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from tdm.future.abstract.datamodel import AbstractNode, BaseNodeMetadata
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractNode, BaseNodeMetadata
+from tdm.abstract.json_schema import generate_model
 
 
 @dataclass(frozen=True)
 class ListNodeMetadata(BaseNodeMetadata):
     bullet: Optional[str] = None
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/datamodel/nodes/text.py` & `talisman-dm-1.0.0a5/tdm/datamodel/nodes/text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from tdm.future.abstract.datamodel import AbstractContentNode, BaseNodeMetadata
-from tdm.future.abstract.json_schema import generate_model
+from tdm.abstract.datamodel import AbstractContentNode, BaseNodeMetadata
+from tdm.abstract.json_schema import generate_model
 
 
 @dataclass(frozen=True)
 class TextNodeMetadata(BaseNodeMetadata):
     language: Optional[str] = None
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/helper.py` & `talisman-dm-1.0.0a5/tdm/helper.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a4/tdm/future/json_schema/directives.py` & `talisman-dm-1.0.0a5/tdm/json_schema/directives.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
-from tdm.future.abstract.datamodel import AbstractDirective
-from tdm.future.abstract.json_schema import AbstractLabeledModel, get_model_generator
+from tdm.abstract.datamodel import AbstractDirective
+from tdm.abstract.json_schema import AbstractLabeledModel, get_model_generator
 
 
 def register_directives_model() -> Type[AbstractLabeledModel[AbstractDirective]]:
-    import tdm.future.datamodel.directives as directives
+    import tdm.datamodel.directives as directives
     directives
 
     # TODO: here plugin for extra document nodes could be added
 
     return get_model_generator(AbstractDirective).generate_labeled_model('DirectivesModel')
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/json_schema/document.py` & `talisman-dm-1.0.0a5/tdm/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, Optional, Tuple
 
 from pydantic import BaseModel, root_validator
 from typing_extensions import Literal
 
-from tdm.future.abstract.datamodel import AbstractNode, TalismanDocument
-from tdm.future.datamodel.document import TalismanDocumentFactory
-from tdm.json_schema import DocumentMetadataModel
-from .directives import DirectivesModel
-from .facts import FactsModel
-from .links import NodeLinksModel
-from .nodes import NodeModel, fill_children, serialize_node
+from .abstract.datamodel import AbstractNode, TalismanDocument
+from .datamodel.document import TalismanDocumentFactory
+from .json_schema.directives import DirectivesModel
+from .json_schema.facts import FactsModel
+from .json_schema.links import NodeLinksModel
+from .json_schema.nodes import NodeModel, fill_children, serialize_node
+from .legacy import DocumentMetadataModel
 
 
 class TalismanDocumentModel(BaseModel):
     VERSION: Literal['1.0'] = ...
     id: str
     main_node: str
     content: Tuple[NodeModel, ...]
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/json_schema/facts.py` & `talisman-dm-1.0.0a5/tdm/json_schema/facts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
-from tdm.future.abstract.datamodel import AbstractFact
-from tdm.future.abstract.json_schema import AbstractLabeledModel, get_model_generator
+from tdm.abstract.datamodel import AbstractFact
+from tdm.abstract.json_schema import AbstractLabeledModel, get_model_generator
 
 
 def register_fact_models() -> Type[AbstractLabeledModel[AbstractFact]]:
-    import tdm.future.datamodel.facts as facts  # we need this import for serializers registration
+    import tdm.datamodel.facts as facts  # we need this import for serializers registration
     facts
 
     # TODO: here plugin for extra document nodes could be added
 
     return get_model_generator(AbstractFact).generate_labeled_model('FactsModel')
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/json_schema/mentions.py` & `talisman-dm-1.0.0a5/tdm/json_schema/mentions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable, Dict, Tuple, Type
 
-from tdm.future.abstract.datamodel import AbstractNodeMention
-from tdm.future.abstract.json_schema import ElementModel, get_model_generator
+from tdm.abstract.datamodel import AbstractNodeMention
+from tdm.abstract.json_schema import ElementModel, get_model_generator
 
 
 def register_mention_models() -> \
         Tuple[Dict[Type[AbstractNodeMention], Type[ElementModel]], Callable[[AbstractNodeMention], ElementModel]]:
-    import tdm.future.datamodel.mentions as mentions  # we need mentions models to be registered
+    import tdm.datamodel.mentions as mentions  # we need mentions models to be registered
     mentions
 
     # TODO: add plugins support here
 
     return get_model_generator(AbstractNodeMention).generate_union_model(discriminator='type')
```

### Comparing `talisman-dm-1.0.0a4/tdm/future/json_schema/nodes.py` & `talisman-dm-1.0.0a5/tdm/json_schema/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Callable, Iterable, Tuple, Type, Union
 
 from pydantic import Field, create_model
 from typing_extensions import Annotated
 
-from tdm.future.abstract.datamodel import AbstractNode, TalismanDocument
-from tdm.future.abstract.json_schema import ElementModel, get_model_generator
-from tdm.future.helper import unfold_union
+from tdm.abstract.datamodel import AbstractNode, TalismanDocument
+from tdm.abstract.json_schema import ElementModel, get_model_generator
+from tdm.helper import unfold_union
 
 
 def register_node_models() -> Tuple[Type[ElementModel[AbstractNode]], Callable[[AbstractNode], ElementModel[AbstractNode]]]:
-    import tdm.future.datamodel.nodes as nodes  # we need this import for serializers registration
+    import tdm.datamodel.nodes as nodes  # we need this import for serializers registration
     nodes
 
     # TODO: here plugin for extra document nodes could be added
 
     models, serialize = get_model_generator(AbstractNode).generate_union_model()
 
     # add children field to all node models. serialize function doesn't generate value for children field
```

### Comparing `talisman-dm-1.0.0a4/tdm/json_schema/directive/create_concept.py` & `talisman-dm-1.0.0a5/tdm/v0/json_schema/directive.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-from typing import Optional, Tuple
+from enum import Enum
+from typing import Optional, Tuple, Union
 
+from pydantic import BaseModel
 from typing_extensions import Literal
 
-from tdm.abstract.datamodel.directive import DirectiveType
-from tdm.datamodel import CreateConceptDirective
-from tdm.json_schema.directive.abstract import AbstractDirectiveModel
+
+class DirectiveType(str, Enum):
+    CREATE_CONCEPT = 'create_concept'
+    CREATE_ACCOUNT = 'create_account'
+    CREATE_PLATFORM = 'create_platform'
+
+
+class AbstractDirectiveModel(BaseModel):
+    directive_type: DirectiveType
 
 
 class CreateConceptDirectiveModel(AbstractDirectiveModel):
     id: str
     name: str
     concept_type: str
     filters: Tuple[dict, ...]
     notes: Optional[str]
     markers: Optional[Tuple[str, ...]]
     access_level: Optional[str]
 
     directive_type: Literal[DirectiveType.CREATE_CONCEPT] = DirectiveType.CREATE_CONCEPT
 
-    @classmethod
-    def build(cls, directive: CreateConceptDirective) -> 'CreateConceptDirectiveModel':
-        return cls.construct(
-            id=directive.id,
-            name=directive.name,
-            concept_type=directive.concept_type,
-            filters=directive.filters,
-            notes=directive.notes,
-            markers=directive.markers,
-            access_level=directive.access_level
-        )
-
-    def to_directive(self) -> CreateConceptDirective:
-        return CreateConceptDirective(
-            name=self.name,
-            concept_type=self.concept_type,
-            filters=self.filters,
-            notes=self.notes,
-            markers=self.markers,
-            access_level=self.access_level,
-            id_=self.id
-        )
-
     def __hash__(self):
         return hash((self.directive_type, self.concept_type, self.id))
+
+
+class CreateAccountDirectiveModel(AbstractDirectiveModel):
+    key: str
+    platform_key: str
+    name: str
+    url: str
+
+    directive_type: Literal[DirectiveType.CREATE_ACCOUNT] = DirectiveType.CREATE_ACCOUNT
+
+    def __hash__(self):
+        return hash((self.directive_type, self.key))
+
+
+class CreatePlatformDirectiveModel(AbstractDirectiveModel):
+    key: str
+    platform_type: str
+    name: str
+    url: str
+
+    directive_type: Literal[DirectiveType.CREATE_PLATFORM] = DirectiveType.CREATE_PLATFORM
+
+    def __hash__(self):
+        return hash((self.directive_type, self.key))
+
+
+DirectiveModel = Union[CreateAccountDirectiveModel, CreateConceptDirectiveModel, CreatePlatformDirectiveModel]
```

