# Comparing `tmp/dolby-0.0.1.tar.gz` & `tmp/dolby-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolby-0.0.1.tar", last modified: Sun Apr  9 07:27:48 2023, max compression
+gzip compressed data, was "dolby-0.0.2.tar", last modified: Sun Apr  9 22:03:12 2023, max compression
```

## Comparing `dolby-0.0.1.tar` & `dolby-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:27:48.513414 dolby-0.0.1/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:06:31.000000 dolby-0.0.1/LICENSE
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      894 2023-04-09 07:27:48.513144 dolby-0.0.1/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      463 2023-04-09 07:06:31.000000 dolby-0.0.1/README.md
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      511 2023-04-09 07:27:38.000000 dolby-0.0.1/pyproject.toml
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 07:27:48.513471 dolby-0.0.1/setup.cfg
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:27:48.508606 dolby-0.0.1/src/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:25:01.000000 dolby-0.0.1/src/__init__.py
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:27:48.512714 dolby-0.0.1/src/dolby.egg-info/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      894 2023-04-09 07:27:48.000000 dolby-0.0.1/src/dolby.egg-info/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      180 2023-04-09 07:27:48.000000 dolby-0.0.1/src/dolby.egg-info/SOURCES.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 07:27:48.000000 dolby-0.0.1/src/dolby.egg-info/dependency_links.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 07:27:48.000000 dolby-0.0.1/src/dolby.egg-info/top_level.txt
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.633502 dolby-0.0.2/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      426 2023-04-09 22:03:12.633241 dolby-0.0.2/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 20:52:32.000000 dolby-0.0.2/README.md
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      520 2023-04-09 17:12:39.000000 dolby-0.0.2/pyproject.toml
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 22:03:12.633550 dolby-0.0.2/setup.cfg
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.621189 dolby-0.0.2/src/
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.629521 dolby-0.0.2/src/dolby/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1849 2023-04-09 21:56:51.000000 dolby-0.0.2/src/dolby/DolbyAudio.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2709 2023-04-09 21:56:17.000000 dolby-0.0.2/src/dolby/DolbyImage.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      158 2023-04-09 20:59:29.000000 dolby-0.0.2/src/dolby/DolbyText.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1835 2023-04-09 21:57:37.000000 dolby-0.0.2/src/dolby/DolbyVideo.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2224 2023-04-09 21:59:54.000000 dolby-0.0.2/src/dolby/YouTube.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      164 2023-04-09 19:41:00.000000 dolby-0.0.2/src/dolby/__init__.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1279 2023-04-09 21:52:25.000000 dolby-0.0.2/src/dolby/constants.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      801 2023-04-09 21:58:18.000000 dolby-0.0.2/src/dolby/override.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.632782 dolby-0.0.2/src/dolby.egg-info/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      426 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      351 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/SOURCES.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/dependency_links.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/top_level.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      499 2023-04-09 22:02:17.000000 dolby-0.0.2/src/test.py
```

