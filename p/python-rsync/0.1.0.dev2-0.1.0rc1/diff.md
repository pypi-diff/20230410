# Comparing `tmp/python-rsync-0.1.0.dev2.tar.gz` & `tmp/python-rsync-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-rsync-0.1.0.dev2.tar", last modified: Sat Aug 27 17:58:27 2022, max compression
+gzip compressed data, was "python-rsync-0.1.0rc1.tar", last modified: Mon Oct 31 06:43:26 2022, max compression
```

## Comparing `python-rsync-0.1.0.dev2.tar` & `python-rsync-0.1.0rc1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/README.markdown
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/dep/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/dep/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/base64.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/dep/src/blake2/
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/blake2/blake2-impl.h
--rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/blake2/blake2.h
--rw-r--r--   0 runner    (1001) docker     (121)    10057 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/blake2/blake2b-ref.c
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/buf.c
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/buf.h
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/checksum.c
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/checksum.h
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/command.c
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/command.h
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-08-27 17:58:11.000000 python-rsync-0.1.0.dev2/dep/src/config.h
--rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/config.h.in
--rw-r--r--   0 runner    (1001) docker     (121)    15991 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/delta.c
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/emit.c
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/emit.h
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/fileutil.c
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/hashtable.c
--rw-r--r--   0 runner    (1001) docker     (121)    13155 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/hashtable.h
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/hex.c
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/isprefix.c
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/isprefix.h
--rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/job.c
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/job.h
--rw-r--r--   0 runner    (1001) docker     (121)    23755 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/librsync.h
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/librsync_export.h
--rw-r--r--   0 runner    (1001) docker     (121)     9656 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/mdfour.c
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/mdfour.h
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/mksum.c
--rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/msg.c
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/netint.c
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/netint.h
--rw-r--r--   0 runner    (1001) docker     (121)     7479 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/patch.c
--rw-r--r--   0 runner    (1001) docker     (121)    19037 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/prototab.c
--rw-r--r--   0 runner    (1001) docker     (121)     9523 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/prototab.h
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/rabinkarp.c
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/rabinkarp.h
--rw-r--r--   0 runner    (1001) docker     (121)    11398 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/rdiff.c
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/rdiff.magic
--rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/readsums.c
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/rollsum.c
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/rollsum.h
--rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/scoop.c
--rw-r--r--   0 runner    (1001) docker     (121)     7277 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/scoop.h
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/stats.c
--rw-r--r--   0 runner    (1001) docker     (121)    11717 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/sumset.c
--rw-r--r--   0 runner    (1001) docker     (121)     5878 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/sumset.h
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/trace.c
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/trace.h
--rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/tube.c
--rw-r--r--   0 runner    (1001) docker     (121)     2333 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/util.c
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/util.h
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/version.c
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/whole.c
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/dep/src/whole.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/pyrsync/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/pyrsync/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cffi/
--rw-r--r--   0 runner    (1001) docker     (121)     8392 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26292 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cffi/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cffi/cbarg.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cython/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   464562 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cython/_rsync_cy.c
--rw-r--r--   0 runner    (1001) docker     (121)    10887 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cython/_rsync_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/pyrsync/backends/cython/rsync.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/python_rsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/python_rsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/python_rsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/python_rsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/python_rsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/python_rsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/python_rsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 17:58:27.000000 python-rsync-0.1.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4443 2022-08-27 17:58:08.000000 python-rsync-0.1.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/README.markdown
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.080430 python-rsync-0.1.0rc1/dep/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/dep/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/base64.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/dep/src/blake2/
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/blake2/blake2-impl.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/blake2/blake2.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10057 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/blake2/blake2b-ref.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/buf.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/buf.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/checksum.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/checksum.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/command.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/command.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-10-31 06:43:08.000000 python-rsync-0.1.0rc1/dep/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (121)    15991 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/delta.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/emit.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/emit.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/fileutil.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/hashtable.c
+-rw-r--r--   0 runner    (1001) docker     (121)    13155 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/hashtable.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/hex.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/isprefix.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/isprefix.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/job.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/job.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23755 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/librsync.h
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/librsync_export.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9656 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/mdfour.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/mdfour.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/mksum.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/msg.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/netint.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/netint.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7479 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/patch.c
+-rw-r--r--   0 runner    (1001) docker     (121)    19037 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/prototab.c
+-rw-r--r--   0 runner    (1001) docker     (121)     9523 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/prototab.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/rabinkarp.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/rabinkarp.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11398 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/rdiff.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/rdiff.magic
+-rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/readsums.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/rollsum.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/rollsum.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/scoop.c
+-rw-r--r--   0 runner    (1001) docker     (121)     7277 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/scoop.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/stats.c
+-rw-r--r--   0 runner    (1001) docker     (121)    11717 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/sumset.c
+-rw-r--r--   0 runner    (1001) docker     (121)     5878 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/sumset.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/trace.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/trace.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/tube.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2333 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/util.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/util.h
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/version.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/whole.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-10-31 06:43:05.000000 python-rsync-0.1.0rc1/dep/src/whole.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/pyrsync/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/pyrsync/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/pyrsync/backends/cffi/
+-rw-r--r--   0 runner    (1001) docker     (121)     8387 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/backends/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26287 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/backends/cffi/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/backends/cffi/cbarg.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/pyrsync/backends/cython/
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/backends/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   459318 2022-10-31 06:43:25.000000 python-rsync-0.1.0rc1/pyrsync/backends/cython/_rsync.c
+-rw-r--r--   0 runner    (1001) docker     (121)    10939 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/backends/cython/_rsync.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     6883 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/pyrsync/backends/cython/rsync.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/python_rsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-10-31 06:43:26.000000 python-rsync-0.1.0rc1/python_rsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-10-31 06:43:26.000000 python-rsync-0.1.0rc1/python_rsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 06:43:26.000000 python-rsync-0.1.0rc1/python_rsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 06:43:26.000000 python-rsync-0.1.0rc1/python_rsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-31 06:43:26.000000 python-rsync-0.1.0rc1/python_rsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-31 06:43:26.000000 python-rsync-0.1.0rc1/python_rsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 06:43:26.088431 python-rsync-0.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-10-31 06:43:04.000000 python-rsync-0.1.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-rsync-0.1.0.dev2/PKG-INFO` & `python-rsync-0.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rsync
-Version: 0.1.0.dev2
+Version: 0.1.0rc1
 Summary: python binding for librsync
 Home-page: https://github.com/synodriver/pyrsync
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: compress,decompress
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-rsync-0.1.0.dev2/README.markdown` & `python-rsync-0.1.0rc1/README.markdown`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/base64.c` & `python-rsync-0.1.0rc1/dep/src/base64.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/blake2/blake2-impl.h` & `python-rsync-0.1.0rc1/dep/src/blake2/blake2-impl.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/blake2/blake2.h` & `python-rsync-0.1.0rc1/dep/src/blake2/blake2.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/blake2/blake2b-ref.c` & `python-rsync-0.1.0rc1/dep/src/blake2/blake2b-ref.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/buf.c` & `python-rsync-0.1.0rc1/dep/src/buf.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/buf.h` & `python-rsync-0.1.0rc1/dep/src/buf.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/checksum.c` & `python-rsync-0.1.0rc1/dep/src/checksum.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/checksum.h` & `python-rsync-0.1.0rc1/dep/src/checksum.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/command.c` & `python-rsync-0.1.0rc1/dep/src/command.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/command.h` & `python-rsync-0.1.0rc1/dep/src/command.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/config.h` & `python-rsync-0.1.0rc1/dep/src/config.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/config.h.in` & `python-rsync-0.1.0rc1/dep/src/config.h.in`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/delta.c` & `python-rsync-0.1.0rc1/dep/src/delta.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/emit.c` & `python-rsync-0.1.0rc1/dep/src/emit.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/emit.h` & `python-rsync-0.1.0rc1/dep/src/emit.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/fileutil.c` & `python-rsync-0.1.0rc1/dep/src/fileutil.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/hashtable.c` & `python-rsync-0.1.0rc1/dep/src/hashtable.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/hashtable.h` & `python-rsync-0.1.0rc1/dep/src/hashtable.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/hex.c` & `python-rsync-0.1.0rc1/dep/src/hex.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/isprefix.c` & `python-rsync-0.1.0rc1/dep/src/isprefix.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/isprefix.h` & `python-rsync-0.1.0rc1/dep/src/isprefix.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/job.c` & `python-rsync-0.1.0rc1/dep/src/job.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/job.h` & `python-rsync-0.1.0rc1/dep/src/job.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/librsync.h` & `python-rsync-0.1.0rc1/dep/src/librsync.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/mdfour.c` & `python-rsync-0.1.0rc1/dep/src/mdfour.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/mdfour.h` & `python-rsync-0.1.0rc1/dep/src/mdfour.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/mksum.c` & `python-rsync-0.1.0rc1/dep/src/mksum.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/msg.c` & `python-rsync-0.1.0rc1/dep/src/msg.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/netint.c` & `python-rsync-0.1.0rc1/dep/src/netint.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/netint.h` & `python-rsync-0.1.0rc1/dep/src/netint.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/patch.c` & `python-rsync-0.1.0rc1/dep/src/patch.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/prototab.c` & `python-rsync-0.1.0rc1/dep/src/prototab.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/prototab.h` & `python-rsync-0.1.0rc1/dep/src/prototab.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/rabinkarp.c` & `python-rsync-0.1.0rc1/dep/src/rabinkarp.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/rabinkarp.h` & `python-rsync-0.1.0rc1/dep/src/rabinkarp.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/rdiff.c` & `python-rsync-0.1.0rc1/dep/src/rdiff.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/rdiff.magic` & `python-rsync-0.1.0rc1/dep/src/rdiff.magic`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/readsums.c` & `python-rsync-0.1.0rc1/dep/src/readsums.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/rollsum.c` & `python-rsync-0.1.0rc1/dep/src/rollsum.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/rollsum.h` & `python-rsync-0.1.0rc1/dep/src/rollsum.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/scoop.c` & `python-rsync-0.1.0rc1/dep/src/scoop.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/scoop.h` & `python-rsync-0.1.0rc1/dep/src/scoop.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/stats.c` & `python-rsync-0.1.0rc1/dep/src/stats.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/sumset.c` & `python-rsync-0.1.0rc1/dep/src/sumset.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/sumset.h` & `python-rsync-0.1.0rc1/dep/src/sumset.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/trace.c` & `python-rsync-0.1.0rc1/dep/src/trace.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/trace.h` & `python-rsync-0.1.0rc1/dep/src/trace.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/tube.c` & `python-rsync-0.1.0rc1/dep/src/tube.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/util.c` & `python-rsync-0.1.0rc1/dep/src/util.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/util.h` & `python-rsync-0.1.0rc1/dep/src/util.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/version.c` & `python-rsync-0.1.0rc1/dep/src/version.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/whole.c` & `python-rsync-0.1.0rc1/dep/src/whole.c`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/dep/src/whole.h` & `python-rsync-0.1.0rc1/dep/src/whole.h`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/pyrsync/backends/__init__.py` & `python-rsync-0.1.0rc1/pyrsync/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `python-rsync-0.1.0.dev2/pyrsync/backends/cffi/__init__.py` & `python-rsync-0.1.0rc1/pyrsync/backends/cffi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Copyright (c) 2008-2021 synodriver <synodriver@gmail.com>
 """
-from pyrsync.backends.cffi._rsync_cffi import ffi, lib
+from pyrsync.backends.cffi._rsync import ffi, lib
 
 
 class LibrsyncError(Exception):
     def __init__(self, result):
         self.code = result
 
     def __str__(self):
```

### Comparing `python-rsync-0.1.0.dev2/pyrsync/backends/cffi/build.py` & `python-rsync-0.1.0rc1/pyrsync/backends/cffi/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -722,15 +722,15 @@
 #include <stdlib.h>
 #include <time.h>
 #include "job.h"
 #include "librsync.h"
 #include "cbarg.h"
 """
 ffibuilder.set_source(
-    "pyrsync.backends.cffi._rsync_cffi",
+    "pyrsync.backends.cffi._rsync",
     source,
     sources=c_src,
     include_dirs=["./dep/src", "./dep/src/blake2", "./pyrsync/backends/cffi"],
     define_macros=[("rsync_EXPORTS", None)],
 )
 
 if __name__ == "__main__":
```

### Comparing `python-rsync-0.1.0.dev2/pyrsync/backends/cython/_rsync_cy.c` & `python-rsync-0.1.0rc1/pyrsync/backends/cython/_rsync.c`

 * *Files 3% similar despite different names*

```diff
@@ -13,49 +13,49 @@
             "dep/src/job.h",
             "dep/src/librsync.h"
         ],
         "include_dirs": [
             "./dep/src",
             "./dep/src/blake2"
         ],
-        "name": "pyrsync.backends.cython._rsync_cy",
+        "name": "pyrsync.backends.cython._rsync",
         "sources": [
-            "pyrsync/backends/cython/_rsync_cy.pyx",
-            "./dep/src/netint.c",
+            "pyrsync/backends/cython/_rsync.pyx",
+            "./dep/src/version.c",
+            "./dep/src/sumset.c",
+            "./dep/src/trace.c",
+            "./dep/src/msg.c",
             "./dep/src/mdfour.c",
+            "./dep/src/checksum.c",
+            "./dep/src/scoop.c",
+            "./dep/src/prototab.c",
+            "./dep/src/buf.c",
+            "./dep/src/stats.c",
+            "./dep/src/rollsum.c",
+            "./dep/src/delta.c",
+            "./dep/src/emit.c",
             "./dep/src/isprefix.c",
             "./dep/src/fileutil.c",
-            "./dep/src/patch.c",
-            "./dep/src/hex.c",
-            "./dep/src/trace.c",
+            "./dep/src/command.c",
+            "./dep/src/mksum.c",
             "./dep/src/tube.c",
-            "./dep/src/delta.c",
-            "./dep/src/readsums.c",
-            "./dep/src/stats.c",
-            "./dep/src/sumset.c",
-            "./dep/src/hashtable.c",
-            "./dep/src/emit.c",
-            "./dep/src/buf.c",
             "./dep/src/whole.c",
-            "./dep/src/version.c",
             "./dep/src/util.c",
-            "./dep/src/rollsum.c",
             "./dep/src/base64.c",
-            "./dep/src/job.c",
-            "./dep/src/checksum.c",
-            "./dep/src/msg.c",
-            "./dep/src/mksum.c",
-            "./dep/src/command.c",
-            "./dep/src/prototab.c",
+            "./dep/src/hex.c",
+            "./dep/src/hashtable.c",
+            "./dep/src/netint.c",
+            "./dep/src/patch.c",
+            "./dep/src/readsums.c",
             "./dep/src/rabinkarp.c",
-            "./dep/src/scoop.c",
+            "./dep/src/job.c",
             "./dep/src/blake2/blake2b-ref.c"
         ]
     },
-    "module_name": "pyrsync.backends.cython._rsync_cy"
+    "module_name": "pyrsync.backends.cython._rsync"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
@@ -789,16 +789,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__pyrsync__backends__cython___rsync_cy
-#define __PYX_HAVE_API__pyrsync__backends__cython___rsync_cy
+#define __PYX_HAVE__pyrsync__backends__cython___rsync
+#define __PYX_HAVE_API__pyrsync__backends__cython___rsync
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include <stdint.h>
 #include <stddef.h>
 #include <time.h>
 #include "librsync.h"
@@ -1009,15 +1009,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "stringsource",
-  "pyrsync/backends/cython/_rsync_cy.pyx",
+  "pyrsync/backends/cython/_rsync.pyx",
   "type.pxd",
 };
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
@@ -1026,135 +1026,135 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
 /*--- Type declarations ---*/
-struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats;
-struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job;
-struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute;
-struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args;
-struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_signature;
-struct __pyx_t_7pyrsync_8backends_6cython_9_rsync_cy_input_args;
+struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats;
+struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job;
+struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute;
+struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_get_signature_args;
+struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_signature;
+struct __pyx_t_7pyrsync_8backends_6cython_6_rsync_input_args;
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":170
+/* "pyrsync/backends/cython/_rsync.pyx":171
  *         return Stats.from_ptr(state)
  * 
  *     cpdef inline int execute(self, object input, object output = None) except -1:             # <<<<<<<<<<<<<<
  *         if not PyFile_Check(input):
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  */
-struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute {
+struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute {
   int __pyx_n;
   PyObject *output;
 };
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":215
+/* "pyrsync/backends/cython/_rsync.pyx":216
  *         self.job = NULL
  * 
  * cpdef inline tuple get_signature_args(rs_long_t old_fsize, int magic = 0, size_t block_len = 0, size_t strong_len= 0):             # <<<<<<<<<<<<<<
  *     cdef:
  *         rs_result result
  */
-struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args {
+struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_get_signature_args {
   int __pyx_n;
   int magic;
   size_t block_len;
   size_t strong_len;
 };
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":226
+/* "pyrsync/backends/cython/_rsync.pyx":227
  *     return c_magic, block_len, strong_len
  * 
  * cpdef inline signature(object input, object output, size_t strong_len, rs_magic_number sig_magic,             # <<<<<<<<<<<<<<
  *                            size_t block_size=RS_DEFAULT_BLOCK_LEN):
  *     """
  */
-struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_signature {
+struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_signature {
   int __pyx_n;
   size_t block_size;
 };
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":272
+/* "pyrsync/backends/cython/_rsync.pyx":273
  *         rs_free_sumset(sig)
  * 
  * cdef struct input_args:             # <<<<<<<<<<<<<<
  *     PyObject *file
  *     char* buffer
  */
-struct __pyx_t_7pyrsync_8backends_6cython_9_rsync_cy_input_args {
+struct __pyx_t_7pyrsync_8backends_6cython_6_rsync_input_args {
   PyObject *file;
   char *buffer;
   Py_ssize_t len;
 };
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":85
+/* "pyrsync/backends/cython/_rsync.pyx":85
  * @cython.final
  * @cython.no_gc
  * cdef class Stats:             # <<<<<<<<<<<<<<
  *     cdef rs_stats_t * state
  * 
  */
-struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats {
+struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats {
   PyObject_HEAD
-  struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_vtab;
+  struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_vtab;
   rs_stats_t *state;
 };
 
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":151
- * @cython.final
+/* "pyrsync/backends/cython/_rsync.pyx":152
  * @cython.no_gc
+ * @cython.internal
  * cdef class Job:             # <<<<<<<<<<<<<<
  *     cdef  rs_job_t * job
  * 
  */
-struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job {
+struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job {
   PyObject_HEAD
-  struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_vtab;
+  struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_vtab;
   rs_job_t *job;
 };
 
 
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":85
+/* "pyrsync/backends/cython/_rsync.pyx":85
  * @cython.final
  * @cython.no_gc
  * cdef class Stats:             # <<<<<<<<<<<<<<
  *     cdef rs_stats_t * state
  * 
  */
 
-struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Stats {
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *(*from_ptr)(rs_stats_t *);
+struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Stats {
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *(*from_ptr)(rs_stats_t *);
 };
-static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Stats;
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_from_ptr(rs_stats_t *);
+static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Stats;
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_f_7pyrsync_8backends_6cython_6_rsync_5Stats_from_ptr(rs_stats_t *);
 
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":151
- * @cython.final
+/* "pyrsync/backends/cython/_rsync.pyx":152
  * @cython.no_gc
+ * @cython.internal
  * cdef class Job:             # <<<<<<<<<<<<<<
  *     cdef  rs_job_t * job
  * 
  */
 
-struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Job {
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *(*from_ptr)(rs_job_t *);
-  rs_result (*iter)(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, rs_buffers_t *);
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *(*statistics)(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, int __pyx_skip_dispatch);
-  int (*execute)(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute *__pyx_optional_args);
+struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Job {
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *(*from_ptr)(rs_job_t *);
+  rs_result (*iter)(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, rs_buffers_t *);
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *(*statistics)(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, int __pyx_skip_dispatch);
+  int (*execute)(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute *__pyx_optional_args);
 };
-static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Job;
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr(rs_job_t *);
-static CYTHON_INLINE rs_result __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_iter(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, rs_buffers_t *);
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, int __pyx_skip_dispatch);
-static CYTHON_INLINE int __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute *__pyx_optional_args);
+static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Job;
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr(rs_job_t *);
+static CYTHON_INLINE rs_result __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_iter(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, rs_buffers_t *);
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, int __pyx_skip_dispatch);
+static CYTHON_INLINE int __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute *__pyx_optional_args);
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1454,22 +1454,14 @@
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
 #define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
 #define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
 #endif
 
-/* ReRaiseException.proto */
-static CYTHON_INLINE void __Pyx_ReraiseException(void);
-
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
-
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
@@ -1666,19 +1658,19 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_from_ptr(rs_stats_t *__pyx_v_state); /* proto*/
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr(rs_job_t *__pyx_v_job); /* proto*/
-static CYTHON_INLINE rs_result __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_iter(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, rs_buffers_t *__pyx_v_buffer); /* proto*/
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch); /* proto*/
-static CYTHON_INLINE int __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, PyObject *__pyx_v_input, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute *__pyx_optional_args); /* proto*/
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_f_7pyrsync_8backends_6cython_6_rsync_5Stats_from_ptr(rs_stats_t *__pyx_v_state); /* proto*/
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr(rs_job_t *__pyx_v_job); /* proto*/
+static CYTHON_INLINE rs_result __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_iter(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, rs_buffers_t *__pyx_v_buffer); /* proto*/
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch); /* proto*/
+static CYTHON_INLINE int __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, PyObject *__pyx_v_input, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute *__pyx_optional_args); /* proto*/
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'libc.string' */
 
 /* Module declarations from 'libc.stdio' */
 
@@ -1699,31 +1691,30 @@
 
 /* Module declarations from 'libc.stddef' */
 
 /* Module declarations from 'libc.time' */
 
 /* Module declarations from 'pyrsync.backends.cython.rsync' */
 
-/* Module declarations from 'pyrsync.backends.cython._rsync_cy' */
-static PyTypeObject *__pyx_ptype_7pyrsync_8backends_6cython_9_rsync_cy_Stats = 0;
-static PyTypeObject *__pyx_ptype_7pyrsync_8backends_6cython_9_rsync_cy_Job = 0;
-static CYTHON_INLINE uint8_t __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_PyFile_Check(PyObject *); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args(rs_long_t, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args *__pyx_optional_args); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_signature(PyObject *, PyObject *, size_t, rs_magic_number, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_signature *__pyx_optional_args); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_delta(PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
-static rs_result __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_read_cb(void *, rs_long_t, size_t *, void **); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_patch(PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
-#define __Pyx_MODULE_NAME "pyrsync.backends.cython._rsync_cy"
-extern int __pyx_module_is_main_pyrsync__backends__cython___rsync_cy;
-int __pyx_module_is_main_pyrsync__backends__cython___rsync_cy = 0;
+/* Module declarations from 'pyrsync.backends.cython._rsync' */
+static PyTypeObject *__pyx_ptype_7pyrsync_8backends_6cython_6_rsync_Stats = 0;
+static PyTypeObject *__pyx_ptype_7pyrsync_8backends_6cython_6_rsync_Job = 0;
+static CYTHON_INLINE uint8_t __pyx_f_7pyrsync_8backends_6cython_6_rsync_PyFile_Check(PyObject *); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_get_signature_args(rs_long_t, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_get_signature_args *__pyx_optional_args); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_signature(PyObject *, PyObject *, size_t, rs_magic_number, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_signature *__pyx_optional_args); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_delta(PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
+static rs_result __pyx_f_7pyrsync_8backends_6cython_6_rsync_read_cb(void *, rs_long_t, size_t *, void **); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_patch(PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
+#define __Pyx_MODULE_NAME "pyrsync.backends.cython._rsync"
+extern int __pyx_module_is_main_pyrsync__backends__cython___rsync;
+int __pyx_module_is_main_pyrsync__backends__cython___rsync = 0;
 
-/* Implementation of 'pyrsync.backends.cython._rsync_cy' */
+/* Implementation of 'pyrsync.backends.cython._rsync' */
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_MemoryError;
-static const char __pyx_k_Job[] = "Job";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_str[] = "__str__";
 static const char __pyx_k_code[] = "code";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_read[] = "read";
@@ -1774,21 +1765,20 @@
 static const char __pyx_k_RS_INTERNAL_ERROR[] = "RS_INTERNAL_ERROR";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_LibrsyncError___str[] = "LibrsyncError.__str__";
 static const char __pyx_k_RS_BLAKE2_SIG_MAGIC[] = "RS_BLAKE2_SIG_MAGIC";
 static const char __pyx_k_RS_RK_MD4_SIG_MAGIC[] = "RS_RK_MD4_SIG_MAGIC";
 static const char __pyx_k_LibrsyncError___init[] = "LibrsyncError.__init__";
 static const char __pyx_k_RS_RK_BLAKE2_SIG_MAGIC[] = "RS_RK_BLAKE2_SIG_MAGIC";
+static const char __pyx_k_pyrsync_backends_cython__rsync[] = "pyrsync.backends.cython._rsync";
 static const char __pyx_k_input_except_a_file_like_object[] = "input except a file-like object, got %s";
 static const char __pyx_k_self_job_cannot_be_converted_to[] = "self.job cannot be converted to a Python object for pickling";
-static const char __pyx_k_pyrsync_backends_cython__rsync_c[] = "pyrsync.backends.cython._rsync_cy";
+static const char __pyx_k_pyrsync_backends_cython__rsync_p[] = "pyrsync/backends/cython/_rsync.pyx";
 static const char __pyx_k_self_state_cannot_be_converted_t[] = "self.state cannot be converted to a Python object for pickling";
 static const char __pyx_k_sigfile_except_a_file_like_objec[] = "sigfile except a file-like object, got %s";
-static const char __pyx_k_pyrsync_backends_cython__rsync_c_2[] = "pyrsync/backends/cython/_rsync_cy.pyx";
-static PyObject *__pyx_n_s_Job;
 static PyObject *__pyx_n_s_LibrsyncError;
 static PyObject *__pyx_n_s_LibrsyncError___init;
 static PyObject *__pyx_n_s_LibrsyncError___str;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_n_u_RS_BAD_MAGIC;
 static PyObject *__pyx_n_s_RS_BLAKE2_SIG_MAGIC;
 static PyObject *__pyx_n_u_RS_CORRUPT;
@@ -1822,16 +1812,16 @@
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_old_fsize;
 static PyObject *__pyx_n_s_output;
 static PyObject *__pyx_n_s_prepare;
-static PyObject *__pyx_n_s_pyrsync_backends_cython__rsync_c;
-static PyObject *__pyx_kp_s_pyrsync_backends_cython__rsync_c_2;
+static PyObject *__pyx_n_s_pyrsync_backends_cython__rsync;
+static PyObject *__pyx_kp_s_pyrsync_backends_cython__rsync_p;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_read;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_result;
@@ -1845,70 +1835,70 @@
 static PyObject *__pyx_n_s_sigfile;
 static PyObject *__pyx_kp_u_sigfile_except_a_file_like_objec;
 static PyObject *__pyx_n_s_str;
 static PyObject *__pyx_n_s_strong_len;
 static PyObject *__pyx_n_s_tell;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_write;
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_result); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_2__str__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2op___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8lit_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9lit_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_12lit_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9copy_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10copy_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13copy_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8sig_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9sig_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13false_matches___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10sig_blocks___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9block_len___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8in_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9out_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_5start___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3end___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats___reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_2execute(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output); /* proto */
-static void __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_4__dealloc__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args(CYTHON_UNUSED PyObject *__pyx_self, rs_long_t __pyx_v_old_fsize, int __pyx_v_magic, size_t __pyx_v_block_len, size_t __pyx_v_strong_len); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_2signature(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output, size_t __pyx_v_strong_len, rs_magic_number __pyx_v_sig_magic, size_t __pyx_v_block_size); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_4delta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_sigfile, PyObject *__pyx_v_output); /* proto */
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_6patch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_delta, PyObject *__pyx_v_output); /* proto */
-static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Stats(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Job(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_result); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_2__str__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_2op___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8lit_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9lit_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_12lit_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9copy_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_10copy_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_13copy_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8sig_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9sig_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_13false_matches___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_10sig_blocks___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9block_len___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8in_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9out_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_5start___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_3end___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats___reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_2__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_2execute(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output); /* proto */
+static void __pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_4__dealloc__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_get_signature_args(CYTHON_UNUSED PyObject *__pyx_self, rs_long_t __pyx_v_old_fsize, int __pyx_v_magic, size_t __pyx_v_block_len, size_t __pyx_v_strong_len); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_2signature(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output, size_t __pyx_v_strong_len, rs_magic_number __pyx_v_sig_magic, size_t __pyx_v_block_size); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_4delta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_sigfile, PyObject *__pyx_v_output); /* proto */
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_6patch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_delta, PyObject *__pyx_v_output); /* proto */
+static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Stats(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Job(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_65535;
 static size_t __pyx_k__5;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_codeobj__7;
 static PyObject *__pyx_codeobj__9;
 /* Late includes */
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":40
+/* "pyrsync/backends/cython/_rsync.pyx":40
  * 
  * class LibrsyncError(Exception):
  *     def __init__(self, result):             # <<<<<<<<<<<<<<
  *         self.code = result
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError___init__[] = "LibrsyncError.__init__(self, result)";
-static PyMethodDef __pyx_mdef_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError___init__};
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError___init__[] = "LibrsyncError.__init__(self, result)";
+static PyMethodDef __pyx_mdef_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError___init__};
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_result = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -1951,98 +1941,98 @@
     __pyx_v_self = values[0];
     __pyx_v_result = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 40, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.LibrsyncError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.LibrsyncError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError___init__(__pyx_self, __pyx_v_self, __pyx_v_result);
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError___init__(__pyx_self, __pyx_v_self, __pyx_v_result);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_result) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_result) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":41
+  /* "pyrsync/backends/cython/_rsync.pyx":41
  * class LibrsyncError(Exception):
  *     def __init__(self, result):
  *         self.code = result             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_code, __pyx_v_result) < 0) __PYX_ERR(1, 41, __pyx_L1_error)
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":40
+  /* "pyrsync/backends/cython/_rsync.pyx":40
  * 
  * class LibrsyncError(Exception):
  *     def __init__(self, result):             # <<<<<<<<<<<<<<
  *         self.code = result
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.LibrsyncError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.LibrsyncError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":43
+/* "pyrsync/backends/cython/_rsync.pyx":43
  *         self.code = result
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         if self.code == RS_RUNNING:
  *             return "RS_RUNNING"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_3__str__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_2__str__[] = "LibrsyncError.__str__(self)";
-static PyMethodDef __pyx_mdef_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_3__str__ = {"__str__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_3__str__, METH_O, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_2__str__};
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_3__str__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_3__str__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_2__str__[] = "LibrsyncError.__str__(self)";
+static PyMethodDef __pyx_mdef_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_3__str__ = {"__str__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_3__str__, METH_O, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_2__str__};
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_3__str__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__str__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_2__str__(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_2__str__(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_2__str__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_2__str__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":44
+  /* "pyrsync/backends/cython/_rsync.pyx":44
  * 
  *     def __str__(self):
  *         if self.code == RS_RUNNING:             # <<<<<<<<<<<<<<
  *             return "RS_RUNNING"
  *         elif self.code == RS_TEST_SKIPPED:
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 44, __pyx_L1_error)
@@ -2052,36 +2042,36 @@
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":45
+    /* "pyrsync/backends/cython/_rsync.pyx":45
  *     def __str__(self):
  *         if self.code == RS_RUNNING:
  *             return "RS_RUNNING"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_TEST_SKIPPED:
  *             return "RS_TEST_SKIPPED"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_RUNNING);
     __pyx_r = __pyx_n_u_RS_RUNNING;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":44
+    /* "pyrsync/backends/cython/_rsync.pyx":44
  * 
  *     def __str__(self):
  *         if self.code == RS_RUNNING:             # <<<<<<<<<<<<<<
  *             return "RS_RUNNING"
  *         elif self.code == RS_TEST_SKIPPED:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":46
+  /* "pyrsync/backends/cython/_rsync.pyx":46
  *         if self.code == RS_RUNNING:
  *             return "RS_RUNNING"
  *         elif self.code == RS_TEST_SKIPPED:             # <<<<<<<<<<<<<<
  *             return "RS_TEST_SKIPPED"
  *         elif self.code == RS_IO_ERROR:
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 46, __pyx_L1_error)
@@ -2091,36 +2081,36 @@
   __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":47
+    /* "pyrsync/backends/cython/_rsync.pyx":47
  *             return "RS_RUNNING"
  *         elif self.code == RS_TEST_SKIPPED:
  *             return "RS_TEST_SKIPPED"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_IO_ERROR:
  *             return "RS_IO_ERROR"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_TEST_SKIPPED);
     __pyx_r = __pyx_n_u_RS_TEST_SKIPPED;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":46
+    /* "pyrsync/backends/cython/_rsync.pyx":46
  *         if self.code == RS_RUNNING:
  *             return "RS_RUNNING"
  *         elif self.code == RS_TEST_SKIPPED:             # <<<<<<<<<<<<<<
  *             return "RS_TEST_SKIPPED"
  *         elif self.code == RS_IO_ERROR:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":48
+  /* "pyrsync/backends/cython/_rsync.pyx":48
  *         elif self.code == RS_TEST_SKIPPED:
  *             return "RS_TEST_SKIPPED"
  *         elif self.code == RS_IO_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_IO_ERROR"
  *         elif self.code == RS_SYNTAX_ERROR:
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 48, __pyx_L1_error)
@@ -2130,36 +2120,36 @@
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":49
+    /* "pyrsync/backends/cython/_rsync.pyx":49
  *             return "RS_TEST_SKIPPED"
  *         elif self.code == RS_IO_ERROR:
  *             return "RS_IO_ERROR"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_SYNTAX_ERROR:
  *             return "RS_SYNTAX_ERROR"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_IO_ERROR);
     __pyx_r = __pyx_n_u_RS_IO_ERROR;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":48
+    /* "pyrsync/backends/cython/_rsync.pyx":48
  *         elif self.code == RS_TEST_SKIPPED:
  *             return "RS_TEST_SKIPPED"
  *         elif self.code == RS_IO_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_IO_ERROR"
  *         elif self.code == RS_SYNTAX_ERROR:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":50
+  /* "pyrsync/backends/cython/_rsync.pyx":50
  *         elif self.code == RS_IO_ERROR:
  *             return "RS_IO_ERROR"
  *         elif self.code == RS_SYNTAX_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_SYNTAX_ERROR"
  *         elif self.code == RS_MEM_ERROR:
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 50, __pyx_L1_error)
@@ -2169,36 +2159,36 @@
   __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":51
+    /* "pyrsync/backends/cython/_rsync.pyx":51
  *             return "RS_IO_ERROR"
  *         elif self.code == RS_SYNTAX_ERROR:
  *             return "RS_SYNTAX_ERROR"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_MEM_ERROR:
  *             return "RS_MEM_ERROR"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_SYNTAX_ERROR);
     __pyx_r = __pyx_n_u_RS_SYNTAX_ERROR;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":50
+    /* "pyrsync/backends/cython/_rsync.pyx":50
  *         elif self.code == RS_IO_ERROR:
  *             return "RS_IO_ERROR"
  *         elif self.code == RS_SYNTAX_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_SYNTAX_ERROR"
  *         elif self.code == RS_MEM_ERROR:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":52
+  /* "pyrsync/backends/cython/_rsync.pyx":52
  *         elif self.code == RS_SYNTAX_ERROR:
  *             return "RS_SYNTAX_ERROR"
  *         elif self.code == RS_MEM_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_MEM_ERROR"
  *         elif self.code == RS_INPUT_ENDED:
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 52, __pyx_L1_error)
@@ -2208,36 +2198,36 @@
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":53
+    /* "pyrsync/backends/cython/_rsync.pyx":53
  *             return "RS_SYNTAX_ERROR"
  *         elif self.code == RS_MEM_ERROR:
  *             return "RS_MEM_ERROR"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_INPUT_ENDED:
  *             return "RS_INPUT_ENDED"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_MEM_ERROR);
     __pyx_r = __pyx_n_u_RS_MEM_ERROR;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":52
+    /* "pyrsync/backends/cython/_rsync.pyx":52
  *         elif self.code == RS_SYNTAX_ERROR:
  *             return "RS_SYNTAX_ERROR"
  *         elif self.code == RS_MEM_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_MEM_ERROR"
  *         elif self.code == RS_INPUT_ENDED:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":54
+  /* "pyrsync/backends/cython/_rsync.pyx":54
  *         elif self.code == RS_MEM_ERROR:
  *             return "RS_MEM_ERROR"
  *         elif self.code == RS_INPUT_ENDED:             # <<<<<<<<<<<<<<
  *             return "RS_INPUT_ENDED"
  *         elif self.code == RS_BAD_MAGIC:
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 54, __pyx_L1_error)
@@ -2247,36 +2237,36 @@
   __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":55
+    /* "pyrsync/backends/cython/_rsync.pyx":55
  *             return "RS_MEM_ERROR"
  *         elif self.code == RS_INPUT_ENDED:
  *             return "RS_INPUT_ENDED"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_BAD_MAGIC:
  *             return "RS_BAD_MAGIC"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_INPUT_ENDED);
     __pyx_r = __pyx_n_u_RS_INPUT_ENDED;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":54
+    /* "pyrsync/backends/cython/_rsync.pyx":54
  *         elif self.code == RS_MEM_ERROR:
  *             return "RS_MEM_ERROR"
  *         elif self.code == RS_INPUT_ENDED:             # <<<<<<<<<<<<<<
  *             return "RS_INPUT_ENDED"
  *         elif self.code == RS_BAD_MAGIC:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":56
+  /* "pyrsync/backends/cython/_rsync.pyx":56
  *         elif self.code == RS_INPUT_ENDED:
  *             return "RS_INPUT_ENDED"
  *         elif self.code == RS_BAD_MAGIC:             # <<<<<<<<<<<<<<
  *             return "RS_BAD_MAGIC"
  *         elif self.code == RS_UNIMPLEMENTED:
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 56, __pyx_L1_error)
@@ -2286,36 +2276,36 @@
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":57
+    /* "pyrsync/backends/cython/_rsync.pyx":57
  *             return "RS_INPUT_ENDED"
  *         elif self.code == RS_BAD_MAGIC:
  *             return "RS_BAD_MAGIC"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_UNIMPLEMENTED:
  *             return "RS_UNIMPLEMENTED"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_BAD_MAGIC);
     __pyx_r = __pyx_n_u_RS_BAD_MAGIC;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":56
+    /* "pyrsync/backends/cython/_rsync.pyx":56
  *         elif self.code == RS_INPUT_ENDED:
  *             return "RS_INPUT_ENDED"
  *         elif self.code == RS_BAD_MAGIC:             # <<<<<<<<<<<<<<
  *             return "RS_BAD_MAGIC"
  *         elif self.code == RS_UNIMPLEMENTED:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":58
+  /* "pyrsync/backends/cython/_rsync.pyx":58
  *         elif self.code == RS_BAD_MAGIC:
  *             return "RS_BAD_MAGIC"
  *         elif self.code == RS_UNIMPLEMENTED:             # <<<<<<<<<<<<<<
  *             return "RS_UNIMPLEMENTED"
  *         elif self.code == RS_CORRUPT:
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 58, __pyx_L1_error)
@@ -2325,36 +2315,36 @@
   __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":59
+    /* "pyrsync/backends/cython/_rsync.pyx":59
  *             return "RS_BAD_MAGIC"
  *         elif self.code == RS_UNIMPLEMENTED:
  *             return "RS_UNIMPLEMENTED"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_CORRUPT:
  *             return "RS_CORRUPT"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_UNIMPLEMENTED);
     __pyx_r = __pyx_n_u_RS_UNIMPLEMENTED;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":58
+    /* "pyrsync/backends/cython/_rsync.pyx":58
  *         elif self.code == RS_BAD_MAGIC:
  *             return "RS_BAD_MAGIC"
  *         elif self.code == RS_UNIMPLEMENTED:             # <<<<<<<<<<<<<<
  *             return "RS_UNIMPLEMENTED"
  *         elif self.code == RS_CORRUPT:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":60
+  /* "pyrsync/backends/cython/_rsync.pyx":60
  *         elif self.code == RS_UNIMPLEMENTED:
  *             return "RS_UNIMPLEMENTED"
  *         elif self.code == RS_CORRUPT:             # <<<<<<<<<<<<<<
  *             return "RS_CORRUPT"
  *         elif self.code == RS_INTERNAL_ERROR:
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 60, __pyx_L1_error)
@@ -2364,36 +2354,36 @@
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":61
+    /* "pyrsync/backends/cython/_rsync.pyx":61
  *             return "RS_UNIMPLEMENTED"
  *         elif self.code == RS_CORRUPT:
  *             return "RS_CORRUPT"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_INTERNAL_ERROR:
  *             return "RS_INTERNAL_ERROR"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_CORRUPT);
     __pyx_r = __pyx_n_u_RS_CORRUPT;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":60
+    /* "pyrsync/backends/cython/_rsync.pyx":60
  *         elif self.code == RS_UNIMPLEMENTED:
  *             return "RS_UNIMPLEMENTED"
  *         elif self.code == RS_CORRUPT:             # <<<<<<<<<<<<<<
  *             return "RS_CORRUPT"
  *         elif self.code == RS_INTERNAL_ERROR:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":62
+  /* "pyrsync/backends/cython/_rsync.pyx":62
  *         elif self.code == RS_CORRUPT:
  *             return "RS_CORRUPT"
  *         elif self.code == RS_INTERNAL_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_INTERNAL_ERROR"
  *         elif self.code == RS_PARAM_ERROR:
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 62, __pyx_L1_error)
@@ -2403,36 +2393,36 @@
   __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":63
+    /* "pyrsync/backends/cython/_rsync.pyx":63
  *             return "RS_CORRUPT"
  *         elif self.code == RS_INTERNAL_ERROR:
  *             return "RS_INTERNAL_ERROR"             # <<<<<<<<<<<<<<
  *         elif self.code == RS_PARAM_ERROR:
  *             return "RS_PARAM_ERROR"
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_INTERNAL_ERROR);
     __pyx_r = __pyx_n_u_RS_INTERNAL_ERROR;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":62
+    /* "pyrsync/backends/cython/_rsync.pyx":62
  *         elif self.code == RS_CORRUPT:
  *             return "RS_CORRUPT"
  *         elif self.code == RS_INTERNAL_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_INTERNAL_ERROR"
  *         elif self.code == RS_PARAM_ERROR:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":64
+  /* "pyrsync/backends/cython/_rsync.pyx":64
  *         elif self.code == RS_INTERNAL_ERROR:
  *             return "RS_INTERNAL_ERROR"
  *         elif self.code == RS_PARAM_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_PARAM_ERROR"
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 64, __pyx_L1_error)
@@ -2442,74 +2432,74 @@
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":65
+    /* "pyrsync/backends/cython/_rsync.pyx":65
  *             return "RS_INTERNAL_ERROR"
  *         elif self.code == RS_PARAM_ERROR:
  *             return "RS_PARAM_ERROR"             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_RS_PARAM_ERROR);
     __pyx_r = __pyx_n_u_RS_PARAM_ERROR;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":64
+    /* "pyrsync/backends/cython/_rsync.pyx":64
  *         elif self.code == RS_INTERNAL_ERROR:
  *             return "RS_INTERNAL_ERROR"
  *         elif self.code == RS_PARAM_ERROR:             # <<<<<<<<<<<<<<
  *             return "RS_PARAM_ERROR"
  * 
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":43
+  /* "pyrsync/backends/cython/_rsync.pyx":43
  *         self.code = result
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         if self.code == RS_RUNNING:
  *             return "RS_RUNNING"
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.LibrsyncError.__str__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.LibrsyncError.__str__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":76
+/* "pyrsync/backends/cython/_rsync.pyx":76
  * RS_RK_BLAKE2_SIG_MAGIC= C_RS_RK_BLAKE2_SIG_MAGIC
  * 
  * cdef inline uint8_t PyFile_Check(object file):             # <<<<<<<<<<<<<<
  *     if PyObject_HasAttrString(file, "read") and PyObject_HasAttrString(file, "write") and PyObject_HasAttrString(file,
  *                                                                                                                  "seek"):
  */
 
-static CYTHON_INLINE uint8_t __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_PyFile_Check(PyObject *__pyx_v_file) {
+static CYTHON_INLINE uint8_t __pyx_f_7pyrsync_8backends_6cython_6_rsync_PyFile_Check(PyObject *__pyx_v_file) {
   uint8_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("PyFile_Check", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":77
+  /* "pyrsync/backends/cython/_rsync.pyx":77
  * 
  * cdef inline uint8_t PyFile_Check(object file):
  *     if PyObject_HasAttrString(file, "read") and PyObject_HasAttrString(file, "write") and PyObject_HasAttrString(file,             # <<<<<<<<<<<<<<
  *                                                                                                                  "seek"):
  *         return 1
  */
   __pyx_t_2 = (PyObject_HasAttrString(__pyx_v_file, ((char const *)"read")) != 0);
@@ -2525,160 +2515,160 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (PyObject_HasAttrString(__pyx_v_file, ((char const *)"seek")) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":79
+    /* "pyrsync/backends/cython/_rsync.pyx":79
  *     if PyObject_HasAttrString(file, "read") and PyObject_HasAttrString(file, "write") and PyObject_HasAttrString(file,
  *                                                                                                                  "seek"):
  *         return 1             # <<<<<<<<<<<<<<
  *     return 0
  * # copyed sthing from https://github.com/smartfile/python-librsync/blob/master/librsync/__init__.py
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":77
+    /* "pyrsync/backends/cython/_rsync.pyx":77
  * 
  * cdef inline uint8_t PyFile_Check(object file):
  *     if PyObject_HasAttrString(file, "read") and PyObject_HasAttrString(file, "write") and PyObject_HasAttrString(file,             # <<<<<<<<<<<<<<
  *                                                                                                                  "seek"):
  *         return 1
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":80
+  /* "pyrsync/backends/cython/_rsync.pyx":80
  *                                                                                                                  "seek"):
  *         return 1
  *     return 0             # <<<<<<<<<<<<<<
  * # copyed sthing from https://github.com/smartfile/python-librsync/blob/master/librsync/__init__.py
  * @cython.freelist(8)
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":76
+  /* "pyrsync/backends/cython/_rsync.pyx":76
  * RS_RK_BLAKE2_SIG_MAGIC= C_RS_RK_BLAKE2_SIG_MAGIC
  * 
  * cdef inline uint8_t PyFile_Check(object file):             # <<<<<<<<<<<<<<
  *     if PyObject_HasAttrString(file, "read") and PyObject_HasAttrString(file, "write") and PyObject_HasAttrString(file,
  *                                                                                                                  "seek"):
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":89
+/* "pyrsync/backends/cython/_rsync.pyx":89
  * 
  *     @staticmethod
  *     cdef inline Stats from_ptr(rs_stats_t * state):             # <<<<<<<<<<<<<<
  *         cdef Stats self = Stats.__new__(Stats)
  *         self.state = state
  */
 
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_from_ptr(rs_stats_t *__pyx_v_state) {
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self = 0;
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_r = NULL;
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_f_7pyrsync_8backends_6cython_6_rsync_5Stats_from_ptr(rs_stats_t *__pyx_v_state) {
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self = 0;
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("from_ptr", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":90
+  /* "pyrsync/backends/cython/_rsync.pyx":90
  *     @staticmethod
  *     cdef inline Stats from_ptr(rs_stats_t * state):
  *         cdef Stats self = Stats.__new__(Stats)             # <<<<<<<<<<<<<<
  *         self.state = state
  *         return self
  */
-  __pyx_t_1 = ((PyObject *)__pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Stats(((PyTypeObject *)__pyx_ptype_7pyrsync_8backends_6cython_9_rsync_cy_Stats), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Stats(((PyTypeObject *)__pyx_ptype_7pyrsync_8backends_6cython_6_rsync_Stats), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 90, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_1));
-  __pyx_v_self = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_t_1);
+  __pyx_v_self = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":91
+  /* "pyrsync/backends/cython/_rsync.pyx":91
  *     cdef inline Stats from_ptr(rs_stats_t * state):
  *         cdef Stats self = Stats.__new__(Stats)
  *         self.state = state             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->state = __pyx_v_state;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":92
+  /* "pyrsync/backends/cython/_rsync.pyx":92
  *         cdef Stats self = Stats.__new__(Stats)
  *         self.state = state
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = __pyx_v_self;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":89
+  /* "pyrsync/backends/cython/_rsync.pyx":89
  * 
  *     @staticmethod
  *     cdef inline Stats from_ptr(rs_stats_t * state):             # <<<<<<<<<<<<<<
  *         cdef Stats self = Stats.__new__(Stats)
  *         self.state = state
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.from_ptr", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.from_ptr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_self);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":95
+/* "pyrsync/backends/cython/_rsync.pyx":95
  * 
  *     @property
  *     def op(self):             # <<<<<<<<<<<<<<
  *         return (<bytes>self.state.op).decode()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2op_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2op_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_2op_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_2op_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2op___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_2op___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2op___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_2op___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":96
+  /* "pyrsync/backends/cython/_rsync.pyx":96
  *     @property
  *     def op(self):
  *         return (<bytes>self.state.op).decode()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
@@ -2691,1000 +2681,1000 @@
   __pyx_t_2 = __Pyx_decode_bytes(((PyObject*)__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":95
+  /* "pyrsync/backends/cython/_rsync.pyx":95
  * 
  *     @property
  *     def op(self):             # <<<<<<<<<<<<<<
  *         return (<bytes>self.state.op).decode()
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.op.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.op.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":99
+/* "pyrsync/backends/cython/_rsync.pyx":99
  * 
  *     @property
  *     def lit_cmds(self):             # <<<<<<<<<<<<<<
  *         return self.state.lit_cmds
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8lit_cmds_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8lit_cmds_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8lit_cmds_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8lit_cmds_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8lit_cmds___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8lit_cmds___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8lit_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8lit_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":100
+  /* "pyrsync/backends/cython/_rsync.pyx":100
  *     @property
  *     def lit_cmds(self):
  *         return self.state.lit_cmds             # <<<<<<<<<<<<<<
  *     @property
  *     def lit_bytes(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->state->lit_cmds); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":99
+  /* "pyrsync/backends/cython/_rsync.pyx":99
  * 
  *     @property
  *     def lit_cmds(self):             # <<<<<<<<<<<<<<
  *         return self.state.lit_cmds
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.lit_cmds.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.lit_cmds.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":102
+/* "pyrsync/backends/cython/_rsync.pyx":102
  *         return self.state.lit_cmds
  *     @property
  *     def lit_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.lit_bytes
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9lit_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9lit_bytes_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9lit_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9lit_bytes_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9lit_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9lit_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9lit_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9lit_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":103
+  /* "pyrsync/backends/cython/_rsync.pyx":103
  *     @property
  *     def lit_bytes(self):
  *         return self.state.lit_bytes             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->lit_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":102
+  /* "pyrsync/backends/cython/_rsync.pyx":102
  *         return self.state.lit_cmds
  *     @property
  *     def lit_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.lit_bytes
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.lit_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.lit_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":106
+/* "pyrsync/backends/cython/_rsync.pyx":106
  * 
  *     @property
  *     def lit_cmdbytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.lit_cmdbytes
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_12lit_cmdbytes_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_12lit_cmdbytes_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_12lit_cmdbytes_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_12lit_cmdbytes_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_12lit_cmdbytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_12lit_cmdbytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_12lit_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_12lit_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":107
+  /* "pyrsync/backends/cython/_rsync.pyx":107
  *     @property
  *     def lit_cmdbytes(self):
  *         return self.state.lit_cmdbytes             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->lit_cmdbytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":106
+  /* "pyrsync/backends/cython/_rsync.pyx":106
  * 
  *     @property
  *     def lit_cmdbytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.lit_cmdbytes
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.lit_cmdbytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.lit_cmdbytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":110
+/* "pyrsync/backends/cython/_rsync.pyx":110
  * 
  *     @property
  *     def copy_cmds(self):             # <<<<<<<<<<<<<<
  *         return self.state.copy_cmds
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9copy_cmds_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9copy_cmds_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9copy_cmds_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9copy_cmds_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9copy_cmds___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9copy_cmds___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9copy_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9copy_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":111
+  /* "pyrsync/backends/cython/_rsync.pyx":111
  *     @property
  *     def copy_cmds(self):
  *         return self.state.copy_cmds             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->copy_cmds); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":110
+  /* "pyrsync/backends/cython/_rsync.pyx":110
  * 
  *     @property
  *     def copy_cmds(self):             # <<<<<<<<<<<<<<
  *         return self.state.copy_cmds
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.copy_cmds.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.copy_cmds.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":114
+/* "pyrsync/backends/cython/_rsync.pyx":114
  * 
  *     @property
  *     def copy_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.copy_bytes
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10copy_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10copy_bytes_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_10copy_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_10copy_bytes_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10copy_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_10copy_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10copy_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_10copy_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":115
+  /* "pyrsync/backends/cython/_rsync.pyx":115
  *     @property
  *     def copy_bytes(self):
  *         return self.state.copy_bytes             # <<<<<<<<<<<<<<
  *     @property
  *     def copy_cmdbytes(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->copy_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":114
+  /* "pyrsync/backends/cython/_rsync.pyx":114
  * 
  *     @property
  *     def copy_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.copy_bytes
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.copy_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.copy_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":117
+/* "pyrsync/backends/cython/_rsync.pyx":117
  *         return self.state.copy_bytes
  *     @property
  *     def copy_cmdbytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.copy_cmdbytes
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13copy_cmdbytes_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13copy_cmdbytes_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_13copy_cmdbytes_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_13copy_cmdbytes_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13copy_cmdbytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_13copy_cmdbytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13copy_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_13copy_cmdbytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":118
+  /* "pyrsync/backends/cython/_rsync.pyx":118
  *     @property
  *     def copy_cmdbytes(self):
  *         return self.state.copy_cmdbytes             # <<<<<<<<<<<<<<
  *     @property
  *     def sig_cmds(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->copy_cmdbytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":117
+  /* "pyrsync/backends/cython/_rsync.pyx":117
  *         return self.state.copy_bytes
  *     @property
  *     def copy_cmdbytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.copy_cmdbytes
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.copy_cmdbytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.copy_cmdbytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":120
+/* "pyrsync/backends/cython/_rsync.pyx":120
  *         return self.state.copy_cmdbytes
  *     @property
  *     def sig_cmds(self):             # <<<<<<<<<<<<<<
  *         return self.state.sig_cmds
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8sig_cmds_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8sig_cmds_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8sig_cmds_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8sig_cmds_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8sig_cmds___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8sig_cmds___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8sig_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8sig_cmds___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":121
+  /* "pyrsync/backends/cython/_rsync.pyx":121
  *     @property
  *     def sig_cmds(self):
  *         return self.state.sig_cmds             # <<<<<<<<<<<<<<
  *     @property
  *     def sig_bytes(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->sig_cmds); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":120
+  /* "pyrsync/backends/cython/_rsync.pyx":120
  *         return self.state.copy_cmdbytes
  *     @property
  *     def sig_cmds(self):             # <<<<<<<<<<<<<<
  *         return self.state.sig_cmds
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.sig_cmds.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.sig_cmds.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":123
+/* "pyrsync/backends/cython/_rsync.pyx":123
  *         return self.state.sig_cmds
  *     @property
  *     def sig_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.sig_bytes
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9sig_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9sig_bytes_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9sig_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9sig_bytes_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9sig_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9sig_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9sig_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9sig_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":124
+  /* "pyrsync/backends/cython/_rsync.pyx":124
  *     @property
  *     def sig_bytes(self):
  *         return self.state.sig_bytes             # <<<<<<<<<<<<<<
  *     @property
  *     def false_matches(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->sig_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":123
+  /* "pyrsync/backends/cython/_rsync.pyx":123
  *         return self.state.sig_cmds
  *     @property
  *     def sig_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.sig_bytes
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.sig_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.sig_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":126
+/* "pyrsync/backends/cython/_rsync.pyx":126
  *         return self.state.sig_bytes
  *     @property
  *     def false_matches(self):             # <<<<<<<<<<<<<<
  *         return self.state.false_matches
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13false_matches_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13false_matches_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_13false_matches_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_13false_matches_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13false_matches___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_13false_matches___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13false_matches___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_13false_matches___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":127
+  /* "pyrsync/backends/cython/_rsync.pyx":127
  *     @property
  *     def false_matches(self):
  *         return self.state.false_matches             # <<<<<<<<<<<<<<
  *     @property
  *     def sig_blocks (self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->state->false_matches); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":126
+  /* "pyrsync/backends/cython/_rsync.pyx":126
  *         return self.state.sig_bytes
  *     @property
  *     def false_matches(self):             # <<<<<<<<<<<<<<
  *         return self.state.false_matches
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.false_matches.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.false_matches.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":129
+/* "pyrsync/backends/cython/_rsync.pyx":129
  *         return self.state.false_matches
  *     @property
  *     def sig_blocks (self):             # <<<<<<<<<<<<<<
  *         return self.state.sig_blocks
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10sig_blocks_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10sig_blocks_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_10sig_blocks_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_10sig_blocks_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10sig_blocks___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_10sig_blocks___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10sig_blocks___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_10sig_blocks___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":130
+  /* "pyrsync/backends/cython/_rsync.pyx":130
  *     @property
  *     def sig_blocks (self):
  *         return self.state.sig_blocks             # <<<<<<<<<<<<<<
  *     @property
  *     def block_len(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->sig_blocks); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":129
+  /* "pyrsync/backends/cython/_rsync.pyx":129
  *         return self.state.false_matches
  *     @property
  *     def sig_blocks (self):             # <<<<<<<<<<<<<<
  *         return self.state.sig_blocks
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.sig_blocks.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.sig_blocks.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":132
+/* "pyrsync/backends/cython/_rsync.pyx":132
  *         return self.state.sig_blocks
  *     @property
  *     def block_len(self):             # <<<<<<<<<<<<<<
  *         return self.state.block_len
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9block_len_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9block_len_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9block_len_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9block_len_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9block_len___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9block_len___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9block_len___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9block_len___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":133
+  /* "pyrsync/backends/cython/_rsync.pyx":133
  *     @property
  *     def block_len(self):
  *         return self.state.block_len             # <<<<<<<<<<<<<<
  *     @property
  *     def in_bytes  (self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_self->state->block_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":132
+  /* "pyrsync/backends/cython/_rsync.pyx":132
  *         return self.state.sig_blocks
  *     @property
  *     def block_len(self):             # <<<<<<<<<<<<<<
  *         return self.state.block_len
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.block_len.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.block_len.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":135
+/* "pyrsync/backends/cython/_rsync.pyx":135
  *         return self.state.block_len
  *     @property
  *     def in_bytes  (self):             # <<<<<<<<<<<<<<
  *         return self.state.in_bytes
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8in_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8in_bytes_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8in_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8in_bytes_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8in_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8in_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8in_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_8in_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":136
+  /* "pyrsync/backends/cython/_rsync.pyx":136
  *     @property
  *     def in_bytes  (self):
  *         return self.state.in_bytes             # <<<<<<<<<<<<<<
  *     @property
  *     def out_bytes(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->in_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":135
+  /* "pyrsync/backends/cython/_rsync.pyx":135
  *         return self.state.block_len
  *     @property
  *     def in_bytes  (self):             # <<<<<<<<<<<<<<
  *         return self.state.in_bytes
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.in_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.in_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":138
+/* "pyrsync/backends/cython/_rsync.pyx":138
  *         return self.state.in_bytes
  *     @property
  *     def out_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.out_bytes
  *     @property
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9out_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9out_bytes_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9out_bytes_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9out_bytes_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9out_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9out_bytes___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9out_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_9out_bytes___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":139
+  /* "pyrsync/backends/cython/_rsync.pyx":139
  *     @property
  *     def out_bytes(self):
  *         return self.state.out_bytes             # <<<<<<<<<<<<<<
  *     @property
  *     def start(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_intmax_t(__pyx_v_self->state->out_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":138
+  /* "pyrsync/backends/cython/_rsync.pyx":138
  *         return self.state.in_bytes
  *     @property
  *     def out_bytes(self):             # <<<<<<<<<<<<<<
  *         return self.state.out_bytes
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.out_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.out_bytes.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":141
+/* "pyrsync/backends/cython/_rsync.pyx":141
  *         return self.state.out_bytes
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.state.start
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_5start_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_5start_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_5start_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_5start_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_5start___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_5start___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_5start___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_5start___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":142
+  /* "pyrsync/backends/cython/_rsync.pyx":142
  *     @property
  *     def start(self):
  *         return self.state.start             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_time_t(__pyx_v_self->state->start); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":141
+  /* "pyrsync/backends/cython/_rsync.pyx":141
  *         return self.state.out_bytes
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.state.start
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.start.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.start.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":145
+/* "pyrsync/backends/cython/_rsync.pyx":145
  * 
  *     @property
  *     def end(self):             # <<<<<<<<<<<<<<
  *         return self.state.end
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3end_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3end_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_3end_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_3end_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3end___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_3end___get__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3end___get__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_3end___get__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":146
+  /* "pyrsync/backends/cython/_rsync.pyx":146
  *     @property
  *     def end(self):
  *         return self.state.end             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(8)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_time_t(__pyx_v_self->state->end); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":145
+  /* "pyrsync/backends/cython/_rsync.pyx":145
  * 
  *     @property
  *     def end(self):             # <<<<<<<<<<<<<<
  *         return self.state.end
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.end.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.end.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.state cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_5Stats___reduce_cython__[] = "Stats.__reduce_cython__(self)";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_5Stats___reduce_cython__[] = "Stats.__reduce_cython__(self)";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats___reduce_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats___reduce_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats___reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats___reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -3706,43 +3696,43 @@
  *     raise TypeError("self.state cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("self.state cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.state cannot be converted to a Python object for pickling")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2__setstate_cython__[] = "Stats.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_5Stats_2__setstate_cython__[] = "Stats.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2__setstate_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_2__setstate_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_5Stats_2__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -3764,132 +3754,132 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.state cannot be converted to a Python object for pickling")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Stats.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Stats.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":155
+/* "pyrsync/backends/cython/_rsync.pyx":156
  * 
  *     @staticmethod
  *     cdef inline Job from_ptr(rs_job_t * job):             # <<<<<<<<<<<<<<
  *         cdef Job self = Job.__new__(Job)
  *         self.job = job
  */
 
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr(rs_job_t *__pyx_v_job) {
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self = 0;
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_r = NULL;
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr(rs_job_t *__pyx_v_job) {
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self = 0;
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("from_ptr", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":156
+  /* "pyrsync/backends/cython/_rsync.pyx":157
  *     @staticmethod
  *     cdef inline Job from_ptr(rs_job_t * job):
  *         cdef Job self = Job.__new__(Job)             # <<<<<<<<<<<<<<
  *         self.job = job
  *         return self
  */
-  __pyx_t_1 = ((PyObject *)__pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Job(((PyTypeObject *)__pyx_ptype_7pyrsync_8backends_6cython_9_rsync_cy_Job), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 156, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Job(((PyTypeObject *)__pyx_ptype_7pyrsync_8backends_6cython_6_rsync_Job), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 157, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_1));
-  __pyx_v_self = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_t_1);
+  __pyx_v_self = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":157
+  /* "pyrsync/backends/cython/_rsync.pyx":158
  *     cdef inline Job from_ptr(rs_job_t * job):
  *         cdef Job self = Job.__new__(Job)
  *         self.job = job             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->job = __pyx_v_job;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":158
+  /* "pyrsync/backends/cython/_rsync.pyx":159
  *         cdef Job self = Job.__new__(Job)
  *         self.job = job
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     cdef inline rs_result iter(self, rs_buffers_t * buffer):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = __pyx_v_self;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":155
+  /* "pyrsync/backends/cython/_rsync.pyx":156
  * 
  *     @staticmethod
  *     cdef inline Job from_ptr(rs_job_t * job):             # <<<<<<<<<<<<<<
  *         cdef Job self = Job.__new__(Job)
  *         self.job = job
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.from_ptr", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.from_ptr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_self);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":160
+/* "pyrsync/backends/cython/_rsync.pyx":161
  *         return self
  * 
  *     cdef inline rs_result iter(self, rs_buffers_t * buffer):             # <<<<<<<<<<<<<<
  *         cdef rs_result result
  *         with nogil:
  */
 
-static CYTHON_INLINE rs_result __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_iter(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, rs_buffers_t *__pyx_v_buffer) {
+static CYTHON_INLINE rs_result __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_iter(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, rs_buffers_t *__pyx_v_buffer) {
   rs_result __pyx_v_result;
   rs_result __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("iter", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":162
+  /* "pyrsync/backends/cython/_rsync.pyx":163
  *     cdef inline rs_result iter(self, rs_buffers_t * buffer):
  *         cdef rs_result result
  *         with nogil:             # <<<<<<<<<<<<<<
  *             result = rs_job_iter(self.job, buffer)
  *         return result
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":163
+        /* "pyrsync/backends/cython/_rsync.pyx":164
  *         cdef rs_result result
  *         with nogil:
  *             result = rs_job_iter(self.job, buffer)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
         __pyx_v_result = rs_job_iter(__pyx_v_self->job, __pyx_v_buffer);
       }
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":162
+      /* "pyrsync/backends/cython/_rsync.pyx":163
  *     cdef inline rs_result iter(self, rs_buffers_t * buffer):
  *         cdef rs_result result
  *         with nogil:             # <<<<<<<<<<<<<<
  *             result = rs_job_iter(self.job, buffer)
  *         return result
  */
       /*finally:*/ {
@@ -3900,149 +3890,149 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":164
+  /* "pyrsync/backends/cython/_rsync.pyx":165
  *         with nogil:
  *             result = rs_job_iter(self.job, buffer)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline Stats statistics(self):
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":160
+  /* "pyrsync/backends/cython/_rsync.pyx":161
  *         return self
  * 
  *     cdef inline rs_result iter(self, rs_buffers_t * buffer):             # <<<<<<<<<<<<<<
  *         cdef rs_result result
  *         with nogil:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":166
+/* "pyrsync/backends/cython/_rsync.pyx":167
  *         return result
  * 
  *     cpdef inline Stats statistics(self):             # <<<<<<<<<<<<<<
- *         cdef rs_stats_t * state = rs_job_statistics(self.job)
+ *         cdef rs_stats_t * state = <rs_stats_t *>rs_job_statistics(self.job)
  *         return Stats.from_ptr(state)
  */
 
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_1statistics(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_1statistics(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static CYTHON_INLINE struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   rs_stats_t *__pyx_v_state;
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_r = NULL;
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("statistics", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":167
+  /* "pyrsync/backends/cython/_rsync.pyx":168
  * 
  *     cpdef inline Stats statistics(self):
- *         cdef rs_stats_t * state = rs_job_statistics(self.job)             # <<<<<<<<<<<<<<
+ *         cdef rs_stats_t * state = <rs_stats_t *>rs_job_statistics(self.job)             # <<<<<<<<<<<<<<
  *         return Stats.from_ptr(state)
  * 
  */
-  __pyx_v_state = rs_job_statistics(__pyx_v_self->job);
+  __pyx_v_state = ((rs_stats_t *)rs_job_statistics(__pyx_v_self->job));
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":168
+  /* "pyrsync/backends/cython/_rsync.pyx":169
  *     cpdef inline Stats statistics(self):
- *         cdef rs_stats_t * state = rs_job_statistics(self.job)
+ *         cdef rs_stats_t * state = <rs_stats_t *>rs_job_statistics(self.job)
  *         return Stats.from_ptr(state)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline int execute(self, object input, object output = None) except -1:
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_from_ptr(__pyx_v_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 168, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_6_rsync_5Stats_from_ptr(__pyx_v_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)__pyx_t_1);
+  __pyx_r = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":166
+  /* "pyrsync/backends/cython/_rsync.pyx":167
  *         return result
  * 
  *     cpdef inline Stats statistics(self):             # <<<<<<<<<<<<<<
- *         cdef rs_stats_t * state = rs_job_statistics(self.job)
+ *         cdef rs_stats_t * state = <rs_stats_t *>rs_job_statistics(self.job)
  *         return Stats.from_ptr(state)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.statistics", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.statistics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_1statistics(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics[] = "Job.statistics(self) -> Stats";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_1statistics(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_1statistics(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_statistics[] = "Job.statistics(self) -> Stats";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_1statistics(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("statistics (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_statistics(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_statistics(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("statistics", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 166, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_statistics(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.statistics", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.statistics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":170
+/* "pyrsync/backends/cython/_rsync.pyx":171
  *         return Stats.from_ptr(state)
  * 
  *     cpdef inline int execute(self, object input, object output = None) except -1:             # <<<<<<<<<<<<<<
  *         if not PyFile_Check(input):
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  */
 
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_3execute(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static CYTHON_INLINE int __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, PyObject *__pyx_v_input, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute *__pyx_optional_args) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_3execute(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static CYTHON_INLINE int __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, PyObject *__pyx_v_input, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute *__pyx_optional_args) {
   PyObject *__pyx_v_output = ((PyObject *)Py_None);
   rs_buffers_t __pyx_v_buffer;
   void *__pyx_v_out;
   PyObject *__pyx_v_block = 0;
   rs_result __pyx_v_result;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -4071,432 +4061,432 @@
   __Pyx_RefNannySetupContext("execute", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_output = __pyx_optional_args->output;
     }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":171
+  /* "pyrsync/backends/cython/_rsync.pyx":172
  * 
  *     cpdef inline int execute(self, object input, object output = None) except -1:
  *         if not PyFile_Check(input):             # <<<<<<<<<<<<<<
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  *         if output is not None and not PyFile_Check(output):
  */
-  __pyx_t_1 = ((!(__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_PyFile_Check(__pyx_v_input) != 0)) != 0);
+  __pyx_t_1 = ((!(__pyx_f_7pyrsync_8backends_6cython_6_rsync_PyFile_Check(__pyx_v_input) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":172
+    /* "pyrsync/backends/cython/_rsync.pyx":173
  *     cpdef inline int execute(self, object input, object output = None) except -1:
  *         if not PyFile_Check(input):
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)             # <<<<<<<<<<<<<<
  *         if output is not None and not PyFile_Check(output):
  *             raise TypeError("sigfile except a file-like object, got %s" % type(output).__name__)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)Py_TYPE(__pyx_v_input)), __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 172, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)Py_TYPE(__pyx_v_input)), __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_input_except_a_file_like_object, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 172, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_input_except_a_file_like_object, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 172, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 172, __pyx_L1_error)
+    __PYX_ERR(1, 173, __pyx_L1_error)
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":171
+    /* "pyrsync/backends/cython/_rsync.pyx":172
  * 
  *     cpdef inline int execute(self, object input, object output = None) except -1:
  *         if not PyFile_Check(input):             # <<<<<<<<<<<<<<
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  *         if output is not None and not PyFile_Check(output):
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":173
+  /* "pyrsync/backends/cython/_rsync.pyx":174
  *         if not PyFile_Check(input):
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  *         if output is not None and not PyFile_Check(output):             # <<<<<<<<<<<<<<
  *             raise TypeError("sigfile except a file-like object, got %s" % type(output).__name__)
  *         cdef:
  */
   __pyx_t_4 = (__pyx_v_output != Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
   } else {
     __pyx_t_1 = __pyx_t_5;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_5 = ((!(__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_PyFile_Check(__pyx_v_output) != 0)) != 0);
+  __pyx_t_5 = ((!(__pyx_f_7pyrsync_8backends_6cython_6_rsync_PyFile_Check(__pyx_v_output) != 0)) != 0);
   __pyx_t_1 = __pyx_t_5;
   __pyx_L5_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":174
+    /* "pyrsync/backends/cython/_rsync.pyx":175
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  *         if output is not None and not PyFile_Check(output):
  *             raise TypeError("sigfile except a file-like object, got %s" % type(output).__name__)             # <<<<<<<<<<<<<<
  *         cdef:
  *             rs_buffers_t buffer
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)Py_TYPE(__pyx_v_output)), __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 174, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)Py_TYPE(__pyx_v_output)), __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_sigfile_except_a_file_like_objec, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 174, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_sigfile_except_a_file_like_objec, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 174, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 174, __pyx_L1_error)
+    __PYX_ERR(1, 175, __pyx_L1_error)
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":173
+    /* "pyrsync/backends/cython/_rsync.pyx":174
  *         if not PyFile_Check(input):
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  *         if output is not None and not PyFile_Check(output):             # <<<<<<<<<<<<<<
  *             raise TypeError("sigfile except a file-like object, got %s" % type(output).__name__)
  *         cdef:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":181
+  /* "pyrsync/backends/cython/_rsync.pyx":182
  *             rs_result result
  * 
  *         out = PyMem_Malloc(RS_JOB_BLOCKSIZE)             # <<<<<<<<<<<<<<
  *         if not out:
  *             raise MemoryError
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 181, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 181, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_out = PyMem_Malloc(__pyx_t_6);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":182
+  /* "pyrsync/backends/cython/_rsync.pyx":183
  * 
  *         out = PyMem_Malloc(RS_JOB_BLOCKSIZE)
  *         if not out:             # <<<<<<<<<<<<<<
  *             raise MemoryError
  *         try:
  */
   __pyx_t_1 = ((!(__pyx_v_out != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":183
+    /* "pyrsync/backends/cython/_rsync.pyx":184
  *         out = PyMem_Malloc(RS_JOB_BLOCKSIZE)
  *         if not out:
  *             raise MemoryError             # <<<<<<<<<<<<<<
  *         try:
  *             while True:
  */
-    PyErr_NoMemory(); __PYX_ERR(1, 183, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(1, 184, __pyx_L1_error)
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":182
+    /* "pyrsync/backends/cython/_rsync.pyx":183
  * 
  *         out = PyMem_Malloc(RS_JOB_BLOCKSIZE)
  *         if not out:             # <<<<<<<<<<<<<<
  *             raise MemoryError
  *         try:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":184
+  /* "pyrsync/backends/cython/_rsync.pyx":185
  *         if not out:
  *             raise MemoryError
  *         try:             # <<<<<<<<<<<<<<
  *             while True:
  *                 block = input.read(RS_JOB_BLOCKSIZE)  # type: bytes
  */
   /*try:*/ {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":185
+    /* "pyrsync/backends/cython/_rsync.pyx":186
  *             raise MemoryError
  *         try:
  *             while True:             # <<<<<<<<<<<<<<
  *                 block = input.read(RS_JOB_BLOCKSIZE)  # type: bytes
  *                 buffer.next_in = PyBytes_AS_STRING(block)
  */
     while (1) {
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":186
+      /* "pyrsync/backends/cython/_rsync.pyx":187
  *         try:
  *             while True:
  *                 block = input.read(RS_JOB_BLOCKSIZE)  # type: bytes             # <<<<<<<<<<<<<<
  *                 buffer.next_in = PyBytes_AS_STRING(block)
  *                 buffer.avail_in = <size_t> PyBytes_GET_SIZE(block)
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 186, __pyx_L9_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 187, __pyx_L9_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 186, __pyx_L9_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 187, __pyx_L9_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 186, __pyx_L9_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 187, __pyx_L9_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(1, 186, __pyx_L9_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(1, 187, __pyx_L9_error)
       __Pyx_XDECREF_SET(__pyx_v_block, ((PyObject*)__pyx_t_2));
       __pyx_t_2 = 0;
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":187
+      /* "pyrsync/backends/cython/_rsync.pyx":188
  *             while True:
  *                 block = input.read(RS_JOB_BLOCKSIZE)  # type: bytes
  *                 buffer.next_in = PyBytes_AS_STRING(block)             # <<<<<<<<<<<<<<
  *                 buffer.avail_in = <size_t> PyBytes_GET_SIZE(block)
  *                 buffer.eof_in = not block
  */
       __pyx_v_buffer.next_in = PyBytes_AS_STRING(__pyx_v_block);
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":188
+      /* "pyrsync/backends/cython/_rsync.pyx":189
  *                 block = input.read(RS_JOB_BLOCKSIZE)  # type: bytes
  *                 buffer.next_in = PyBytes_AS_STRING(block)
  *                 buffer.avail_in = <size_t> PyBytes_GET_SIZE(block)             # <<<<<<<<<<<<<<
  *                 buffer.eof_in = not block
  *                 buffer.next_out = <char *> out
  */
       __pyx_v_buffer.avail_in = ((size_t)PyBytes_GET_SIZE(__pyx_v_block));
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":189
+      /* "pyrsync/backends/cython/_rsync.pyx":190
  *                 buffer.next_in = PyBytes_AS_STRING(block)
  *                 buffer.avail_in = <size_t> PyBytes_GET_SIZE(block)
  *                 buffer.eof_in = not block             # <<<<<<<<<<<<<<
  *                 buffer.next_out = <char *> out
  *                 buffer.avail_out = <size_t> RS_JOB_BLOCKSIZE
  */
       __pyx_t_1 = (__pyx_v_block != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_block) != 0);
       __pyx_v_buffer.eof_in = (!__pyx_t_1);
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":190
+      /* "pyrsync/backends/cython/_rsync.pyx":191
  *                 buffer.avail_in = <size_t> PyBytes_GET_SIZE(block)
  *                 buffer.eof_in = not block
  *                 buffer.next_out = <char *> out             # <<<<<<<<<<<<<<
  *                 buffer.avail_out = <size_t> RS_JOB_BLOCKSIZE
  *                 result = self.iter(&buffer)
  */
       __pyx_v_buffer.next_out = ((char *)__pyx_v_out);
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":191
+      /* "pyrsync/backends/cython/_rsync.pyx":192
  *                 buffer.eof_in = not block
  *                 buffer.next_out = <char *> out
  *                 buffer.avail_out = <size_t> RS_JOB_BLOCKSIZE             # <<<<<<<<<<<<<<
  *                 result = self.iter(&buffer)
  *                 if output is not None:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 191, __pyx_L9_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 192, __pyx_L9_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 191, __pyx_L9_error)
+      __pyx_t_6 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 192, __pyx_L9_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_v_buffer.avail_out = ((size_t)__pyx_t_6);
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":192
+      /* "pyrsync/backends/cython/_rsync.pyx":193
  *                 buffer.next_out = <char *> out
  *                 buffer.avail_out = <size_t> RS_JOB_BLOCKSIZE
  *                 result = self.iter(&buffer)             # <<<<<<<<<<<<<<
  *                 if output is not None:
  *                     output.write(
  */
-      __pyx_v_result = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_iter(__pyx_v_self, (&__pyx_v_buffer));
+      __pyx_v_result = __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_iter(__pyx_v_self, (&__pyx_v_buffer));
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":193
+      /* "pyrsync/backends/cython/_rsync.pyx":194
  *                 buffer.avail_out = <size_t> RS_JOB_BLOCKSIZE
  *                 result = self.iter(&buffer)
  *                 if output is not None:             # <<<<<<<<<<<<<<
  *                     output.write(
  *                         PyBytes_FromStringAndSize(<char *> out, <Py_ssize_t> (RS_JOB_BLOCKSIZE - buffer.avail_out)))
  */
       __pyx_t_1 = (__pyx_v_output != Py_None);
       __pyx_t_5 = (__pyx_t_1 != 0);
       if (__pyx_t_5) {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":194
+        /* "pyrsync/backends/cython/_rsync.pyx":195
  *                 result = self.iter(&buffer)
  *                 if output is not None:
  *                     output.write(             # <<<<<<<<<<<<<<
  *                         PyBytes_FromStringAndSize(<char *> out, <Py_ssize_t> (RS_JOB_BLOCKSIZE - buffer.avail_out)))
  *                 if result == RS_DONE:
  */
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_output, __pyx_n_s_write); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 194, __pyx_L9_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_output, __pyx_n_s_write); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 195, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_3);
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":195
+        /* "pyrsync/backends/cython/_rsync.pyx":196
  *                 if output is not None:
  *                     output.write(
  *                         PyBytes_FromStringAndSize(<char *> out, <Py_ssize_t> (RS_JOB_BLOCKSIZE - buffer.avail_out)))             # <<<<<<<<<<<<<<
  *                 if result == RS_DONE:
  *                     break
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 195, __pyx_L9_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_RS_JOB_BLOCKSIZE); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 196, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_buffer.avail_out); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 195, __pyx_L9_error)
+        __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_buffer.avail_out); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 196, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_9 = PyNumber_Subtract(__pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 195, __pyx_L9_error)
+        __pyx_t_9 = PyNumber_Subtract(__pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 196, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 195, __pyx_L9_error)
+        __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L9_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_9 = PyBytes_FromStringAndSize(((char *)__pyx_v_out), ((Py_ssize_t)__pyx_t_10)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 195, __pyx_L9_error)
+        __pyx_t_9 = PyBytes_FromStringAndSize(((char *)__pyx_v_out), ((Py_ssize_t)__pyx_t_10)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 196, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_8 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_8)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_8);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_9);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 194, __pyx_L9_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 195, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":193
+        /* "pyrsync/backends/cython/_rsync.pyx":194
  *                 buffer.avail_out = <size_t> RS_JOB_BLOCKSIZE
  *                 result = self.iter(&buffer)
  *                 if output is not None:             # <<<<<<<<<<<<<<
  *                     output.write(
  *                         PyBytes_FromStringAndSize(<char *> out, <Py_ssize_t> (RS_JOB_BLOCKSIZE - buffer.avail_out)))
  */
       }
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":196
+      /* "pyrsync/backends/cython/_rsync.pyx":197
  *                     output.write(
  *                         PyBytes_FromStringAndSize(<char *> out, <Py_ssize_t> (RS_JOB_BLOCKSIZE - buffer.avail_out)))
  *                 if result == RS_DONE:             # <<<<<<<<<<<<<<
  *                     break
  *                 elif result != RS_BLOCKED:
  */
       __pyx_t_5 = ((__pyx_v_result == RS_DONE) != 0);
       if (__pyx_t_5) {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":197
+        /* "pyrsync/backends/cython/_rsync.pyx":198
  *                         PyBytes_FromStringAndSize(<char *> out, <Py_ssize_t> (RS_JOB_BLOCKSIZE - buffer.avail_out)))
  *                 if result == RS_DONE:
  *                     break             # <<<<<<<<<<<<<<
  *                 elif result != RS_BLOCKED:
  *                     raise LibrsyncError(result)
  */
         goto __pyx_L12_break;
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":196
+        /* "pyrsync/backends/cython/_rsync.pyx":197
  *                     output.write(
  *                         PyBytes_FromStringAndSize(<char *> out, <Py_ssize_t> (RS_JOB_BLOCKSIZE - buffer.avail_out)))
  *                 if result == RS_DONE:             # <<<<<<<<<<<<<<
  *                     break
  *                 elif result != RS_BLOCKED:
  */
       }
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":198
+      /* "pyrsync/backends/cython/_rsync.pyx":199
  *                 if result == RS_DONE:
  *                     break
  *                 elif result != RS_BLOCKED:             # <<<<<<<<<<<<<<
  *                     raise LibrsyncError(result)
  *                 if buffer.avail_in > 0:
  */
       __pyx_t_5 = ((__pyx_v_result != RS_BLOCKED) != 0);
       if (unlikely(__pyx_t_5)) {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":199
+        /* "pyrsync/backends/cython/_rsync.pyx":200
  *                     break
  *                 elif result != RS_BLOCKED:
  *                     raise LibrsyncError(result)             # <<<<<<<<<<<<<<
  *                 if buffer.avail_in > 0:
  *                     # There is data left in the input buffer, librsync did not consume
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LibrsyncError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 199, __pyx_L9_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LibrsyncError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 200, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_9 = __Pyx_PyInt_From_rs_result(__pyx_v_result); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 199, __pyx_L9_error)
+        __pyx_t_9 = __Pyx_PyInt_From_rs_result(__pyx_v_result); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 200, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_8 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_8)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_8);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_9);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 199, __pyx_L9_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 200, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_2, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __PYX_ERR(1, 199, __pyx_L9_error)
+        __PYX_ERR(1, 200, __pyx_L9_error)
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":198
+        /* "pyrsync/backends/cython/_rsync.pyx":199
  *                 if result == RS_DONE:
  *                     break
  *                 elif result != RS_BLOCKED:             # <<<<<<<<<<<<<<
  *                     raise LibrsyncError(result)
  *                 if buffer.avail_in > 0:
  */
       }
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":200
+      /* "pyrsync/backends/cython/_rsync.pyx":201
  *                 elif result != RS_BLOCKED:
  *                     raise LibrsyncError(result)
  *                 if buffer.avail_in > 0:             # <<<<<<<<<<<<<<
  *                     # There is data left in the input buffer, librsync did not consume
  *                     # all of it. Rewind the file a bit so we include that data in our
  */
       __pyx_t_5 = ((__pyx_v_buffer.avail_in > 0) != 0);
       if (__pyx_t_5) {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":205
+        /* "pyrsync/backends/cython/_rsync.pyx":206
  *                     # next read. It would be better to simply tack data to the end of
  *                     # this buffer, but that is very difficult in Python.
  *                     input.seek(input.tell() - buffer.avail_in)             # <<<<<<<<<<<<<<
  *         finally:
  *             PyMem_Free(out)
  */
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_seek); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 205, __pyx_L9_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_seek); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 206, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_tell); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 205, __pyx_L9_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_tell); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 206, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_8, function);
           }
         }
         __pyx_t_9 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 205, __pyx_L9_error)
+        if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 206, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_buffer.avail_in); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 205, __pyx_L9_error)
+        __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_buffer.avail_in); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 206, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_7 = PyNumber_Subtract(__pyx_t_9, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 205, __pyx_L9_error)
+        __pyx_t_7 = PyNumber_Subtract(__pyx_t_9, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 206, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_8 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_8)) {
@@ -4505,32 +4495,32 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 205, __pyx_L9_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 206, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":200
+        /* "pyrsync/backends/cython/_rsync.pyx":201
  *                 elif result != RS_BLOCKED:
  *                     raise LibrsyncError(result)
  *                 if buffer.avail_in > 0:             # <<<<<<<<<<<<<<
  *                     # There is data left in the input buffer, librsync did not consume
  *                     # all of it. Rewind the file a bit so we include that data in our
  */
       }
     }
     __pyx_L12_break:;
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":207
+  /* "pyrsync/backends/cython/_rsync.pyx":208
  *                     input.seek(input.tell() - buffer.avail_in)
  *         finally:
  *             PyMem_Free(out)             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
   /*finally:*/ {
@@ -4573,51 +4563,51 @@
       __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
       __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_12; __pyx_filename = __pyx_t_13;
       goto __pyx_L1_error;
     }
     __pyx_L10:;
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":208
+  /* "pyrsync/backends/cython/_rsync.pyx":209
  *         finally:
  *             PyMem_Free(out)
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":170
+  /* "pyrsync/backends/cython/_rsync.pyx":171
  *         return Stats.from_ptr(state)
  * 
  *     cpdef inline int execute(self, object input, object output = None) except -1:             # <<<<<<<<<<<<<<
  *         if not PyFile_Check(input):
  *             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_block);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_3execute(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_2execute[] = "Job.execute(self, input, output=None) -> int";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_3execute(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_3execute(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_2execute[] = "Job.execute(self, input, output=None) -> int";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_3execute(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_input = 0;
   PyObject *__pyx_v_output = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4646,15 +4636,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "execute") < 0)) __PYX_ERR(1, 170, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "execute") < 0)) __PYX_ERR(1, 171, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -4662,120 +4652,120 @@
       }
     }
     __pyx_v_input = values[0];
     __pyx_v_output = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("execute", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 170, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("execute", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 171, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_2execute(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_v_self), __pyx_v_input, __pyx_v_output);
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_2execute(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_v_self), __pyx_v_input, __pyx_v_output);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_2execute(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_2execute(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute __pyx_t_2;
+  struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("execute", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.output = __pyx_v_output;
-  __pyx_t_1 = __pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Job->execute(__pyx_v_self, __pyx_v_input, 1, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 170, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Job->execute(__pyx_v_self, __pyx_v_input, 1, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 171, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.execute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":210
+/* "pyrsync/backends/cython/_rsync.pyx":211
  *         return 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.job:
  *             rs_job_free(self.job)
  */
 
 /* Python wrapper */
-static void __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_5__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_5__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_4__dealloc__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_v_self));
+  __pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_4__dealloc__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_4__dealloc__(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self) {
+static void __pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_4__dealloc__(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":211
+  /* "pyrsync/backends/cython/_rsync.pyx":212
  * 
  *     def __dealloc__(self):
  *         if self.job:             # <<<<<<<<<<<<<<
  *             rs_job_free(self.job)
  *         self.job = NULL
  */
   __pyx_t_1 = (__pyx_v_self->job != 0);
   if (__pyx_t_1) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":212
+    /* "pyrsync/backends/cython/_rsync.pyx":213
  *     def __dealloc__(self):
  *         if self.job:
  *             rs_job_free(self.job)             # <<<<<<<<<<<<<<
  *         self.job = NULL
  * 
  */
     (void)(rs_job_free(__pyx_v_self->job));
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":211
+    /* "pyrsync/backends/cython/_rsync.pyx":212
  * 
  *     def __dealloc__(self):
  *         if self.job:             # <<<<<<<<<<<<<<
  *             rs_job_free(self.job)
  *         self.job = NULL
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":213
+  /* "pyrsync/backends/cython/_rsync.pyx":214
  *         if self.job:
  *             rs_job_free(self.job)
  *         self.job = NULL             # <<<<<<<<<<<<<<
  * 
  * cpdef inline tuple get_signature_args(rs_long_t old_fsize, int magic = 0, size_t block_len = 0, size_t strong_len= 0):
  */
   __pyx_v_self->job = NULL;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":210
+  /* "pyrsync/backends/cython/_rsync.pyx":211
  *         return 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.job:
  *             rs_job_free(self.job)
  */
 
@@ -4786,28 +4776,28 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.job cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_6__reduce_cython__[] = "Job.__reduce_cython__(self)";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_6__reduce_cython__[] = "Job.__reduce_cython__(self)";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_6__reduce_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_6__reduce_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -4829,43 +4819,43 @@
  *     raise TypeError("self.job cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("self.job cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.job cannot be converted to a Python object for pickling")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_8__setstate_cython__[] = "Job.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_8__setstate_cython__[] = "Job.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_8__setstate_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_8__setstate_cython__(((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_3Job_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_3Job_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -4887,31 +4877,31 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.job cannot be converted to a Python object for pickling")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.Job.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.Job.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":215
+/* "pyrsync/backends/cython/_rsync.pyx":216
  *         self.job = NULL
  * 
  * cpdef inline tuple get_signature_args(rs_long_t old_fsize, int magic = 0, size_t block_len = 0, size_t strong_len= 0):             # <<<<<<<<<<<<<<
  *     cdef:
  *         rs_result result
  */
 
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_1get_signature_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args(rs_long_t __pyx_v_old_fsize, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args *__pyx_optional_args) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_1get_signature_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_get_signature_args(rs_long_t __pyx_v_old_fsize, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_get_signature_args *__pyx_optional_args) {
   int __pyx_v_magic = ((int)0);
   size_t __pyx_v_block_len = ((size_t)0);
   size_t __pyx_v_strong_len = ((size_t)0);
   rs_result __pyx_v_result;
   rs_magic_number __pyx_v_c_magic;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -4932,49 +4922,49 @@
         if (__pyx_optional_args->__pyx_n > 2) {
           __pyx_v_strong_len = __pyx_optional_args->strong_len;
         }
       }
     }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":218
+  /* "pyrsync/backends/cython/_rsync.pyx":219
  *     cdef:
  *         rs_result result
  *         rs_magic_number c_magic = <rs_magic_number>magic             # <<<<<<<<<<<<<<
  *         # size_t cblock_len, strong_len
  *     with nogil:
  */
   __pyx_v_c_magic = ((rs_magic_number)__pyx_v_magic);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":220
+  /* "pyrsync/backends/cython/_rsync.pyx":221
  *         rs_magic_number c_magic = <rs_magic_number>magic
  *         # size_t cblock_len, strong_len
  *     with nogil:             # <<<<<<<<<<<<<<
  *         result = rs_sig_args(old_fsize, &c_magic, &block_len, &strong_len)
  *     if result != RS_DONE:
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":221
+        /* "pyrsync/backends/cython/_rsync.pyx":222
  *         # size_t cblock_len, strong_len
  *     with nogil:
  *         result = rs_sig_args(old_fsize, &c_magic, &block_len, &strong_len)             # <<<<<<<<<<<<<<
  *     if result != RS_DONE:
  *         raise LibrsyncError(result)
  */
         __pyx_v_result = rs_sig_args(__pyx_v_old_fsize, (&__pyx_v_c_magic), (&__pyx_v_block_len), (&__pyx_v_strong_len));
       }
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":220
+      /* "pyrsync/backends/cython/_rsync.pyx":221
  *         rs_magic_number c_magic = <rs_magic_number>magic
  *         # size_t cblock_len, strong_len
  *     with nogil:             # <<<<<<<<<<<<<<
  *         result = rs_sig_args(old_fsize, &c_magic, &block_len, &strong_len)
  *     if result != RS_DONE:
  */
       /*finally:*/ {
@@ -4985,119 +4975,119 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":222
+  /* "pyrsync/backends/cython/_rsync.pyx":223
  *     with nogil:
  *         result = rs_sig_args(old_fsize, &c_magic, &block_len, &strong_len)
  *     if result != RS_DONE:             # <<<<<<<<<<<<<<
  *         raise LibrsyncError(result)
  *     return c_magic, block_len, strong_len
  */
   __pyx_t_1 = ((__pyx_v_result != RS_DONE) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":223
+    /* "pyrsync/backends/cython/_rsync.pyx":224
  *         result = rs_sig_args(old_fsize, &c_magic, &block_len, &strong_len)
  *     if result != RS_DONE:
  *         raise LibrsyncError(result)             # <<<<<<<<<<<<<<
  *     return c_magic, block_len, strong_len
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LibrsyncError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 223, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LibrsyncError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_rs_result(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 223, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_rs_result(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 223, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 223, __pyx_L1_error)
+    __PYX_ERR(1, 224, __pyx_L1_error)
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":222
+    /* "pyrsync/backends/cython/_rsync.pyx":223
  *     with nogil:
  *         result = rs_sig_args(old_fsize, &c_magic, &block_len, &strong_len)
  *     if result != RS_DONE:             # <<<<<<<<<<<<<<
  *         raise LibrsyncError(result)
  *     return c_magic, block_len, strong_len
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":224
+  /* "pyrsync/backends/cython/_rsync.pyx":225
  *     if result != RS_DONE:
  *         raise LibrsyncError(result)
  *     return c_magic, block_len, strong_len             # <<<<<<<<<<<<<<
  * 
  * cpdef inline signature(object input, object output, size_t strong_len, rs_magic_number sig_magic,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_rs_magic_number(__pyx_v_c_magic); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 224, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_rs_magic_number(__pyx_v_c_magic); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_block_len); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 224, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_block_len); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_strong_len); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 224, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_strong_len); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 224, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":215
+  /* "pyrsync/backends/cython/_rsync.pyx":216
  *         self.job = NULL
  * 
  * cpdef inline tuple get_signature_args(rs_long_t old_fsize, int magic = 0, size_t block_len = 0, size_t strong_len= 0):             # <<<<<<<<<<<<<<
  *     cdef:
  *         rs_result result
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.get_signature_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.get_signature_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_1get_signature_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args[] = "get_signature_args(rs_long_t old_fsize, int magic=0, size_t block_len=0, size_t strong_len=0) -> tuple";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_1get_signature_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_1get_signature_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_get_signature_args[] = "get_signature_args(rs_long_t old_fsize, int magic=0, size_t block_len=0, size_t strong_len=0) -> tuple";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_1get_signature_args(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   rs_long_t __pyx_v_old_fsize;
   int __pyx_v_magic;
   size_t __pyx_v_block_len;
   size_t __pyx_v_strong_len;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5143,146 +5133,146 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_strong_len);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_signature_args") < 0)) __PYX_ERR(1, 215, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_signature_args") < 0)) __PYX_ERR(1, 216, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_old_fsize = __Pyx_PyInt_As_intmax_t(values[0]); if (unlikely((__pyx_v_old_fsize == ((rs_long_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 215, __pyx_L3_error)
+    __pyx_v_old_fsize = __Pyx_PyInt_As_intmax_t(values[0]); if (unlikely((__pyx_v_old_fsize == ((rs_long_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 216, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_magic = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_magic == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 215, __pyx_L3_error)
+      __pyx_v_magic = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_magic == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 216, __pyx_L3_error)
     } else {
       __pyx_v_magic = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_block_len = __Pyx_PyInt_As_size_t(values[2]); if (unlikely((__pyx_v_block_len == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 215, __pyx_L3_error)
+      __pyx_v_block_len = __Pyx_PyInt_As_size_t(values[2]); if (unlikely((__pyx_v_block_len == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 216, __pyx_L3_error)
     } else {
       __pyx_v_block_len = ((size_t)0);
     }
     if (values[3]) {
-      __pyx_v_strong_len = __Pyx_PyInt_As_size_t(values[3]); if (unlikely((__pyx_v_strong_len == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 215, __pyx_L3_error)
+      __pyx_v_strong_len = __Pyx_PyInt_As_size_t(values[3]); if (unlikely((__pyx_v_strong_len == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 216, __pyx_L3_error)
     } else {
       __pyx_v_strong_len = ((size_t)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_signature_args", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 215, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_signature_args", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 216, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.get_signature_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.get_signature_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args(__pyx_self, __pyx_v_old_fsize, __pyx_v_magic, __pyx_v_block_len, __pyx_v_strong_len);
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_get_signature_args(__pyx_self, __pyx_v_old_fsize, __pyx_v_magic, __pyx_v_block_len, __pyx_v_strong_len);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args(CYTHON_UNUSED PyObject *__pyx_self, rs_long_t __pyx_v_old_fsize, int __pyx_v_magic, size_t __pyx_v_block_len, size_t __pyx_v_strong_len) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_get_signature_args(CYTHON_UNUSED PyObject *__pyx_self, rs_long_t __pyx_v_old_fsize, int __pyx_v_magic, size_t __pyx_v_block_len, size_t __pyx_v_strong_len) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args __pyx_t_2;
+  struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_get_signature_args __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_signature_args", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 3;
   __pyx_t_2.magic = __pyx_v_magic;
   __pyx_t_2.block_len = __pyx_v_block_len;
   __pyx_t_2.strong_len = __pyx_v_strong_len;
-  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args(__pyx_v_old_fsize, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 215, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_get_signature_args(__pyx_v_old_fsize, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.get_signature_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.get_signature_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":226
+/* "pyrsync/backends/cython/_rsync.pyx":227
  *     return c_magic, block_len, strong_len
  * 
  * cpdef inline signature(object input, object output, size_t strong_len, rs_magic_number sig_magic,             # <<<<<<<<<<<<<<
  *                            size_t block_size=RS_DEFAULT_BLOCK_LEN):
  *     """
  */
 
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_signature(PyObject *__pyx_v_input, PyObject *__pyx_v_output, size_t __pyx_v_strong_len, rs_magic_number __pyx_v_sig_magic, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_signature *__pyx_optional_args) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_signature(PyObject *__pyx_v_input, PyObject *__pyx_v_output, size_t __pyx_v_strong_len, rs_magic_number __pyx_v_sig_magic, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_signature *__pyx_optional_args) {
   size_t __pyx_v_block_size = __pyx_k__5;
   rs_job_t *__pyx_v_c_job;
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_job = 0;
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_job = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
-  struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute __pyx_t_3;
+  struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signature", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_block_size = __pyx_optional_args->block_size;
     }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":239
+  /* "pyrsync/backends/cython/_rsync.pyx":240
  *     """
  *     cdef rs_job_t * c_job
  *     with nogil:             # <<<<<<<<<<<<<<
  *         c_job = rs_sig_begin(block_size, strong_len, sig_magic)
  *     cdef Job job = Job.from_ptr(c_job)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":240
+        /* "pyrsync/backends/cython/_rsync.pyx":241
  *     cdef rs_job_t * c_job
  *     with nogil:
  *         c_job = rs_sig_begin(block_size, strong_len, sig_magic)             # <<<<<<<<<<<<<<
  *     cdef Job job = Job.from_ptr(c_job)
  *     job.execute(input, output)
  */
         __pyx_v_c_job = rs_sig_begin(__pyx_v_block_size, __pyx_v_strong_len, __pyx_v_sig_magic);
       }
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":239
+      /* "pyrsync/backends/cython/_rsync.pyx":240
  *     """
  *     cdef rs_job_t * c_job
  *     with nogil:             # <<<<<<<<<<<<<<
  *         c_job = rs_sig_begin(block_size, strong_len, sig_magic)
  *     cdef Job job = Job.from_ptr(c_job)
  */
       /*finally:*/ {
@@ -5293,63 +5283,63 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":241
+  /* "pyrsync/backends/cython/_rsync.pyx":242
  *     with nogil:
  *         c_job = rs_sig_begin(block_size, strong_len, sig_magic)
  *     cdef Job job = Job.from_ptr(c_job)             # <<<<<<<<<<<<<<
  *     job.execute(input, output)
  * 
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 241, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_job = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_t_1);
+  __pyx_v_job = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":242
+  /* "pyrsync/backends/cython/_rsync.pyx":243
  *         c_job = rs_sig_begin(block_size, strong_len, sig_magic)
  *     cdef Job job = Job.from_ptr(c_job)
  *     job.execute(input, output)             # <<<<<<<<<<<<<<
  * 
  * cpdef inline delta(object input, object sigfile, object output):
  */
   __pyx_t_3.__pyx_n = 1;
   __pyx_t_3.output = __pyx_v_output;
-  __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute(__pyx_v_job, __pyx_v_input, 0, &__pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 242, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute(__pyx_v_job, __pyx_v_input, 0, &__pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 243, __pyx_L1_error)
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":226
+  /* "pyrsync/backends/cython/_rsync.pyx":227
  *     return c_magic, block_len, strong_len
  * 
  * cpdef inline signature(object input, object output, size_t strong_len, rs_magic_number sig_magic,             # <<<<<<<<<<<<<<
  *                            size_t block_size=RS_DEFAULT_BLOCK_LEN):
  *     """
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.signature", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.signature", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_job);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_2signature[] = "signature(input, output, size_t strong_len, rs_magic_number sig_magic, size_t block_size=RS_DEFAULT_BLOCK_LEN)\n\n     Generate a signature for the file input. The signature will be written to output.\n    You can specify the size of the blocks using the optional `block_size` parameter.\n    :param input: \n    :param output: \n    :param strong_len: \n    :param sig_magic: \n    :param block_size: \n    :return: \n    ";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_2signature[] = "signature(input, output, size_t strong_len, rs_magic_number sig_magic, size_t block_size=RS_DEFAULT_BLOCK_LEN)\n\n     Generate a signature for the file input. The signature will be written to output.\n    You can specify the size of the blocks using the optional `block_size` parameter.\n    :param input: \n    :param output: \n    :param strong_len: \n    :param sig_magic: \n    :param block_size: \n    :return: \n    ";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3signature(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_input = 0;
   PyObject *__pyx_v_output = 0;
   size_t __pyx_v_strong_len;
   rs_magic_number __pyx_v_sig_magic;
   size_t __pyx_v_block_size;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -5382,37 +5372,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_input)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, 1); __PYX_ERR(1, 226, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, 1); __PYX_ERR(1, 227, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_strong_len)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, 2); __PYX_ERR(1, 226, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, 2); __PYX_ERR(1, 227, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sig_magic)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, 3); __PYX_ERR(1, 226, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, 3); __PYX_ERR(1, 227, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_block_size);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "signature") < 0)) __PYX_ERR(1, 226, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "signature") < 0)) __PYX_ERR(1, 227, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -5420,167 +5410,167 @@
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_input = values[0];
     __pyx_v_output = values[1];
-    __pyx_v_strong_len = __Pyx_PyInt_As_size_t(values[2]); if (unlikely((__pyx_v_strong_len == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 226, __pyx_L3_error)
-    __pyx_v_sig_magic = ((rs_magic_number)__Pyx_PyInt_As_rs_magic_number(values[3])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 226, __pyx_L3_error)
+    __pyx_v_strong_len = __Pyx_PyInt_As_size_t(values[2]); if (unlikely((__pyx_v_strong_len == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 227, __pyx_L3_error)
+    __pyx_v_sig_magic = ((rs_magic_number)__Pyx_PyInt_As_rs_magic_number(values[3])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 227, __pyx_L3_error)
     if (values[4]) {
-      __pyx_v_block_size = __Pyx_PyInt_As_size_t(values[4]); if (unlikely((__pyx_v_block_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 227, __pyx_L3_error)
+      __pyx_v_block_size = __Pyx_PyInt_As_size_t(values[4]); if (unlikely((__pyx_v_block_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 228, __pyx_L3_error)
     } else {
       __pyx_v_block_size = __pyx_k__5;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 226, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("signature", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 227, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.signature", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.signature", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_2signature(__pyx_self, __pyx_v_input, __pyx_v_output, __pyx_v_strong_len, __pyx_v_sig_magic, __pyx_v_block_size);
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_2signature(__pyx_self, __pyx_v_input, __pyx_v_output, __pyx_v_strong_len, __pyx_v_sig_magic, __pyx_v_block_size);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_2signature(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output, size_t __pyx_v_strong_len, rs_magic_number __pyx_v_sig_magic, size_t __pyx_v_block_size) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_2signature(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_output, size_t __pyx_v_strong_len, rs_magic_number __pyx_v_sig_magic, size_t __pyx_v_block_size) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_signature __pyx_t_2;
+  struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_signature __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signature", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.block_size = __pyx_v_block_size;
-  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_signature(__pyx_v_input, __pyx_v_output, __pyx_v_strong_len, __pyx_v_sig_magic, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_signature(__pyx_v_input, __pyx_v_output, __pyx_v_strong_len, __pyx_v_sig_magic, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.signature", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.signature", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":244
+/* "pyrsync/backends/cython/_rsync.pyx":245
  *     job.execute(input, output)
  * 
  * cpdef inline delta(object input, object sigfile, object output):             # <<<<<<<<<<<<<<
  *     """
  *     Create a delta for the file input using the signature read from sigfile. The delta
  */
 
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5delta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_delta(PyObject *__pyx_v_input, PyObject *__pyx_v_sigfile, PyObject *__pyx_v_output, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5delta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_delta(PyObject *__pyx_v_input, PyObject *__pyx_v_sigfile, PyObject *__pyx_v_output, CYTHON_UNUSED int __pyx_skip_dispatch) {
   rs_signature_t *__pyx_v_sig;
   rs_job_t *__pyx_v_c_job;
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_job = 0;
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_job = 0;
   rs_result __pyx_v_result;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute __pyx_t_7;
+  struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute __pyx_t_7;
   int __pyx_t_8;
   char const *__pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delta", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":255
+  /* "pyrsync/backends/cython/_rsync.pyx":256
  *     cdef:
  *         rs_signature_t* sig
  *         rs_job_t * c_job = rs_loadsig_begin(&sig)             # <<<<<<<<<<<<<<
  *         Job job
  *         rs_result result
  */
   __pyx_v_c_job = rs_loadsig_begin((&__pyx_v_sig));
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":258
+  /* "pyrsync/backends/cython/_rsync.pyx":259
  *         Job job
  *         rs_result result
  *     try:             # <<<<<<<<<<<<<<
  *         job = Job.from_ptr(c_job)
  *         job.execute(sigfile)
  */
   /*try:*/ {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":259
+    /* "pyrsync/backends/cython/_rsync.pyx":260
  *         rs_result result
  *     try:
  *         job = Job.from_ptr(c_job)             # <<<<<<<<<<<<<<
  *         job.execute(sigfile)
  *         with nogil:
  */
-    __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 259, __pyx_L4_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 260, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_v_job = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_t_1);
+    __pyx_v_job = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":260
+    /* "pyrsync/backends/cython/_rsync.pyx":261
  *     try:
  *         job = Job.from_ptr(c_job)
  *         job.execute(sigfile)             # <<<<<<<<<<<<<<
  *         with nogil:
  *             result = rs_build_hash_table(sig)
  */
-    __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute(__pyx_v_job, __pyx_v_sigfile, 0, NULL); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 260, __pyx_L4_error)
+    __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute(__pyx_v_job, __pyx_v_sigfile, 0, NULL); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 261, __pyx_L4_error)
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":261
+    /* "pyrsync/backends/cython/_rsync.pyx":262
  *         job = Job.from_ptr(c_job)
  *         job.execute(sigfile)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             result = rs_build_hash_table(sig)
  *         if result != RS_DONE:
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "pyrsync/backends/cython/_rsync_cy.pyx":262
+          /* "pyrsync/backends/cython/_rsync.pyx":263
  *         job.execute(sigfile)
  *         with nogil:
  *             result = rs_build_hash_table(sig)             # <<<<<<<<<<<<<<
  *         if result != RS_DONE:
  *             raise LibrsyncError(result)
  */
           __pyx_v_result = rs_build_hash_table(__pyx_v_sig);
         }
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":261
+        /* "pyrsync/backends/cython/_rsync.pyx":262
  *         job = Job.from_ptr(c_job)
  *         job.execute(sigfile)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             result = rs_build_hash_table(sig)
  *         if result != RS_DONE:
  */
         /*finally:*/ {
@@ -5591,90 +5581,90 @@
             #endif
             goto __pyx_L8;
           }
           __pyx_L8:;
         }
     }
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":263
+    /* "pyrsync/backends/cython/_rsync.pyx":264
  *         with nogil:
  *             result = rs_build_hash_table(sig)
  *         if result != RS_DONE:             # <<<<<<<<<<<<<<
  *             raise LibrsyncError(result)
  *         with nogil:
  */
     __pyx_t_3 = ((__pyx_v_result != RS_DONE) != 0);
     if (unlikely(__pyx_t_3)) {
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":264
+      /* "pyrsync/backends/cython/_rsync.pyx":265
  *             result = rs_build_hash_table(sig)
  *         if result != RS_DONE:
  *             raise LibrsyncError(result)             # <<<<<<<<<<<<<<
  *         with nogil:
  *             c_job = rs_delta_begin(sig)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_LibrsyncError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 264, __pyx_L4_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_LibrsyncError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 265, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_From_rs_result(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 264, __pyx_L4_error)
+      __pyx_t_5 = __Pyx_PyInt_From_rs_result(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 265, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 264, __pyx_L4_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 265, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(1, 264, __pyx_L4_error)
+      __PYX_ERR(1, 265, __pyx_L4_error)
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":263
+      /* "pyrsync/backends/cython/_rsync.pyx":264
  *         with nogil:
  *             result = rs_build_hash_table(sig)
  *         if result != RS_DONE:             # <<<<<<<<<<<<<<
  *             raise LibrsyncError(result)
  *         with nogil:
  */
     }
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":265
+    /* "pyrsync/backends/cython/_rsync.pyx":266
  *         if result != RS_DONE:
  *             raise LibrsyncError(result)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_job = rs_delta_begin(sig)
  *         job = Job.from_ptr(c_job)
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "pyrsync/backends/cython/_rsync_cy.pyx":266
+          /* "pyrsync/backends/cython/_rsync.pyx":267
  *             raise LibrsyncError(result)
  *         with nogil:
  *             c_job = rs_delta_begin(sig)             # <<<<<<<<<<<<<<
  *         job = Job.from_ptr(c_job)
  *         return job.execute(input, output)
  */
           __pyx_v_c_job = rs_delta_begin(__pyx_v_sig);
         }
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":265
+        /* "pyrsync/backends/cython/_rsync.pyx":266
  *         if result != RS_DONE:
  *             raise LibrsyncError(result)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_job = rs_delta_begin(sig)
  *         job = Job.from_ptr(c_job)
  */
         /*finally:*/ {
@@ -5685,45 +5675,45 @@
             #endif
             goto __pyx_L12;
           }
           __pyx_L12:;
         }
     }
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":267
+    /* "pyrsync/backends/cython/_rsync.pyx":268
  *         with nogil:
  *             c_job = rs_delta_begin(sig)
  *         job = Job.from_ptr(c_job)             # <<<<<<<<<<<<<<
  *         return job.execute(input, output)
  *     finally:
  */
-    __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 267, __pyx_L4_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 268, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF_SET(__pyx_v_job, ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_t_1));
+    __Pyx_DECREF_SET(__pyx_v_job, ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":268
+    /* "pyrsync/backends/cython/_rsync.pyx":269
  *             c_job = rs_delta_begin(sig)
  *         job = Job.from_ptr(c_job)
  *         return job.execute(input, output)             # <<<<<<<<<<<<<<
  *     finally:
  *         rs_free_sumset(sig)
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_7.__pyx_n = 1;
     __pyx_t_7.output = __pyx_v_output;
-    __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute(__pyx_v_job, __pyx_v_input, 0, &__pyx_t_7); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 268, __pyx_L4_error)
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 268, __pyx_L4_error)
+    __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute(__pyx_v_job, __pyx_v_input, 0, &__pyx_t_7); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 269, __pyx_L4_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 269, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L3_return;
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":270
+  /* "pyrsync/backends/cython/_rsync.pyx":271
  *         return job.execute(input, output)
  *     finally:
  *         rs_free_sumset(sig)             # <<<<<<<<<<<<<<
  * 
  * cdef struct input_args:
  */
   /*finally:*/ {
@@ -5768,41 +5758,41 @@
       rs_free_sumset(__pyx_v_sig);
       __pyx_r = __pyx_t_15;
       __pyx_t_15 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":244
+  /* "pyrsync/backends/cython/_rsync.pyx":245
  *     job.execute(input, output)
  * 
  * cpdef inline delta(object input, object sigfile, object output):             # <<<<<<<<<<<<<<
  *     """
  *     Create a delta for the file input using the signature read from sigfile. The delta
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.delta", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.delta", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_job);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5delta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_4delta[] = "delta(input, sigfile, output)\n\n    Create a delta for the file input using the signature read from sigfile. The delta\n    will be written to  output.\n    :param input: \n    :param sigfile: \n    :param output: delta file\n    :return: \n    ";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5delta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5delta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_4delta[] = "delta(input, sigfile, output)\n\n    Create a delta for the file input using the signature read from sigfile. The delta\n    will be written to  output.\n    :param input: \n    :param sigfile: \n    :param output: delta file\n    :return: \n    ";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5delta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_input = 0;
   PyObject *__pyx_v_sigfile = 0;
   PyObject *__pyx_v_output = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -5829,88 +5819,88 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_input)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sigfile)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("delta", 1, 3, 3, 1); __PYX_ERR(1, 244, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("delta", 1, 3, 3, 1); __PYX_ERR(1, 245, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("delta", 1, 3, 3, 2); __PYX_ERR(1, 244, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("delta", 1, 3, 3, 2); __PYX_ERR(1, 245, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "delta") < 0)) __PYX_ERR(1, 244, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "delta") < 0)) __PYX_ERR(1, 245, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_input = values[0];
     __pyx_v_sigfile = values[1];
     __pyx_v_output = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("delta", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 244, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("delta", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 245, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.delta", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.delta", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_4delta(__pyx_self, __pyx_v_input, __pyx_v_sigfile, __pyx_v_output);
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_4delta(__pyx_self, __pyx_v_input, __pyx_v_sigfile, __pyx_v_output);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_4delta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_sigfile, PyObject *__pyx_v_output) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_4delta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_sigfile, PyObject *__pyx_v_output) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delta", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_delta(__pyx_v_input, __pyx_v_sigfile, __pyx_v_output, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 244, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_delta(__pyx_v_input, __pyx_v_sigfile, __pyx_v_output, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.delta", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.delta", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":277
+/* "pyrsync/backends/cython/_rsync.pyx":278
  *     Py_ssize_t len
  * 
- * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) with gil:             # <<<<<<<<<<<<<<
+ * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) except * with gil:             # <<<<<<<<<<<<<<
  *     cdef  input_args* args = <input_args*>opaque
  *     input = <object>args.file
  */
 
-static rs_result __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_read_cb(void *__pyx_v_opaque, rs_long_t __pyx_v_pos, size_t *__pyx_v_len, void **__pyx_v_buf) {
-  struct __pyx_t_7pyrsync_8backends_6cython_9_rsync_cy_input_args *__pyx_v_args;
+static rs_result __pyx_f_7pyrsync_8backends_6cython_6_rsync_read_cb(void *__pyx_v_opaque, rs_long_t __pyx_v_pos, size_t *__pyx_v_len, void **__pyx_v_buf) {
+  struct __pyx_t_7pyrsync_8backends_6cython_6_rsync_input_args *__pyx_v_args;
   PyObject *__pyx_v_input = NULL;
   PyObject *__pyx_v_block = NULL;
   Py_ssize_t __pyx_v_block_size;
   void *__pyx_v_temp;
   rs_result __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -5923,325 +5913,325 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("read_cb", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":278
+  /* "pyrsync/backends/cython/_rsync.pyx":279
  * 
- * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) with gil:
+ * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) except * with gil:
  *     cdef  input_args* args = <input_args*>opaque             # <<<<<<<<<<<<<<
  *     input = <object>args.file
  *     input.seek(pos)
  */
-  __pyx_v_args = ((struct __pyx_t_7pyrsync_8backends_6cython_9_rsync_cy_input_args *)__pyx_v_opaque);
+  __pyx_v_args = ((struct __pyx_t_7pyrsync_8backends_6cython_6_rsync_input_args *)__pyx_v_opaque);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":279
- * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) with gil:
+  /* "pyrsync/backends/cython/_rsync.pyx":280
+ * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) except * with gil:
  *     cdef  input_args* args = <input_args*>opaque
  *     input = <object>args.file             # <<<<<<<<<<<<<<
  *     input.seek(pos)
  *     block = input.read(len[0]) # type: bytes
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_args->file);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_input = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":280
+  /* "pyrsync/backends/cython/_rsync.pyx":281
  *     cdef  input_args* args = <input_args*>opaque
  *     input = <object>args.file
  *     input.seek(pos)             # <<<<<<<<<<<<<<
  *     block = input.read(len[0]) # type: bytes
  *     cdef Py_ssize_t block_size = PyBytes_GET_SIZE(block)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_seek); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 280, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_seek); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_intmax_t(__pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 280, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_intmax_t(__pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":281
+  /* "pyrsync/backends/cython/_rsync.pyx":282
  *     input = <object>args.file
  *     input.seek(pos)
  *     block = input.read(len[0]) # type: bytes             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t block_size = PyBytes_GET_SIZE(block)
  *     cdef void* temp
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 281, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_input, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t((__pyx_v_len[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 281, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t((__pyx_v_len[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 281, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_block = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":282
+  /* "pyrsync/backends/cython/_rsync.pyx":283
  *     input.seek(pos)
  *     block = input.read(len[0]) # type: bytes
  *     cdef Py_ssize_t block_size = PyBytes_GET_SIZE(block)             # <<<<<<<<<<<<<<
  *     cdef void* temp
  *     if block_size > args.len:
  */
   __pyx_v_block_size = PyBytes_GET_SIZE(__pyx_v_block);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":284
+  /* "pyrsync/backends/cython/_rsync.pyx":285
  *     cdef Py_ssize_t block_size = PyBytes_GET_SIZE(block)
  *     cdef void* temp
  *     if block_size > args.len:             # <<<<<<<<<<<<<<
  *         temp = PyMem_Realloc(<void*>args.buffer, <size_t>block_size)
  *         if temp==NULL:
  */
   __pyx_t_5 = ((__pyx_v_block_size > __pyx_v_args->len) != 0);
   if (__pyx_t_5) {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":285
+    /* "pyrsync/backends/cython/_rsync.pyx":286
  *     cdef void* temp
  *     if block_size > args.len:
  *         temp = PyMem_Realloc(<void*>args.buffer, <size_t>block_size)             # <<<<<<<<<<<<<<
  *         if temp==NULL:
- *             raise
+ *             raise MemoryError
  */
     __pyx_v_temp = PyMem_Realloc(((void *)__pyx_v_args->buffer), ((size_t)__pyx_v_block_size));
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":286
+    /* "pyrsync/backends/cython/_rsync.pyx":287
  *     if block_size > args.len:
  *         temp = PyMem_Realloc(<void*>args.buffer, <size_t>block_size)
  *         if temp==NULL:             # <<<<<<<<<<<<<<
- *             raise
+ *             raise MemoryError
  *         args.buffer = <char*>temp
  */
     __pyx_t_5 = ((__pyx_v_temp == NULL) != 0);
     if (unlikely(__pyx_t_5)) {
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":287
+      /* "pyrsync/backends/cython/_rsync.pyx":288
  *         temp = PyMem_Realloc(<void*>args.buffer, <size_t>block_size)
  *         if temp==NULL:
- *             raise             # <<<<<<<<<<<<<<
+ *             raise MemoryError             # <<<<<<<<<<<<<<
  *         args.buffer = <char*>temp
  *         args.len = block_size
  */
-      __Pyx_ReraiseException(); __PYX_ERR(1, 287, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(1, 288, __pyx_L1_error)
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":286
+      /* "pyrsync/backends/cython/_rsync.pyx":287
  *     if block_size > args.len:
  *         temp = PyMem_Realloc(<void*>args.buffer, <size_t>block_size)
  *         if temp==NULL:             # <<<<<<<<<<<<<<
- *             raise
+ *             raise MemoryError
  *         args.buffer = <char*>temp
  */
     }
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":288
+    /* "pyrsync/backends/cython/_rsync.pyx":289
  *         if temp==NULL:
- *             raise
+ *             raise MemoryError
  *         args.buffer = <char*>temp             # <<<<<<<<<<<<<<
  *         args.len = block_size
  * 
  */
     __pyx_v_args->buffer = ((char *)__pyx_v_temp);
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":289
- *             raise
+    /* "pyrsync/backends/cython/_rsync.pyx":290
+ *             raise MemoryError
  *         args.buffer = <char*>temp
  *         args.len = block_size             # <<<<<<<<<<<<<<
  * 
  *     len[0] = <size_t>block_size
  */
     __pyx_v_args->len = __pyx_v_block_size;
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":284
+    /* "pyrsync/backends/cython/_rsync.pyx":285
  *     cdef Py_ssize_t block_size = PyBytes_GET_SIZE(block)
  *     cdef void* temp
  *     if block_size > args.len:             # <<<<<<<<<<<<<<
  *         temp = PyMem_Realloc(<void*>args.buffer, <size_t>block_size)
  *         if temp==NULL:
  */
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":291
+  /* "pyrsync/backends/cython/_rsync.pyx":292
  *         args.len = block_size
  * 
  *     len[0] = <size_t>block_size             # <<<<<<<<<<<<<<
  *     memcpy(args.buffer, PyBytes_AS_STRING(block), <size_t>block_size)
  *     (<char**> buf)[0] = args.buffer
  */
   (__pyx_v_len[0]) = ((size_t)__pyx_v_block_size);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":292
+  /* "pyrsync/backends/cython/_rsync.pyx":293
  * 
  *     len[0] = <size_t>block_size
  *     memcpy(args.buffer, PyBytes_AS_STRING(block), <size_t>block_size)             # <<<<<<<<<<<<<<
  *     (<char**> buf)[0] = args.buffer
  *     return RS_DONE
  */
   (void)(memcpy(__pyx_v_args->buffer, PyBytes_AS_STRING(__pyx_v_block), ((size_t)__pyx_v_block_size)));
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":293
+  /* "pyrsync/backends/cython/_rsync.pyx":294
  *     len[0] = <size_t>block_size
  *     memcpy(args.buffer, PyBytes_AS_STRING(block), <size_t>block_size)
  *     (<char**> buf)[0] = args.buffer             # <<<<<<<<<<<<<<
  *     return RS_DONE
  * 
  */
   __pyx_t_6 = __pyx_v_args->buffer;
   (((char **)__pyx_v_buf)[0]) = __pyx_t_6;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":294
+  /* "pyrsync/backends/cython/_rsync.pyx":295
  *     memcpy(args.buffer, PyBytes_AS_STRING(block), <size_t>block_size)
  *     (<char**> buf)[0] = args.buffer
  *     return RS_DONE             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = RS_DONE;
   goto __pyx_L0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":277
+  /* "pyrsync/backends/cython/_rsync.pyx":278
  *     Py_ssize_t len
  * 
- * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) with gil:             # <<<<<<<<<<<<<<
+ * cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) except * with gil:             # <<<<<<<<<<<<<<
  *     cdef  input_args* args = <input_args*>opaque
  *     input = <object>args.file
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_WriteUnraisable("pyrsync.backends.cython._rsync_cy.read_cb", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.read_cb", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = (rs_result) 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_input);
   __Pyx_XDECREF(__pyx_v_block);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "pyrsync/backends/cython/_rsync_cy.pyx":297
+/* "pyrsync/backends/cython/_rsync.pyx":298
  * 
  * 
  * cpdef inline patch(object input, object delta, object output):             # <<<<<<<<<<<<<<
  *     """
  *     Patch the file  input using the delta . The patched file will be written to
  */
 
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_7patch(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_patch(PyObject *__pyx_v_input, PyObject *__pyx_v_delta, PyObject *__pyx_v_output, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  struct __pyx_t_7pyrsync_8backends_6cython_9_rsync_cy_input_args __pyx_v_args;
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_7patch(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_f_7pyrsync_8backends_6cython_6_rsync_patch(PyObject *__pyx_v_input, PyObject *__pyx_v_delta, PyObject *__pyx_v_output, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  struct __pyx_t_7pyrsync_8backends_6cython_6_rsync_input_args __pyx_v_args;
   rs_job_t *__pyx_v_c_job;
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_v_job = 0;
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_v_job = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
-  struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute __pyx_t_3;
+  struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute __pyx_t_3;
   int __pyx_t_4;
   char const *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("patch", 0);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":307
+  /* "pyrsync/backends/cython/_rsync.pyx":308
  *     """
  *     cdef input_args args
  *     args.file= <PyObject *>input             # <<<<<<<<<<<<<<
  *     args.buffer = NULL
  *     args.len = 0
  */
   __pyx_v_args.file = ((PyObject *)__pyx_v_input);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":308
+  /* "pyrsync/backends/cython/_rsync.pyx":309
  *     cdef input_args args
  *     args.file= <PyObject *>input
  *     args.buffer = NULL             # <<<<<<<<<<<<<<
  *     args.len = 0
  *     cdef rs_job_t * c_job
  */
   __pyx_v_args.buffer = NULL;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":309
+  /* "pyrsync/backends/cython/_rsync.pyx":310
  *     args.file= <PyObject *>input
  *     args.buffer = NULL
  *     args.len = 0             # <<<<<<<<<<<<<<
  *     cdef rs_job_t * c_job
  *     with nogil:
  */
   __pyx_v_args.len = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":311
+  /* "pyrsync/backends/cython/_rsync.pyx":312
  *     args.len = 0
  *     cdef rs_job_t * c_job
  *     with nogil:             # <<<<<<<<<<<<<<
  *         c_job = rs_patch_begin(read_cb, <void*>&args)
  *     cdef Job job = Job.from_ptr(c_job)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyrsync/backends/cython/_rsync_cy.pyx":312
+        /* "pyrsync/backends/cython/_rsync.pyx":313
  *     cdef rs_job_t * c_job
  *     with nogil:
  *         c_job = rs_patch_begin(read_cb, <void*>&args)             # <<<<<<<<<<<<<<
  *     cdef Job job = Job.from_ptr(c_job)
  *     try:
  */
-        __pyx_v_c_job = rs_patch_begin(__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_read_cb, ((void *)(&__pyx_v_args)));
+        __pyx_v_c_job = rs_patch_begin(__pyx_f_7pyrsync_8backends_6cython_6_rsync_read_cb, ((void *)(&__pyx_v_args)));
       }
 
-      /* "pyrsync/backends/cython/_rsync_cy.pyx":311
+      /* "pyrsync/backends/cython/_rsync.pyx":312
  *     args.len = 0
  *     cdef rs_job_t * c_job
  *     with nogil:             # <<<<<<<<<<<<<<
  *         c_job = rs_patch_begin(read_cb, <void*>&args)
  *     cdef Job job = Job.from_ptr(c_job)
  */
       /*finally:*/ {
@@ -6252,48 +6242,48 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":313
+  /* "pyrsync/backends/cython/_rsync.pyx":314
  *     with nogil:
  *         c_job = rs_patch_begin(read_cb, <void*>&args)
  *     cdef Job job = Job.from_ptr(c_job)             # <<<<<<<<<<<<<<
  *     try:
  *         job.execute(delta, output)
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 313, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr(__pyx_v_c_job)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_job = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)__pyx_t_1);
+  __pyx_v_job = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":314
+  /* "pyrsync/backends/cython/_rsync.pyx":315
  *         c_job = rs_patch_begin(read_cb, <void*>&args)
  *     cdef Job job = Job.from_ptr(c_job)
  *     try:             # <<<<<<<<<<<<<<
  *         job.execute(delta, output)
  *     finally:
  */
   /*try:*/ {
 
-    /* "pyrsync/backends/cython/_rsync_cy.pyx":315
+    /* "pyrsync/backends/cython/_rsync.pyx":316
  *     cdef Job job = Job.from_ptr(c_job)
  *     try:
  *         job.execute(delta, output)             # <<<<<<<<<<<<<<
  *     finally:
  *         PyMem_Free(args.buffer)
  */
     __pyx_t_3.__pyx_n = 1;
     __pyx_t_3.output = __pyx_v_output;
-    __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute(__pyx_v_job, __pyx_v_delta, 0, &__pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 315, __pyx_L7_error)
+    __pyx_t_2 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute(__pyx_v_job, __pyx_v_delta, 0, &__pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 316, __pyx_L7_error)
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":317
+  /* "pyrsync/backends/cython/_rsync.pyx":318
  *         job.execute(delta, output)
  *     finally:
  *         PyMem_Free(args.buffer)             # <<<<<<<<<<<<<<
  */
   /*finally:*/ {
     /*normal exit:*/{
       PyMem_Free(__pyx_v_args.buffer);
@@ -6330,40 +6320,40 @@
       __pyx_t_6 = 0; __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0;
       __pyx_lineno = __pyx_t_2; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_5;
       goto __pyx_L1_error;
     }
     __pyx_L8:;
   }
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":297
+  /* "pyrsync/backends/cython/_rsync.pyx":298
  * 
  * 
  * cpdef inline patch(object input, object delta, object output):             # <<<<<<<<<<<<<<
  *     """
  *     Patch the file  input using the delta . The patched file will be written to
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.patch", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.patch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_job);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_7patch(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_6patch[] = "patch(input, delta, output)\n\n    Patch the file  input using the delta . The patched file will be written to\n    output.\n    :param input: \n    :param delta: \n    :param output: \n    :return: \n    ";
-static PyObject *__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_7patch(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_7patch(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7pyrsync_8backends_6cython_6_rsync_6patch[] = "patch(input, delta, output)\n\n    Patch the file  input using the delta . The patched file will be written to\n    output.\n    :param input: \n    :param delta: \n    :param output: \n    :return: \n    ";
+static PyObject *__pyx_pw_7pyrsync_8backends_6cython_6_rsync_7patch(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_input = 0;
   PyObject *__pyx_v_delta = 0;
   PyObject *__pyx_v_output = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -6390,202 +6380,202 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_input)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_delta)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("patch", 1, 3, 3, 1); __PYX_ERR(1, 297, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("patch", 1, 3, 3, 1); __PYX_ERR(1, 298, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("patch", 1, 3, 3, 2); __PYX_ERR(1, 297, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("patch", 1, 3, 3, 2); __PYX_ERR(1, 298, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "patch") < 0)) __PYX_ERR(1, 297, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "patch") < 0)) __PYX_ERR(1, 298, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_input = values[0];
     __pyx_v_delta = values[1];
     __pyx_v_output = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("patch", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 297, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("patch", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 298, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.patch", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.patch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_6patch(__pyx_self, __pyx_v_input, __pyx_v_delta, __pyx_v_output);
+  __pyx_r = __pyx_pf_7pyrsync_8backends_6cython_6_rsync_6patch(__pyx_self, __pyx_v_input, __pyx_v_delta, __pyx_v_output);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7pyrsync_8backends_6cython_9_rsync_cy_6patch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_delta, PyObject *__pyx_v_output) {
+static PyObject *__pyx_pf_7pyrsync_8backends_6cython_6_rsync_6patch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input, PyObject *__pyx_v_delta, PyObject *__pyx_v_output) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("patch", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_patch(__pyx_v_input, __pyx_v_delta, __pyx_v_output, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 297, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7pyrsync_8backends_6cython_6_rsync_patch(__pyx_v_input, __pyx_v_delta, __pyx_v_output, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pyrsync.backends.cython._rsync_cy.patch", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyrsync.backends.cython._rsync.patch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Stats __pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Stats;
+static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Stats __pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Stats;
 
-static struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *__pyx_freelist_7pyrsync_8backends_6cython_9_rsync_cy_Stats[8];
-static int __pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Stats = 0;
+static struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *__pyx_freelist_7pyrsync_8backends_6cython_6_rsync_Stats[8];
+static int __pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Stats = 0;
 
-static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Stats(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *p;
+static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Stats(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *p;
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Stats > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats)))) {
-    o = (PyObject*)__pyx_freelist_7pyrsync_8backends_6cython_9_rsync_cy_Stats[--__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Stats];
-    memset(o, 0, sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Stats > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats)))) {
+    o = (PyObject*)__pyx_freelist_7pyrsync_8backends_6cython_6_rsync_Stats[--__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Stats];
+    memset(o, 0, sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats));
     (void) PyObject_INIT(o, t);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
-  p = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)o);
-  p->__pyx_vtab = __pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Stats;
+  p = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)o);
+  p->__pyx_vtab = __pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Stats;
   return o;
 }
 
-static void __pyx_tp_dealloc_7pyrsync_8backends_6cython_9_rsync_cy_Stats(PyObject *o) {
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Stats < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats)))) {
-    __pyx_freelist_7pyrsync_8backends_6cython_9_rsync_cy_Stats[__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Stats++] = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *)o);
+static void __pyx_tp_dealloc_7pyrsync_8backends_6cython_6_rsync_Stats(PyObject *o) {
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Stats < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats)))) {
+    __pyx_freelist_7pyrsync_8backends_6cython_6_rsync_Stats[__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Stats++] = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_op(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2op_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_op(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_2op_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_lit_cmds(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8lit_cmds_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_lit_cmds(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8lit_cmds_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_lit_bytes(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9lit_bytes_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_lit_bytes(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9lit_bytes_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_lit_cmdbytes(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_12lit_cmdbytes_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_lit_cmdbytes(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_12lit_cmdbytes_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_copy_cmds(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9copy_cmds_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_copy_cmds(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9copy_cmds_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_copy_bytes(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10copy_bytes_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_copy_bytes(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_10copy_bytes_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_copy_cmdbytes(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13copy_cmdbytes_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_copy_cmdbytes(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_13copy_cmdbytes_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_sig_cmds(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8sig_cmds_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_sig_cmds(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8sig_cmds_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_sig_bytes(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9sig_bytes_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_sig_bytes(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9sig_bytes_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_false_matches(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_13false_matches_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_false_matches(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_13false_matches_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_sig_blocks(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_10sig_blocks_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_sig_blocks(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_10sig_blocks_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_block_len(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9block_len_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_block_len(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9block_len_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_in_bytes(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_8in_bytes_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_in_bytes(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_8in_bytes_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_out_bytes(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_9out_bytes_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_out_bytes(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_9out_bytes_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_start(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_5start_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_start(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_5start_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_end(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3end_1__get__(o);
+static PyObject *__pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_end(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_3end_1__get__(o);
 }
 
-static PyMethodDef __pyx_methods_7pyrsync_8backends_6cython_9_rsync_cy_Stats[] = {
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_1__reduce_cython__, METH_NOARGS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_5Stats___reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_3__setstate_cython__, METH_O, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_2__setstate_cython__},
+static PyMethodDef __pyx_methods_7pyrsync_8backends_6cython_6_rsync_Stats[] = {
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_1__reduce_cython__, METH_NOARGS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_5Stats___reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5Stats_3__setstate_cython__, METH_O, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_5Stats_2__setstate_cython__},
   {0, 0, 0, 0}
 };
 
-static struct PyGetSetDef __pyx_getsets_7pyrsync_8backends_6cython_9_rsync_cy_Stats[] = {
-  {(char *)"op", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_op, 0, (char *)0, 0},
-  {(char *)"lit_cmds", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_lit_cmds, 0, (char *)0, 0},
-  {(char *)"lit_bytes", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_lit_bytes, 0, (char *)0, 0},
-  {(char *)"lit_cmdbytes", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_lit_cmdbytes, 0, (char *)0, 0},
-  {(char *)"copy_cmds", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_copy_cmds, 0, (char *)0, 0},
-  {(char *)"copy_bytes", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_copy_bytes, 0, (char *)0, 0},
-  {(char *)"copy_cmdbytes", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_copy_cmdbytes, 0, (char *)0, 0},
-  {(char *)"sig_cmds", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_sig_cmds, 0, (char *)0, 0},
-  {(char *)"sig_bytes", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_sig_bytes, 0, (char *)0, 0},
-  {(char *)"false_matches", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_false_matches, 0, (char *)0, 0},
-  {(char *)"sig_blocks", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_sig_blocks, 0, (char *)0, 0},
-  {(char *)"block_len", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_block_len, 0, (char *)0, 0},
-  {(char *)"in_bytes", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_in_bytes, 0, (char *)0, 0},
-  {(char *)"out_bytes", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_out_bytes, 0, (char *)0, 0},
-  {(char *)"start", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_start, 0, (char *)0, 0},
-  {(char *)"end", __pyx_getprop_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_end, 0, (char *)0, 0},
+static struct PyGetSetDef __pyx_getsets_7pyrsync_8backends_6cython_6_rsync_Stats[] = {
+  {(char *)"op", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_op, 0, (char *)0, 0},
+  {(char *)"lit_cmds", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_lit_cmds, 0, (char *)0, 0},
+  {(char *)"lit_bytes", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_lit_bytes, 0, (char *)0, 0},
+  {(char *)"lit_cmdbytes", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_lit_cmdbytes, 0, (char *)0, 0},
+  {(char *)"copy_cmds", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_copy_cmds, 0, (char *)0, 0},
+  {(char *)"copy_bytes", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_copy_bytes, 0, (char *)0, 0},
+  {(char *)"copy_cmdbytes", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_copy_cmdbytes, 0, (char *)0, 0},
+  {(char *)"sig_cmds", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_sig_cmds, 0, (char *)0, 0},
+  {(char *)"sig_bytes", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_sig_bytes, 0, (char *)0, 0},
+  {(char *)"false_matches", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_false_matches, 0, (char *)0, 0},
+  {(char *)"sig_blocks", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_sig_blocks, 0, (char *)0, 0},
+  {(char *)"block_len", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_block_len, 0, (char *)0, 0},
+  {(char *)"in_bytes", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_in_bytes, 0, (char *)0, 0},
+  {(char *)"out_bytes", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_out_bytes, 0, (char *)0, 0},
+  {(char *)"start", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_start, 0, (char *)0, 0},
+  {(char *)"end", __pyx_getprop_7pyrsync_8backends_6cython_6_rsync_5Stats_end, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats = {
+static PyTypeObject __pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pyrsync.backends.cython._rsync_cy.Stats", /*tp_name*/
-  sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats), /*tp_basicsize*/
+  "pyrsync.backends.cython._rsync.Stats", /*tp_name*/
+  sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_7pyrsync_8backends_6cython_9_rsync_cy_Stats, /*tp_dealloc*/
+  __pyx_tp_dealloc_7pyrsync_8backends_6cython_6_rsync_Stats, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -6610,25 +6600,25 @@
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_7pyrsync_8backends_6cython_9_rsync_cy_Stats, /*tp_methods*/
+  __pyx_methods_7pyrsync_8backends_6cython_6_rsync_Stats, /*tp_methods*/
   0, /*tp_members*/
-  __pyx_getsets_7pyrsync_8backends_6cython_9_rsync_cy_Stats, /*tp_getset*/
+  __pyx_getsets_7pyrsync_8backends_6cython_6_rsync_Stats, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Stats, /*tp_new*/
+  __pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Stats, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -6643,65 +6633,65 @@
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
-static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_9_rsync_cy_Job __pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Job;
+static struct __pyx_vtabstruct_7pyrsync_8backends_6cython_6_rsync_Job __pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Job;
 
-static struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *__pyx_freelist_7pyrsync_8backends_6cython_9_rsync_cy_Job[8];
-static int __pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Job = 0;
+static struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *__pyx_freelist_7pyrsync_8backends_6cython_6_rsync_Job[8];
+static int __pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Job = 0;
 
-static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Job(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *p;
+static PyObject *__pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Job(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *p;
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Job > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job)))) {
-    o = (PyObject*)__pyx_freelist_7pyrsync_8backends_6cython_9_rsync_cy_Job[--__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Job];
-    memset(o, 0, sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Job > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job)))) {
+    o = (PyObject*)__pyx_freelist_7pyrsync_8backends_6cython_6_rsync_Job[--__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Job];
+    memset(o, 0, sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job));
     (void) PyObject_INIT(o, t);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
-  p = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)o);
-  p->__pyx_vtab = __pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Job;
+  p = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)o);
+  p->__pyx_vtab = __pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Job;
   return o;
 }
 
-static void __pyx_tp_dealloc_7pyrsync_8backends_6cython_9_rsync_cy_Job(PyObject *o) {
+static void __pyx_tp_dealloc_7pyrsync_8backends_6cython_6_rsync_Job(PyObject *o) {
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_5__dealloc__(o);
+    __pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_5__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Job < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job)))) {
-    __pyx_freelist_7pyrsync_8backends_6cython_9_rsync_cy_Job[__pyx_freecount_7pyrsync_8backends_6cython_9_rsync_cy_Job++] = ((struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Job < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job)))) {
+    __pyx_freelist_7pyrsync_8backends_6cython_6_rsync_Job[__pyx_freecount_7pyrsync_8backends_6cython_6_rsync_Job++] = ((struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static PyMethodDef __pyx_methods_7pyrsync_8backends_6cython_9_rsync_cy_Job[] = {
-  {"statistics", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_1statistics, METH_NOARGS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics},
-  {"execute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_3execute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_2execute},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_7__reduce_cython__, METH_NOARGS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_6__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3Job_9__setstate_cython__, METH_O, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_3Job_8__setstate_cython__},
+static PyMethodDef __pyx_methods_7pyrsync_8backends_6cython_6_rsync_Job[] = {
+  {"statistics", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_1statistics, METH_NOARGS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_statistics},
+  {"execute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_3execute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_2execute},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_7__reduce_cython__, METH_NOARGS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_6__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3Job_9__setstate_cython__, METH_O, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_3Job_8__setstate_cython__},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job = {
+static PyTypeObject __pyx_type_7pyrsync_8backends_6cython_6_rsync_Job = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pyrsync.backends.cython._rsync_cy.Job", /*tp_name*/
-  sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job), /*tp_basicsize*/
+  "pyrsync.backends.cython._rsync.Job", /*tp_name*/
+  sizeof(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_7pyrsync_8backends_6cython_9_rsync_cy_Job, /*tp_dealloc*/
+  __pyx_tp_dealloc_7pyrsync_8backends_6cython_6_rsync_Job, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -6726,25 +6716,25 @@
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_7pyrsync_8backends_6cython_9_rsync_cy_Job, /*tp_methods*/
+  __pyx_methods_7pyrsync_8backends_6cython_6_rsync_Job, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_7pyrsync_8backends_6cython_9_rsync_cy_Job, /*tp_new*/
+  __pyx_tp_new_7pyrsync_8backends_6cython_6_rsync_Job, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -6761,35 +6751,35 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
-  {"get_signature_args", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_1get_signature_args, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_get_signature_args},
-  {"signature", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_3signature, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_2signature},
-  {"delta", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_5delta, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_4delta},
-  {"patch", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_9_rsync_cy_7patch, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_9_rsync_cy_6patch},
+  {"get_signature_args", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_1get_signature_args, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_get_signature_args},
+  {"signature", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_3signature, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_2signature},
+  {"delta", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_5delta, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_4delta},
+  {"patch", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyrsync_8backends_6cython_6_rsync_7patch, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pyrsync_8backends_6cython_6_rsync_6patch},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec__rsync_cy(PyObject* module); /*proto*/
+static int __pyx_pymod_exec__rsync(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec__rsync_cy},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__rsync},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "_rsync_cy",
+    "_rsync",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -6810,15 +6800,14 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_Job, __pyx_k_Job, sizeof(__pyx_k_Job), 0, 0, 1, 1},
   {&__pyx_n_s_LibrsyncError, __pyx_k_LibrsyncError, sizeof(__pyx_k_LibrsyncError), 0, 0, 1, 1},
   {&__pyx_n_s_LibrsyncError___init, __pyx_k_LibrsyncError___init, sizeof(__pyx_k_LibrsyncError___init), 0, 0, 1, 1},
   {&__pyx_n_s_LibrsyncError___str, __pyx_k_LibrsyncError___str, sizeof(__pyx_k_LibrsyncError___str), 0, 0, 1, 1},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_n_u_RS_BAD_MAGIC, __pyx_k_RS_BAD_MAGIC, sizeof(__pyx_k_RS_BAD_MAGIC), 0, 1, 0, 1},
   {&__pyx_n_s_RS_BLAKE2_SIG_MAGIC, __pyx_k_RS_BLAKE2_SIG_MAGIC, sizeof(__pyx_k_RS_BLAKE2_SIG_MAGIC), 0, 0, 1, 1},
   {&__pyx_n_u_RS_CORRUPT, __pyx_k_RS_CORRUPT, sizeof(__pyx_k_RS_CORRUPT), 0, 1, 0, 1},
@@ -6852,16 +6841,16 @@
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_old_fsize, __pyx_k_old_fsize, sizeof(__pyx_k_old_fsize), 0, 0, 1, 1},
   {&__pyx_n_s_output, __pyx_k_output, sizeof(__pyx_k_output), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
-  {&__pyx_n_s_pyrsync_backends_cython__rsync_c, __pyx_k_pyrsync_backends_cython__rsync_c, sizeof(__pyx_k_pyrsync_backends_cython__rsync_c), 0, 0, 1, 1},
-  {&__pyx_kp_s_pyrsync_backends_cython__rsync_c_2, __pyx_k_pyrsync_backends_cython__rsync_c_2, sizeof(__pyx_k_pyrsync_backends_cython__rsync_c_2), 0, 0, 1, 0},
+  {&__pyx_n_s_pyrsync_backends_cython__rsync, __pyx_k_pyrsync_backends_cython__rsync, sizeof(__pyx_k_pyrsync_backends_cython__rsync), 0, 0, 1, 1},
+  {&__pyx_kp_s_pyrsync_backends_cython__rsync_p, __pyx_k_pyrsync_backends_cython__rsync_p, sizeof(__pyx_k_pyrsync_backends_cython__rsync_p), 0, 0, 1, 0},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
@@ -6879,15 +6868,15 @@
   {&__pyx_n_s_tell, __pyx_k_tell, sizeof(__pyx_k_tell), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 183, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 184, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6927,37 +6916,37 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.job cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_self_job_cannot_be_converted_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":40
+  /* "pyrsync/backends/cython/_rsync.pyx":40
  * 
  * class LibrsyncError(Exception):
  *     def __init__(self, result):             # <<<<<<<<<<<<<<
  *         self.code = result
  * 
  */
   __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyrsync_backends_cython__rsync_c_2, __pyx_n_s_init, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyrsync_backends_cython__rsync_p, __pyx_n_s_init, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 40, __pyx_L1_error)
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":43
+  /* "pyrsync/backends/cython/_rsync.pyx":43
  *         self.code = result
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         if self.code == RS_RUNNING:
  *             return "RS_RUNNING"
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyrsync_backends_cython__rsync_c_2, __pyx_n_s_str, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 43, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyrsync_backends_cython__rsync_p, __pyx_n_s_str, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 43, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -7004,43 +6993,42 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Stats = &__pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Stats;
-  __pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Stats.from_ptr = (struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *(*)(rs_stats_t *))__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_5Stats_from_ptr;
-  if (PyType_Ready(&__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Stats = &__pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Stats;
+  __pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Stats.from_ptr = (struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *(*)(rs_stats_t *))__pyx_f_7pyrsync_8backends_6cython_6_rsync_5Stats_from_ptr;
+  if (PyType_Ready(&__pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats.tp_print = 0;
+  __pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats.tp_dictoffset && __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats.tp_dictoffset && __pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (__Pyx_SetVtable(__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats.tp_dict, __pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Stats, (PyObject *)&__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
-  __pyx_ptype_7pyrsync_8backends_6cython_9_rsync_cy_Stats = &__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Stats;
-  __pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Job = &__pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Job;
-  __pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Job.from_ptr = (struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *(*)(rs_job_t *))__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_from_ptr;
-  __pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Job.iter = (rs_result (*)(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, rs_buffers_t *))__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_iter;
-  __pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Job.statistics = (struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Stats *(*)(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, int __pyx_skip_dispatch))__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_statistics;
-  __pyx_vtable_7pyrsync_8backends_6cython_9_rsync_cy_Job.execute = (int (*)(struct __pyx_obj_7pyrsync_8backends_6cython_9_rsync_cy_Job *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute *__pyx_optional_args))__pyx_f_7pyrsync_8backends_6cython_9_rsync_cy_3Job_execute;
-  if (PyType_Ready(&__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats.tp_dict, __pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Stats, (PyObject *)&__pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_ptype_7pyrsync_8backends_6cython_6_rsync_Stats = &__pyx_type_7pyrsync_8backends_6cython_6_rsync_Stats;
+  __pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Job = &__pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Job;
+  __pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Job.from_ptr = (struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *(*)(rs_job_t *))__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_from_ptr;
+  __pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Job.iter = (rs_result (*)(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, rs_buffers_t *))__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_iter;
+  __pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Job.statistics = (struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Stats *(*)(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, int __pyx_skip_dispatch))__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_statistics;
+  __pyx_vtable_7pyrsync_8backends_6cython_6_rsync_Job.execute = (int (*)(struct __pyx_obj_7pyrsync_8backends_6cython_6_rsync_Job *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_7pyrsync_8backends_6cython_6_rsync_3Job_execute *__pyx_optional_args))__pyx_f_7pyrsync_8backends_6cython_6_rsync_3Job_execute;
+  if (PyType_Ready(&__pyx_type_7pyrsync_8backends_6cython_6_rsync_Job) < 0) __PYX_ERR(1, 152, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job.tp_print = 0;
+  __pyx_type_7pyrsync_8backends_6cython_6_rsync_Job.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job.tp_dictoffset && __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pyrsync_8backends_6cython_6_rsync_Job.tp_dictoffset && __pyx_type_7pyrsync_8backends_6cython_6_rsync_Job.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7pyrsync_8backends_6cython_6_rsync_Job.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (__Pyx_SetVtable(__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job.tp_dict, __pyx_vtabptr_7pyrsync_8backends_6cython_9_rsync_cy_Job) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Job, (PyObject *)&__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
-  __pyx_ptype_7pyrsync_8backends_6cython_9_rsync_cy_Job = &__pyx_type_7pyrsync_8backends_6cython_9_rsync_cy_Job;
+  if (__Pyx_SetVtable(__pyx_type_7pyrsync_8backends_6cython_6_rsync_Job.tp_dict, __pyx_vtabptr_7pyrsync_8backends_6cython_6_rsync_Job) < 0) __PYX_ERR(1, 152, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pyrsync_8backends_6cython_6_rsync_Job) < 0) __PYX_ERR(1, 152, __pyx_L1_error)
+  __pyx_ptype_7pyrsync_8backends_6cython_6_rsync_Job = &__pyx_type_7pyrsync_8backends_6cython_6_rsync_Job;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -7102,19 +7090,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC init_rsync_cy(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC init_rsync_cy(void)
+__Pyx_PyMODINIT_FUNC init_rsync(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC init_rsync(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit__rsync_cy(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit__rsync_cy(void)
+__Pyx_PyMODINIT_FUNC PyInit__rsync(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit__rsync(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -7173,45 +7161,45 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec__rsync_cy(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec__rsync(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module '_rsync_cy' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module '_rsync' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__rsync_cy(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__rsync(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -7240,15 +7228,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("_rsync_cy", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("_rsync", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -7258,22 +7246,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_pyrsync__backends__cython___rsync_cy) {
+  if (__pyx_module_is_main_pyrsync__backends__cython___rsync) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(1, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "pyrsync.backends.cython._rsync_cy")) {
-      if (unlikely(PyDict_SetItemString(modules, "pyrsync.backends.cython._rsync_cy", __pyx_m) < 0)) __PYX_ERR(1, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "pyrsync.backends.cython._rsync")) {
+      if (unlikely(PyDict_SetItemString(modules, "pyrsync.backends.cython._rsync", __pyx_m) < 0)) __PYX_ERR(1, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -7286,158 +7274,158 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":39
+  /* "pyrsync/backends/cython/_rsync.pyx":39
  * 
  * 
  * class LibrsyncError(Exception):             # <<<<<<<<<<<<<<
  *     def __init__(self, result):
  *         self.code = result
  */
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_LibrsyncError, __pyx_n_s_LibrsyncError, (PyObject *) NULL, __pyx_n_s_pyrsync_backends_cython__rsync_c, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 39, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_LibrsyncError, __pyx_n_s_LibrsyncError, (PyObject *) NULL, __pyx_n_s_pyrsync_backends_cython__rsync, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":40
+  /* "pyrsync/backends/cython/_rsync.pyx":40
  * 
  * class LibrsyncError(Exception):
  *     def __init__(self, result):             # <<<<<<<<<<<<<<
  *         self.code = result
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_1__init__, 0, __pyx_n_s_LibrsyncError___init, NULL, __pyx_n_s_pyrsync_backends_cython__rsync_c, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_1__init__, 0, __pyx_n_s_LibrsyncError___init, NULL, __pyx_n_s_pyrsync_backends_cython__rsync, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(1, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":43
+  /* "pyrsync/backends/cython/_rsync.pyx":43
  *         self.code = result
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         if self.code == RS_RUNNING:
  *             return "RS_RUNNING"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pyrsync_8backends_6cython_9_rsync_cy_13LibrsyncError_3__str__, 0, __pyx_n_s_LibrsyncError___str, NULL, __pyx_n_s_pyrsync_backends_cython__rsync_c, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 43, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pyrsync_8backends_6cython_6_rsync_13LibrsyncError_3__str__, 0, __pyx_n_s_LibrsyncError___str, NULL, __pyx_n_s_pyrsync_backends_cython__rsync, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_str, __pyx_t_4) < 0) __PYX_ERR(1, 43, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":39
+  /* "pyrsync/backends/cython/_rsync.pyx":39
  * 
  * 
  * class LibrsyncError(Exception):             # <<<<<<<<<<<<<<
  *     def __init__(self, result):
  *         self.code = result
  */
   __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_LibrsyncError, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_LibrsyncError, __pyx_t_4) < 0) __PYX_ERR(1, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":68
+  /* "pyrsync/backends/cython/_rsync.pyx":68
  * 
  * 
  * RS_JOB_BLOCKSIZE = 65535             # <<<<<<<<<<<<<<
  * 
  * RS_DELTA_MAGIC = C_RS_DELTA_MAGIC
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RS_JOB_BLOCKSIZE, __pyx_int_65535) < 0) __PYX_ERR(1, 68, __pyx_L1_error)
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":70
+  /* "pyrsync/backends/cython/_rsync.pyx":70
  * RS_JOB_BLOCKSIZE = 65535
  * 
  * RS_DELTA_MAGIC = C_RS_DELTA_MAGIC             # <<<<<<<<<<<<<<
  * RS_MD4_SIG_MAGIC = C_RS_MD4_SIG_MAGIC
  * RS_BLAKE2_SIG_MAGIC = C_RS_BLAKE2_SIG_MAGIC
  */
   __pyx_t_1 = __Pyx_PyInt_From_rs_magic_number(RS_DELTA_MAGIC); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RS_DELTA_MAGIC, __pyx_t_1) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":71
+  /* "pyrsync/backends/cython/_rsync.pyx":71
  * 
  * RS_DELTA_MAGIC = C_RS_DELTA_MAGIC
  * RS_MD4_SIG_MAGIC = C_RS_MD4_SIG_MAGIC             # <<<<<<<<<<<<<<
  * RS_BLAKE2_SIG_MAGIC = C_RS_BLAKE2_SIG_MAGIC
  * RS_RK_MD4_SIG_MAGIC = C_RS_RK_MD4_SIG_MAGIC
  */
   __pyx_t_1 = __Pyx_PyInt_From_rs_magic_number(RS_MD4_SIG_MAGIC); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RS_MD4_SIG_MAGIC, __pyx_t_1) < 0) __PYX_ERR(1, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":72
+  /* "pyrsync/backends/cython/_rsync.pyx":72
  * RS_DELTA_MAGIC = C_RS_DELTA_MAGIC
  * RS_MD4_SIG_MAGIC = C_RS_MD4_SIG_MAGIC
  * RS_BLAKE2_SIG_MAGIC = C_RS_BLAKE2_SIG_MAGIC             # <<<<<<<<<<<<<<
  * RS_RK_MD4_SIG_MAGIC = C_RS_RK_MD4_SIG_MAGIC
  * RS_RK_BLAKE2_SIG_MAGIC= C_RS_RK_BLAKE2_SIG_MAGIC
  */
   __pyx_t_1 = __Pyx_PyInt_From_rs_magic_number(RS_BLAKE2_SIG_MAGIC); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RS_BLAKE2_SIG_MAGIC, __pyx_t_1) < 0) __PYX_ERR(1, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":73
+  /* "pyrsync/backends/cython/_rsync.pyx":73
  * RS_MD4_SIG_MAGIC = C_RS_MD4_SIG_MAGIC
  * RS_BLAKE2_SIG_MAGIC = C_RS_BLAKE2_SIG_MAGIC
  * RS_RK_MD4_SIG_MAGIC = C_RS_RK_MD4_SIG_MAGIC             # <<<<<<<<<<<<<<
  * RS_RK_BLAKE2_SIG_MAGIC= C_RS_RK_BLAKE2_SIG_MAGIC
  * 
  */
   __pyx_t_1 = __Pyx_PyInt_From_rs_magic_number(RS_RK_MD4_SIG_MAGIC); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RS_RK_MD4_SIG_MAGIC, __pyx_t_1) < 0) __PYX_ERR(1, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":74
+  /* "pyrsync/backends/cython/_rsync.pyx":74
  * RS_BLAKE2_SIG_MAGIC = C_RS_BLAKE2_SIG_MAGIC
  * RS_RK_MD4_SIG_MAGIC = C_RS_RK_MD4_SIG_MAGIC
  * RS_RK_BLAKE2_SIG_MAGIC= C_RS_RK_BLAKE2_SIG_MAGIC             # <<<<<<<<<<<<<<
  * 
  * cdef inline uint8_t PyFile_Check(object file):
  */
   __pyx_t_1 = __Pyx_PyInt_From_rs_magic_number(RS_RK_BLAKE2_SIG_MAGIC); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RS_RK_BLAKE2_SIG_MAGIC, __pyx_t_1) < 0) __PYX_ERR(1, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":227
+  /* "pyrsync/backends/cython/_rsync.pyx":228
  * 
  * cpdef inline signature(object input, object output, size_t strong_len, rs_magic_number sig_magic,
  *                            size_t block_size=RS_DEFAULT_BLOCK_LEN):             # <<<<<<<<<<<<<<
  *     """
  *      Generate a signature for the file input. The signature will be written to output.
  */
   __pyx_k__5 = RS_DEFAULT_BLOCK_LEN;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":226
+  /* "pyrsync/backends/cython/_rsync.pyx":227
  *     return c_magic, block_len, strong_len
  * 
  * cpdef inline signature(object input, object output, size_t strong_len, rs_magic_number sig_magic,             # <<<<<<<<<<<<<<
  *                            size_t block_size=RS_DEFAULT_BLOCK_LEN):
  *     """
  */
   __pyx_k__5 = RS_DEFAULT_BLOCK_LEN;
 
-  /* "pyrsync/backends/cython/_rsync_cy.pyx":1
+  /* "pyrsync/backends/cython/_rsync.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # cython: cdivision=True
  * cimport cython
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -7449,19 +7437,19 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init pyrsync.backends.cython._rsync_cy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init pyrsync.backends.cython._rsync", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init pyrsync.backends.cython._rsync_cy");
+    PyErr_SetString(PyExc_ImportError, "init pyrsync.backends.cython._rsync");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -8377,92 +8365,14 @@
     #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
 }
 #endif
 
-/* ReRaiseException */
-static CYTHON_INLINE void __Pyx_ReraiseException(void) {
-    PyObject *type = NULL, *value = NULL, *tb = NULL;
-#if CYTHON_FAST_THREAD_STATE
-    PyThreadState *tstate = PyThreadState_GET();
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    type = exc_info->exc_type;
-    value = exc_info->exc_value;
-    tb = exc_info->exc_traceback;
-    #else
-    type = tstate->exc_type;
-    value = tstate->exc_value;
-    tb = tstate->exc_traceback;
-    #endif
-#else
-    PyErr_GetExcInfo(&type, &value, &tb);
-#endif
-    if (!type || type == Py_None) {
-#if !CYTHON_FAST_THREAD_STATE
-        Py_XDECREF(type);
-        Py_XDECREF(value);
-        Py_XDECREF(tb);
-#endif
-        PyErr_SetString(PyExc_RuntimeError,
-            "No active exception to reraise");
-    } else {
-#if CYTHON_FAST_THREAD_STATE
-        Py_INCREF(type);
-        Py_XINCREF(value);
-        Py_XINCREF(tb);
-#endif
-        PyErr_Restore(type, value, tb);
-    }
-}
-
-/* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
-                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
-                                  int full_traceback, CYTHON_UNUSED int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
-    __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
-#endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
-    }
-    #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
-    #else
-    ctx = PyUnicode_FromString(name);
-    #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
-    } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
-    }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
-#endif
-}
-
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'%.50s' object has no attribute '%U'",
                  tp->tp_name, attr_name);
```

### Comparing `python-rsync-0.1.0.dev2/pyrsync/backends/cython/_rsync_cy.pyx` & `python-rsync-0.1.0rc1/pyrsync/backends/cython/_rsync.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
     @property
     def end(self):
         return self.state.end
 
 @cython.freelist(8)
 @cython.final
 @cython.no_gc
+@cython.internal
 cdef class Job:
     cdef  rs_job_t * job
 
     @staticmethod
     cdef inline Job from_ptr(rs_job_t * job):
         cdef Job self = Job.__new__(Job)
         self.job = job
@@ -160,15 +161,15 @@
     cdef inline rs_result iter(self, rs_buffers_t * buffer):
         cdef rs_result result
         with nogil:
             result = rs_job_iter(self.job, buffer)
         return result
 
     cpdef inline Stats statistics(self):
-        cdef rs_stats_t * state = rs_job_statistics(self.job)
+        cdef rs_stats_t * state = <rs_stats_t *>rs_job_statistics(self.job)
         return Stats.from_ptr(state)
 
     cpdef inline int execute(self, object input, object output = None) except -1:
         if not PyFile_Check(input):
             raise TypeError("input except a file-like object, got %s" % type(input).__name__)
         if output is not None and not PyFile_Check(output):
             raise TypeError("sigfile except a file-like object, got %s" % type(output).__name__)
@@ -270,25 +271,25 @@
         rs_free_sumset(sig)
 
 cdef struct input_args:
     PyObject *file
     char* buffer
     Py_ssize_t len
 
-cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) with gil:
+cdef rs_result read_cb(void *opaque, rs_long_t pos, size_t *len, void ** buf) except * with gil:
     cdef  input_args* args = <input_args*>opaque
     input = <object>args.file
     input.seek(pos)
     block = input.read(len[0]) # type: bytes
     cdef Py_ssize_t block_size = PyBytes_GET_SIZE(block)
     cdef void* temp
     if block_size > args.len:
         temp = PyMem_Realloc(<void*>args.buffer, <size_t>block_size)
         if temp==NULL:
-            raise
+            raise MemoryError
         args.buffer = <char*>temp
         args.len = block_size
 
     len[0] = <size_t>block_size
     memcpy(args.buffer, PyBytes_AS_STRING(block), <size_t>block_size)
     (<char**> buf)[0] = args.buffer
     return RS_DONE
```

### Comparing `python-rsync-0.1.0.dev2/pyrsync/backends/cython/rsync.pxd` & `python-rsync-0.1.0rc1/pyrsync/backends/cython/rsync.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     rs_job_t *rs_sig_begin(size_t block_len, size_t strong_len,
                            rs_magic_number sig_magic)
 
     rs_job_t *rs_delta_begin(rs_signature_t *)
     rs_job_t *rs_loadsig_begin(rs_signature_t **)
     rs_result rs_build_hash_table(rs_signature_t *sums)
     ctypedef rs_result rs_copy_cb(void *opaque, rs_long_t pos, size_t *len,
-                         void ** buf)
+                         void ** buf)  except * with gil
     rs_job_t *rs_patch_begin(rs_copy_cb * copy_cb, void *copy_arg)
     FILE *rs_file_open(char * filename, char  * mode, int force )
     int rs_file_close(FILE *file)
     rs_long_t rs_file_size(FILE *file)
     rs_result rs_file_copy_cb(void *arg, rs_long_t pos, size_t *len,
                               void ** buf)
     extern int rs_inbuflen, rs_outbuflen
```

### Comparing `python-rsync-0.1.0.dev2/python_rsync.egg-info/PKG-INFO` & `python-rsync-0.1.0rc1/python_rsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rsync
-Version: 0.1.0.dev2
+Version: 0.1.0rc1
 Summary: python binding for librsync
 Home-page: https://github.com/synodriver/pyrsync
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: compress,decompress
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-rsync-0.1.0.dev2/python_rsync.egg-info/SOURCES.txt` & `python-rsync-0.1.0rc1/python_rsync.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 dep/src/blake2/blake2b-ref.c
 pyrsync/__init__.py
 pyrsync/backends/__init__.py
 pyrsync/backends/cffi/__init__.py
 pyrsync/backends/cffi/build.py
 pyrsync/backends/cffi/cbarg.h
 pyrsync/backends/cython/__init__.py
-pyrsync/backends/cython/_rsync_cy.c
-pyrsync/backends/cython/_rsync_cy.pyx
+pyrsync/backends/cython/_rsync.c
+pyrsync/backends/cython/_rsync.pyx
 pyrsync/backends/cython/rsync.pxd
 python_rsync.egg-info/PKG-INFO
 python_rsync.egg-info/SOURCES.txt
 python_rsync.egg-info/dependency_links.txt
 python_rsync.egg-info/not-zip-safe
 python_rsync.egg-info/requires.txt
 python_rsync.egg-info/top_level.txt
```

### Comparing `python-rsync-0.1.0.dev2/setup.py` & `python-rsync-0.1.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         for ext in self.extensions:
             ext.extra_compile_args = args
             if os.name == "nt":
                 ext.libraries.append("ws2_32")
         super().build_extensions()
 
 
-c_src = ["pyrsync/backends/cython/_rsync_cy.pyx"]
+c_src = ["pyrsync/backends/cython/_rsync.pyx"]
 include_dirs = []
 libraries = []
 extra_objects = []
 
 if has_option("--use-lib"):
     include_dirs.extend(["./dep/src", "./dep/src/blake2"])
     libraries.append("rsync")
@@ -52,15 +52,15 @@
     for root, dirs, files in os.walk("./dep/src"):
         for file in files:
             if file.endswith(".c") and "rdiff" not in file:
                 c_src.append(os.path.join(root, file))
 
 extensions = [
     Extension(
-        "pyrsync.backends.cython._rsync_cy",
+        "pyrsync.backends.cython._rsync",
         c_src,
         include_dirs=include_dirs,
         # library_dirs=[r"F:\pyproject\pyrsync\dep\Debug"],
         # libraries=libraries,
         define_macros=[("rsync_EXPORTS", None)],
         extra_objects=extra_objects,
     ),
```

