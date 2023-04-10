# Comparing `tmp/scmrepo-0.2.1.tar.gz` & `tmp/scmrepo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-0.2.1.tar", last modified: Wed Apr  5 07:13:53 2023, max compression
+gzip compressed data, was "scmrepo-1.0.0.tar", last modified: Mon Apr 10 08:50:52 2023, max compression
```

## Comparing `scmrepo-0.2.1.tar` & `scmrepo-1.0.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.109128 scmrepo-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.109128 scmrepo-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-05 07:13:28.000000 scmrepo-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-05 07:13:28.000000 scmrepo-0.2.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-05 07:13:28.000000 scmrepo-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-05 07:13:28.000000 scmrepo-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-05 07:13:53.113128 scmrepo-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-05 07:13:28.000000 scmrepo-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-05 07:13:28.000000 scmrepo-0.2.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-05 07:13:28.000000 scmrepo-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-05 07:13:53.117128 scmrepo-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.105127 scmrepo-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.109128 scmrepo-0.2.1/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (123)    28907 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (123)    27543 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19779 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-05 07:13:28.000000 scmrepo-0.2.1/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-05 07:13:53.000000 scmrepo-0.2.1/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-05 07:13:53.000000 scmrepo-0.2.1/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 07:13:53.000000 scmrepo-0.2.1/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 07:13:52.000000 scmrepo-0.2.1/src/scmrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-05 07:13:53.000000 scmrepo-0.2.1/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 07:13:53.000000 scmrepo-0.2.1/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 07:13:53.113128 scmrepo-0.2.1/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-05 07:13:28.000000 scmrepo-0.2.1/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.317601 scmrepo-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-10 08:50:30.000000 scmrepo-1.0.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-10 08:50:30.000000 scmrepo-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-10 08:50:30.000000 scmrepo-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 08:50:52.317601 scmrepo-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-10 08:50:30.000000 scmrepo-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-10 08:50:30.000000 scmrepo-1.0.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-10 08:50:30.000000 scmrepo-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-10 08:50:52.317601 scmrepo-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.309601 scmrepo-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19779 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.317601 scmrepo-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.317601 scmrepo-1.0.0/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/user.key.pub
```

### Comparing `scmrepo-0.2.1/.cruft.json` & `scmrepo-1.0.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/.github/dependabot.yml` & `scmrepo-1.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/.github/workflows/release.yaml` & `scmrepo-1.0.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/.github/workflows/tests.yaml` & `scmrepo-1.0.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/.gitignore` & `scmrepo-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/.pre-commit-config.yaml` & `scmrepo-1.0.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
@@ -21,15 +21,15 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
@@ -44,12 +44,12 @@
       - id: flake8
         additional_dependencies:
           - flake8-bugbear==23.1.20
           - flake8-comprehensions==3.10.1
           - flake8-debugger==4.1.2
           - flake8-string-format==0.3.0
   - repo: https://github.com/pycqa/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
-        args: [-c, pyproject.toml]
-        additional_dependencies: ["toml"]
+        args: ["-c", "pyproject.toml"]
+        additional_dependencies: [".[toml]"]
```

### Comparing `scmrepo-0.2.1/CODE_OF_CONDUCT.rst` & `scmrepo-1.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/CONTRIBUTING.rst` & `scmrepo-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/LICENSE` & `scmrepo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/PKG-INFO` & `scmrepo-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 0.2.1
+Version: 1.0.0
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-0.2.1/README.rst` & `scmrepo-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/noxfile.py` & `scmrepo-1.0.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/pyproject.toml` & `scmrepo-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/setup.cfg` & `scmrepo-1.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 	pytest-test-utils==0.0.8
 	pytest-asyncio==0.18.3
 	pytest-docker==0.12.0; python_version < '3.10' or sys_platform != 'win32'
 	mock==5.0.1
 	paramiko==3.1.0
 	types-certifi==2021.10.8.3
 	types-mock==5.0.0.6
-	types-paramiko==3.0.0.5
+	types-paramiko==3.0.0.6
 dev = 
 	%(tests)s
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `scmrepo-0.2.1/src/scmrepo/asyn.py` & `scmrepo-1.0.0/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/base.py` & `scmrepo-1.0.0/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/exceptions.py` & `scmrepo-1.0.0/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/fs.py` & `scmrepo-1.0.0/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/git/__init__.py` & `scmrepo-1.0.0/src/scmrepo/git/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/git/backend/base.py` & `scmrepo-1.0.0/src/scmrepo/git/backend/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,20 @@
 
     @property
     @abstractmethod
     def dir(self) -> str:
         pass
 
     @abstractmethod
-    def add(self, paths: Union[str, Iterable[str]], update=False):
+    def add(
+        self,
+        paths: Union[str, Iterable[str]],
+        update: bool = False,
+        force: bool = False,
+    ):
         pass
 
     @abstractmethod
     def commit(self, msg: str, no_verify: bool = False):
         pass
 
     @abstractmethod
```

### Comparing `scmrepo-0.2.1/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from io import BytesIO, StringIO
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
+    Iterator,
     List,
     Mapping,
     Optional,
     Tuple,
     Union,
 )
 
@@ -244,25 +245,45 @@
 
         init(path, bare=bare)
 
     @property
     def dir(self) -> str:
         return self.repo.commondir()
 
-    def add(self, paths: Union[str, Iterable[str]], update=False):
+    def add(
+        self,
+        paths: Union[str, Iterable[str]],
+        update: bool = False,
+        force: bool = False,
+    ):
         assert paths or update
 
-        if isinstance(paths, str):
-            paths = [paths]
+        paths = [paths] if isinstance(paths, str) else list(paths)
 
         if update and not paths:
             self.repo.stage(list(self.repo.open_index()))
             return
 
-        files: List[bytes] = []
+        files: List[bytes] = [
+            os.fsencode(fpath) for fpath in self._expand_paths(paths, force=force)
+        ]
+        if update:
+            index = self.repo.open_index()
+            if os.name == "nt":
+                # NOTE: we need git/unix separator to compare against index
+                # paths but repo.stage() expects to be called with OS paths
+                self.repo.stage(
+                    [fname for fname in files if fname.replace(b"\\", b"/") in index]
+                )
+            else:
+                self.repo.stage([fname for fname in files if fname in index])
+        else:
+            self.repo.stage(files)
+
+    def _expand_paths(self, paths: List[str], force: bool = False) -> Iterator[str]:
         for path in paths:
             if not os.path.isabs(path) and self._submodules:
                 # NOTE: If path is inside a submodule, Dulwich expects the
                 # staged paths to be relative to the submodule root (not the
                 # parent git repo root). We append path to root_dir here so
                 # that the result of relpath(path, root_dir) is actually the
                 # path relative to the submodule root.
@@ -271,35 +292,23 @@
                     if fs_path.startswith(sm_path):
                         path = os.path.join(
                             self.root_dir,
                             relpath(fs_path, sm_path),
                         )
                         break
             if os.path.isdir(path):
-                files.extend(
-                    os.fsencode(relpath(os.path.join(root, fpath), self.root_dir))
-                    for root, _, fs in os.walk(path)
-                    for fpath in fs
-                )
-            else:
-                files.append(os.fsencode(relpath(path, self.root_dir)))
-
-        # NOTE: this doesn't check gitignore, same as GitPythonBackend.add
-        if update:
-            index = self.repo.open_index()
-            if os.name == "nt":
-                # NOTE: we need git/unix separator to compare against index
-                # paths but repo.stage() expects to be called with OS paths
-                self.repo.stage(
-                    [fname for fname in files if fname.replace(b"\\", b"/") in index]
-                )
+                for root, _, fs in os.walk(path):
+                    for fpath in fs:
+                        rel = relpath(os.path.join(root, fpath), self.root_dir)
+                        if force or not self.ignore_manager.is_ignored(rel):
+                            yield rel
             else:
-                self.repo.stage([fname for fname in files if fname in index])
-        else:
-            self.repo.stage(files)
+                rel = relpath(path, self.root_dir)
+                if force or not self.ignore_manager.is_ignored(rel):
+                    yield rel
 
     def commit(self, msg: str, no_verify: bool = False):
         from dulwich.errors import CommitError
         from dulwich.porcelain import Error, TimezoneFormatError, commit
         from dulwich.repo import InvalidUserIdentity
 
         with reraise((Error, CommitError), SCMError("Git commit failed")):
```

### Comparing `scmrepo-0.2.1/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py` & `scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/git/backend/gitpython.py` & `scmrepo-1.0.0/src/scmrepo/git/backend/gitpython.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import locale
 import logging
 import os
 import sys
 from functools import partial
 from typing import (
     TYPE_CHECKING,
+    Any,
     Callable,
     Dict,
     Iterable,
     List,
     Mapping,
     Optional,
     Tuple,
@@ -207,25 +208,37 @@
 
         return rev and git.Repo.re_hexsha_shortened.search(rev)
 
     @property
     def dir(self) -> str:
         return self.repo.git_dir
 
-    def add(self, paths: Union[str, Iterable[str]], update=False):
-        # NOTE: GitPython is not currently able to handle index version >= 3.
-        # See https://github.com/iterative/dvc/issues/610 for more details.
+    def add(
+        self,
+        paths: Union[str, Iterable[str]],
+        update: bool = False,
+        force: bool = False,
+    ):
         try:
-            if update:
+            if update or not force:
+                # NOTE: git-python index.add() defines force parameter but
+                # ignores it (index.add() behavior is always force=True)
+                kwargs: Dict[str, Any] = {}
+                if update:
+                    kwargs["update"] = True
                 if isinstance(paths, str):
                     paths = [paths]
-                self.git.add(*paths, update=True)
+                if not force:
+                    paths = [path for path in paths if not self.is_ignored(path)]
+                self.git.add(*paths, **kwargs)
             else:
                 self.repo.index.add(paths)
         except AssertionError as exc:
+            # NOTE: GitPython is not currently able to handle index version >= 3.
+            # See https://github.com/iterative/dvc/issues/610 for more details.
             raise UnsupportedIndexFormat from exc
 
     def commit(self, msg: str, no_verify: bool = False):
         from git.exc import HookExecutionError
 
         try:
             self.repo.index.commit(msg, skip_hooks=no_verify)
```

### Comparing `scmrepo-0.2.1/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,20 @@
 
         init_repository(path, bare=bare)
 
     @property
     def dir(self) -> str:
         raise NotImplementedError
 
-    def add(self, paths: Union[str, Iterable[str]], update=False):
+    def add(
+        self,
+        paths: Union[str, Iterable[str]],
+        update: bool = False,
+        force: bool = False,
+    ):
         raise NotImplementedError
 
     def commit(self, msg: str, no_verify: bool = False):
         raise NotImplementedError
 
     def checkout(
         self,
```

### Comparing `scmrepo-0.2.1/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/git/credentials.py` & `scmrepo-1.0.0/src/scmrepo/git/credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/git/objects.py` & `scmrepo-1.0.0/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/git/stash.py` & `scmrepo-1.0.0/src/scmrepo/git/stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/progress.py` & `scmrepo-1.0.0/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo/utils.py` & `scmrepo-1.0.0/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-1.0.0/src/scmrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 0.2.1
+Version: 1.0.0
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-0.2.1/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-1.0.0/src/scmrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/src/scmrepo.egg-info/requires.txt` & `scmrepo-1.0.0/src/scmrepo.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 mypy==0.971
 pytest-test-utils==0.0.8
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
-types-paramiko==3.0.0.5
+types-paramiko==3.0.0.6
 
 [dev:python_version < "3.10" or sys_platform != "win32"]
 pytest-docker==0.12.0
 
 [tests]
 pytest==7.2.0
 pytest-sugar==0.9.5
@@ -35,11 +35,11 @@
 mypy==0.971
 pytest-test-utils==0.0.8
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
-types-paramiko==3.0.0.5
+types-paramiko==3.0.0.6
 
 [tests:python_version < "3.10" or sys_platform != "win32"]
 pytest-docker==0.12.0
```

### Comparing `scmrepo-0.2.1/tests/conftest.py` & `scmrepo-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/test_credentials.py` & `scmrepo-1.0.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/test_dulwich.py` & `scmrepo-1.0.0/tests/test_dulwich.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/test_fs.py` & `scmrepo-1.0.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/test_git.py` & `scmrepo-1.0.0/tests/test_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,14 +665,30 @@
     git.add(["dir"], update=True)
     staged, unstaged, _ = scm.status()
     assert set(staged["modify"]) == {"dir/baz"}
     assert len(unstaged) == 1
     assert len(untracked) == 1
 
 
+@pytest.mark.skip_git_backend("pygit2")
+def test_add_force(tmp_dir: TmpDir, scm: Git, git: Git):
+    tmp_dir.gen({"foo": "foo", "bar": "bar", "dir": {"baz": "baz"}})
+    tmp_dir.gen({".gitignore": "foo\ndir/"})
+
+    git.add(["foo", "bar", "dir"])
+    staged, _unstaged, untracked = scm.status()
+    assert set(staged["add"]) == {"bar"}
+    assert set(untracked) == {".gitignore"}
+
+    git.add(["foo", "bar", "dir"], force=True)
+    staged, _unstaged, untracked = scm.status()
+    assert set(staged["add"]) == {"foo", "bar", "dir/baz"}
+    assert set(untracked) == {".gitignore"}
+
+
 @pytest.mark.skip_git_backend("dulwich", "gitpython")
 def test_checkout_subdir(tmp_dir: TmpDir, scm: Git, git: Git):
     tmp_dir.gen("foo", "foo")
     scm.add_commit("foo", message="init")
     rev = scm.get_rev()
 
     tmp_dir.gen({"dir": {"bar": "bar"}})
```

### Comparing `scmrepo-0.2.1/tests/test_noscm.py` & `scmrepo-1.0.0/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/test_pygit2.py` & `scmrepo-1.0.0/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/test_scmrepo.py` & `scmrepo-1.0.0/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/test_stash.py` & `scmrepo-1.0.0/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-0.2.1/tests/user.key` & `scmrepo-1.0.0/tests/user.key`

 * *Files identical despite different names*

