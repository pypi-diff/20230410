# Comparing `tmp/caso-4.0.1.dev1.tar.gz` & `tmp/caso-4.1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caso-4.0.1.dev1.tar", last modified: Thu Mar 30 22:06:06 2023, max compression
+gzip compressed data, was "caso-4.1.0.0rc1.tar", last modified: Mon Apr 10 13:59:34 2023, max compression
```

## Comparing `caso-4.0.1.dev1.tar` & `caso-4.1.0.0rc1.tar`

### file list

```diff
@@ -1,120 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.922064 caso-4.0.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.906064 caso-4.0.1.dev1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.906064 caso-4.0.1.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.github/workflows/packaging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.stestr.conf
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.testr.conf
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-30 22:06:06.922064 caso-4.0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.910064 caso-4.0.1.dev1/caso/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.910064 caso-4.0.1.dev1/caso/_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/_cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/_cmd/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.910064 caso-4.0.1.dev1/caso/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.914065 caso-4.0.1.dev1/caso/extract/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/openstack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/openstack/cinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)    18119 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/extract/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/keystone_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.914065 caso-4.0.1.dev1/caso/messenger/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/messenger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/messenger/logstash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/messenger/noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/messenger/ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/opts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.914065 caso-4.0.1.dev1/caso/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.914065 caso-4.0.1.dev1/caso/tests/extract/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/tests/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/tests/extract/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/tests/extract/test_nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/caso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.910064 caso-4.0.1.dev1/caso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 22:06:06.000000 caso-4.0.1.dev1/caso.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.914065 caso-4.0.1.dev1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.914065 caso-4.0.1.dev1/doc/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2980 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/configuration-file.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/multi-region.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.918064 caso-4.0.1.dev1/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)    58956 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/static/caso-diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)   111404 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/static/caso-diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/static/caso.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/static/caso.png
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/doc/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.902064 caso-4.0.1.dev1/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.918064 caso-4.0.1.dev1/etc/caso/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/etc/caso/caso-config-generator.conf
--rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/etc/caso/caso.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/etc/caso/voms.json.sample
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.902064 caso-4.0.1.dev1/packaging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.918064 caso-4.0.1.dev1/packaging/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/README.Debian
--rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/clean
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/cron.hourly
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/gbp.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/postinst
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.918064 caso-4.0.1.dev1/packaging/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/debian/source/format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.918064 caso-4.0.1.dev1/packaging/redhat/
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/packaging/redhat/caso.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.902064 caso-4.0.1.dev1/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:06:06.922064 caso-4.0.1.dev1/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/releasenotes/notes/support-for-storage-34675eff431608d1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-30 22:06:06.922064 caso-4.0.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-03-30 22:05:46.000000 caso-4.0.1.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.600937 caso-4.1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.592937 caso-4.1.0.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.592937 caso-4.1.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.stestr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.testr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 13:59:34.600937 caso-4.1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.592937 caso-4.1.0.0rc1/caso/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/caso/_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/_cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/_cmd/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/_cmd/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/caso/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/caso/extract/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/openstack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/openstack/cinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/extract/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/keystone_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/caso/messenger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/messenger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/messenger/logstash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/messenger/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/messenger/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/caso/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/caso/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/tests/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/tests/extract/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/tests/extract/test_nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/caso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/caso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 13:59:34.000000 caso-4.1.0.0rc1/caso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/doc/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2980 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/configuration-file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/multi-region.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    58956 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/static/caso-diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)   111404 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/static/caso-diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/static/caso.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/static/caso.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/doc/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.592937 caso-4.1.0.0rc1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.596937 caso-4.1.0.0rc1/etc/caso/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/etc/caso/caso-config-generator.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/etc/caso/caso.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/etc/caso/voms.json.sample
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.592937 caso-4.1.0.0rc1/packaging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.600937 caso-4.1.0.0rc1/packaging/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/README.Debian
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/clean
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/cron.hourly
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/gbp.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/postinst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.600937 caso-4.1.0.0rc1/packaging/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.600937 caso-4.1.0.0rc1/packaging/redhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/packaging/redhat/caso.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.592937 caso-4.1.0.0rc1/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:59:34.600937 caso-4.1.0.0rc1/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/support-for-storage-34675eff431608d1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/releasenotes/notes/tags-for-projects-3b9b6b5a92bcc6df.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-10 13:59:34.600937 caso-4.1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-10 13:59:17.000000 caso-4.1.0.0rc1/tox.ini
```

### Comparing `caso-4.0.1.dev1/.github/PULL_REQUEST_TEMPLATE.md` & `caso-4.1.0.0rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/.github/workflows/packaging.yml` & `caso-4.1.0.0rc1/.github/workflows/packaging.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10"]
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
@@ -39,15 +39,15 @@
         with:
           ref: ${{ github.ref_name }}
       
       - name: Copy debian file into the correct place for the build
         run: cp -r packaging/debian debian
 
       - name: Build Debian package
-        uses: alvarolopez/action-debian-python-package@v3
+        uses: alvarolopez/action-debian-python-package@v4
         with:
           artifacts_directory: output
           os_distribution: stable
 
       - name: Update DEB artifacts to release
         if: github.event_name == 'release'
         uses: AButler/upload-release-assets@v2.0
@@ -67,15 +67,15 @@
           ref: ${{ github.ref_name }}
       
       - name: Build sdist to use as source
         run: python setup.py sdist
 
       - name: Build RPM package
         id: rpm
-        uses: alvarolopez/rpmbuild@rockylinux8
+        uses: alvarolopez/rpmbuild@rockylinux9
         with:
           source_file: dist/caso-${{ github.ref_name}}.tar.gz
           spec_file: "packaging/redhat/caso.spec"
 
       - name: Update RPM artifacts to release
         if: github.event_name == 'release'
         uses: AButler/upload-release-assets@v2.0
```

### Comparing `caso-4.0.1.dev1/.github/workflows/python-publish.yml` & `caso-4.1.0.0rc1/.github/workflows/python-publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10"]
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
@@ -33,15 +33,15 @@
   publish:
     runs-on: ubuntu-latest
     needs: test
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
```

### Comparing `caso-4.0.1.dev1/.github/workflows/python-test.yml` & `caso-4.1.0.0rc1/.github/workflows/python-test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10"]
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
```

### Comparing `caso-4.0.1.dev1/.readthedocs.yml` & `caso-4.1.0.0rc1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/CODE_OF_CONDUCT.md` & `caso-4.1.0.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/CONTRIBUTING.md` & `caso-4.1.0.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/LICENSE` & `caso-4.1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/PKG-INFO` & `caso-4.1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caso
-Version: 4.0.1.dev1
+Version: 4.1.0.0rc1
 Summary: cASO is an OpenStack Accounting extractor.
 Home-page: http://github.com/IFCA/caso
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/IFCA/caso/issues
 Project-URL: Documentation, https://caso.readthedocs.io/
```

### Comparing `caso-4.0.1.dev1/README.md` & `caso-4.1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/__init__.py` & `caso-4.1.0.0rc1/caso/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/_cmd/extract.py` & `caso-4.1.0.0rc1/caso/_cmd/extract.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/config.py` & `caso-4.1.0.0rc1/caso/config.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/exception.py` & `caso-4.1.0.0rc1/caso/exception.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/extract/__init__.py` & `caso-4.1.0.0rc1/caso/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/extract/manager.py` & `caso-4.1.0.0rc1/caso/extract/manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,44 +13,67 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Module containing the manager for all extractors configured in cASO."""
 
 import datetime
+import json
 import os.path
 import sys
+import warnings
 
 import dateutil.parser
 from dateutil import tz
 from oslo_config import cfg
 from oslo_log import log
 import six
 
+from caso import keystone_client
 from caso import loading
 
 cli_opts = [
     cfg.ListOpt(
         "projects",
         default=[],
-        deprecated_name="tenants",
-        help="List of projects to extract accounting records from.",
+        help="List of projects to extract accounting records from. You can "
+        "use this option, or add 'caso' tag to the project in Keystone. "
+        "Please refer to the documentation for more details.",
+    ),
+    cfg.StrOpt(
+        "caso_tag",
+        default="caso",
+        help="Tag used to mark a project in Keystone to be extracted by cASO",
+    ),
+    cfg.StrOpt(
+        "vo_property",
+        default="accounting:VO",
+        help="Property key used to get the VO name from the project properties. ",
+    ),
+    cfg.StrOpt(
+        "mapping_file",
+        default="/etc/caso/voms.json",
+        deprecated_group="extractor",
+        deprecated_for_removal=True,
+        deprecated_reason="This option is marked for removal in the next release. "
+        "Please see the release notes, and migrate your current configuration "
+        "to use the new project mapping as soon as possible. If you already migrated "
+        "your configuration, please remove the JSON file to get rid of this message.",
+        help="File containing the VO <-> project mapping as used in Keystone-VOMS.",
     ),
     cfg.StrOpt(
         "extract-to",
-        deprecated_name="extract_to",
         help="Extract record changes until this date. "
         "If it is not set, we use now. If a server has "
         "ended after this date, it will be included, but "
         "the consuption reported will end on this date. "
         "If no time zone is specified, UTC will be used.",
     ),
     cfg.StrOpt(
         "extract-from",
-        deprecated_name="extract_from",
         help="Extract records that have changed after this date. This "
         "means that if a record has started before this date, and "
         "it has changed after this date (i.e. it is still running "
         "or it has ended) it will be reported. \n"
         "If it is not set, extract records from last run. "
         "If it is set to None and last run file is not present, "
         "it will extract records from the beginning of time. "
@@ -58,23 +81,22 @@
     ),
     cfg.ListOpt(
         "extractor",
         default=["nova"],
         help="Which extractor to use for getting the data. "
         "If you do not specify anything, nova will be "
         "used. Available choices are {}".format(
-            loading.get_available_extractor_names()
+            sorted(loading.get_available_extractor_names())
         ),
     ),
 ]
 
 CONF = cfg.CONF
 
 CONF.register_cli_opts(cli_opts)
-CONF.import_opt("projects", "caso.extract.base")
 
 LOG = log.getLogger(__name__)
 
 
 class Manager(object):
     """A manager for the configured extractors.
 
@@ -86,24 +108,32 @@
         """Initialize a extractor manager, loading all configured extractors."""
         extractors = [
             (i, loading.get_available_extractors()[i]) for i in CONF.extractor
         ]
         self.extractors = extractors
         self.last_run_base = os.path.join(CONF.spooldir, "lastrun")
 
+        self._voms_map = {}
+        self.keystone = self._get_keystone_client()
+
+    @property
+    def projects(self):
+        """Get list of configured projects."""
+        projects = CONF.projects
+        aux = [i.id for i in self.keystone.projects.list(tags=CONF.caso_tag)]
+        return set(projects + aux)
+
+    def _get_keystone_client(self):
+        """Get a Keystone Client to get the projects that we will use."""
+        client = keystone_client.get_client(CONF, system_scope="all")
+        return client
+
     def get_lastrun(self, project):
         """Get lastrun file for a given project."""
         lfile = f"{self.last_run_base}.{project}"
-        if not os.path.exists(lfile):
-            LOG.warning(
-                "WARNING: Old global lastrun file detected and no "
-                "project specific file found, using it for this run"
-            )
-            lfile = self.last_run_base
-
         date = "1970-01-01"
 
         if os.path.exists(lfile):
             with open(lfile, "r") as fd:
                 date = fd.read()
         else:
             LOG.info(f"No lastrun file found, using '{date}'")
@@ -120,14 +150,81 @@
         """Write a lastrun file for a given project."""
         if CONF.dry_run:
             return
         lfile = f"{self.last_run_base}.{project}"
         with open(lfile, "w") as fd:
             fd.write(str(datetime.datetime.now(tz.tzutc())))
 
+    @property
+    def voms_map(self):
+        """Get the VO map."""
+        if self._voms_map:
+            return self._voms_map
+
+        if not os.path.exists(CONF.mapping_file):
+            return {}
+
+        try:
+            mapping = json.loads(open(CONF.mapping_file).read())
+        except ValueError:
+            # FIXME(aloga): raise a proper exception here
+            raise
+        else:
+            self._voms_map = {}
+            for vo, vomap in six.iteritems(mapping):
+                tenant = vomap.get("tenant", None)
+                tenants = vomap.get("tenants", [])
+                if tenant is not None:
+                    warnings.warn(
+                        "Using deprecated 'tenant' mapping, please "
+                        "use 'projects' instead",
+                        DeprecationWarning,
+                    )
+                if tenants:
+                    warnings.warn(
+                        "Using deprecated 'tenants' mapping, please "
+                        "use 'projects' instead",
+                        DeprecationWarning,
+                    )
+                tenants.append(tenant)
+                projects = vomap.get("projects", tenants)
+                if not projects:
+                    LOG.warning(f"No project mapping found for VO {vo}")
+                for project in projects:
+                    self._voms_map[project] = vo
+            return self._voms_map
+
+    def get_project_vo(self, project_id):
+        """Get the VO where the project should be mapped."""
+        project = self.keystone.projects.get(project_id)
+        project.get()
+        vo = project.to_dict().get(CONF.vo_property, None)
+        if vo is None:
+            LOG.warning(
+                f"No mapping could be found for project '{project_id}' in the "
+                "Keystone project metadata, please check cASO documentation."
+            )
+            vo = self.voms_map.get(project_id, None)
+            if vo is None:
+                LOG.warning(
+                    "No mapping could be found for project "
+                    f"'{project_id}', please check mapping file!"
+                )
+            else:
+                LOG.warning(
+                    "Using deprecated mapping file, please check cASO documentation "
+                    "and migrate to Keystone properties as soon as possible."
+                )
+        else:
+            LOG.debug(
+                f"Found VO mapping ({vo}) in Keystone project '{project_id}' "
+                "metadata."
+            )
+        return vo
+
     def get_records(self):
         """Get records from given date.
 
         If CONF.extract_from is present, it will be used instead of the
         lastrun parameter. If CONF.extract_to is present, it will be used
         instead of the extract_to parameter
         """
@@ -145,17 +242,19 @@
                 "current date and time, cASO will limit the record "
                 "generation to the current date and time. "
                 f"(extract-to: {extract_to}"
             )
             extract_to = now
 
         all_records = []
-        for project in CONF.projects:
+        for project in self.projects:
             LOG.info(f"Extracting records for project '{project}'")
 
+            vo = self.get_project_vo(project)
+
             extract_from = CONF.extract_from or self.get_lastrun(project)
             if isinstance(extract_from, six.string_types):
                 extract_from = dateutil.parser.parse(extract_from)
             if extract_from.tzinfo is None:
                 extract_from = extract_from.replace(tzinfo=tz.tzutc())
 
             if extract_from >= now:
@@ -171,15 +270,15 @@
             for extractor_name, extractor_cls in self.extractors:
                 LOG.debug(
                     f"Extractor {extractor_name}: extracting records "
                     f"for project {project} "
                     f"({extract_from} to {extract_to})"
                 )
                 try:
-                    extractor = extractor_cls(project)
+                    extractor = extractor_cls(project, vo)
                     records = extractor.extract(extract_from, extract_to)
                     current_count = len(records)
                     record_count += current_count
                     all_records.extend(records)
 
                     LOG.debug(
                         f"Extractor {extractor_name}: extracted "
```

### Comparing `caso-4.0.1.dev1/caso/extract/openstack/__init__.py` & `caso-4.1.0.0rc1/caso/extract/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/extract/openstack/base.py` & `caso-4.1.0.0rc1/caso/extract/openstack/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,51 +14,55 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Module containing the base class for all OpenStack extractors."""
 
 import datetime
 
+import cinderclient.v3.client
+import glanceclient.client
 import keystoneauth1.exceptions.http
+import neutronclient.v2_0.client
+import novaclient.client
 from oslo_config import cfg
 from oslo_log import log
 
 from caso.extract import base
 from caso import keystone_client
 
 CONF = cfg.CONF
 
 opts = [
     cfg.StrOpt(
         "region_name",
         default=None,
         help="OpenStack Region to use. This option will force cASO to "
-        "extract records from a specific OpenStack Region, in "
+        "extract records from a specific OpenStack Region, if "
         "there are several defined in the OpenStack site. "
         "Defaults to None.",
-    )
+    ),
 ]
 
 CONF.register_opts(opts)
 
 LOG = log.getLogger(__name__)
 
 
 class BaseOpenStackExtractor(base.BaseProjectExtractor):
     """Base OpenStack Extractor that all other extractors should inherit from."""
 
-    def __init__(self, project):
+    def __init__(self, project, vo):
         """Initialize the OpenStack extractor for a given project."""
         super(BaseOpenStackExtractor, self).__init__(project)
 
-        self.vo = self._get_vo()
-
         self.keystone = self._get_keystone_client()
         self.project_id = self._get_project_id()
 
+        self.vo = vo
+
         class Users:
             def __init__(self, parent):
                 self._users = {}
                 self.parent = parent
 
             def get(self, key, default):
                 return self[key]
@@ -87,14 +91,35 @@
         return session
 
     def _get_keystone_client(self):
         """Get a Keystone Client for the configured project in the object."""
         client = keystone_client.get_client(CONF, self.project)
         return client
 
+    def _get_cinder_client(self):
+        """Get Cinder client with keystone session."""
+        session = self._get_keystone_session()
+        return cinderclient.v3.client.Client(session=session)
+
+    def _get_glance_client(self):
+        """Get a glance client with a keystone session."""
+        session = self._get_keystone_session()
+        return glanceclient.client.Client(2, session=session)
+
+    def _get_neutron_client(self):
+        """Get a neutron client with a keystone session."""
+        session = self._get_keystone_session()
+        return neutronclient.v2_0.client.Client(session=session)
+
+    def _get_nova_client(self):
+        """Get a nova client with a keystone session."""
+        region_name = CONF.region_name
+        session = self._get_keystone_session()
+        return novaclient.client.Client(2, session=session, region_name=region_name)
+
     def _get_project_id(self):
         """Get the project ID from the project in the object."""
         return self.keystone.projects.get(self.project).id
 
     def _get_keystone_user(self, uuid):
         """Get the Keystone username for a given uuid."""
         try:
@@ -105,23 +130,13 @@
             LOG.exception(e)
             return None
         except Exception as e:
             LOG.debug("Exception while getting user")
             LOG.exception(e)
             return None
 
-    def _get_vo(self):
-        """Get the VO where the project should be mapped."""
-        vo = self.voms_map.get(self.project)
-        if vo is None:
-            LOG.warning(
-                "No mapping could be found for project "
-                f"'{self.project}', please check mapping file!"
-            )
-        return vo
-
     # FIXME(aloga): this has to go inside a record
     @staticmethod
     def _get_measure_time():
         """Get current measurement time."""
         measure_time = datetime.datetime.now()
         return measure_time
```

### Comparing `caso-4.0.1.dev1/caso/extract/openstack/cinder.py` & `caso-4.1.0.0rc1/caso/extract/openstack/cinder.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Module containing the OpenStack Volume (Cinder) record extractor."""
 
 import operator
 
-import cinderclient.v3.client
 import dateutil.parser
 from oslo_config import cfg
 from oslo_log import log
 
 from caso.extract.openstack import base
 from caso import record
 
@@ -33,25 +32,20 @@
 
 LOG = log.getLogger(__name__)
 
 
 class CinderExtractor(base.BaseOpenStackExtractor):
     """An OpenStack Volume (Cinder) record extractor for cASO."""
 
-    def __init__(self, project):
+    def __init__(self, project, vo):
         """Get a Cinder record extractor for a given project."""
-        super(CinderExtractor, self).__init__(project)
+        super(CinderExtractor, self).__init__(project, vo)
 
         self.cinder = self._get_cinder_client()
 
-    def _get_cinder_client(self):
-        """Get Cinder client with keystone session."""
-        session = self._get_keystone_session()
-        return cinderclient.v3.client.Client(session=session)
-
     def _build_record(self, volume, extract_from, extract_to):
         """Build an individual record."""
         user = self.users[volume.user_id]
         measure_time = self._get_measure_time()
 
         vol_start = volume.__getattr__("created_at")
         vol_created = dateutil.parser.parse(vol_start)
```

### Comparing `caso-4.0.1.dev1/caso/extract/openstack/neutron.py` & `caso-4.1.0.0rc1/caso/extract/openstack/neutron.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,52 +14,47 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Module containing the  OpenStack Network (Neutron) record extractor."""
 
 import collections
 import ipaddress
+import uuid
 
-import neutronclient.v2_0.client
 from oslo_config import cfg
 from oslo_log import log
 
 from caso.extract.openstack import base
 from caso import record
 from datetime import datetime
 
 CONF = cfg.CONF
 
 CONF.import_opt("region_name", "caso.extract.openstack")
 CONF.import_opt("site_name", "caso.extract.base")
-CONF.import_group("benchmark", "caso.extract.base")
-CONF.import_group("accelerator", "caso.extract.base")
 
 LOG = log.getLogger(__name__)
 
 
 class NeutronExtractor(base.BaseOpenStackExtractor):
     """An OpenStack Network (Neutron) record extractor for cASO."""
 
-    def __init__(self, project):
+    def __init__(self, project, vo):
         """Get a Neutron record extractor for a given project."""
-        super(NeutronExtractor, self).__init__(project)
+        super(NeutronExtractor, self).__init__(project, vo)
 
         self.neutron = self._get_neutron_client()
 
-    def _get_neutron_client(self):
-        session = self._get_keystone_session()
-        return neutronclient.v2_0.client.Client(session=session)
-
     def _build_ip_record(self, user_id, ip_count, version):
         user = self.users[user_id]
 
         measure_time = self._get_measure_time()
 
         r = record.IPRecord(
+            uuid=uuid.uuid4().hex,
             measure_time=measure_time,
             site_name=CONF.site_name,
             user_id=user_id,
             group_id=self.project_id,
             user_dn=user,
             fqan=self.vo,
             ip_version=version,
```

### Comparing `caso-4.0.1.dev1/caso/extract/openstack/nova.py` & `caso-4.1.0.0rc1/caso/extract/openstack/nova.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,65 +18,88 @@
 
 import operator
 
 import dateutil.parser
 from dateutil.relativedelta import relativedelta
 from dateutil.rrule import MONTHLY
 from dateutil.rrule import rrule
-import glanceclient.client
-import neutronclient.v2_0.client
-import novaclient.client
 import novaclient.exceptions
 from oslo_config import cfg
 from oslo_log import log
 
 from caso.extract.openstack import base
 from caso import record
 from datetime import datetime
 
+accelerator_opts = [
+    cfg.StrOpt(
+        "type_key",
+        default="Accelerator:Type",
+        help="Metadata key used to retrieve the accelerator type "
+        "from the flavor properties.",
+    ),
+    cfg.StrOpt(
+        "vendor_key",
+        default="Accelerator:Vendor",
+        help="Metadata key used to retrieve the accelerator vendor "
+        "from the flavor properties.",
+    ),
+    cfg.StrOpt(
+        "model_key",
+        default="Accelerator:Model",
+        help="Metadata key used to retrieve the accelerator model "
+        "from the flavor properties.",
+    ),
+    cfg.StrOpt(
+        "number_key",
+        default="Accelerator:Number",
+        help="Metadata key used to retrieve the accelerator number "
+        "from the flavor properties.",
+    ),
+]
+
+benchmark_opts = [
+    cfg.StrOpt(
+        "name_key",
+        default="accounting:benchmark_type",
+        help="Metadata key used to retrieve the benchmark type "
+        "from the flavor properties.",
+    ),
+    cfg.StrOpt(
+        "value_key",
+        default="accounting:benchmark_value",
+        help="Metadata key used to retrieve the benchmark value "
+        "from the flavor properties.",
+    ),
+]
+
 CONF = cfg.CONF
 
 CONF.import_opt("region_name", "caso.extract.openstack")
 CONF.import_opt("site_name", "caso.extract.base")
-CONF.import_group("benchmark", "caso.extract.base")
-CONF.import_group("accelerator", "caso.extract.base")
+CONF.register_opts(benchmark_opts, group="benchmark")
+CONF.register_opts(accelerator_opts, group="accelerator")
 
 LOG = log.getLogger(__name__)
 
 
 class NovaExtractor(base.BaseOpenStackExtractor):
     """An OpenStack Compute (Nova) record extractor for cASO."""
 
-    def __init__(self, project):
+    def __init__(self, project, vo):
         """Get a Nova record extractor for a given project."""
-        super(NovaExtractor, self).__init__(project)
+        super(NovaExtractor, self).__init__(project, vo)
 
         self.nova = self._get_nova_client()
         self.glance = self._get_glance_client()
         self.neutron = self._get_neutron_client()
 
         self.flavors = self._get_flavors()
         self.images = self._get_images()
 
-    def _get_nova_client(self):
-        """Get a nova client with a keystone session."""
-        region_name = CONF.region_name
-        session = self._get_keystone_session()
-        return novaclient.client.Client(2, session=session, region_name=region_name)
-
-    def _get_glance_client(self):
-        """Get a glance client with a keystone session."""
-        session = self._get_keystone_session()
-        return glanceclient.client.Client(2, session=session)
-
-    def _get_neutron_client(self):
-        """Get a neutron client with a keystone session."""
-        session = self._get_keystone_session()
-        return neutronclient.v2_0.client.Client(session=session)
-
     def _build_acc_records(self, server, server_record, extract_from, extract_to):
         records = {}
         flavor = self.flavors.get(server.flavor["id"])
         if not flavor:
             return records
 
         acc_type = flavor["extra"].get(CONF.accelerator.type_key)
@@ -127,14 +150,44 @@
         count = 0
         for _name, value in server.addresses.items():
             for ip in value:
                 if ip["OS-EXT-IPS:type"] == "floating":
                     count += 1
         return count
 
+    def vm_status(self, status):
+        """Return the status corresponding to the OpenStack status.
+
+        :param status: OpenStack status.
+        """
+        openstack_vm_statuses = {
+            "active": "started",
+            "build": "started",
+            "confirming_resize": "started",
+            "deleted": "completed",
+            "error": "error",
+            "hard_reboot": "started",
+            "migrating": "started",
+            "password": "started",
+            "paused": "paused",
+            "reboot": "started",
+            "rebuild": "started",
+            "rescue": "started",
+            "resize": "started",
+            "revert_resize": "started",
+            "verify_resize": "started",
+            "shutoff": "completed",
+            "suspended": "suspended",
+            "terminated": "completed",
+            "stopped": "stopped",
+            "saving": "started",
+            "unknown": "unknown",
+        }
+        return openstack_vm_statuses.get(status.lower(), "unknown")
+
     def _build_record(self, server):
         user = self.users[server.user_id]
 
         server_start = self._get_server_start(server)
         server_end = self._get_server_end(server)
 
         status = self.vm_status(server.status)
```

### Comparing `caso-4.0.1.dev1/caso/keystone_client.py` & `caso-4.1.0.0rc1/caso/keystone_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 
 opts = []
 opts += loading.get_auth_common_conf_options()
 opts += loading.get_session_conf_options()
 opts += loading.get_auth_plugin_conf_options("password")
 
 
-def get_session(conf, project):
+def get_session(conf, project, system_scope=None):
     """Get an auth session."""
     # First try using project_id
     auth_plugin = loading.load_auth_from_conf_options(
-        conf, CFG_GROUP, project_id=project
+        conf, CFG_GROUP, project_id=project, system_scope=system_scope
     )
     sess = loading.load_session_from_conf_options(conf, CFG_GROUP, auth=auth_plugin)
     try:
         sess.get_token()
     except exceptions.Unauthorized:
         # Failure, now try project_name
         auth_plugin = loading.load_auth_from_conf_options(
             conf, CFG_GROUP, project_name=project, project_id=None
         )
         sess = loading.load_session_from_conf_options(conf, CFG_GROUP, auth=auth_plugin)
     return sess
 
 
-def get_client(conf, project):
+def get_client(conf, project=None, system_scope=None):
     """Return a client for Keystone."""
-    sess = get_session(conf, project)
+    sess = get_session(conf, project, system_scope)
     return ks_client_v3.Client(session=sess, interface="public")
```

### Comparing `caso-4.0.1.dev1/caso/loading.py` & `caso-4.1.0.0rc1/caso/loading.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/manager.py` & `caso-4.1.0.0rc1/caso/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 """The cASO manager: get configured records and push to configured messengers."""
 
 import os
 import os.path
 
 from oslo_concurrency import lockutils
 from oslo_config import cfg
+from oslo_log import log
 
 import caso.extract.manager
 from caso import loading
 import caso.messenger
 from caso import utils
 
 opts = [
@@ -49,51 +50,71 @@
     "CASO_LOCK_PATH or $spooldir",
 )
 opts.append(override_lock)
 
 cli_opts = [
     cfg.BoolOpt(
         "dry-run",
-        deprecated_name="dry_run",
         default=False,
         help="Extract records but do not push records to SSM. This "
         "will not update the last run date.",
     ),
 ]
 
 CONF = cfg.CONF
 
 CONF.register_opts(opts)
 CONF.register_cli_opts(cli_opts)
 
+LOG = log.getLogger(__name__)
+
 
 class Manager(object):
     """cASO manager class to deal with the main functionality."""
 
     def __init__(self):
         """Initialize the cASO manager with configued options."""
         utils.makedirs(CONF.spooldir)
 
         self.extractor_manager = None
         self.messenger = None
 
         self.lock_path = CONF.lock_path
 
+    def _load_managers(self):
+        # Load the managers here to have the config options loaded and
+        # available
+        self.extractor_manager = caso.extract.manager.Manager()
+        self.messenger = caso.messenger.Manager()
+
+    def projects(self):
+        """Get the configured projects."""
+        self._load_managers()
+
+        return self.extractor_manager.projects
+
+    def projects_and_vos(self):
+        """Get the configured projects and VOs as tuples."""
+        self._load_managers()
+
+        for prj in self.extractor_manager.projects:
+            try:
+                yield (prj, self.extractor_manager.get_project_vo(prj))
+            except Exception as e:
+                LOG.error(e)
+
     def run(self):
         """Run the manager.
 
         This method runs the main cASo functionality, namely:
             - Gets the global lock
             - Gets all records from the configured extractors
             - Pushes all the records to the messengers
         """
-        # Load the managers here to have the config options loaded and
-        # available
-        self.extractor_manager = caso.extract.manager.Manager()
-        self.messenger = caso.messenger.Manager()
+        self._load_managers()
 
         @lockutils.synchronized(
             "caso_should_not_run_in_parallel", lock_path=self.lock_path, external=True
         )
         def synchronized():
             records = self.extractor_manager.get_records()
             if not CONF.dry_run:
```

### Comparing `caso-4.0.1.dev1/caso/messenger/__init__.py` & `caso-4.1.0.0rc1/caso/messenger/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,8 +52,9 @@
 
     def push_to_all(self, records):
         """Push records to all the configured messengers."""
         try:
             self.mgr.map_method("push", records)
         except Exception as e:
             # Capture exception so that we can continue working
-            LOG.error(e)
+            LOG.error("Something happeneded when pushing records.")
+            LOG.exception(e)
```

### Comparing `caso-4.0.1.dev1/caso/messenger/logstash.py` & `caso-4.1.0.0rc1/caso/messenger/logstash.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/messenger/noop.py` & `caso-4.1.0.0rc1/caso/messenger/noop.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Module containing a No-Op (No Operation) messenger that does nothing."""
 
 from oslo_log import log
-import six
 
 import caso.messenger
 
 LOG = log.getLogger(__name__)
 
 
 class NoopMessenger(caso.messenger.BaseMessenger):
     """Noop messenger that does nothing."""
 
     def push(self, records):
         """Push records to nowhere."""
-        for uuid, _ in six.iteritems(records):
-            LOG.info(f"nooping {uuid}")
+        for record in records:
+            LOG.info(f"nooping {record.uuid} for record {record.__class__}")
```

### Comparing `caso-4.0.1.dev1/caso/messenger/ssm.py` & `caso-4.1.0.0rc1/caso/messenger/ssm.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/opts.py` & `caso-4.1.0.0rc1/caso/opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 """Module defining all the options to be managed by oslo."""
 
 import itertools
 
 import caso.extract.base
 import caso.extract.manager
+import caso.extract.openstack.nova
 import caso.keystone_client
 import caso.manager
 import caso.messenger.logstash
 import caso.messenger.ssm
 
 
 def list_opts():
@@ -34,13 +35,13 @@
             itertools.chain(
                 caso.manager.opts,
                 caso.manager.cli_opts,
                 caso.extract.base.opts,
                 caso.extract.manager.cli_opts,
             ),
         ),
-        ("accelerator", caso.extract.base.accelerator_opts),
-        ("benchmark", caso.extract.base.benchmark_opts),
+        ("accelerator", caso.extract.openstack.nova.accelerator_opts),
+        ("benchmark", caso.extract.openstack.nova.benchmark_opts),
         ("keystone_auth", caso.keystone_client.opts),
         ("logstash", caso.messenger.logstash.opts),
         ("ssm", caso.messenger.ssm.opts),
     ]
```

### Comparing `caso-4.0.1.dev1/caso/record.py` & `caso-4.1.0.0rc1/caso/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     """The IPRecord class holds information for each of the records.
 
     This class is versioned, following the Public IP Usage Record versions.
     """
 
     version = "0.2"
 
+    uuid: m_uuid.UUID
+
     user_id: typing.Optional[str]
     user_dn: typing.Optional[str]
     group_id: str
     fqan: str
 
     measure_time: datetime.datetime
```

### Comparing `caso-4.0.1.dev1/caso/tests/base.py` & `caso-4.1.0.0rc1/caso/tests/base.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/tests/extract/test_manager.py` & `caso-4.1.0.0rc1/caso/tests/extract/test_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,26 @@
         self.flags(extractor="mock")
         self.p_extractors = mock.patch("caso.loading.get_available_extractors")
         patched = self.p_extractors.start()
         self.records = [{uuid.uuid4().hex: None}]
         self.m_extractor = mock.MagicMock()
         self.m_extractor.return_value.extract.return_value = self.records
         patched.return_value = {"mock": self.m_extractor}
+
+        self.p_keystone = mock.patch(
+            "caso.extract.manager.Manager._get_keystone_client"
+        )
+        self.p_keystone.start()
+
         self.manager = manager.Manager()
 
     def tearDown(self):
         """Run after each test, reset state and environment."""
         self.p_extractors.stop()
+        self.p_keystone.stop()
         self.reset_flags()
 
         super(TestCasoManager, self).tearDown()
 
     def test_extract_empty_projects(self):
         """Test that we can extract from empty projects."""
         self.flags(projects=[])
@@ -64,14 +71,15 @@
         extract_to = "2015-12-19"
         self.flags(extract_from=extract_from)
         self.flags(extract_to=extract_to)
 
         ret = self.manager.get_records()
         self.m_extractor.assert_called_once_with(
             "bazonk",
+            mock.ANY,
         )
         self.m_extractor.return_value.extract.assert_called_once_with(
             dateutil.parser.parse(extract_from).replace(tzinfo=tz.tzutc()),
             dateutil.parser.parse(extract_to).replace(tzinfo=tz.tzutc()),
         )
         self.assertEqual(self.records, ret)
 
@@ -98,14 +106,15 @@
             m.return_value = lastrun
 
             ret = self.manager.get_records()
 
             m.assert_called_once_with("bazonk")
             self.m_extractor.assert_called_once_with(
                 "bazonk",
+                mock.ANY,
             )
             self.m_extractor.return_value.extract.assert_called_once_with(
                 dateutil.parser.parse(lastrun).replace(tzinfo=tz.tzutc()),
                 dateutil.parser.parse(extract_to).replace(tzinfo=tz.tzutc()),
             )
         self.assertEqual(self.records, ret)
```

### Comparing `caso-4.0.1.dev1/caso/tests/extract/test_nova.py` & `caso-4.1.0.0rc1/caso/tests/extract/test_nova.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/tests/test_manager.py` & `caso-4.1.0.0rc1/caso/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso/utils.py` & `caso-4.1.0.0rc1/caso/utils.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/caso.egg-info/PKG-INFO` & `caso-4.1.0.0rc1/caso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caso
-Version: 4.0.1.dev1
+Version: 4.1.0.0rc1
 Summary: cASO is an OpenStack Accounting extractor.
 Home-page: http://github.com/IFCA/caso
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/IFCA/caso/issues
 Project-URL: Documentation, https://caso.readthedocs.io/
```

### Comparing `caso-4.0.1.dev1/caso.egg-info/SOURCES.txt` & `caso-4.1.0.0rc1/caso.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 caso.egg-info/entry_points.txt
 caso.egg-info/not-zip-safe
 caso.egg-info/pbr.json
 caso.egg-info/requires.txt
 caso.egg-info/top_level.txt
 caso/_cmd/__init__.py
 caso/_cmd/extract.py
+caso/_cmd/projects.py
 caso/extract/__init__.py
 caso/extract/base.py
 caso/extract/manager.py
 caso/extract/openstack/__init__.py
 caso/extract/openstack/base.py
 caso/extract/openstack/cinder.py
 caso/extract/openstack/neutron.py
@@ -84,14 +85,16 @@
 packaging/debian/cron.hourly
 packaging/debian/gbp.conf
 packaging/debian/postinst
 packaging/debian/rules
 packaging/debian/source/format
 packaging/redhat/caso.spec
 releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
+releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
 releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
 releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
 releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
 releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
 releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
 releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
-releasenotes/notes/support-for-storage-34675eff431608d1.yaml
+releasenotes/notes/support-for-storage-34675eff431608d1.yaml
+releasenotes/notes/tags-for-projects-3b9b6b5a92bcc6df.yaml
```

### Comparing `caso-4.0.1.dev1/doc/source/conf.py` & `caso-4.1.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/configuration.rst` & `caso-4.1.0.0rc1/doc/source/configuration.rst`

 * *Files 17% similar despite different names*

```diff
@@ -21,37 +21,47 @@
 
 Apart from configuring cASO, several actions need to be performed in your
 OpenStack installation in order to be able to extract accounting records.
 
 User credentials (required)
 ---------------------------
 
-In the next section you will configure an OpenStack Keystone credentials in
-order to extract the records. The cASO user has to be a member of each of the
-projects (another option is to convert that user in an administrator, but the
-former option is a safer approach) for which it is extracting the accounting.
-Otherwise, ``cASO`` will not be able to get the usages and will fail.
+In the next section you will configure an OpenStack Keystone credentials in order to
+extract the records. The cASO user has to be a member of each of the projects (another
+option is to convert that user in an administrator, but the former option is a safer
+approach) for which it is extracting the accounting, with the ``reader`` role (this is
+a default OpenStack Keystone role). Otherwise, ``cASO`` will not be able to get the
+usages and will fail::
 
-In order to do so, we are going to setup a new role ``accounting`` a new user
-``accounting``, adding it to each of the projects with that role::
-
-    openstack role create accounting
     openstack user create --password <password> accounting
     # For each of the projects, add the user with the accounting role
-    openstack role add --user accounting --project <project> accounting
+    openstack role add --user accounting --project <project> reader
+
+Moreover, if you wish to gather the list of projects that ``cASO`` should use directly
+from OpenStack, you need to grant the user the role reader with a system scope of
+``all``::
+
+    openstack role add --system all --user accounting reader
 
 Policy modifications
---------------------
-The accounting user needs access to Keystone so as to extract the users
-information. In this case, we can can grant the user just the rights for
-listing the users adding the appropriate rules in your policy configuration.
+------------------------
+
+.. important:: No policy modifications are needed
+
+    The following policy modifications are just shown here for reference, if you wish to
+    use a different role. You do not need to use them.
+
+If you use the role ``reader`` as configured above, you do not need to configure
+anything else in the policy. However, if you wish to use a different role mapping, the
+accounting user needs access to Keystone so as to extract the users information.
 Depending on your configuration, you need to modify the JSON policy file
 (``/etc/keystone/policy.json``) or the YAML policy file (``/etc/keystone/policy-yaml``).
-The modifications in the policy depend on the Keystone version, please ensure
-that you are applying the correct changes as listed in the following table.
+The modifications in the policy depend on the Keystone version, please ensure that you
+are applying the correct changes as listed in the following table. In the example show,
+we are using a dedicated role ``accounting``.
 
 +-------------+------------------------------------------------------------------------------+
 |  OpenStack  |                                Policy contents                               |
 |   Version   |                                                                              |
 +=============+==========+===================================================================+
 | From Stein  | Original | ``“identity:get_user”: “(role:reader and system_scope:all) or     |
 | (>= 15.0.0) |          | (role:reader and token.domain.id:%(target.user.domain_id)s) or    |
@@ -62,14 +72,45 @@
 |             |          | user_id:%(target.user.id)s or role:accounting”``                  |
 +-------------+----------+-------------------------------------------------------------------+
 | Up to Rocky | Original | ``“identity:get_user”: “rule:admin_or_owner”``                    |
 | (<= 14.0.0) +----------+-------------------------------------------------------------------+
 |             | Modified | ``“identity:get_user”: “rule:admin_or_owner or role:accounting”`` |
 +-------------+----------+-------------------------------------------------------------------+
 
+Selecting projects to get usages
+================================
+
+``cASO`` will extract project usages for those projects that have been explictly marked
+by the operator by either of the ways explained below. The final project list will
+result from the merge of both methods, so thay are not mutually exclusive.
+
+* Tagging the project with the configured ``caso_tag`` in OpenStack Keystone. By default
+  this option is set to ``caso``, so in order to mark a project to get extracted you
+  should use the following command for each of the projects::
+
+    openstack project set --tag caso <project id>
+
+  You can check the list of projects to get usages by using::
+
+    openstack project list --tags caso
+
+* Using the ``projects`` list in the ``[DEFAULT]`` section of your configuration file
+  (see below).
+
+Setting VO mapping
+------------------
+
+In order to publish correct accounting records, ``cASO`` needs to know the VO that
+should be used to publish the records from a given project. In order to do so, you need
+to specify the correct mapping in each of the projects properties. The name of the
+property that will be used is defined in the ``vo_property`` configuration option, and
+defaults to ``accounting:VO``, therefore you can configure it as follows::
+
+     openstack project set --property accounting:VO=<VO FQAN> <project id>
+
 cASO configuration
 ==================
 
 ``cASO`` uses a config file (default at ``/etc/caso/caso.conf``) with several
 sections. A sample file is available at
 :download:`etc/caso/caso.conf.sample <static/caso.conf.sample>`.
 
@@ -87,44 +128,47 @@
   GOCDB.
 * ``service_name`` (default value: ``$site_name``). Name of the service within
   a site. This is used if you have several endpoints within your site.
 * ``projects`` (list value, default empty). List of the projects to extract
   records from. You can use either the project ID or the project name. We
   recommend that you use the project ID, especially if you are using
   domain-based authentication, as otherwise gathering the information might
-  fail.
+  fail. This option, and the usage of ``caso_tag`` below will set up the final
+  project list.
+* ``caso_tag`` (default value: ``caso``), specified the tag to be used filter projects
+  to extract their usage. The projects that are listed with this tag, as well as the
+  ``projects`` list set above will set up the final project list. If you only use tags,
+  and want to remove a project from being published, you just need to remove the tag
+  from the project.
 * ``messengers`` (list, default: ``noop``). List of the messengers to publish
   data to. Records will be pushed to all these messengers, in order. Valid
   messengers shipped with cASO are:
 
-      * ``ssm`` for publishing APEL V0.2 records (deprecated).
-      * ``ssmv2`` for publishing APEL V0.2 records (deprecated).
-      * ``ssmv4`` for publishing APEL V0.3 records (current).
+      * ``ssm`` for publishing APEL records.
       * ``logstash`` for publishing to Logstash.
       * ``noop`` do nothing at all.
 
   Note that there might be other messengers available in the system if they are
-  registered into the ``caso.messenger`` entry point namespace.
-* ``mapping_file`` (default: ``/etc/caso/voms.json``). File containing the
-  mapping from VOs to local projects as configured in Keystone-VOMS, in the
+  registered into the ``caso.messenger`` entry point namespace. Please also note that
+  versioning of the SSM messenger is deprecated.
+* ``vo_property`` (default: ``accounting:VO``). The project that will be set in the
+  OpenStack Keystone project to map a given project to a specific VO.
+* **DEPRECATED** ``mapping_file`` (default: ``/etc/caso/voms.json``). File containing
+  the mapping from VOs to local projects as configured in Keystone-VOMS, in the
   following form::
 
     {
         "VO": {
             "projects": ["foo", "bar"],
         }
     }
 
   Note that you have to use either the project ID or project name for the
   mapping, as configured in the ``projects`` configuration variable.
 
-* ``benchmark_name_key`` and ``benchmark_value_key``. These two configuration
-  options are used by ``cASO`` to retrieve the benchmark information form the
-  OpenStack flavors.
-
 ``[keystone_auth]`` section
 ---------------------------
 
 This section is used to specify the authentication credentials to be used to
 connect to the OpenStack APIs. cASO leverages the `OpenStack keystoneauth
 <https://docs.openstack.org/developer/keystoneauth/>`_ library for
 authentication, so that it is possible to use any authentication plugin that is
```

### Comparing `caso-4.0.1.dev1/doc/source/index.rst` & `caso-4.1.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/installation.rst` & `caso-4.1.0.0rc1/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/multi-region.rst` & `caso-4.1.0.0rc1/doc/source/multi-region.rst`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/static/caso-diagram.drawio` & `caso-4.1.0.0rc1/doc/source/static/caso-diagram.drawio`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/static/caso-diagram.png` & `caso-4.1.0.0rc1/doc/source/static/caso-diagram.png`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/static/caso.conf.sample` & `caso-4.1.0.0rc1/doc/source/static/caso.conf.sample`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/static/caso.png` & `caso-4.1.0.0rc1/doc/source/static/caso.png`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/troubleshooting.rst` & `caso-4.1.0.0rc1/doc/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/doc/source/usage.rst` & `caso-4.1.0.0rc1/doc/source/usage.rst`

 * *Files 6% similar despite different names*

```diff
@@ -81,22 +81,32 @@
 
 .. option:: --extract-to EXTRACT_TO, --extract_to EXTRACT_TO
 
    Extract record changes until this date. If it is not set, we use now. If a
    server has ended after this date, it will be included, but the consuption
    reported will end on this date. If no time zone is specified, UTC will be
    used.
+
 .. option:: --extractor EXTRACTOR
 
    Which extractor to use for getting the data. If you do not specify anything,
    nova will be used. Allowed values: nova
 
-.. option:: --projects PROJECTS, --tenants PROJECTS
+.. option:: --projects PROJECTS
 
    List of projects to extract accounting records from.
 
 Running as a cron job
 ---------------------
 
 The best way of running ``cASO`` is via a cron job like the following::
 
     10 * * * * caso-extract
+
+Other commands
+--------------
+
+caso-projects
+=============
+
+``cASO`` provides the ``caso-projects`` command line tool, that will print the list of
+configured OpenStack Keystone projects and their mappings.
```

### Comparing `caso-4.0.1.dev1/etc/caso/caso.conf.sample` & `caso-4.1.0.0rc1/etc/caso/caso.conf.sample`

 * *Files 4% similar despite different names*

```diff
@@ -24,20 +24,34 @@
 
 # Site name as in GOCDB. (string value)
 #site_name = <None>
 
 # Service name within the site (string value)
 #service_name = $site_name
 
-# List of projects to extract accounting records from. (list value)
-# Deprecated group/name - [DEFAULT]/tenants
+# List of projects to extract accounting records from. You can use this option,
+# or add 'caso' tag to the project in Keystone. Please refer to the
+# documentation for more details. (list value)
 #projects =
 
-# File containing the VO <-> project mapping as used in Keystone-VOMS. (string
+# Tag used to mark a project in Keystone to be extracted by cASO (string value)
+#caso_tag = caso
+
+# Property key used to get the VO name from the project properties.  (string
 # value)
+#vo_property = accounting:VO
+
+# DEPRECATED: File containing the VO <-> project mapping as used in Keystone-
+# VOMS. (string value)
+# This option is deprecated for removal.
+# Its value may be silently ignored in the future.
+# Reason: This option is marked for removal in the next release. Please see the
+# release notes, and migrate your current configuration to use the new project
+# mapping as soon as possible. If you already migrated your configuration,
+# please remove the JSON file to get rid of this message.
 #mapping_file = /etc/caso/voms.json
 
 # Extract record changes until this date. If it is not set, we use now. If a
 # server has ended after this date, it will be included, but the consuption
 # reported will end on this date. If no time zone is specified, UTC will be
 # used. (string value)
 # Deprecated group/name - [DEFAULT]/extract_to
@@ -49,16 +63,16 @@
 # If it is not set, extract records from last run. If it is set to None and
 # last run file is not present, it will extract records from the beginning of
 # time. If no time zone is specified, UTC will be used. (string value)
 # Deprecated group/name - [DEFAULT]/extract_from
 #extract_from = <None>
 
 # Which extractor to use for getting the data. If you do not specify anything,
-# nova will be used. Available choices are frozenset({'neutron', 'nova',
-# 'cinder'}) (list value)
+# nova will be used. Available choices are ['cinder', 'neutron', 'nova'] (list
+# value)
 #extractor = nova
 
 #
 # From oslo.config
 #
 
 # Path to a config file to use. Multiple config files can be specified, with
```

### Comparing `caso-4.0.1.dev1/packaging/debian/changelog` & `caso-4.1.0.0rc1/packaging/debian/changelog`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,30 @@
-python3-caso (4.0.0) stable; urgency=medium
+python3-caso (4.1.0-1) stable; urgency=medium
+
+  * [a74fb28] Remove duplicated option
+  * [1142758] Let operators mark projects directly on keystone
+  * [ce9e416] Use Keystone properties to load VO mapping.
+  * [fc039e2] Move VM status method to Nova extractor
+  * [3982e48] nova: move accelerator and benchmark options to correct place
+  * [416d2f7] extractors: move projects options to correct place
+  * [91f4e8e] Load VO mapping in correct place
+  * [8fef5fe] Move all clients to the base class
+  * [01eab94] Remove old last run file management
+  * [4f0252c] Add migrate command to ease migration
+  * [b89fbc1] Set UUID also for IP records
+  * [a8e6d5b] Provide better error message when pushing records
+  * [4bda67d] Fix noop messenger
+  * [bb8ffee] Include project names in project listing
+  * [93b9df3] Update documentation
+  * [b014846] Include caso-projects in usage commands
+  * [6aaad9d] Remove deprecated option
+
+ -- Alvaro Lopez Garcia <aloga@ifca.unican.es>  Mon, 10 Apr 2023 14:29:16 +0200
+
+python3-caso (4.0.0-1) stable; urgency=medium
 
   [ Alvaro Lopez Garcia ]
   * [2dc5334] Remove deprecated extractor base class
   * [9ebf351] Allow to configure more than one extractor
   * [5d234a1] Adapt neutron extractor code to new format
   * [9c99261] Transform records into pydantic models, and start using typing hints
   * [455053a] Include type checking with mypy
```

### Comparing `caso-4.0.1.dev1/packaging/debian/control` & `caso-4.1.0.0rc1/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/packaging/debian/copyright` & `caso-4.1.0.0rc1/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/packaging/debian/postinst` & `caso-4.1.0.0rc1/packaging/debian/postinst`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/packaging/redhat/caso.spec` & `caso-4.1.0.0rc1/packaging/redhat/caso.spec`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 Source0:      https://github.com/IFCA/caso/caso-%{version}.tar.gz
 
 BuildArch: noarch
 BuildRequires: python3-devel
 BuildRequires: python3-setuptools
 BuildRequires: python3-pbr
 BuildRequires: python3-rpm-macros
-BuildRequires: python3-tox
 Requires: python3
 Requires: python3-oslo-config
 Requires: python3-oslo-concurrency
 Requires: python3-oslo-log
 Requires: python3-oslo-utils
 Requires: python3-six
 Requires: python3-glanceclient
@@ -45,25 +44,44 @@
 %install
 %py3_install
 mv %{buildroot}/usr/etc/ %{buildroot}/etc
 
 %check
 # No tests available on py3.6, so lets use only the others. The GH action
 # build also builds on Ubuntu, that tests the other versions.
-tox -e pep8,pip-missing-reqs,bandit,pypi
 
 %files 
 %{_bindir}/caso-extract
+%{_bindir}/caso-mapping-migrate
+%{_bindir}/caso-projects
 %{python3_sitelib}/caso/
 %{python3_sitelib}/caso-%{version}*
 %config /etc/caso/caso.conf.sample
 %config /etc/caso/voms.json.sample
 %exclude /etc/caso/caso-config-generator.conf
 
 %changelog
+* Mon Apr 10 2023 Alvaro Lopez Garcia <aloga@ifca.unican.es> 4.1.0
+- Remove duplicated option
+- Let operators mark projects directly on keystone
+- Use Keystone properties to load VO mapping.
+- Move VM status method to Nova extractor
+- nova: move accelerator and benchmark options to correct place
+- extractors: move projects options to correct place
+- Load VO mapping in correct place
+- Move all clients to the base class
+- Remove old last run file management
+- Add migrate command to ease migration
+- Set UUID also for IP records
+- Provide better error message when pushing records
+- Fix noop messenger
+- Include project names in project listing
+- Update documentation
+- Include caso-projects in usage commands
+- Remove deprecated option
 * Thu Mar 20 2023 Alvaro Lopez Garcia <aloga@ifca.unican.es> 4.0.0
 - Remove deprecated extractor base class
 - Allow to configure more than one extractor
 - Adapt neutron extractor code to new format
 - Transform records into pydantic models, and start using typing hints
 - Include type checking with mypy
 - Add Cinder storage extractor
```

### Comparing `caso-4.0.1.dev1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml` & `caso-4.1.0.0rc1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml` & `caso-4.1.0.0rc1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/requirements.txt` & `caso-4.1.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/setup.cfg` & `caso-4.1.0.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 	etc/caso/ = etc/caso/*
 
 [entry_points]
 oslo.config.opts = 
 	caso = caso.opts:list_opts
 console_scripts = 
 	caso-extract = caso._cmd.extract:main
+	caso-projects = caso._cmd.projects:main
+	caso-mapping-migrate = caso._cmd.projects:migrate
 caso.extractors = 
 	nova = caso.extract.openstack.nova:NovaExtractor
 	neutron = caso.extract.openstack.neutron:NeutronExtractor
 	cinder = caso.extract.openstack.cinder:CinderExtractor
 caso.messenger = 
 	noop = caso.messenger.noop:NoopMessenger
 	ssm = caso.messenger.ssm:SSMMessenger
```

### Comparing `caso-4.0.1.dev1/setup.py` & `caso-4.1.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `caso-4.0.1.dev1/tox.ini` & `caso-4.1.0.0rc1/tox.ini`

 * *Files identical despite different names*

