# Comparing `tmp/caso-4.1.0.0rc2.tar.gz` & `tmp/caso-4.1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caso-4.1.0.0rc2.tar", last modified: Mon Apr 10 14:45:11 2023, max compression
+gzip compressed data, was "caso-4.1.1.0rc1.tar", last modified: Mon Apr 10 20:41:03 2023, max compression
```

## Comparing `caso-4.1.0.0rc2.tar` & `caso-4.1.1.0rc1.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.471928 caso-4.1.0.0rc2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.github/workflows/packaging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.stestr.conf
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.testr.conf
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso/_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/_cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/_cmd/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/_cmd/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso/extract/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/openstack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/openstack/cinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/extract/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/keystone_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso/messenger/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/messenger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/messenger/logstash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/messenger/noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/messenger/ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/opts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso/tests/extract/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/tests/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/tests/extract/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/tests/extract/test_nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/caso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/caso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 14:45:11.000000 caso-4.1.0.0rc2/caso.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.475928 caso-4.1.0.0rc2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/doc/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2980 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/configuration-file.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/multi-region.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)    58956 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/static/caso-diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)   111404 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/static/caso-diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/static/caso.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/static/caso.png
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/doc/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.471928 caso-4.1.0.0rc2/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/etc/caso/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/etc/caso/caso-config-generator.conf
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/etc/caso/caso.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/etc/caso/voms.json.sample
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.471928 caso-4.1.0.0rc2/packaging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/packaging/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/README.Debian
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/clean
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/cron.hourly
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/gbp.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/postinst
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/packaging/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/debian/source/format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/packaging/redhat/
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/packaging/redhat/caso.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.471928 caso-4.1.0.0rc2/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/default-to-all-extractors-0da9448a00091bc1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/support-for-storage-34675eff431608d1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/releasenotes/notes/tags-for-projects-3b9b6b5a92bcc6df.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-10 14:45:11.479928 caso-4.1.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-10 14:44:57.000000 caso-4.1.0.0rc2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.246920 caso-4.1.1.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.246920 caso-4.1.1.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.stestr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.testr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.246920 caso-4.1.1.0rc1/caso/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/_cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/_cmd/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/_cmd/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/extract/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/cinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/keystone_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/messenger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/logstash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/extract/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/extract/test_nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/doc/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2980 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/configuration-file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/multi-region.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    58956 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso-diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)   111404 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso-diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.242920 caso-4.1.1.0rc1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/etc/caso/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/etc/caso/caso-config-generator.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/etc/caso/caso.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/etc/caso/voms.json.sample
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.242920 caso-4.1.1.0rc1/packaging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/packaging/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/README.Debian
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/clean
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/cron.hourly
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/gbp.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/postinst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/packaging/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/packaging/redhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/redhat/caso.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.242920 caso-4.1.1.0rc1/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/default-to-all-extractors-0da9448a00091bc1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/require-system-scope-67d0d11681beea27.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/support-for-storage-34675eff431608d1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/tags-for-projects-3b9b6b5a92bcc6df.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/tox.ini
```

### Comparing `caso-4.1.0.0rc2/.github/PULL_REQUEST_TEMPLATE.md` & `caso-4.1.1.0rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/.github/workflows/packaging.yml` & `caso-4.1.1.0rc1/.github/workflows/packaging.yml`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/.github/workflows/python-publish.yml` & `caso-4.1.1.0rc1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/.github/workflows/python-test.yml` & `caso-4.1.1.0rc1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/.readthedocs.yml` & `caso-4.1.1.0rc1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/CODE_OF_CONDUCT.md` & `caso-4.1.1.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/CONTRIBUTING.md` & `caso-4.1.1.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/LICENSE` & `caso-4.1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/PKG-INFO` & `caso-4.1.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caso
-Version: 4.1.0.0rc2
+Version: 4.1.1.0rc1
 Summary: cASO is an OpenStack Accounting extractor.
 Home-page: http://github.com/IFCA/caso
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/IFCA/caso/issues
 Project-URL: Documentation, https://caso.readthedocs.io/
```

### Comparing `caso-4.1.0.0rc2/README.md` & `caso-4.1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/__init__.py` & `caso-4.1.1.0rc1/caso/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/_cmd/extract.py` & `caso-4.1.1.0rc1/caso/_cmd/extract.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/_cmd/projects.py` & `caso-4.1.1.0rc1/caso/_cmd/projects.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/config.py` & `caso-4.1.1.0rc1/caso/config.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/exception.py` & `caso-4.1.1.0rc1/caso/exception.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/extract/__init__.py` & `caso-4.1.1.0rc1/caso/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/extract/base.py` & `caso-4.1.1.0rc1/caso/extract/base.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/extract/manager.py` & `caso-4.1.1.0rc1/caso/extract/manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/extract/openstack/__init__.py` & `caso-4.1.1.0rc1/caso/extract/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/extract/openstack/base.py` & `caso-4.1.1.0rc1/caso/extract/openstack/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def _get_keystone_session(self):
         """Get a Keystone session for the configured project in the object."""
         session = keystone_client.get_session(CONF, self.project)
         return session
 
     def _get_keystone_client(self):
         """Get a Keystone Client for the configured project in the object."""
-        client = keystone_client.get_client(CONF, self.project)
+        client = keystone_client.get_client(CONF, system_scope="all")
         return client
 
     def _get_cinder_client(self):
         """Get Cinder client with keystone session."""
         session = self._get_keystone_session()
         return cinderclient.v3.client.Client(session=session)
 
@@ -122,19 +122,19 @@
 
     def _get_keystone_user(self, uuid):
         """Get the Keystone username for a given uuid."""
         try:
             user = self.keystone.users.get(user=uuid)
             return user.name
         except keystoneauth1.exceptions.http.Forbidden as e:
-            LOG.error("Unauthorized to get user")
+            LOG.error(f"Unauthorized to get user {uuid}")
             LOG.exception(e)
             return None
         except Exception as e:
-            LOG.debug("Exception while getting user")
+            LOG.debug(f"Exception while getting user {uuid}")
             LOG.exception(e)
             return None
 
     # FIXME(aloga): this has to go inside a record
     @staticmethod
     def _get_measure_time():
         """Get current measurement time."""
```

### Comparing `caso-4.1.0.0rc2/caso/extract/openstack/cinder.py` & `caso-4.1.1.0rc1/caso/extract/openstack/cinder.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/extract/openstack/neutron.py` & `caso-4.1.1.0rc1/caso/extract/openstack/neutron.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/extract/openstack/nova.py` & `caso-4.1.1.0rc1/caso/extract/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/keystone_client.py` & `caso-4.1.1.0rc1/caso/keystone_client.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/loading.py` & `caso-4.1.1.0rc1/caso/loading.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/manager.py` & `caso-4.1.1.0rc1/caso/manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/messenger/__init__.py` & `caso-4.1.1.0rc1/caso/messenger/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/messenger/logstash.py` & `caso-4.1.1.0rc1/caso/messenger/logstash.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/messenger/noop.py` & `caso-4.1.1.0rc1/caso/messenger/noop.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/messenger/ssm.py` & `caso-4.1.1.0rc1/caso/messenger/ssm.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/opts.py` & `caso-4.1.1.0rc1/caso/opts.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/record.py` & `caso-4.1.1.0rc1/caso/record.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/tests/base.py` & `caso-4.1.1.0rc1/caso/tests/base.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/tests/extract/test_manager.py` & `caso-4.1.1.0rc1/caso/tests/extract/test_manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/tests/extract/test_nova.py` & `caso-4.1.1.0rc1/caso/tests/extract/test_nova.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/tests/test_manager.py` & `caso-4.1.1.0rc1/caso/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso/utils.py` & `caso-4.1.1.0rc1/caso/utils.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/caso.egg-info/PKG-INFO` & `caso-4.1.1.0rc1/caso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caso
-Version: 4.1.0.0rc2
+Version: 4.1.1.0rc1
 Summary: cASO is an OpenStack Accounting extractor.
 Home-page: http://github.com/IFCA/caso
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/IFCA/caso/issues
 Project-URL: Documentation, https://caso.readthedocs.io/
```

### Comparing `caso-4.1.0.0rc2/caso.egg-info/SOURCES.txt` & `caso-4.1.1.0rc1/caso.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -93,9 +93,10 @@
 releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
 releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
 releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
 releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
 releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
 releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
 releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
+releasenotes/notes/require-system-scope-67d0d11681beea27.yaml
 releasenotes/notes/support-for-storage-34675eff431608d1.yaml
 releasenotes/notes/tags-for-projects-3b9b6b5a92bcc6df.yaml
```

### Comparing `caso-4.1.0.0rc2/caso.egg-info/entry_points.txt` & `caso-4.1.1.0rc1/caso.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/conf.py` & `caso-4.1.1.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/configuration.rst` & `caso-4.1.1.0rc1/doc/source/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,16 @@
 a default OpenStack Keystone role). Otherwise, ``cASO`` will not be able to get the
 usages and will fail::
 
     openstack user create --password <password> accounting
     # For each of the projects, add the user with the accounting role
     openstack role add --user accounting --project <project> reader
 
-Moreover, if you wish to gather the list of projects that ``cASO`` should use directly
-from OpenStack, you need to grant the user the role reader with a system scope of
-``all``::
+Moreover, you need to grant the user the role reader with a system scope of ``all`` in
+order to get all the project tags, as well as the other user's information::
 
     openstack role add --system all --user accounting reader
 
 Policy modifications
 ------------------------
 
 .. important:: No policy modifications are needed
```

### Comparing `caso-4.1.0.0rc2/doc/source/index.rst` & `caso-4.1.1.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/installation.rst` & `caso-4.1.1.0rc1/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/multi-region.rst` & `caso-4.1.1.0rc1/doc/source/multi-region.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/static/caso-diagram.drawio` & `caso-4.1.1.0rc1/doc/source/static/caso-diagram.drawio`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/static/caso-diagram.png` & `caso-4.1.1.0rc1/doc/source/static/caso-diagram.png`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/static/caso.conf.sample` & `caso-4.1.1.0rc1/doc/source/static/caso.conf.sample`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/static/caso.png` & `caso-4.1.1.0rc1/doc/source/static/caso.png`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/troubleshooting.rst` & `caso-4.1.1.0rc1/doc/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/doc/source/usage.rst` & `caso-4.1.1.0rc1/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/etc/caso/caso.conf.sample` & `caso-4.1.1.0rc1/etc/caso/caso.conf.sample`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/packaging/debian/changelog` & `caso-4.1.1.0rc1/packaging/debian/changelog`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/packaging/debian/control` & `caso-4.1.1.0rc1/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/packaging/debian/copyright` & `caso-4.1.1.0rc1/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/packaging/debian/postinst` & `caso-4.1.1.0rc1/packaging/debian/postinst`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/packaging/redhat/caso.spec` & `caso-4.1.1.0rc1/packaging/redhat/caso.spec`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml` & `caso-4.1.1.0rc1/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml` & `caso-4.1.1.0rc1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml` & `caso-4.1.1.0rc1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/requirements.txt` & `caso-4.1.1.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/setup.cfg` & `caso-4.1.1.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/setup.py` & `caso-4.1.1.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.0.0rc2/tox.ini` & `caso-4.1.1.0rc1/tox.ini`

 * *Files identical despite different names*

