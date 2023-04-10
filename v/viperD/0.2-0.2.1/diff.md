# Comparing `tmp/viperD-0.2.tar.gz` & `tmp/viperD-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viperD-0.2.tar", last modified: Mon Nov 21 14:22:18 2022, max compression
+gzip compressed data, was "viperD-0.2.1.tar", last modified: Wed Apr  5 09:06:21 2023, max compression
```

## Comparing `viperD-0.2.tar` & `viperD-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.736092 viperD-0.2/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-17 06:33:53.000000 viperD-0.2/LICENSE
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)       37 2022-11-21 14:21:23.000000 viperD-0.2/MANIFEST.in
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      350 2022-11-21 14:22:18.736238 viperD-0.2/PKG-INFO
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-17 06:35:49.000000 viperD-0.2/README.md
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)       80 2022-11-21 13:39:20.000000 viperD-0.2/pyproject.toml
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      571 2022-11-21 14:22:18.739251 viperD-0.2/setup.cfg
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.616287 viperD-0.2/viperD/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-18 09:02:10.000000 viperD-0.2/viperD/__init__.py
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     1055 2022-11-21 07:17:49.000000 viperD-0.2/viperD/command_line.py
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      959 2022-11-21 07:18:33.000000 viperD-0.2/viperD/dir_file_names.pkl
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.637823 viperD-0.2/viperD/templates/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     6148 2022-11-16 07:15:57.000000 viperD-0.2/viperD/templates/.DS_Store
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.640521 viperD-0.2/viperD/templates/Dockers_file/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     8196 2022-11-15 09:41:06.000000 viperD-0.2/viperD/templates/Dockers_file/.DS_Store
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.642603 viperD-0.2/viperD/templates/Dockers_file/app/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      307 2022-11-21 07:34:49.000000 viperD-0.2/viperD/templates/Dockers_file/app/Dockerfile
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.643986 viperD-0.2/viperD/templates/Dockers_file/app_backup/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)       18 2022-11-21 06:30:09.000000 viperD-0.2/viperD/templates/Dockers_file/app_backup/Dockerfile
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.645214 viperD-0.2/viperD/templates/Dockers_file/app_initiatory/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      493 2022-11-21 06:35:14.000000 viperD-0.2/viperD/templates/Dockers_file/app_initiatory/Dockerfile
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.654064 viperD-0.2/viperD/templates/Dockers_file/nginx/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      155 2022-08-17 06:03:07.000000 viperD-0.2/viperD/templates/Dockers_file/nginx/Dockerfile
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1850 2022-11-21 06:31:28.000000 viperD-0.2/viperD/templates/Dockers_file/nginx/nginx.conf
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      432 2022-11-21 06:31:59.000000 viperD-0.2/viperD/templates/Dockers_file/nginx/project.conf
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.670517 viperD-0.2/viperD/templates/Dockers_file/requirements/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)       39 2022-08-17 06:03:07.000000 viperD-0.2/viperD/templates/Dockers_file/requirements/requirements.py
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      252 2022-11-21 08:18:02.000000 viperD-0.2/viperD/templates/Dockers_file/requirements/requirements.txt
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.675868 viperD-0.2/viperD/templates/Dockers_file/ubuntu_image/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     2200 2022-11-21 06:25:09.000000 viperD-0.2/viperD/templates/Dockers_file/ubuntu_image/Dockerfile
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.678393 viperD-0.2/viperD/templates/code_mount/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-18 10:21:23.000000 viperD-0.2/viperD/templates/code_mount/__init__.py
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.689496 viperD-0.2/viperD/templates/data_mount/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-18 10:21:31.000000 viperD-0.2/viperD/templates/data_mount/__init__.py
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.695041 viperD-0.2/viperD/templates/execute/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     6148 2022-11-15 09:41:06.000000 viperD-0.2/viperD/templates/execute/.DS_Store
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.711291 viperD-0.2/viperD/templates/execute/Linux/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      744 2022-11-21 08:12:08.000000 viperD-0.2/viperD/templates/execute/Linux/build_images.sh
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1200 2022-11-21 07:51:57.000000 viperD-0.2/viperD/templates/execute/Linux/build_images_initiatory.sh
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      631 2022-11-21 08:15:38.000000 viperD-0.2/viperD/templates/execute/Linux/run_docker.sh
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      610 2022-11-21 08:14:06.000000 viperD-0.2/viperD/templates/execute/Linux/run_docker_dev host.sh
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      592 2022-11-21 08:12:43.000000 viperD-0.2/viperD/templates/execute/Linux/run_docker_dev.sh
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.735102 viperD-0.2/viperD/templates/execute/Windows/
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1727 2022-08-17 06:03:07.000000 viperD-0.2/viperD/templates/execute/Windows/build_images.bat
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1934 2022-08-17 06:03:07.000000 viperD-0.2/viperD/templates/execute/Windows/build_images_initiatory.bat
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      958 2022-08-17 06:03:07.000000 viperD-0.2/viperD/templates/execute/Windows/run_docker.bat
--rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      738 2022-08-17 06:03:07.000000 viperD-0.2/viperD/templates/execute/Windows/run_docker_dev.bat
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      215 2022-11-21 13:45:12.000000 viperD-0.2/viperD/templates/execute/readme.md
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     2621 2022-11-21 12:03:27.000000 viperD-0.2/viperD/utils.py
-drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-21 14:22:18.632774 viperD-0.2/viperD.egg-info/
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      350 2022-11-21 14:22:18.000000 viperD-0.2/viperD.egg-info/PKG-INFO
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     1495 2022-11-21 14:22:18.000000 viperD-0.2/viperD.egg-info/SOURCES.txt
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        1 2022-11-21 14:22:18.000000 viperD-0.2/viperD.egg-info/dependency_links.txt
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)       50 2022-11-21 14:22:18.000000 viperD-0.2/viperD.egg-info/entry_points.txt
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        6 2022-11-21 14:22:18.000000 viperD-0.2/viperD.egg-info/requires.txt
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        7 2022-11-21 14:22:18.000000 viperD-0.2/viperD.egg-info/top_level.txt
--rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        1 2022-11-21 14:21:35.000000 viperD-0.2/viperD.egg-info/zip-safe
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.152026 viperD-0.2.1/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     1076 2023-04-05 09:02:28.000000 viperD-0.2.1/LICENSE
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)       37 2022-11-21 14:21:23.000000 viperD-0.2.1/MANIFEST.in
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      376 2023-04-05 09:06:21.152166 viperD-0.2.1/PKG-INFO
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-17 06:35:49.000000 viperD-0.2.1/README.md
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)       80 2022-11-21 13:39:20.000000 viperD-0.2.1/pyproject.toml
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      598 2023-04-05 09:06:21.153494 viperD-0.2.1/setup.cfg
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.072147 viperD-0.2.1/viperD/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-18 09:02:10.000000 viperD-0.2.1/viperD/__init__.py
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     1055 2022-11-21 07:17:49.000000 viperD-0.2.1/viperD/command_line.py
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      959 2022-11-21 07:18:33.000000 viperD-0.2.1/viperD/dir_file_names.pkl
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.082273 viperD-0.2.1/viperD/templates/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     6148 2022-11-16 07:15:57.000000 viperD-0.2.1/viperD/templates/.DS_Store
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.084901 viperD-0.2.1/viperD/templates/Dockers_file/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     8196 2022-11-15 09:41:06.000000 viperD-0.2.1/viperD/templates/Dockers_file/.DS_Store
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.088429 viperD-0.2.1/viperD/templates/Dockers_file/app/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      307 2022-11-21 07:34:49.000000 viperD-0.2.1/viperD/templates/Dockers_file/app/Dockerfile
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.093234 viperD-0.2.1/viperD/templates/Dockers_file/app_backup/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)       18 2022-11-21 06:30:09.000000 viperD-0.2.1/viperD/templates/Dockers_file/app_backup/Dockerfile
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.096219 viperD-0.2.1/viperD/templates/Dockers_file/app_initiatory/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      493 2022-11-21 06:35:14.000000 viperD-0.2.1/viperD/templates/Dockers_file/app_initiatory/Dockerfile
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.104019 viperD-0.2.1/viperD/templates/Dockers_file/nginx/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      155 2022-08-17 06:03:07.000000 viperD-0.2.1/viperD/templates/Dockers_file/nginx/Dockerfile
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1850 2022-11-21 06:31:28.000000 viperD-0.2.1/viperD/templates/Dockers_file/nginx/nginx.conf
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      432 2022-11-21 06:31:59.000000 viperD-0.2.1/viperD/templates/Dockers_file/nginx/project.conf
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.109406 viperD-0.2.1/viperD/templates/Dockers_file/requirements/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)       39 2022-08-17 06:03:07.000000 viperD-0.2.1/viperD/templates/Dockers_file/requirements/requirements.py
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      252 2022-11-21 08:18:02.000000 viperD-0.2.1/viperD/templates/Dockers_file/requirements/requirements.txt
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.112810 viperD-0.2.1/viperD/templates/Dockers_file/ubuntu_image/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     2200 2022-11-21 06:25:09.000000 viperD-0.2.1/viperD/templates/Dockers_file/ubuntu_image/Dockerfile
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.114313 viperD-0.2.1/viperD/templates/code_mount/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-18 10:21:23.000000 viperD-0.2.1/viperD/templates/code_mount/__init__.py
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.115211 viperD-0.2.1/viperD/templates/data_mount/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2022-11-18 10:21:31.000000 viperD-0.2.1/viperD/templates/data_mount/__init__.py
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.121785 viperD-0.2.1/viperD/templates/execute/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     6148 2022-11-15 09:41:06.000000 viperD-0.2.1/viperD/templates/execute/.DS_Store
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.136984 viperD-0.2.1/viperD/templates/execute/Linux/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      744 2022-11-21 08:12:08.000000 viperD-0.2.1/viperD/templates/execute/Linux/build_images.sh
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1200 2022-11-21 07:51:57.000000 viperD-0.2.1/viperD/templates/execute/Linux/build_images_initiatory.sh
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      631 2022-11-21 08:15:38.000000 viperD-0.2.1/viperD/templates/execute/Linux/run_docker.sh
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      610 2022-11-21 08:14:06.000000 viperD-0.2.1/viperD/templates/execute/Linux/run_docker_dev host.sh
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      592 2022-11-21 08:12:43.000000 viperD-0.2.1/viperD/templates/execute/Linux/run_docker_dev.sh
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.151587 viperD-0.2.1/viperD/templates/execute/Windows/
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1727 2022-08-17 06:03:07.000000 viperD-0.2.1/viperD/templates/execute/Windows/build_images.bat
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)     1934 2022-08-17 06:03:07.000000 viperD-0.2.1/viperD/templates/execute/Windows/build_images_initiatory.bat
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      958 2022-08-17 06:03:07.000000 viperD-0.2.1/viperD/templates/execute/Windows/run_docker.bat
+-rwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)      738 2022-08-17 06:03:07.000000 viperD-0.2.1/viperD/templates/execute/Windows/run_docker_dev.bat
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      216 2023-04-05 07:43:44.000000 viperD-0.2.1/viperD/templates/execute/readme.md
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     2621 2022-11-21 12:03:27.000000 viperD-0.2.1/viperD/utils.py
+drwxr-xr-x   0 mohammad_nawaz_ahmad   (501) staff       (20)        0 2023-04-05 09:06:21.079591 viperD-0.2.1/viperD.egg-info/
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)      376 2023-04-05 09:06:21.000000 viperD-0.2.1/viperD.egg-info/PKG-INFO
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)     1495 2023-04-05 09:06:21.000000 viperD-0.2.1/viperD.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        1 2023-04-05 09:06:21.000000 viperD-0.2.1/viperD.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)       50 2023-04-05 09:06:21.000000 viperD-0.2.1/viperD.egg-info/entry_points.txt
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        6 2023-04-05 09:06:21.000000 viperD-0.2.1/viperD.egg-info/requires.txt
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        7 2023-04-05 09:06:21.000000 viperD-0.2.1/viperD.egg-info/top_level.txt
+-rw-r--r--   0 mohammad_nawaz_ahmad   (501) staff       (20)        1 2022-11-21 14:21:35.000000 viperD-0.2.1/viperD.egg-info/zip-safe
```

### Comparing `viperD-0.2/setup.cfg` & `viperD-0.2.1/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = viperD
-version = 0.2
+version = 0.2.1
 author = Mohammad Nawaz Ahmad
-author_email = mohammad_nawaz_ahmad@mckinsey.com
-description = Example package description
+author_email = nawazahmad20@hotmail.com
+description = package for running python applications using dockers
 long_description = file: README.md
-keywords = deploy, python applications
+keywords = deploy, python applications, docker
 license = BSD 3-Clause License
 classifiers = 
-	License :: OSI Approved :: BSD License
+	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires =
```

### Comparing `viperD-0.2/viperD/command_line.py` & `viperD-0.2.1/viperD/command_line.py`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/dir_file_names.pkl` & `viperD-0.2.1/viperD/dir_file_names.pkl`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/.DS_Store` & `viperD-0.2.1/viperD/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/Dockers_file/.DS_Store` & `viperD-0.2.1/viperD/templates/Dockers_file/.DS_Store`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/Dockers_file/nginx/nginx.conf` & `viperD-0.2.1/viperD/templates/Dockers_file/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/Dockers_file/ubuntu_image/Dockerfile` & `viperD-0.2.1/viperD/templates/Dockers_file/ubuntu_image/Dockerfile`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/.DS_Store` & `viperD-0.2.1/viperD/templates/execute/.DS_Store`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Linux/build_images.sh` & `viperD-0.2.1/viperD/templates/execute/Linux/build_images.sh`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Linux/build_images_initiatory.sh` & `viperD-0.2.1/viperD/templates/execute/Linux/build_images_initiatory.sh`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Linux/run_docker.sh` & `viperD-0.2.1/viperD/templates/execute/Linux/run_docker.sh`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Linux/run_docker_dev host.sh` & `viperD-0.2.1/viperD/templates/execute/Linux/run_docker_dev host.sh`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Linux/run_docker_dev.sh` & `viperD-0.2.1/viperD/templates/execute/Linux/run_docker_dev.sh`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Windows/build_images.bat` & `viperD-0.2.1/viperD/templates/execute/Windows/build_images.bat`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Windows/build_images_initiatory.bat` & `viperD-0.2.1/viperD/templates/execute/Windows/build_images_initiatory.bat`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Windows/run_docker.bat` & `viperD-0.2.1/viperD/templates/execute/Windows/run_docker.bat`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/templates/execute/Windows/run_docker_dev.bat` & `viperD-0.2.1/viperD/templates/execute/Windows/run_docker_dev.bat`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD/utils.py` & `viperD-0.2.1/viperD/utils.py`

 * *Files identical despite different names*

### Comparing `viperD-0.2/viperD.egg-info/SOURCES.txt` & `viperD-0.2.1/viperD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

