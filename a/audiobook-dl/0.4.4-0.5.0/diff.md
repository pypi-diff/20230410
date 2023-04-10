# Comparing `tmp/audiobook-dl-0.4.4.tar.gz` & `tmp/audiobook-dl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-dl-0.4.4.tar", last modified: Fri Mar 17 17:20:39 2023, max compression
+gzip compressed data, was "audiobook-dl-0.5.0.tar", last modified: Mon Apr 10 11:40:48 2023, max compression
```

## Comparing `audiobook-dl-0.4.4.tar` & `audiobook-dl-0.5.0.tar`

### file list

```diff
@@ -1,73 +1,77 @@
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.362453 audiobook-dl-0.4.4/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.357453 audiobook-dl-0.4.4/.github/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.358453 audiobook-dl-0.4.4/.github/workflows/
--rw-r--r--   0 jo1gi     (1000) users      (100)      315 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/.github/workflows/ci.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-01-24 12:59:12.000000 audiobook-dl-0.4.4/.github/workflows/pytest.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      539 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/.gitignore
--rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/LICENSE
--rw-r--r--   0 jo1gi     (1000) users      (100)     4693 2023-03-17 17:20:39.362453 audiobook-dl-0.4.4/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     4122 2023-02-22 10:33:18.000000 audiobook-dl-0.4.4/README.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.358453 audiobook-dl-0.4.4/audiobook_dl.egg-info/
--rw-r--r--   0 jo1gi     (1000) users      (100)     4693 2023-03-17 17:20:39.000000 audiobook-dl-0.4.4/audiobook_dl.egg-info/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     1823 2023-03-17 17:20:39.000000 audiobook-dl-0.4.4/audiobook_dl.egg-info/SOURCES.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-03-17 17:20:39.000000 audiobook-dl-0.4.4/audiobook_dl.egg-info/dependency_links.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       58 2023-03-17 17:20:39.000000 audiobook-dl-0.4.4/audiobook_dl.egg-info/entry_points.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       87 2023-03-17 17:20:39.000000 audiobook-dl-0.4.4/audiobook_dl.egg-info/requires.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-03-17 17:20:39.000000 audiobook-dl-0.4.4/audiobook_dl.egg-info/top_level.txt
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.359453 audiobook-dl-0.4.4/audiobookdl/
--rw-r--r--   0 jo1gi     (1000) users      (100)      130 2023-03-17 17:17:09.000000 audiobook-dl-0.4.4/audiobookdl/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2845 2023-02-13 19:40:54.000000 audiobook-dl-0.4.4/audiobookdl/__main__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2488 2023-02-13 19:29:52.000000 audiobook-dl-0.4.4/audiobookdl/args.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.359453 audiobook-dl-0.4.4/audiobookdl/assets/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.360453 audiobook-dl-0.4.4/audiobookdl/assets/errors/
--rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-02-03 15:39:07.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/book_access.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/chapters_add.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      468 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/data_not_present.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       45 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/failed_combining.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/missing_dependency.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/no_files_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-01-25 13:57:49.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/no_source_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       55 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/request_error.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-01-15 14:23:15.000000 audiobook-dl-0.4.4/audiobookdl/assets/errors/user_not_authorized.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/assets/ffmpeg_chapter_template.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      317 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/audiobookdl/assets/simple_help.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)     1238 2023-02-03 15:34:28.000000 audiobook-dl-0.4.4/audiobookdl/exceptions.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1054 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/logging.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.360453 audiobook-dl-0.4.4/audiobookdl/output/
--rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-01-14 14:07:32.000000 audiobook-dl-0.4.4/audiobookdl/output/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     6392 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/output/download.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      529 2023-01-26 09:38:39.000000 audiobook-dl-0.4.4/audiobookdl/output/encryption.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.361453 audiobook-dl-0.4.4/audiobookdl/output/metadata/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1349 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/output/metadata/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/output/metadata/ffmpeg.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2375 2023-02-08 20:30:24.000000 audiobook-dl-0.4.4/audiobookdl/output/metadata/id3.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1411 2023-02-08 21:14:30.000000 audiobook-dl-0.4.4/audiobookdl/output/metadata/mp4.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2283 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/output/output.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.361453 audiobook-dl-0.4.4/audiobookdl/sources/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1401 2023-02-08 16:47:55.000000 audiobook-dl-0.4.4/audiobookdl/sources/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1409 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/sources/audiobooksdotcom.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4356 2023-02-13 18:59:49.000000 audiobook-dl-0.4.4/audiobookdl/sources/bookbeat.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3871 2023-02-08 20:37:42.000000 audiobook-dl-0.4.4/audiobookdl/sources/chirp.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3285 2023-02-08 20:32:00.000000 audiobook-dl-0.4.4/audiobookdl/sources/ereolen.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      906 2023-01-24 13:17:18.000000 audiobook-dl-0.4.4/audiobookdl/sources/librivox.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4664 2023-02-13 18:59:49.000000 audiobook-dl-0.4.4/audiobookdl/sources/nextory.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2898 2023-03-07 11:45:52.000000 audiobook-dl-0.4.4/audiobookdl/sources/overdrive.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5466 2023-02-08 20:36:07.000000 audiobook-dl-0.4.4/audiobookdl/sources/scribd.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.361453 audiobook-dl-0.4.4/audiobookdl/sources/source/
--rw-r--r--   0 jo1gi     (1000) users      (100)     5050 2023-02-13 18:59:49.000000 audiobook-dl-0.4.4/audiobookdl/sources/source/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1849 2023-01-26 09:42:50.000000 audiobook-dl-0.4.4/audiobookdl/sources/source/networking.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4168 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/sources/storytel.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4028 2023-02-08 20:37:15.000000 audiobook-dl-0.4.4/audiobookdl/sources/yourcloudlibrary.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.362453 audiobook-dl-0.4.4/audiobookdl/utils/
--rw-r--r--   0 jo1gi     (1000) users      (100)      755 2023-03-07 11:37:34.000000 audiobook-dl-0.4.4/audiobookdl/utils/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1168 2023-02-08 20:30:35.000000 audiobook-dl-0.4.4/audiobookdl/utils/audiobook.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      659 2023-01-14 13:31:23.000000 audiobook-dl-0.4.4/audiobookdl/utils/dependencies.py
--rw-r--r--   0 jo1gi     (1000) users      (100)       37 2023-01-12 22:22:17.000000 audiobook-dl-0.4.4/mypy.ini
--rw-r--r--   0 jo1gi     (1000) users      (100)     1032 2023-02-05 10:54:46.000000 audiobook-dl-0.4.4/pyproject.toml
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-03-17 17:20:39.362453 audiobook-dl-0.4.4/setup.cfg
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-02-03 18:54:01.000000 audiobook-dl-0.4.4/setup.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      396 2023-03-08 18:58:29.000000 audiobook-dl-0.4.4/shell.nix
--rw-r--r--   0 jo1gi     (1000) users      (100)     1835 2023-02-08 16:47:55.000000 audiobook-dl-0.4.4/supported_sites.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-03-17 17:20:39.362453 audiobook-dl-0.4.4/tests/
--rw-r--r--   0 jo1gi     (1000) users      (100)      664 2023-02-13 19:53:54.000000 audiobook-dl-0.4.4/tests/test_output.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-02-13 19:42:19.000000 audiobook-dl-0.4.4/tests/test_urls.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.200801 audiobook-dl-0.5.0/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.183801 audiobook-dl-0.5.0/.github/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       13 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/.github/FUNDING.yml
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.183801 audiobook-dl-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      349 2023-03-21 07:18:57.000000 audiobook-dl-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.184801 audiobook-dl-0.5.0/.github/workflows/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      315 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-01-19 22:18:06.000000 audiobook-dl-0.5.0/.github/workflows/pytest.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      539 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/.gitignore
+-rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/LICENSE
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4902 2023-04-10 11:40:48.200801 audiobook-dl-0.5.0/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4331 2023-04-07 08:43:53.000000 audiobook-dl-0.5.0/README.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.186801 audiobook-dl-0.5.0/audiobook_dl.egg-info/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4902 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1935 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       58 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/entry_points.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       82 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/requires.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/top_level.txt
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.188801 audiobook-dl-0.5.0/audiobookdl/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      167 2023-04-10 11:35:29.000000 audiobook-dl-0.5.0/audiobookdl/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3102 2023-04-06 21:14:29.000000 audiobook-dl-0.5.0/audiobookdl/__main__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2696 2023-04-05 19:24:53.000000 audiobook-dl-0.5.0/audiobookdl/args.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.188801 audiobook-dl-0.5.0/audiobookdl/assets/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.191801 audiobook-dl-0.5.0/audiobookdl/assets/errors/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-02-05 08:49:39.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/book_access.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-02-16 19:20:53.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/chapters_add.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      468 2022-09-01 08:49:16.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/data_not_present.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       45 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/failed_combining.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-02-16 19:20:51.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/missing_dependency.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/no_files_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-02-02 07:28:40.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/no_source_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       55 2022-04-05 11:33:45.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/request_error.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-01-19 21:44:13.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/user_not_authorized.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-02-16 17:36:53.000000 audiobook-dl-0.5.0/audiobookdl/assets/ffmpeg_chapter_template.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      317 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/audiobookdl/assets/simple_help.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1254 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/exceptions.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1401 2023-04-10 11:35:15.000000 audiobook-dl-0.5.0/audiobookdl/logging.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.193801 audiobook-dl-0.5.0/audiobookdl/output/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-01-19 21:44:13.000000 audiobook-dl-0.5.0/audiobookdl/output/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     6858 2023-04-06 21:10:31.000000 audiobook-dl-0.5.0/audiobookdl/output/download.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      641 2023-04-03 16:18:40.000000 audiobook-dl-0.5.0/audiobookdl/output/encryption.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1786 2023-04-05 18:17:14.000000 audiobook-dl-0.5.0/audiobookdl/output/formats.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.194801 audiobook-dl-0.5.0/audiobookdl/output/metadata/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1340 2023-04-09 10:25:30.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-02-16 20:23:47.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/ffmpeg.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2435 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/id3.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1476 2023-04-09 10:22:01.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/mp4.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2476 2023-04-02 15:33:26.000000 audiobook-dl-0.5.0/audiobookdl/output/output.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.198801 audiobook-dl-0.5.0/audiobookdl/sources/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1548 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1589 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/audiobooksdotcom.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4230 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/bookbeat.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4001 2023-04-05 12:31:35.000000 audiobook-dl-0.5.0/audiobookdl/sources/chirp.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3373 2023-04-06 11:50:10.000000 audiobook-dl-0.5.0/audiobookdl/sources/ereolen.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1067 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/librivox.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4750 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/nextory.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2914 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/overdrive.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      155 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/rss.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4078 2023-04-09 09:22:07.000000 audiobook-dl-0.5.0/audiobookdl/sources/saxo.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5187 2023-04-10 11:35:19.000000 audiobook-dl-0.5.0/audiobookdl/sources/scribd.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.198801 audiobook-dl-0.5.0/audiobookdl/sources/source/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5146 2023-04-10 11:35:15.000000 audiobook-dl-0.5.0/audiobookdl/sources/source/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2374 2023-04-10 11:35:19.000000 audiobook-dl-0.5.0/audiobookdl/sources/source/networking.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4311 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/storytel.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4169 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/yourcloudlibrary.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.199801 audiobook-dl-0.5.0/audiobookdl/utils/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      972 2023-03-24 11:47:59.000000 audiobook-dl-0.5.0/audiobookdl/utils/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2924 2023-04-03 15:48:37.000000 audiobook-dl-0.5.0/audiobookdl/utils/audiobook.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      655 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/utils/dependencies.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1298 2023-04-03 15:54:34.000000 audiobook-dl-0.5.0/pyproject.toml
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-04-10 11:40:48.200801 audiobook-dl-0.5.0/setup.cfg
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-04-06 21:10:31.000000 audiobook-dl-0.5.0/setup.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      396 2023-04-10 11:35:15.000000 audiobook-dl-0.5.0/shell.nix
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1987 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/supported_sites.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.199801 audiobook-dl-0.5.0/tests/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-02-13 07:19:44.000000 audiobook-dl-0.5.0/tests/test_urls.py
```

### Comparing `audiobook-dl-0.4.4/.gitignore` & `audiobook-dl-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.4.4/LICENSE` & `audiobook-dl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.4.4/PKG-INFO` & `audiobook-dl-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.4.4
+Version: 0.5.0
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -25,31 +25,38 @@
 - [audiobooks.com](https://audiobooks.com)
 - [BookBeat](https://www.bookbeat.com/)
 - [Chirp](https://www.chirpbooks.com/)
 - [eReolen (Danish Library)](https://ereolen.dk)
 - [Librivox](https://librivox.org)
 - [Nextory](https://nextory.com)
 - [Overdrive (Library service)](https://www.overdrive.com/)
+- [Saxo](https://saxo.com)
 - [Scribd](https://scribd.com)
 - [Storytel](https://www.storytel.com/)
 - [YourCloudLibrary](https://www.yourcloudlibrary.com/)
 
 [More info](./supported_sites.md)
 
 ## Installation
 audiobook-dl can be installed from the repo itself or through pip.
 
+To get the newest stable version with pip run:
 ```shell
-git clone https://github.com/jo1gi/audiobook-dl.git
-cd audiobook-dl
-python3 setup.py install
+pip install audiobook-dl
+```
+
+If you want to use the newest version (can be unstable) run:
+```shell
+pip install "git+https://github.com/jo1gi/audiobook-dl.git"
 ```
 or
 ```shell
-pip install audiobook-dl
+git clone https://github.com/jo1gi/audiobook-dl.git
+cd audiobook-dl
+python3 setup.py install
 ```
 
 Some features require [ffmpeg](https://ffmpeg.org/) which can be installed
 through most package managers or from [ffmpeg.org/download.html](https://ffmpeg.org/download.html).
 
 ## Authentication
```

### Comparing `audiobook-dl-0.4.4/README.md` & `audiobook-dl-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,38 @@
 - [audiobooks.com](https://audiobooks.com)
 - [BookBeat](https://www.bookbeat.com/)
 - [Chirp](https://www.chirpbooks.com/)
 - [eReolen (Danish Library)](https://ereolen.dk)
 - [Librivox](https://librivox.org)
 - [Nextory](https://nextory.com)
 - [Overdrive (Library service)](https://www.overdrive.com/)
+- [Saxo](https://saxo.com)
 - [Scribd](https://scribd.com)
 - [Storytel](https://www.storytel.com/)
 - [YourCloudLibrary](https://www.yourcloudlibrary.com/)
 
 [More info](./supported_sites.md)
 
 ## Installation
 audiobook-dl can be installed from the repo itself or through pip.
 
+To get the newest stable version with pip run:
 ```shell
-git clone https://github.com/jo1gi/audiobook-dl.git
-cd audiobook-dl
-python3 setup.py install
+pip install audiobook-dl
+```
+
+If you want to use the newest version (can be unstable) run:
+```shell
+pip install "git+https://github.com/jo1gi/audiobook-dl.git"
 ```
 or
 ```shell
-pip install audiobook-dl
+git clone https://github.com/jo1gi/audiobook-dl.git
+cd audiobook-dl
+python3 setup.py install
 ```
 
 Some features require [ffmpeg](https://ffmpeg.org/) which can be installed
 through most package managers or from [ffmpeg.org/download.html](https://ffmpeg.org/download.html).
 
 ## Authentication
```

### Comparing `audiobook-dl-0.4.4/audiobook_dl.egg-info/PKG-INFO` & `audiobook-dl-0.5.0/audiobook_dl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.4.4
+Version: 0.5.0
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -25,31 +25,38 @@
 - [audiobooks.com](https://audiobooks.com)
 - [BookBeat](https://www.bookbeat.com/)
 - [Chirp](https://www.chirpbooks.com/)
 - [eReolen (Danish Library)](https://ereolen.dk)
 - [Librivox](https://librivox.org)
 - [Nextory](https://nextory.com)
 - [Overdrive (Library service)](https://www.overdrive.com/)
+- [Saxo](https://saxo.com)
 - [Scribd](https://scribd.com)
 - [Storytel](https://www.storytel.com/)
 - [YourCloudLibrary](https://www.yourcloudlibrary.com/)
 
 [More info](./supported_sites.md)
 
 ## Installation
 audiobook-dl can be installed from the repo itself or through pip.
 
+To get the newest stable version with pip run:
 ```shell
-git clone https://github.com/jo1gi/audiobook-dl.git
-cd audiobook-dl
-python3 setup.py install
+pip install audiobook-dl
+```
+
+If you want to use the newest version (can be unstable) run:
+```shell
+pip install "git+https://github.com/jo1gi/audiobook-dl.git"
 ```
 or
 ```shell
-pip install audiobook-dl
+git clone https://github.com/jo1gi/audiobook-dl.git
+cd audiobook-dl
+python3 setup.py install
 ```
 
 Some features require [ffmpeg](https://ffmpeg.org/) which can be installed
 through most package managers or from [ffmpeg.org/download.html](https://ffmpeg.org/download.html).
 
 ## Authentication
```

### Comparing `audiobook-dl-0.4.4/audiobook_dl.egg-info/SOURCES.txt` & `audiobook-dl-0.5.0/audiobook_dl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 .gitignore
 LICENSE
 README.md
-mypy.ini
 pyproject.toml
 setup.py
 shell.nix
 supported_sites.md
+.github/FUNDING.yml
+.github/ISSUE_TEMPLATE/bug_report.md
 .github/workflows/ci.yml
 .github/workflows/pytest.yml
 audiobook_dl.egg-info/PKG-INFO
 audiobook_dl.egg-info/SOURCES.txt
 audiobook_dl.egg-info/dependency_links.txt
 audiobook_dl.egg-info/entry_points.txt
 audiobook_dl.egg-info/requires.txt
@@ -29,30 +30,32 @@
 audiobookdl/assets/errors/no_files_found.txt
 audiobookdl/assets/errors/no_source_found.txt
 audiobookdl/assets/errors/request_error.txt
 audiobookdl/assets/errors/user_not_authorized.txt
 audiobookdl/output/__init__.py
 audiobookdl/output/download.py
 audiobookdl/output/encryption.py
+audiobookdl/output/formats.py
 audiobookdl/output/output.py
 audiobookdl/output/metadata/__init__.py
 audiobookdl/output/metadata/ffmpeg.py
 audiobookdl/output/metadata/id3.py
 audiobookdl/output/metadata/mp4.py
 audiobookdl/sources/__init__.py
 audiobookdl/sources/audiobooksdotcom.py
 audiobookdl/sources/bookbeat.py
 audiobookdl/sources/chirp.py
 audiobookdl/sources/ereolen.py
 audiobookdl/sources/librivox.py
 audiobookdl/sources/nextory.py
 audiobookdl/sources/overdrive.py
+audiobookdl/sources/rss.py
+audiobookdl/sources/saxo.py
 audiobookdl/sources/scribd.py
 audiobookdl/sources/storytel.py
 audiobookdl/sources/yourcloudlibrary.py
 audiobookdl/sources/source/__init__.py
 audiobookdl/sources/source/networking.py
 audiobookdl/utils/__init__.py
 audiobookdl/utils/audiobook.py
 audiobookdl/utils/dependencies.py
-tests/test_output.py
 tests/test_urls.py
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/__main__.py` & `audiobook-dl-0.5.0/audiobookdl/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,71 @@
-from audiobookdl import Source, logging, args, output
+from audiobookdl import Source, logging, args, output, __version__
 from audiobookdl.exceptions import AudiobookDLException
 from .utils import dependencies
 from .output.download import download
 from .sources import find_compatible_source
 
 import os
 import sys
 from rich.prompt import Prompt
+from typing import Optional
+import traceback
 
-def get_cookie_path(options):
+def get_cookie_path(options) -> Optional[str]:
     """Find path to cookie file"""
     if options.cookie_file is not None and os.path.exists(options.cookie_file):
         return options.cookie_file
     if os.path.exists("./cookies.txt"):
         return "./cookies.txt"
+    return None
 
 def get_or_ask(name: str, hidden: bool, options) -> str:
     """Return `value` if it exists else asks for a value"""
     if hasattr(options, name) and getattr(options, name):
         return getattr(options, name)
     return Prompt.ask(name.capitalize(), password=hidden)
 
 def login(source: Source, options):
     login_data = {}
     for name in source.login_data:
         hidden = name == "password"
         login_data[name] = get_or_ask(name, hidden, options)
     source.login(**login_data)
 
-def get_urls(options):
+def get_urls(options) -> list[str]:
     urls = []
     # Args
     urls.extend(options.urls)
     # File
     if options.input_file:
         with open(options.input_file, "r") as f:
             urls.extend(f.read().split())
     return urls
 
-def run():
+def run() -> None:
     """Main function"""
     # Parsing arguments
     options = args.parse_arguments()
     # Applying arguments as global constants
     logging.debug_mode = options.debug
     logging.quiet_mode = options.quiet
     logging.ffmpeg_output = options.ffmpeg_output or options.debug
+    logging.debug(f"audiobook-dl {__version__}", remove_styling=True)
+    logging.debug(f"python {sys.version}", remove_styling=True)
     urls = get_urls(options)
     if not urls:
         logging.simple_help()
         exit()
     try:
         dependencies.check_dependencies(options)
         for url in urls:
             run_on_url(options, url)
     except AudiobookDLException as e:
         e.print()
+        traceback.print_exc()
         exit(1)
 
 def run_on_url(options, url: str):
     logging.log("Finding compatible source")
     s = find_compatible_source(url)
     # Load cookie file
     cookie_path = get_cookie_path(options)
@@ -75,23 +81,22 @@
         download_cover(s)
     else:
         download(s, options)
 
 
 def print_output(source: Source, options):
     """Prints output location"""
-    source.before()
+    source.prepare()
     meta = source.get_metadata()
     location = output.gen_output_location(options.template, meta, options.remove_chars)
     print(location)
 
 
 def download_cover(source: Source):
-    source.before()
-    ext = source.get_cover_extension()
+    source.prepare()
     cover = source.get_cover()
     if cover:
-        with open(f"cover.{ext}", "wb") as f:
-            f.write(cover)
+        with open(f"cover.{cover.extension}", "wb") as f:
+            f.write(cover.image)
 
 if __name__ == "__main__":
     run()
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/args.py` & `audiobook-dl-0.5.0/audiobookdl/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import argparse
+from audiobookdl import __version__
+from typing import Any
 
 
-def parse_arguments():
+def parse_arguments() -> Any:
     parser = argparse.ArgumentParser(
         prog="audiobook-dl",
         description="Download audiobooks from websites",
     )
     parser.add_argument(
+        '-v',
+        '--version',
+        action = "version",
+        version = f"audiobook-dl {__version__}"
+    )
+    parser.add_argument(
         'urls',
         help="Urls to download from",
         nargs='*',
     )
     parser.add_argument(
         '-c',
         '--cookies',
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/exceptions.py` & `audiobook-dl-0.5.0/audiobookdl/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import audiobookdl.sources as sources
 from .logging import print_error_file, error
 from typing import Optional
 
 class AudiobookDLException(Exception):
     error_description = "unknown"
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         self.data = kwargs
 
-    def print(self):
+    def print(self) -> None:
         print_error_file(self.error_description, **self.data)
 
 class DataNotPresent(AudiobookDLException):
     error_description = "data_not_present"
 
 class FailedCombining(AudiobookDLException):
     error_description = "failed_combining"
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/logging.py` & `audiobook-dl-0.5.0/audiobookdl/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+from rich.text import Text
+from rich.style import Style
+from rich.markup import render, escape
 from rich.console import Console
 from rich.progress import Progress, ProgressColumn
 from typing import Union
 from audiobookdl.utils import read_asset_file
 
 debug_mode = False
 quiet_mode = False
 ffmpeg_output = False
 console = Console(stderr=True)
+DEBUG_PREFIX = render("[yellow bold]DEBUG[/]")
 
-def debug(msg: str):
+def debug(msg: str, remove_styling=False):
     """Print debug msg"""
     if debug_mode:
-        log(f"[yellow bold]DEBUG[/] {msg}")
+        if remove_styling:
+            rendered_msg = render(msg, style=Style(bold=False, color="white"))
+            console.print(DEBUG_PREFIX, rendered_msg)
+        else:
+            console.print(DEBUG_PREFIX, msg)
 
 
 def log(msg: str):
     """Display msg in log"""
     if not quiet_mode:
         console.print(msg)
 
@@ -32,13 +40,13 @@
 
 
 def print_asset_file(path: str):
     """Read asset file and print it"""
     console.print(read_asset_file(path))
 
 
-def simple_help():
+def simple_help() -> None:
     """Print basic help information"""
     print_asset_file("assets/simple_help.txt")
 
 def progress(progress_format: list[Union[str, ProgressColumn]]) -> Progress:
     return Progress(*progress_format, console=console)
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/output/download.py` & `audiobook-dl-0.5.0/audiobookdl/output/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-from audiobookdl import AudiobookFile, Source, logging
-from audiobookdl.exceptions import UserNotAuthorized, NoFilesFound, FailedCombining
+from audiobookdl import AudiobookFile, Source, logging, Audiobook
+from audiobookdl.exceptions import UserNotAuthorized, NoFilesFound
 from . import metadata, output, encryption
 
 import os
 import shutil
 from functools import partial
-from typing import Any, Union
+from typing import Any, Union, Optional
 from rich.progress import Progress, BarColumn, ProgressColumn
 from rich.prompt import Confirm
 from multiprocessing.pool import ThreadPool
 
+
 DOWNLOAD_PROGRESS: list[Union[str, ProgressColumn]] = [
     "{task.description}", BarColumn(), "[progress.percentage]{task.percentage:>3.0f}%"
 ]
 
 
 def download(source: Source, options):
     """Downloads audiobook from source object"""
-    # Downloading audiobook info
+    try:
+        audiobook = create_audiobook(source)
+        output_dir = output.gen_output_location(options.output_template, audiobook.metadata, options.remove_chars)
+        download_audiobook(audiobook, output_dir, options)
+    except KeyboardInterrupt:
+        logging.log("Stopped download")
+        logging.log("Cleaning up files")
+        shutil.rmtree(output_dir)
+
+
+def create_audiobook(source: Source) -> Audiobook:
+    """Creates a new `Audiobook` object from a `Source`"""
     if source.requires_authentication and not source.authenticated:
         raise UserNotAuthorized
-    logging.log("Downloading metadata")
-    source.before()
+    source.prepare()
     files = source.get_files()
     if len(files) == 0:
         raise NoFilesFound
-    output_dir = output.gen_output_location(
-        options.output_template,
-        source.metadata(),
-        options.remove_chars
+    return Audiobook(
+        session = source._session,
+        metadata = source.get_metadata(),
+        chapters = source.get_chapters(),
+        files = files,
+        cover = source.get_cover()
     )
-    # Downloading audio files
-    filenames = download_files_output(source, files, output_dir)
-    # Finding output format
-    if options.output_format:
-        output_format = options.output_format
-    else:
-        output_format = os.path.splitext(filenames[0])[1][1:]
-        if output_format == "ts":
-            output_format = "mp3"
-    # Converting audio files to specified format
-    logging.log("Converting files")
-    filenames = output.convert_output(filenames, output_format)
-    # Single audiofile
-    if options.combine or len(filenames) == 1:
-        combined_audiobook(source, filenames, output_dir, output_format, options)
-    # Multiple audiofiles
+
+
+def download_audiobook(audiobook: Audiobook, output_dir: str, options):
+    """Download, convert, combine, and add metadata to files from `Audiobook` object"""
+    # Downloading files
+    filepaths = download_files_with_cli_output(audiobook, output_dir)
+    # Converting files
+    current_format, output_format = get_output_audio_format(options.output_format, filepaths)
+    if current_format != output_format:
+        logging.log("Converting files")
+        filepaths = output.convert_output(filepaths, output_format)
+    # Combine files
+    if options.combine:
+        logging.log("Combining files")
+        output_path = f"{output_dir}.{output_format}"
+        output.combine_audiofiles(filepaths, output_dir, output_path)
+        filepaths = [output_path]
+    # Add metadata
+    if len(filepaths) == 1:
+        add_metadata_to_file(audiobook, filepaths[0], options)
     else:
-        add_metadata_to_dir(source, filenames, output_dir)
+        add_metadata_to_dir(audiobook, filepaths, output_dir, options)
+
+
+def add_metadata_to_file(audiobook: Audiobook, filepath: str, options):
+    """Embed metadata into a single file"""
+    if audiobook.chapters and not options.no_chapters:
+        logging.log("Adding chapters")
+        metadata.add_chapters(filepath, audiobook.chapters)
+    logging.log("Adding metadata")
+    metadata.add_metadata(filepath, audiobook.metadata)
+    if audiobook.cover:
+        logging.log("Embedding cover")
+        metadata.embed_cover(filepath, audiobook.cover)
 
-def setup_download_dir(path: str):
-    """Creates output folder"""
-    if os.path.isdir(path):
-        answer = Confirm.ask(f"The folder '{path}' already exists. Do you want to override it?")
-        if answer:
-            shutil.rmtree(path)
-        else:
-            exit()
-    os.makedirs(path)
 
-def download_files_output(
-        source: Source,
-        files: list[AudiobookFile],
-        output_dir: str
-    ) -> list[str]:
-    """Download `files` with progress bar in terminal"""
-    if len(files) > 1:
+def add_metadata_to_dir(audiobook: Audiobook, filepaths: list[str], output_dir: str, options):
+    """Add metadata to a directory with audio files"""
+    for filepath in filepaths:
+        metadata.add_metadata(filepath, audiobook.metadata)
+    if audiobook.cover:
+        logging.log("Adding cover")
+        cover_path = os.path.join(output_dir, f"cover.{audiobook.cover.extension}")
+        with open(cover_path, "wb") as f:
+            f.write(audiobook.cover.image)
+
+
+def download_files_with_cli_output(audiobook: Audiobook, output_dir: str) -> list[str]:
+    """
+    Download `audiobook` with cli output
+    Returns a list of paths of the downloaded files
+    """
+    if len(audiobook.files) > 1:
         setup_download_dir(output_dir)
     with logging.progress(DOWNLOAD_PROGRESS) as progress:
         task = progress.add_task(
-            f"Downloading {len(files)} files - [blue]{source.get_title()}",
-            total = len(files)
+            f"Downloading {len(audiobook.files)} files [blue]{audiobook.title}",
+            total = len(audiobook.files)
         )
-        # Function for updating progress bar
-        p = partial(progress.advance, task)
-        # List of new filenames
-        filenames = download_files(source, p, files, output_dir)
-        remaining: float = progress.tasks[0].remaining or 0
-        progress.advance(task, remaining)
-        return filenames
-
-
-def create_filename(
-        title: str,
-        length: int,
-        index: int,
-        output_dir: str,
-        file: AudiobookFile,
-    ) -> str:
-    """Create filename of audiobook file"""
-    if length == 1:
-        path = f"{output_dir}.{file.ext}"
+        update_progress = partial(progress.advance, task)
+        filepaths = download_files(audiobook, output_dir, update_progress)
+        # Make sure progress bar is at 100%
+        remaining_progress: float = progress.tasks[0].remaining or 0
+        update_progress(remaining_progress)
+        # Return filenames of downloaded files
+        return filepaths
+
+
+def create_filepath(audiobook: Audiobook, output_dir: str, index: int) -> str:
+    """Create output file path for file number `index` in `audibook`"""
+    extension = audiobook.files[index].ext
+    if len(audiobook.files) == 1:
+        path = f"{output_dir}.{extension}"
     else:
-        name = f"{title} - Part {index}.{file.ext}"
+        name = f"{audiobook.title} - Part {index}.{extension}"
         path = os.path.join(output_dir, name)
     return path
 
-def download_file(args: tuple[AudiobookFile, int, int, str, Any, Source]):
-    # Setting up variables
-    file, length, index, output_dir, progress, source = args
+
+def download_file(args: tuple[Audiobook, str, int, Any]) -> str:
+    # Prepare download
+    audiobook, output_dir, index, update_progress = args
+    file = audiobook.files[index]
+    filepath = create_filepath(audiobook, output_dir, index)
     logging.debug(f"Starting downloading file: {file.url}")
-    path = create_filename(source.get_title(), length, index, output_dir, file)
-    req = source._session.get(file.url, headers=file.headers, stream=True)
-    file_size = int(req.headers["Content-length"])
-    total: float = 0
-    # Downloading file
-    with open(path, "wb") as f:
-        for chunk in req.iter_content(chunk_size=1024):
+    request = audiobook.session.get(file.url, headers=file.headers, stream=True)
+    total_filesize = int(request.headers["Content-length"])
+    # Download file
+    with open(filepath, "wb") as f:
+        for chunk in request.iter_content(chunk_size=1024):
             f.write(chunk)
-            new = len(chunk)/file_size
-            total += new
-            progress(new)
-    progress(1-total)
-    # Decrypting file if necessary
+            download_progress = len(chunk)/total_filesize
+            update_progress(download_progress)
+    # Decrypt file if necessary
     if file.encryption_method:
-        encryption.decrypt_file(path, file.encryption_method)
-    return path
+        encryption.decrypt_file(filepath, file.encryption_method)
+    # Return filepath
+    return filepath
 
 
-def download_files(
-        source: Source,
-        update,
-        files: list[AudiobookFile],
-        output_dir: str
-    ) -> list[str]:
-    """Downloads and saves audiobook files to disk"""
-    filenames = []
+def download_files(audiobook: Audiobook, output_dir: str, update_progress) -> list[str]:
+    """Download files from audiobook and return paths of the downloaded files"""
+    filepaths = []
     with ThreadPool(processes=20) as pool:
         arguments = []
-        for n, f in enumerate(files):
-            arguments.append((f, len(files), n+1, output_dir, update, source))
-        for i in pool.imap(download_file, arguments):
-            filenames.append(i)
-    return filenames
-
-def combined_audiobook(source: Source,
-                       filenames: list[str],
-                       output_dir: str,
-                       output_format: str,
-                       options):
-    """Combines audiobook into a single audio file and embeds metadata"""
-    # Combining files
-    output_file = f"{output_dir}.{output_format}"
-    if len(filenames) > 1:
-        logging.log("Combining files")
-        output.combine_audiofiles(filenames, output_dir, output_file)
-        if not os.path.exists(output_file):
-            raise FailedCombining
-        shutil.rmtree(output_dir)
-    # Adding metadata
-    embed_metadata_in_file(source, output_file, options)
-
-
-def embed_metadata_in_file(source: Source, output_file: str, options):
-    """Embed metadata into combined audiobook file"""
-    chapters = source.get_chapters()
-    if chapters and not options.no_chapters:
-        logging.log("Adding chapters")
-        metadata.add_chapters(output_file, chapters)
-    if source.metadata is not None:
-        logging.log("Adding metadata")
-        metadata.add_metadata(output_file, source.metadata())
-    cover = source.get_cover()
-    if cover is not None:
-        logging.log("Embedding cover")
-        metadata.embed_cover(output_file, cover, source.get_cover_extension())
+        for index in range(len(audiobook.files)):
+            arguments.append((audiobook, output_dir, index, update_progress))
+        for filepath in pool.imap(download_file, arguments):
+            filepaths.append(filepath)
+    return filepaths
+
+
+def get_output_audio_format(option: Optional[str], files: list[str]) -> tuple[str, str]:
+    """
+    Get output format for files
+
+    `option` is used if specied; else it's based on the file extensions
+    """
+    current_format = os.path.splitext(files[0])[1][1:]
+    if option:
+        output_format = option
+    elif current_format == "ts":
+        output_format = "mp3"
+    else:
+        output_format = current_format
+    return current_format, output_format
 
 
-def add_metadata_to_dir(source: Source, filenames: list[str], output_dir: str):
-    """Adds metadata to dir of audiobook files"""
-    for filename in filenames:
-        metadata.add_metadata(filename, source.metadata())
-    cover = source.get_cover()
-    if cover is not None:
-        logging.log("Downloading cover")
-        cover_path = os.path.join(
-            output_dir,
-            f"cover.{source.get_cover_extension()}"
-        )
-        with open(cover_path, 'wb') as f:
-            f.write(cover)
+def setup_download_dir(path: str):
+    """Creates output folder"""
+    if os.path.isdir(path):
+        answer = Confirm.ask(f"The folder '[blue]{path}[/blue]' already exists. Do you want to override it?")
+        if answer:
+            shutil.rmtree(path)
+        else:
+            exit()
+    os.makedirs(path)
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/output/encryption.py` & `audiobook-dl-0.5.0/audiobookdl/output/encryption.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from Crypto.Cipher import AES
 from audiobookdl.utils.audiobook import AudiobookFileEncryption, AESEncryption
 
-def decrypt_file(path, encryption_method: AudiobookFileEncryption):
+def decrypt_file(path: str, encryption_method: AudiobookFileEncryption):
+    """Decrypt encrypted file in place"""
     if isinstance(encryption_method, AESEncryption):
         decrypt_file_aes(path, encryption_method.key, encryption_method.iv)
 
-def decrypt_file_aes(path, key, iv):
+def decrypt_file_aes(path: str, key: bytes, iv: bytes):
+    """Decrypt AES encrypted file in place"""
     with open(path, "rb") as f:
         cipher = AES.new(key, AES.MODE_CBC, iv)
         decrypted = cipher.decrypt(f.read())
     with open(path, "wb") as f:
         f.write(decrypted)
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/output/metadata/__init__.py` & `audiobook-dl-0.5.0/audiobookdl/output/metadata/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from audiobookdl import logging, Chapter
+from audiobookdl import logging, Chapter, AudiobookMetadata, Cover
 from audiobookdl.utils import dependencies
 from . import id3, mp4, ffmpeg
 import os
 
-def add_metadata(filepath: str, metadata: dict[str, str]):
+def add_metadata(filepath: str, metadata: AudiobookMetadata):
     """Adds metadata to the given audio file"""
     if id3.is_id3_file(filepath):
         id3.add_id3_metadata(filepath, metadata)
     elif mp4.is_mp4_file(filepath):
         mp4.add_mp4_metadata(filepath, metadata)
     else:
         logging.debug("Could not add any metadata")
 
 
-def embed_cover(filepath: str, image: bytes, extension: str):
+def embed_cover(filepath: str, cover: Cover):
     """Embeds an image into the given audio file"""
     if id3.is_id3_file(filepath):
-        id3.embed_id3_cover(filepath, image, extension)
+        id3.embed_id3_cover(filepath, cover)
     elif mp4.is_mp4_file(filepath):
-        mp4.embed_mp4_cover(filepath, image, extension)
+        mp4.embed_mp4_cover(filepath, cover)
     else:
         logging.debug("Could not embed cover")
 
 
 def add_chapters(filepath: str, chapters: list[Chapter]):
     """Adds chapters to the given audio file"""
     if id3.is_id3_file(filepath):
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/output/metadata/ffmpeg.py` & `audiobook-dl-0.5.0/audiobookdl/output/metadata/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.4.4/audiobookdl/output/metadata/id3.py` & `audiobook-dl-0.5.0/audiobookdl/output/metadata/id3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 import os
-from audiobookdl import logging, Chapter
+from audiobookdl import logging, Chapter, AudiobookMetadata, Cover
 
 from mutagen import File as MutagenFile
 from mutagen.easyid3 import EasyID3
 from mutagen.mp3 import MP3
 from mutagen.id3 import ID3, APIC, CHAP, TIT2, CTOC, CTOCFlags, ID3NoHeaderError
 
 # Conversion table between metadata names and ID3 tags
@@ -25,34 +25,34 @@
 }
 
 def is_id3_file(filepath: str) -> bool:
     """Returns true if `filepath` points to an id3 file"""
     ext = re.search(r"(?<=(\.))\w+$", filepath)
     return ext is not None and ext.group(0) in ID3_FORMATS
 
-def add_id3_metadata(filepath: str, metadata: dict[str, str]):
+def add_id3_metadata(filepath: str, metadata: AudiobookMetadata):
     """Add ID3 metadata tags to the given audio file"""
     audio = MP3(filepath, ID3=EasyID3)
     # Adding tags
-    for key, value in metadata.items():
+    for key, value in metadata.all_properties(allow_duplicate_keys=False):
         if key in ID3_CONVERT:
             audio[ID3_CONVERT[key]] = value
         elif key in EasyID3.valid_keys.keys():
             audio[key] = value
         else:
             logging.debug(f"Tried to add invalid id3 tag: {key}")
     audio.save(v2_version=3)
 
-def embed_id3_cover(filepath: str, image: bytes, extension: str):
-    mimetype = EXTENSION_TO_MIMETYPE[extension]
+def embed_id3_cover(filepath: str, cover: Cover):
+    mimetype = EXTENSION_TO_MIMETYPE[cover.extension]
     try:
         audio = ID3(filepath)
     except ID3NoHeaderError:
         return
-    audio.add(APIC(type=0, data=image, mime=mimetype))
+    audio.add(APIC(type=0, data=cover.image, mime=mimetype))
     audio.save()
 
 def add_id3_chapter(audio: ID3, start: int, end: int, title: str, index: int):
     """Adds a single chapter to the given audio file"""
     audio.add(CHAP(
         element_id=u"chp"+str(index),
         start_time=int(start),
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/output/metadata/mp4.py` & `audiobook-dl-0.5.0/audiobookdl/output/metadata/mp4.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from audiobookdl import logging
+from audiobookdl import logging, AudiobookMetadata, Cover
 from mutagen.easymp4 import EasyMP4
 from mutagen.mp4 import MP4, MP4Cover, Chapter as MP4Chapter, MP4Chapters
 
 MP4_EXTENSIONS = ["mp4","m4a","m4p","m4b","m4r","m4v"]
 
 MP4_CONVERT = {
     "author": "artist",
@@ -20,30 +20,30 @@
 
 def is_mp4_file(filepath: str) -> bool:
     """Returns true if `filepath` points to an id3 file"""
     ext = re.search(r"(?<=(\.))\w+$", filepath)
     return ext is not None and ext.group(0) in MP4_EXTENSIONS
 
 
-def add_mp4_metadata(filepath: str, metadata: dict[str, str]):
+def add_mp4_metadata(filepath: str, metadata: AudiobookMetadata):
     """Add mp4 metadata tags to the given audio file"""
     audio = EasyMP4(filepath)
-    for key, value in metadata.items():
+    for key, value in metadata.all_properties(allow_duplicate_keys=True):
         # System defined metadata tags
         if key in MP4_CONVERT:
             audio[MP4_CONVERT[key]] = value
         elif key in audio.Get.keys():
             audio[key] = value
         else:
             audio.tags.RegisterFreeformKey(key, key.capitalize()) # type: ignore
             audio[key] = value
     audio.save()
 
 
-def embed_mp4_cover(filepath: str, image: bytes, extension: str):
-    if not extension in MP4_COVER_FORMATS:
+def embed_mp4_cover(filepath: str, cover: Cover):
+    if not cover.extension in MP4_COVER_FORMATS:
         return
     audio = MP4(filepath)
     audio["covr"] = [
-        MP4Cover(image, imageformat=MP4_COVER_FORMATS[extension])
+        MP4Cover(cover.image, imageformat=MP4_COVER_FORMATS[cover.extension])
     ]
     audio.save()
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/output/output.py` & `audiobook-dl-0.5.0/audiobookdl/output/output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,65 @@
-from audiobookdl import logging
+from audiobookdl import logging, AudiobookMetadata
+from audiobookdl.exceptions import FailedCombining
 
 import os
+import shutil
 import platform
-from typing import List, Dict
 import subprocess
 
 LOCATION_DEFAULTS = {
     'album': 'NA',
     'artist': 'NA',
 }
 
-def gen_output_filename(booktitle: str, file: Dict[str, str], template: str) -> str:
+def gen_output_filename(booktitle: str, file: dict[str, str], template: str) -> str:
     """Generates an output filename based on different attributes of the
     file"""
     arguments = {**file, **{"booktitle": booktitle}}
     filename = template.format(**arguments)
     return _fix_output(filename)
 
 
-def combine_audiofiles(filenames: List[str], tmp_dir: str, output_path: str):
+def combine_audiofiles(filenames: list[str], tmp_dir: str, output_path: str):
     """Combines the given audiofiles in `path` into a new file"""
     inputs = "|".join(filenames)
     subprocess.run(
         ["ffmpeg", "-i", f"concat:{inputs}", "-safe", "0", "-c", "copy", output_path],
         capture_output=not logging.ffmpeg_output,
     )
+    if not os.path.exists(output_path):
+        raise FailedCombining
+    shutil.rmtree(tmp_dir)
 
 
-def convert_output(filenames: List[str], output_format: str):
+def convert_output(filenames: list[str], output_format: str):
     """Converts a list of audio files into another format and return new
     files"""
     new_paths = []
     for old_path in filenames:
         split_path = os.path.splitext(old_path)
         new_path = f"{split_path[0]}.{output_format}"
         if not output_format == split_path[1][1:]:
             subprocess.run(
                 ["ffmpeg", "-i", old_path, new_path],
-                capture_output=not logging.ffmpeg_output)
+                capture_output=not logging.ffmpeg_output
+            )
             os.remove(old_path)
         new_paths.append(f"{os.path.splitext(old_path)[0]}.{output_format}")
     return new_paths
 
 
-def gen_output_location(template: str, metadata: Dict[str, str], remove_chars: str) -> str:
+def gen_output_location(template: str, metadata: AudiobookMetadata, remove_chars: str) -> str:
     """Generates the location of the output based on attributes of the
     audiobook"""
     if metadata is None:
         metadata = {}
-    metadata["title"] = _fix_output(metadata["title"])
-    metadata = {**LOCATION_DEFAULTS, **metadata}
-    formatted = template.format(**metadata)
+    metadata.title = _fix_output(metadata.title)
+    metadata_dict = {**LOCATION_DEFAULTS, **metadata.all_properties_dict()}
+    formatted = template.format(**metadata_dict)
     formatted = _remove_chars(formatted, remove_chars)
     return formatted
 
 
 def _fix_output(title: str) -> str:
     """Returns title without characters system can't handle"""
     title = title.replace("/", "-")
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/__init__.py` & `audiobook-dl-0.5.0/audiobookdl/sources/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from .audiobooksdotcom import AudiobooksdotcomSource
 from .bookbeat import BookBeatSource
 from .chirp import ChirpSource
 from .ereolen import EreolenSource
 from .librivox import LibrivoxSource
 from .nextory import NextorySource
 from .overdrive import OverdriveSource
+from .saxo import SaxoSource
 from .scribd import ScribdSource
 from .storytel import StorytelSource
 from .yourcloudlibrary import YourCloudLibrarySource
 
 from ..exceptions import NoSourceFound
-from typing import List
 import re
 
 def find_compatible_source(url: str) -> Source:
     """Finds the first source that supports the given url"""
     sources = get_source_classes()
     for source in sources:
         for n, m in enumerate(source.match):
@@ -30,18 +30,23 @@
         AudiobooksdotcomSource,
         BookBeatSource,
         ChirpSource,
         EreolenSource,
         LibrivoxSource,
         NextorySource,
         OverdriveSource,
+        SaxoSource,
         ScribdSource,
         StorytelSource,
         YourCloudLibrarySource,
     ]
 
-def get_source_names() -> List[str]:
-    results: List[str] = []
+def get_source_names() -> list[str]:
+    """
+    Returns the names of all sources available
+    There are sometimes multiple names for the same source
+    """
+    results: list[str] = []
     for source in get_source_classes():
         for source_name in source.names:
             results.append(source_name)
     return sorted(results, key=lambda x: x.lower())
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/audiobooksdotcom.py` & `audiobook-dl-0.5.0/audiobookdl/sources/librivox.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 from .source import Source
-from audiobookdl import AudiobookFile
-import re
-from urllib.parse import unquote
+from audiobookdl import AudiobookFile, AudiobookMetadata, Cover
 
-BASEURL = "https://www.audiobooks.com/book/stream/"
 
+class LibrivoxSource(Source):
+    _authentication_methods: list[str] = []
+
+    names = [ "Librivox" ]
 
-class AudiobooksdotcomSource(Source):
     match = [
-        r"{}\d+(/\d)?".format(BASEURL)
+        r"https?://librivox.org/.+"
     ]
-    names = [ "audiobooks.com" ]
 
-    def before(self):
-        self.iden = re.search(
-                r"(?<=({}))\d+".format(BASEURL),
-                self.url).group(0)
-        self.scrape_url = f"{BASEURL}{self.iden}/1"
-
-    def get_title(self):
-        return self.find_elem_in_page(self.scrape_url, "h2#bookTitle")
-
-    def get_cover(self):
-        cover_url = "http:" + self.find_elem_in_page(
-                self.scrape_url,
-                "img.bookimage",
-                data="src")
-        return self.get(cover_url)
-
-    def get_user_agent(self):
-        raw = self._session.cookies.get("ci_session")
-        return unquote(raw).split("\"")[11]
-
-    def get_files(self):
-        headers = {
-            "User-Agent": self.get_user_agent()
-        }
-        page: str = self._session.get(
-                self.scrape_url,
-                headers=headers
-                ).content.decode('utf8')
-        media_url = re.search(r"(?<=(mp3: \")).+(?=(&rs))", page)
-        if media_url is None:
-            return []
-
-        files = [AudiobookFile(
-            url=media_url.group(0),
-            ext="mp3",
-        )]
+
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self.find_elem_in_page(self.url, ".content-wrap h1")
+        return AudiobookMetadata(title)
+
+    def get_cover(self) -> Cover:
+        cover_url = self.find_elem_in_page(
+            self.url,
+            ".book-page-book-cover img",
+            data="src"
+        )
+        cover_data = self.get(cover_url)
+        return Cover(cover_data, "jpg")
+
+    def get_files(self) -> list[AudiobookFile]:
+        parts = self.find_elems_in_page(self.url,
+                                        ".chapter-download .chapter-name")
+        files = []
+        for part in parts:
+            files.append(AudiobookFile(
+                url = part.get("href"),
+                title = part.text,
+                ext = "mp3"
+            ))
         return files
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/bookbeat.py` & `audiobook-dl-0.5.0/audiobookdl/sources/bookbeat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter
+from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover
 from typing import Any, Optional
 import uuid
 from audiobookdl.exceptions import UserNotAuthorized, MissingBookAccess
 import base64
 import re
 
 
@@ -31,32 +31,25 @@
         headers = {
             "accept": "application/hal+json",
             "bb-client": "BookBeatApp",
             "bb-device": get_device_id(),
         }
         self._session.headers = headers
 
-        j = {"username": username, "password": password}
+        login_json = {"username": username, "password": password}
 
-        r = self._session.post("https://api.bookbeat.com/api/login", json=j)
-        if not r.status_code == 200:
-            raise UserNotAuthorized
-
-        tokens = r.json()
+        tokens = self.post_json(
+            "https://api.bookbeat.com/api/login",
+            json=login_json
+        )
         self._session.headers.update({"authorization": "Bearer " + tokens["token"]})
-
-        r = self._session.get(
+        self.saved_books = self.get_json(
             "https://api.bookbeat.com/api/my/books/saved?offset=0&limit=100"
         )
-        if not r.status_code == 200:
-            raise MissingBookAccess
-        self.saved_books = r.json()
 
-    def get_title(self) -> str:
-        return self.book_info["metadata"]["title"]
 
     def get_files(self) -> list[AudiobookFile]:
         dl_info = self.get_json(
             "https://api.bookbeat.com/api/downloadinfo/" + str(self.book_info["bookid"])
         )
         # Find license_url
         if "_embedded" in dl_info:
@@ -77,54 +70,52 @@
                     headers=self._session.headers,
                     ext="mp4",
                 )
             ]
         raise MissingBookAccess
 
 
-    def get_metadata(self) -> dict[str, Any]:
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self.book_info["metadata"]["title"]
+        metadata = AudiobookMetadata(title)
         try:
             contributors = next(
                 iter(
                     [
                         e["contributors"]
                         for e in self.book_info["metadata"]["editions"]
                         if e["format"] == "audioBook"
                     ]
                 ),
                 None,
             )
             if not contributors:
-                return {}
-            metadata = {
-                "authors": [
-                    f"{a['firstname']} {a['lastname']}"
-                    for a in contributors
-                    if "author" in a["role"]
-                ],
-                "narrators": [
-                    f"{n['firstname']} {n['lastname']}"
-                    for n in contributors
-                    if "narrator" in n["role"]
-                ],
-            }
+                return metadata
+            for contributor in contributors:
+                name = f"{contributor['firstname']} {contributor['lastname']}"
+                if "author" in contributor["role"]:
+                    metadata.add_author(name)
+                if "narrator" in contributor["role"]:
+                    metadata.add_narrator(name)
             return metadata
         except:
-            return {}
+            return metadata
 
     def get_chapters(self) -> list[Chapter]:
         chapters = []
         for chapter_number, track in enumerate(self.book_info["license"]["tracks"]):
             chapters.append(Chapter(track["start"], f"Chapter {chapter_number+1}"))
         return chapters
 
-    def get_cover(self) -> Optional[bytes]:
-        return self.get(self.book_info["metadata"]["cover"])
+    def get_cover(self) -> Cover:
+        cover_url = self.book_info["metadata"]["cover"]
+        cover_data = self.get(cover_url)
+        return Cover(cover_data, "jpg")
 
-    def before(self):
+    def prepare(self):
         book_id_re = r"(\d+)$"
         wanted_id_match = re.search(book_id_re, self.url)
         if not wanted_id_match:
             raise ValueError(f"Couldn't get bookid from url {self.url}")
         wanted_id = wanted_id_match.group(1)
         for book in self.saved_books["_embedded"]["savedBooks"]:
             if str(book["bookid"]) == wanted_id:
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/chirp.py` & `audiobook-dl-0.5.0/audiobookdl/sources/chirp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, logging
+from audiobookdl import AudiobookFile, Chapter, logging, AudiobookMetadata, Cover
 
-from typing import List, Optional
+from typing import Optional
 import base64
 from Crypto.Cipher import AES
 
 LOGIN_URL = "https://www.chirpbooks.com/users/sign_in"
 
 class ChirpSource(Source):
     match = [
@@ -14,44 +14,46 @@
 
     names = [ "Chirp" ]
 
     headers = {
         "content-type": "application/json"
     }
 
-    def get_tracks(self, book_id):
+    def _get_tracks(self, book_id):
         response = self.post_json(
             f"https://www.chirpbooks.com/api/graphql",
             json = {
                 "operationName": "fetchAudiobookTracks",
                 "query": "query fetchAudiobookTracks($id:ID!){audiobook(id:$id){tracks{partNumber chapterNumber offsetFromBookStartMs durationMs displayName}}}",
                 "variables": {
                     "id": book_id
                 }
             },
             headers = self.headers,
         )
         return response["data"]["audiobook"]["tracks"]
 
-    def get_title(self) -> str:
-        return self.find_elem_in_page(self.url, "title")
 
-    def get_metadata(self):
-        metadata = {}
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self.find_elem_in_page(self.url, "title")
+        metadata = AudiobookMetadata(title)
         for credit in self.find_elems_in_page(self.url, ".credit"):
             text = credit.text
             if text.startswith("Written by"):
-                metadata["author"] = text[11:]
+                metadata.add_author(text[11:])
             elif text.startswith("Narrated by"):
-                metadata["narrator"] = text[12:]
+                metadata.add_narrator(text[12:])
         return metadata
 
-    def get_cover(self) -> Optional[bytes]:
+
+    def get_cover(self) -> Cover:
         cover_url = self.find_elem_in_page(self.url, "img.cover-image", data="src")
-        return self.get(cover_url)
+        cover_data = self.get(cover_url)
+        return Cover(cover_data, "jpg")
+
 
     def get_audio_url(self, track):
         url_resp = self.post_json(
             f"https://www.chirpbooks.com/api/graphql",
             json = {
                 "operationName": "fetchAudiobookTrackUrl",
                 "query": "query fetchAudiobookTrackUrl($id:ID!,$partNumber:Int!,$chapterNumber:Int!){audiobook(id:$id){track(partNumber:$partNumber,chapterNumber:$chapterNumber){webPlayerMediaUrl}}}",
@@ -64,18 +66,18 @@
             headers = self.headers
         )
         webplayermediaurl = url_resp["data"]["audiobook"]["track"]["webPlayerMediaUrl"]
         ciphertext = base64.b64decode(webplayermediaurl)
         cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
         return cipher.decrypt(ciphertext).decode("utf8")[:-1]
 
-    def get_files(self) -> List[AudiobookFile]:
+
+    def get_files(self) -> list[AudiobookFile]:
         files = []
         for track in self.tracks:
-            pass
             files.append(AudiobookFile(
                 url = self.get_audio_url(track),
                 ext = "mp3",
                 title = track["displayName"],
             ))
         return files
 
@@ -86,22 +88,24 @@
         for track in self.tracks:
             title = track["displayName"]
             chapters.append(Chapter(start_time, title))
             start_time += track["durationMs"]
         return chapters
 
 
-    def calc_iv(self):
-        user_id = self.user_id
-        padded_user_id = f"{'x'*(12-len(str(user_id)))}{user_id}"
+    def _calc_iv(self):
+        """Creates IV based on `user_id` to decrypt audio url"""
+        padding = 'x'*(12-len(str(self.user_id)))
+        padded_user_id = f"{padding}{self.user_id}"
         return base64.b64encode(bytes(padded_user_id, "UTF-8"))
 
-    def before(self):
+
+    def prepare(self):
         self.book_id = int(self.find_elem_in_page(self.url, "div.user-audiobook", "data-audiobook-id"))
         logging.debug(f"{self.book_id=}")
         self.user_id = int(self.find_in_page(self.url, r'"id":(\d+)', 1))
         logging.debug(f"{self.user_id=}")
-        self.tracks = self.get_tracks(self.book_id)
-        self.iv = self.calc_iv()
+        self.tracks = self._get_tracks(self.book_id)
+        self.iv = self._calc_iv()
         logging.debug(f"{self.iv=}")
         self.key = bytes(self.find_elem_in_page(self.url, "div.user-audiobook", "data-dk"), "UTF-8")
         logging.debug(f"{self.key=}")
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/ereolen.py` & `audiobook-dl-0.5.0/audiobookdl/sources/ereolen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .source import Source
-from audiobookdl import  AudiobookFile, logging, utils
+from audiobookdl import  AudiobookFile, logging, utils, AudiobookMetadata, Cover
 from audiobookdl.exceptions import UserNotAuthorized, RequestError
 
-from typing import Dict, Optional, List
+from typing import Optional
 import re
 import json
 
 LOGIN_PAGE_URL = "https://ereolen.dk/adgangsplatformen/login?destination=/user"
 
 class EreolenSource(Source):
     _authentication_methods = [
@@ -19,54 +19,51 @@
     login_data = [ "username", "password", "library" ]
 
     match = [
         r"https?://ereolen.dk/ting/object/.+"
     ]
     book_id: str
 
-    def get_title(self):
-        if not self.meta:
-            return None
-        return self.meta["title"]
-
-    def get_metadata(self):
-        if not self.meta:
-            return {}
-        metadata = {
-            "author": self.meta["artist"]
-        }
+
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self.meta["title"]
+        metadata = AudiobookMetadata(title)
+        metadata.add_author(self.meta["artist"])
         return metadata
 
-    def get_cover(self):
-        if not self.meta:
-            return None
-        return self.get(self.meta["cover"])
-
-    def get_files(self) -> List[AudiobookFile]:
-        if not self.book_id:
-            return []
+
+    def get_cover(self) -> Cover:
+        cover_data = self.get(self.meta["cover"])
+        return Cover(cover_data, "jpg")
+
+    def get_files(self) -> list[AudiobookFile]:
         return self.get_stream_files(
             f"https://audio.api.streaming.pubhub.dk/v1/stream/hls/{self.book_id}/playlist.m3u8"
         )
 
     def _get_libraries(self):
-        libraries_raw = self.find_in_page(LOGIN_PAGE_URL, "libraries = ({.+})<", 1)
+        """Returns list of available libraries for login"""
+        libraries_raw = self.find_in_page(
+            LOGIN_PAGE_URL,
+            "libraries = ({.+})<",
+            group_index=1
+        )
         libraries = {}
         for library in json.loads(libraries_raw)["folk"]:
             library_name = library["name"]
             library_id = library["branchId"]
             libraries[library_name] = library_id
         return libraries
 
     def _login(self, username: str, password: str, library: str): # type: ignore
         login_path = self.find_elem_in_page(LOGIN_PAGE_URL, "#borchk-login-form", "action")
-        logging.debug(f"{login_path=}")
         library_attr_name = self.find_elem_in_page(LOGIN_PAGE_URL, "#borchk-login-form label", "for")
-        logging.debug(f"{library_attr_name=}")
         libraries = self._get_libraries()
+        logging.debug(f"{login_path=}")
+        logging.debug(f"{library_attr_name=}")
         logging.debug(f"{libraries=}")
         if library not in libraries.keys():
             library = utils.nearest_string(library, list(libraries.keys()))
             logging.debug(f"No matching library found. Using nearest: {library}")
         self.post(
             f"https://login.bib.dk{login_path}",
             headers = { "Content-Type": "application/x-www-form-urlencoded" },
@@ -74,23 +71,26 @@
                 library_attr_name: library,
                 "agency": libraries[library],
                 "userId": username,
                 "pincode": password
             }
         )
 
-    def before(self):
-        ajax: Optional[Dict] = self.get_json(f"{self.url}/listen/ajax")
+    def prepare(self):
+        ajax: Optional[dict] = self.get_json(f"{self.url}/listen/ajax")
         if not ajax:
             raise RequestError
         logging.debug(f"{ajax=}")
         if ajax[1]["title"] != "Lyt":
             raise UserNotAuthorized
         id_match = re.search(r"(?<=(o=))[0-9a-f\-]+", ajax[1]["data"])
         if id_match and id_match.group():
             self.book_id = id_match.group()
             logging.debug(f"{self.book_id=}")
         else:
             logging.debug("Could not find book id")
             raise UserNotAuthorized
-        self.meta: Optional[Dict] = self.get_json(f"https://audio.api.streaming.pubhub.dk/v1/orders/{self.book_id}")
+        meta: Optional[dict] = self.get_json(f"https://audio.api.streaming.pubhub.dk/v1/orders/{self.book_id}")
+        if meta is None:
+            raise UserNotAuthorized
+        self.meta = meta
         logging.debug(f"{self.meta=}")
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/nextory.py` & `audiobook-dl-0.5.0/audiobookdl/sources/nextory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter
+from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover
 from typing import Any, Optional
 import hashlib
 import uuid
 import platform
 
 
 def calculate_checksum(username: str, password: str, salt: str) -> str:
@@ -99,37 +99,39 @@
             "login_info": login_info,
             "account_list": account_list,
             "account_info": account_info,
             "active": active,
         }
         self._session.headers.update({'apiver': "7.5"})
 
-    def get_title(self) -> str:
-        return self.book_info["title"]
 
     def get_files(self) -> list[AudiobookFile]:
         return [AudiobookFile(url=self.book_info["file"]["url"], headers=self._session.headers, ext="mp3")]
 
-    def get_metadata(self) -> dict[str,Any]:
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self.book_info["title"]
+        metadata = AudiobookMetadata(title)
         try:
             book_info = self._session.get("https://api.nextory.se/api/app/product/7.5/bookinfo",
                                          params={"id": self.book_info["id"]}).json()
-            metadata = {"authors": [a for a in self.book_info["authors"]],
-                        "narrators": [n for n in book_info["data"]["books"]["narrators"]]}
+            metadata.add_authors(self.book_info["authors"])
+            metadata.add_narrators(book_info["data"]["books"]["narrators"])
             return metadata
         except:
-            return {}
+            return metadata
 
     def get_chapters(self) -> list[Chapter]:
         # Nextory has no chapters...?
         return []
 
-    def get_cover(self) -> Optional[bytes]:
-        return self.get(self.book_info["imgurl"].replace("{$width}", "640"))
+    def get_cover(self) -> Cover:
+        cover_url = self.book_info["imgurl"].replace("{$width}", "640")
+        cover_data = self.get(cover_url)
+        return Cover(cover_data, "jpg")
 
-    def before(self):
+    def prepare(self):
         wanted_id = self.url.split("-")[-1].replace("/", "")
         for book in self.user_data["active"]["data"]["books"]:
             if str(book["id"]) == wanted_id:
                 self.book_info = book
                 return
         raise PermissionError(f"Book with id {wanted_id} was not found in My Library.")
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/scribd.py` & `audiobook-dl-0.5.0/audiobookdl/sources/scribd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, logging
+from audiobookdl import AudiobookFile, Chapter, logging, AudiobookMetadata, Cover
 from audiobookdl.exceptions import UserNotAuthorized, RequestError, DataNotPresent
+from typing import Optional
 
 import io
 from PIL import Image
-from typing import Dict, List
 
 class ScribdSource(Source):
     match = [
         r"https?://(www.)?scribd.com/listen/\d+",
         r"https?://(www.)?scribd.com/audiobook/\d+/"
     ]
     names = [ "Scribd" ]
     _original = False
-    media: Dict = {}
+    media: dict = {}
 
-    def get_title(self):
+    def _get_title(self):
         if self._title[-5:] == ", The":
             split = self._title.split(', ')
             if len(split) == 2:
                 return f"{split[1]} {split[0]}"
         return self._title
 
-    def get_cover(self):
+    def get_cover(self) -> Optional[Cover]:
         # Downloading image from scribd
         raw_cover = self.get(self._cover)
         if raw_cover is None:
             return None
-        # Removing padding on the top and bottom if it is a normal book
         if self._original:
-            return raw_cover
+            return Cover(raw_cover, "jpg")
+        # Removing padding on the top and bottom if it is a normal book
         im = Image.open(io.BytesIO(raw_cover))
         width, height = im.size
         cropped = im.crop((0, int((height-width)/2), width, int(width+(height-width)/2)))
         cover = io.BytesIO()
         cropped.save(cover, format="jpeg")
-        return cover.getvalue()
+        return Cover(cover.getvalue(), "jpg")
 
-    def get_metadata(self):
-        metadata = {}
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self._get_title()
+        metadata = AudiobookMetadata(title)
         if not self._original:
-            if len(self.meta["authors"]):
-                metadata["author"] = "; ".join(self.meta["authors"])
-            if len(self.meta["series"]):
-                metadata["series"] = self.meta["series"][0]
+            metadata.add_authors(self.meta["authors"])
+            if self.meta["series"]:
+                metadata.series = self.meta["series"][0]
         return metadata
 
     def _get_chapter_title(self, chapter):
         number = chapter["chapter_number"]
         if number == 0:
             return "Introduction"
         return f"Chapter {number}"
@@ -58,65 +58,55 @@
             start_time = 0
             for chapter in self.meta["chapters"]:
                 title = self._get_chapter_title(chapter)
                 chapters.append(Chapter(start_time, title))
                 start_time += chapter["duration"]
         return chapters
 
-    def get_files(self) -> List[AudiobookFile]:
+    def get_files(self) -> list[AudiobookFile]:
         if self._original:
             return self.get_stream_files(
                 self._stream_url,
-                headers={"Authorization": self._jwt})
+                headers={"Authorization": self._jwt},
+            )
         else:
             files = []
             for i in self.media["playlist"]:
-            # for _, i in enumerate(self.media["playlist"]):
                 chapter = i["chapter_number"]
-                # chapter_str = "0"*(3-len(str(part)))+str(part)
                 files.append(AudiobookFile(
                     url = i["url"],
                     title = f"Chapter {chapter}",
                     ext = "mp3",
                 ))
-                # files.append({
-                #     "url": i["url"],
-                #     "title": f"Chapter {chapter}",
-                #     "part": chapter_str,
-                #     "ext": "mp3",
-                #     "album": self.get_title(),
-                # })
             return files
 
-    def before(self):
+    def prepare(self):
         try:
+            # Change url to listen page if info page was used
             if self.match_num == 1:
                 book_id = self.url.split("/")[4]
                 self.url = f"https://www.scribd.com/listen/{book_id}"
-            user_id = self.find_in_page(
-                    self.url,
-                    r'(?<=(account_id":"scribd-))\d+')
             book_id = self.find_in_page(
-                    self.url,
-                    r'(?<=(external_id":"))(scribd_)?\d+')
+                self.url,
+                r'(?<=(external_id":"))(scribd_)?\d+',
+                force_cookies = True
+            )
         except DataNotPresent:
             raise UserNotAuthorized
-        headers = {
-            'Session-Key': self.find_in_page(
-                self.url,
-                '(?<=(session_key":"))[^"]+')
-        }
+        # The audiobook is a Scribd original if the id starts with "scribd_"
         if book_id[:7] == "scribd_":
-            self._original_before(book_id)
+            self._original_prepare(book_id)
         else:
-            self._normal_before(book_id, user_id, headers)
+            self._normal_prepare(book_id)
 
-    def _normal_before(self, book_id: str, user_id: str, headers: Dict):
+    def _normal_prepare(self, book_id: str):
         """Download necessary data for normal audiobooks on scribd"""
         try:
+            headers = {'Session-Key': self.find_in_page(self.url, '(?<=(session_key":"))[^"]+')}
+            user_id = self.find_in_page(self.url, r'(?<=(account_id":"scribd-))\d+')
             misc = self.get_json(
                 f"https://api.findawayworld.com/v4/accounts/scribd-{user_id}/audiobooks/{book_id}",
                 headers=headers,
             )
             self.meta = misc['audiobook']
             self._title = self.meta["title"]
             self._cover = self.meta["cover_url"]
@@ -125,26 +115,29 @@
                 headers=headers,
                 json={
                     "license_id": misc['licenses'][0]['id']
                 }
             )
             self.misc = misc
         except RequestError:
-            logging.debug("Could not retrive data from book")
             raise UserNotAuthorized
 
-    def _original_before(self, book_id: str):
+    def _original_prepare(self, book_id: str):
         """Download necessary data for scribd originals"""
         self._original = True
         self._csrf = self.get_json(
             "https://www.scribd.com/csrf_token",
-            headers={"href": self.url})
+            headers={"href": self.url}
+        )
         self._jwt = self.find_in_page(
             self.url,
-            r'(?<=("jwt_token":"))[^"]+')
+            r'(?<=("jwt_token":"))[^"]+'
+        )
         self._stream_url = f"https://audio.production.scribd.com/audiobooks/{book_id[7:]}/192kbps.m3u8"
         self._title = self.find_all_in_page(
             self.url,
-            r'(?:("title":"))([^"]+)')[1][1]
+            r'(?:("title":"))([^"]+)'
+        )[1][1]
         self._cover = self.find_in_page(
             self.url,
-            r'(?<=("cover_url":"))[^"]+')
+            r'(?<=("cover_url":"))[^"]+'
+        )
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/source/__init__.py` & `audiobook-dl-0.5.0/audiobookdl/sources/source/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,153 +1,152 @@
 # Internal imports
 from . import networking
-from audiobookdl import logging, AudiobookFile, Chapter
+from audiobookdl import logging, AudiobookFile, Chapter, AudiobookMetadata, Cover
 from audiobookdl.exceptions import DataNotPresent
 
 # External imports
 import requests
 import lxml.html
 from lxml.cssselect import CSSSelector
 import re
 from http.cookiejar import MozillaCookieJar
 from typing import Any, Optional
 
 class Source:
     """An abstract class for downloading audiobooks from a specific
     online source."""
 
+    # Data required for logging in
+    login_data: list[str] = [ "username", "password" ]
     # A list of regexes that indicates which website a sevice supports
     match: list[str] = []
+    # list of names
+    names: list[str] = []
     # Methods for authenticating
     _authentication_methods: list[str] = [ "cookies" ]
-    # Data required for logging in
-    login_data: list[str] = [ "username", "password" ]
     # If cookies are loaded
-    _authenticated = False
+    __authenticated = False
     # Cache of previously loaded pages
-    _pages: dict[str, bytes] = {}
-    # list of names
-    names: list[str] = []
+    __pages: dict[str, bytes] = {}
 
     def __init__(self, url, match_num):
         self.url = url
         self.match_num = match_num
         self._session = requests.Session()
 
     @property
     def requires_authentication(self):
         """Returns `True` if this source requires authentication to download books"""
         return len(self._authentication_methods) > 0
 
     @property
     def authenticated(self):
         """Returns `True` if the source has been authenticated"""
-        return self._authenticated
+        return self.__authenticated
 
     @property
     def supports_cookies(self):
         return "cookies" in self._authentication_methods
 
     def load_cookie_file(self, cookie_file: str):
         """Loads cookies from a cookie file into session"""
         if self.supports_cookies:
             cookie_jar = MozillaCookieJar()
             cookie_jar.load(cookie_file, ignore_expires=True)
             self._session.cookies.update(cookie_jar)
-            self._authenticated = True
+            self.__authenticated = True
 
     @property
     def supports_login(self):
         return "login" in self._authentication_methods
 
     def _login(self, username: str, password: str):
         pass
 
-    def login(self, **kwargs):
+    def login(self, **kwargs) -> None:
         """Authenticate with source using username and password"""
         if self.supports_login:
             self._login(**kwargs)
-            self._authenticated = True
-
+            self.__authenticated = True
 
-    def before(self):
+    def prepare(self) -> None:
         """Operations to be run before the audiobook is downloaded"""
         pass
 
-    def get_title(self) -> str:
-        return ""
-
-    def get_metadata(self) -> dict[str, Any]:
+    def get_metadata(self) -> AudiobookMetadata:
         """Returns metadata of the audiobook"""
-        return {}
-
-    def metadata(self) -> dict[str, str]:
-        m = self.get_metadata()
-        if "authors" in m:
-            m["author"] = "; ".join(m["authors"])
-        if "narrators" in m:
-            m["narrator"] = "; ".join(m["narrators"])
-        return {
-            **m,
-            "title": self.get_title(),
-            "genre": "Audiobook"
-        }
+        raise NotImplemented
 
-    def get_cover(self) -> Optional[bytes]:
+    def get_cover(self) -> Optional[Cover]:
         """Returns the image data for the audiobook"""
         return None
 
-    def get_cover_extension(self) -> str:
-        """Returns the filetype of the cover from `get_cover`"""
-        return "jpg"
-
     def get_files(self) -> list[AudiobookFile]:
+        """Return a list of audio files for the audiobook"""
         raise NotImplemented
 
     def get_chapters(self) -> list[Chapter]:
-        """Returns a list of tuples with the starting point of the chapter and
-        the title of the chapter"""
+        """
+        Returns a list of tuples with the starting point of the chapter and
+        the title of the chapter
+        """
         return []
 
 
     def _get_page(self, url: str, **kwargs) -> bytes:
-        """Downloads a page and caches it"""
-        if url not in self._pages:
+        """Download a page and caches it"""
+        if url not in self.__pages:
             resp = self.get(url, **kwargs)
-            self._pages[url] = resp
-        return self._pages[url]
+            self.__pages[url] = resp
+        return self.__pages[url]
 
-    def find_elem_in_page(self, url, selector, data=None, **kwargs):
-        """Finds an element in a page based on a css selector"""
+    def find_elem_in_page(self, url: str, selector: str, data=None, **kwargs):
+        """
+        Find the first html element in page from `url` that matches `selector`.
+        Will return the attribute specified in `data`. Will return element text
+        if `data` is `None`.
+        Will cache the page.
+        """
         results = self.find_elems_in_page(url, selector, **kwargs)
         if len(results) == 0:
             logging.debug(f"Could not find matching element from {url} with {selector}")
             raise DataNotPresent
         elem = results[0]
         if data is None:
             return elem.text
         return elem.get(data)
 
-    def find_elems_in_page(self, url, selector, **kwargs) -> list[Any]:
+    def find_elems_in_page(self, url: str, selector: str, **kwargs) -> list[Any]:
+        """
+        Find all html elements in the page from `url` thats matches `selector`.
+        Will cache the page.
+        """
         sel = CSSSelector(selector)
         page: bytes = self._get_page(url, **kwargs)
         tree = lxml.html.fromstring(page.decode("utf8"))
         results = sel(tree)
         return results
 
-    def find_in_page(self, url, regex, group_index=0, **kwargs) -> str:
-        """Find some text in a page based on a regex"""
-        m = re.search(regex, self._get_page(url, **kwargs).decode("utf8"))
+    def find_in_page(self, url: str, regex: str, group_index: int = 0, **kwargs) -> str:
+        """
+        Find some text in a page based on a regex.
+        Will cache the page.
+        """
+        page = self._get_page(url, **kwargs).decode("utf8")
+        m = re.search(regex, page)
         if m is None:
             logging.debug(f"Could not find match from {url} with {regex}")
             raise DataNotPresent
         return m.group(group_index)
 
-    def find_all_in_page(self, url, regex, **kwargs):
-        """Finds all places in a page that matches the regex"""
+    def find_all_in_page(self, url: str, regex: str, **kwargs) -> list[Any]:
+        """
+        Find all places in a page that matches the regex.
+        Will cache the page.
+        """
         return re.findall(regex, self._get_page(url, **kwargs).decode("utf8"))
 
     # Networking
     post = networking.post
     get = networking.get
     post_json = networking.post_json
     get_json = networking.get_json
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/source/networking.py` & `audiobook-dl-0.5.0/audiobookdl/sources/source/networking.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 from audiobookdl import AudiobookFile, exceptions, logging
 from audiobookdl.utils.audiobook import AESEncryption
 
 import json
 import os
 import m3u8
-from typing import List
+import requests
 
-def post(self, url, **kwargs):
+
+def post(self, url: str, **kwargs) -> bytes:
     """Make post request with `Source` session"""
     resp = self._session.post(url, **kwargs)
     if resp.status_code == 200:
         return resp.content
     logging.debug(f"Failed to download data from: {url}\nResponse:\n{resp.content}")
     raise exceptions.RequestError
 
 
-def get(self, url, **kwargs) -> bytes:
+def get(self, url: str, force_cookies: bool = False, **kwargs) -> bytes:
     """Make get request with `Source` session"""
-    resp = self._session.get(url, **kwargs)
+    if force_cookies:
+        resp = self._session.get(
+            url,
+            cookies=_get_all_cookies(self._session),
+            **kwargs
+        )
+    else:
+        resp = self._session.get(url, **kwargs)
     if resp.status_code == 200:
         return resp.content
     logging.debug(f"Failed to download data from: {url}\nResponse:\n{resp.content}")
     raise exceptions.RequestError
 
 
-def post_json(self, url, **kwargs):
+def post_json(self, url: str, **kwargs) -> dict:
     """Downloads data with the given url and converts it to json"""
     resp = self.post(url, **kwargs)
     return json.loads(resp.decode('utf8'))
 
 
-def get_json(self, url, **kwargs):
+def get_json(self, url: str, **kwargs) -> dict:
     """Downloads data with the given url and converts it to json"""
     resp = self.get(url, **kwargs)
     return json.loads(resp.decode('utf8'))
 
-def get_stream_files(self, url, headers={}) -> List[AudiobookFile]:
+
+def get_stream_files(self, url: str, headers={}) -> list[AudiobookFile]:
     """Creates a list of audio files from an m3u8 file"""
     playlist = m3u8.load(url, headers=headers)
     files = []
     for _, seg in enumerate(playlist.segments):
         current = AudiobookFile(
             url = seg.absolute_uri,
             ext = os.path.splitext(seg.absolute_uri)[1][1:],
@@ -48,7 +57,19 @@
         if seg.key:
             current.encryption_method = AESEncryption(
                 key = self._get_page(seg.key.absolute_uri, headers=headers),
                 iv = int(seg.key.iv, 0).to_bytes(16, byteorder='big')
             )
         files.append(current)
     return files
+
+
+def _get_all_cookies(session: requests.Session) -> dict[str, str]:
+    """
+    Retrieves all cookies from session
+
+    :returns: Dictionary of cookies
+    """
+    cookies = {}
+    for cookie in session.cookies:
+        cookies[cookie.name] = str(cookie.value)
+    return cookies
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/storytel.py` & `audiobook-dl-0.5.0/audiobookdl/sources/storytel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, logging
+from audiobookdl import AudiobookFile, Chapter, logging, AudiobookMetadata, Cover
 from audiobookdl.exceptions import UserNotAuthorized, MissingBookAccess
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 from typing import Any, Optional
 
 
 class StorytelSource(Source):
@@ -37,33 +37,35 @@
         })
         resp = self._session.get(url)
         if resp.status_code != 200:
             raise UserNotAuthorized
         self._session.headers.update({"authorization": f"Bearer {resp.json()['accountInfo']['jwt']}"})
         self.user_data = resp.json()
 
-    def get_title(self) -> str:
-        return self.book_info["book"]["name"]
 
     def get_files(self) -> list[AudiobookFile]:
         aid = self.book_info["book"]["AId"]
         url = f"https://www.storytel.com/mp3streamRangeReq?startposition=0&programId={aid}" \
               f"&token={self.user_data['accountInfo']['singleSignToken']}"
         return [AudiobookFile(url=url, headers=self._session.headers, ext="mp3")]
 
-    def get_metadata(self) -> dict[str,Any]:
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self.book_info["book"]["name"]
+        metadata = AudiobookMetadata(title)
         try:
-            metadata = {"authors": [a["name"] for a in self.book_info["book"]["authors"]],
-                        "narrators": [a["name"] for a in self.book_info["abook"]["narrators"]]}
+            for author in self.book_info["book"]["authors"]:
+                metadata.add_author(author["name"])
+            for narrator in self.book_info["abook"]["narrators"]:
+                metadata.add_narrator(narrator["name"])
             if "series" in self.book_info["book"]:
                 if len(self.book_info["book"]["series"]) > 0:
-                    metadata["series"] = self.book_info["book"]["series"][0]["name"]
+                    metadata.series = self.book_info["book"]["series"][0]["name"]
             return metadata
         except:
-            return {}
+            return metadata
 
     def get_chapters(self) -> list[Chapter]:
         url = f"https://api.storytel.net/playback-metadata/consumable/{self.book_info['book']['consumableId']}"
         try:
             chapters: list[Chapter] = []
             storytel_metadata = self._session.get(url).json()
             if "formats" in storytel_metadata and len(storytel_metadata["formats"]) > 0:
@@ -78,19 +80,20 @@
                     for c in f["chapters"]:
                         chapters.append(Chapter(start_time, c["title"] if c["title"] else f"Chapter {c['number']}"))
                         start_time += c["durationInMilliseconds"]
             return chapters
         except:
             return []
 
-    def get_cover(self) -> Optional[bytes]:
-        url = f"https://www.storytel.com/images/{self.book_info['abook']['isbn']}/640x640/cover.jpg"
-        return self.get(url)
+    def get_cover(self) -> Cover:
+        cover_url = f"https://www.storytel.com/images/{self.book_info['abook']['isbn']}/640x640/cover.jpg"
+        cover_data = self.get(cover_url)
+        return Cover(cover_data, "jpg")
 
-    def before(self):
+    def prepare(self):
         wanted_id = self.url.split("-")[-1]
         bookshelf_url = f"https://www.storytel.com/api/getBookShelf.action" \
                         f"?token={self.user_data['accountInfo']['singleSignToken']}"
         self.user_data["bookshelf"] = self._session.get(bookshelf_url).json()
         for book in self.user_data["bookshelf"]["books"]:
             if book["book"]["consumableId"] == wanted_id:
                 self.book_info = book
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/sources/yourcloudlibrary.py` & `audiobook-dl-0.5.0/audiobookdl/sources/yourcloudlibrary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 from .source import Source
-from audiobookdl import AudiobookFile, logging
+from audiobookdl import AudiobookFile, logging, AudiobookMetadata, Cover
 from audiobookdl.exceptions import UserNotAuthorized, RequestError
 
 import requests.utils
 import base64
-from typing import Dict, List
 
 class YourCloudLibrarySource(Source):
     match = [
         r"https?://ebook.yourcloudlibrary.com/library/[^/]+/AudioPlayer/.+"
     ]
     names = [ "YourCloudLibrary" ]
     _authentication_methods = [
         "cookies",
         "login"
     ]
-    meta: Dict
-    playlist: Dict
+    meta: dict
+    playlist: dict
 
-    def get_title(self):
-        return self.book_info["Title"]
 
-    def get_files(self) -> List[AudiobookFile]:
+    def get_files(self) -> list[AudiobookFile]:
         files = []
         for f in self.playlist["playlist"]:
             files.append(AudiobookFile(
                 url = f["url"],
                 ext = "mp3"
             ))
         return files
 
-    def get_metadata(self):
-        metadata = {}
+    def get_metadata(self) -> AudiobookMetadata:
+        title = self.book_info["Title"]
+        metadata = AudiobookMetadata(title)
         if not self.meta is None:
             try:
                 audiobook = self.meta["audiobook"]
-                metadata["authors"] = audiobook["authors"]
-                metadata["narrators"] = audiobook["narrators"]
+                metadata.add_authors(audiobook["authors"])
+                metadata.add_narrators(audiobook["narrators"])
                 if audiobook["series"] is not None and len(audiobook["series"]) >= 1:
-                    metadata["series"] = audiobook["series"][0]
+                    metadata.series = audiobook["series"][0]
             except:
-                return {}
+                return metadata
         return metadata
 
-    def get_cover(self):
-        return self.get(self.meta['audiobook']['cover_url'])
+    def get_cover(self) -> Cover:
+        cover_url = self.meta['audiobook']['cover_url']
+        cover_data = self.get(cover_url)
+        return Cover(cover_data, "jpg")
 
-    def _get_library_id(self):
+    def _get_library_id(self) -> str:
         return self.url.split("/")[-3]
 
 
-    def _get_fullfillmenttoken(self):
+    def _get_fullfillmenttoken(self) -> str:
         token_base64 = self.find_in_page(
             self.url,
             r"(?<=(\"Osi\":\"x-))[^\"]+",
             cookies=requests.utils.dict_from_cookiejar(self._session.cookies),
         )
         if token_base64 is None:
             raise UserNotAuthorized
         token = base64.b64decode(token_base64).decode('utf8')
         logging.debug(f"{token=}")
         return token
 
-    def _get_bookinfo(self):
+    def _get_bookinfo(self) -> dict:
         # Get list of borrowed books
         library = self._get_library_id()
         borrowed = self.get_json(
                 f"https://ebook.yourcloudlibrary.com/uisvc/{library}/Patron/Borrowed",
                 cookies=requests.utils.dict_from_cookiejar(self._session.cookies),
         )
         if borrowed is None:
@@ -86,18 +86,18 @@
         resp = self.post(
             f"https://ebook.yourcloudlibrary.com/uisvc/{library}/Patron/LoginPatron",
             data = {
                 "UserId": username,
                 "Password": password
             }
         )
-        logging.debug(f"Authentication response {resp}")
+        logging.debug(f"Authentication response {resp.decode('utf8')}")
 
 
-    def before(self):
+    def prepare(self):
         self.book_info = self._get_bookinfo()
         token = self._get_fullfillmenttoken()
         library = self._get_library_id()
         audioplayer = self.post_json(f"https://ebook.yourcloudlibrary.com/uisvc/{library}/AudioPlayer",
                 data={"url": f"{self.book_info['fulfillmentTokenUrl']}&token={token}"})
         if audioplayer is None:
             raise RequestError
```

### Comparing `audiobook-dl-0.4.4/audiobookdl/utils/dependencies.py` & `audiobook-dl-0.5.0/audiobookdl/utils/dependencies.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 
 def program_in_path(program) -> bool:
     """Checks if the given program is in the users path"""
     return shutil.which(program) is not None
 
 
-def check_dependencies(options):
+def check_dependencies(options) -> None:
     """Checks if the required dependencies can be found"""
     required = {
-            "combine": ["ffmpeg"]
-            }
+        "combine": ["ffmpeg"]
+    }
     logging.debug("Searching for missing dependencies")
     for key, deps in required.items():
         if getattr(options, key):
             for i in deps:
                 if not program_in_path(i):
                     raise MissingDependency(dependency=i)
```

### Comparing `audiobook-dl-0.4.4/pyproject.toml` & `audiobook-dl-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 dependencies = [
     "requests",
     "lxml",
     "rich",
     "mutagen",
     "pillow",
     "cssselect",
-    "mypy",
     "m3u8",
     "pycryptodome",
     "importlib-resources"
 ]
 dynamic = ["version"]
 
 [project.urls]
@@ -37,7 +36,20 @@
 audiobook-dl = "audiobookdl.__main__:run"
 
 [tool.setuptools.dynamic]
 version = {attr = "audiobookdl.__version__"}
 
 [tool.setuptools.package-data]
 mypkg = ["*.txt"]
+
+[tool.mypy]
+ignore_missing_imports = true
+allow_untyped_globals = false
+disallow_untyped_calls = true
+
+[[tool.mypy.overrides]]
+module = [
+    "audiobookdl.sources.*",
+    "audiobookdl.output.metadata.id3",
+    "audiobookdl.output.metadata.mp4"
+]
+disallow_untyped_calls = false
```

### Comparing `audiobook-dl-0.4.4/supported_sites.md` & `audiobook-dl-0.5.0/supported_sites.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,10 +5,11 @@
 | audiobooks.com   |    ✓    |         ✗         |                                                                                                |
 | BookBeat         |    ✗    |         ✓         | Books must be saved to My Books <br> Not tested with multi-user account <br> No metadata (yet) |
 | Chirp            |    ✓    |         ✗         |                                                                                                |
 | eReolen          |    ✓    |         ✓         | Requires library for login                                                                     |
 | Librivox         |    ✗    |         ✗         | Authentication not required                                                                    |
 | Nextory          |    ✗    |         ✓         | Books must be in "Your Library" <br/>Only single (first) account supported                     |
 | Overdrive        |    ✓    |         ✗         |                                                                                                |
+| Saxo             |    ✗    |         ✓         |                                                                                                |
 | Scribd           |    ✓    |         ✗         |                                                                                                |
 | Storytel         |    ✗    |         ✓         | Books have to be in your bookshelf                                                             |
 | YourCloudLibrary |    ✓    |         ✓         |                                                                                                |
```

### Comparing `audiobook-dl-0.4.4/tests/test_urls.py` & `audiobook-dl-0.5.0/tests/test_urls.py`

 * *Files identical despite different names*

