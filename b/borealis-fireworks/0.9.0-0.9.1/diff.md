# Comparing `tmp/borealis-fireworks-0.9.0.tar.gz` & `tmp/borealis-fireworks-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borealis-fireworks-0.9.0.tar", last modified: Fri Apr 16 06:25:08 2021, max compression
+gzip compressed data, was "borealis-fireworks-0.9.1.tar", last modified: Sat Apr 17 00:59:57 2021, max compression
```

## Comparing `borealis-fireworks-0.9.0.tar` & `borealis-fireworks-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-16 06:25:08.675675 borealis-fireworks-0.9.0/
--rw-r--r--   0 jerry      (501) staff       (20)     1067 2019-12-21 05:22:27.000000 borealis-fireworks-0.9.0/LICENSE
--rw-r--r--   0 jerry      (501) staff       (20)       15 2020-05-08 00:47:35.000000 borealis-fireworks-0.9.0/MANIFEST.in
--rw-r--r--   0 jerry      (501) staff       (20)    19883 2021-04-16 06:25:08.675322 borealis-fireworks-0.9.0/PKG-INFO
--rw-r--r--   0 jerry      (501) staff       (20)    15390 2021-04-13 07:39:29.000000 borealis-fireworks-0.9.0/README.md
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-16 06:25:08.656546 borealis-fireworks-0.9.0/borealis/
--rw-r--r--   0 jerry      (501) staff       (20)        0 2020-02-13 08:02:24.000000 borealis-fireworks-0.9.0/borealis/__init__.py
--rw-r--r--   0 jerry      (501) staff       (20)    17802 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/borealis/docker_task.py
--rwxr-xr-x   0 jerry      (501) staff       (20)    15841 2021-04-16 05:33:05.000000 borealis-fireworks-0.9.0/borealis/fireworker.py
--rwxr-xr-x   0 jerry      (501) staff       (20)    14356 2021-04-13 19:03:42.000000 borealis-fireworks-0.9.0/borealis/gce.py
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-16 06:25:08.661247 borealis-fireworks-0.9.0/borealis/setup/
--rw-r--r--   0 jerry      (501) staff       (20)      699 2020-02-13 08:02:24.000000 borealis-fireworks-0.9.0/borealis/setup/borealis-fireworker.service
--rwxr-xr--   0 jerry      (501) staff       (20)     1518 2020-05-07 06:28:43.000000 borealis-fireworks-0.9.0/borealis/setup/example_mongo_ssh.sh
--rw-r--r--   0 jerry      (501) staff       (20)      582 2020-05-19 05:45:30.000000 borealis-fireworks-0.9.0/borealis/setup/example_my_launchpad.yaml
--rw-r--r--   0 jerry      (501) staff       (20)    12169 2021-04-16 06:23:09.000000 borealis-fireworks-0.9.0/borealis/setup/how-to-install-gce-server.txt
--rw-r--r--   0 jerry      (501) staff       (20)      999 2021-04-16 05:40:55.000000 borealis-fireworks-0.9.0/borealis/setup/requirements.txt
--rwxr-xr-x   0 jerry      (501) staff       (20)      356 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/borealis/setup/startup.sh
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-16 06:25:08.664258 borealis-fireworks-0.9.0/borealis/util/
--rw-r--r--   0 jerry      (501) staff       (20)        0 2020-02-13 08:02:24.000000 borealis-fireworks-0.9.0/borealis/util/__init__.py
--rw-r--r--   0 jerry      (501) staff       (20)      881 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/borealis/util/data.py
--rw-r--r--   0 jerry      (501) staff       (20)     2905 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/borealis/util/filepath.py
--rw-r--r--   0 jerry      (501) staff       (20)     4704 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/borealis/util/gcp.py
--rw-r--r--   0 jerry      (501) staff       (20)     1012 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/borealis/util/log_filter.py
--rw-r--r--   0 jerry      (501) staff       (20)    10787 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/borealis/util/storage.py
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-16 06:25:08.667389 borealis-fireworks-0.9.0/borealis_fireworks.egg-info/
--rw-r--r--   0 jerry      (501) staff       (20)    19883 2021-04-16 06:25:08.000000 borealis-fireworks-0.9.0/borealis_fireworks.egg-info/PKG-INFO
--rw-r--r--   0 jerry      (501) staff       (20)      913 2021-04-16 06:25:08.000000 borealis-fireworks-0.9.0/borealis_fireworks.egg-info/SOURCES.txt
--rw-r--r--   0 jerry      (501) staff       (20)        1 2021-04-16 06:25:08.000000 borealis-fireworks-0.9.0/borealis_fireworks.egg-info/dependency_links.txt
--rw-r--r--   0 jerry      (501) staff       (20)       79 2021-04-16 06:25:08.000000 borealis-fireworks-0.9.0/borealis_fireworks.egg-info/entry_points.txt
--rw-r--r--   0 jerry      (501) staff       (20)      125 2021-04-16 06:25:08.000000 borealis-fireworks-0.9.0/borealis_fireworks.egg-info/requires.txt
--rw-r--r--   0 jerry      (501) staff       (20)        9 2021-04-16 06:25:08.000000 borealis-fireworks-0.9.0/borealis_fireworks.egg-info/top_level.txt
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-16 06:25:08.674445 borealis-fireworks-0.9.0/docs/
--rw-r--r--   0 jerry      (501) staff       (20)   195531 2020-05-13 21:24:04.000000 borealis-fireworks-0.9.0/docs/Borealis-Fireworks-on-Google-Cloud.png
--rw-r--r--   0 jerry      (501) staff       (20)     4942 2021-04-16 05:53:24.000000 borealis-fireworks-0.9.0/docs/changes.md
--rw-r--r--   0 jerry      (501) staff       (20)     5781 2020-11-17 21:03:05.000000 borealis-fireworks-0.9.0/docs/developer-setup.md
--rw-r--r--   0 jerry      (501) staff       (20)     6273 2020-10-25 21:47:05.000000 borealis-fireworks-0.9.0/docs/docker-build.md
--rw-r--r--   0 jerry      (501) staff       (20)     3817 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.0/docs/handy-links.md
--rw-r--r--   0 jerry      (501) staff       (20)     4157 2020-10-25 21:45:59.000000 borealis-fireworks-0.9.0/docs/install-tools.md
--rw-r--r--   0 jerry      (501) staff       (20)     3150 2020-05-13 07:43:26.000000 borealis-fireworks-0.9.0/docs/team-setup.md
--rw-r--r--   0 jerry      (501) staff       (20)       38 2021-04-16 06:25:08.675762 borealis-fireworks-0.9.0/setup.cfg
--rw-r--r--   0 jerry      (501) staff       (20)     2115 2021-04-16 05:50:13.000000 borealis-fireworks-0.9.0/setup.py
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-17 00:59:57.286670 borealis-fireworks-0.9.1/
+-rw-r--r--   0 jerry      (501) staff       (20)     1067 2019-12-21 05:22:27.000000 borealis-fireworks-0.9.1/LICENSE
+-rw-r--r--   0 jerry      (501) staff       (20)       15 2020-05-08 00:47:35.000000 borealis-fireworks-0.9.1/MANIFEST.in
+-rw-r--r--   0 jerry      (501) staff       (20)    19883 2021-04-17 00:59:57.286064 borealis-fireworks-0.9.1/PKG-INFO
+-rw-r--r--   0 jerry      (501) staff       (20)    15390 2021-04-13 07:39:29.000000 borealis-fireworks-0.9.1/README.md
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-17 00:59:57.271685 borealis-fireworks-0.9.1/borealis/
+-rw-r--r--   0 jerry      (501) staff       (20)        0 2020-02-13 08:02:24.000000 borealis-fireworks-0.9.1/borealis/__init__.py
+-rw-r--r--   0 jerry      (501) staff       (20)    17802 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/borealis/docker_task.py
+-rwxr-xr-x   0 jerry      (501) staff       (20)    15841 2021-04-16 05:33:05.000000 borealis-fireworks-0.9.1/borealis/fireworker.py
+-rwxr-xr-x   0 jerry      (501) staff       (20)    14356 2021-04-13 19:03:42.000000 borealis-fireworks-0.9.1/borealis/gce.py
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-17 00:59:57.274409 borealis-fireworks-0.9.1/borealis/setup/
+-rw-r--r--   0 jerry      (501) staff       (20)      699 2020-02-13 08:02:24.000000 borealis-fireworks-0.9.1/borealis/setup/borealis-fireworker.service
+-rwxr-xr--   0 jerry      (501) staff       (20)     1518 2020-05-07 06:28:43.000000 borealis-fireworks-0.9.1/borealis/setup/example_mongo_ssh.sh
+-rw-r--r--   0 jerry      (501) staff       (20)      582 2020-05-19 05:45:30.000000 borealis-fireworks-0.9.1/borealis/setup/example_my_launchpad.yaml
+-rw-r--r--   0 jerry      (501) staff       (20)    12169 2021-04-16 06:23:09.000000 borealis-fireworks-0.9.1/borealis/setup/how-to-install-gce-server.txt
+-rw-r--r--   0 jerry      (501) staff       (20)     1077 2021-04-17 00:55:35.000000 borealis-fireworks-0.9.1/borealis/setup/requirements.txt
+-rwxr-xr-x   0 jerry      (501) staff       (20)      356 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/borealis/setup/startup.sh
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-17 00:59:57.277534 borealis-fireworks-0.9.1/borealis/util/
+-rw-r--r--   0 jerry      (501) staff       (20)        0 2020-02-13 08:02:24.000000 borealis-fireworks-0.9.1/borealis/util/__init__.py
+-rw-r--r--   0 jerry      (501) staff       (20)      881 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/borealis/util/data.py
+-rw-r--r--   0 jerry      (501) staff       (20)     2905 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/borealis/util/filepath.py
+-rw-r--r--   0 jerry      (501) staff       (20)     4704 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/borealis/util/gcp.py
+-rw-r--r--   0 jerry      (501) staff       (20)     1012 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/borealis/util/log_filter.py
+-rw-r--r--   0 jerry      (501) staff       (20)    10787 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/borealis/util/storage.py
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-17 00:59:57.280369 borealis-fireworks-0.9.1/borealis_fireworks.egg-info/
+-rw-r--r--   0 jerry      (501) staff       (20)    19883 2021-04-17 00:59:57.000000 borealis-fireworks-0.9.1/borealis_fireworks.egg-info/PKG-INFO
+-rw-r--r--   0 jerry      (501) staff       (20)      913 2021-04-17 00:59:57.000000 borealis-fireworks-0.9.1/borealis_fireworks.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry      (501) staff       (20)        1 2021-04-17 00:59:57.000000 borealis-fireworks-0.9.1/borealis_fireworks.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry      (501) staff       (20)       79 2021-04-17 00:59:57.000000 borealis-fireworks-0.9.1/borealis_fireworks.egg-info/entry_points.txt
+-rw-r--r--   0 jerry      (501) staff       (20)      125 2021-04-17 00:59:57.000000 borealis-fireworks-0.9.1/borealis_fireworks.egg-info/requires.txt
+-rw-r--r--   0 jerry      (501) staff       (20)        9 2021-04-17 00:59:57.000000 borealis-fireworks-0.9.1/borealis_fireworks.egg-info/top_level.txt
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2021-04-17 00:59:57.285147 borealis-fireworks-0.9.1/docs/
+-rw-r--r--   0 jerry      (501) staff       (20)   195531 2020-05-13 21:24:04.000000 borealis-fireworks-0.9.1/docs/Borealis-Fireworks-on-Google-Cloud.png
+-rw-r--r--   0 jerry      (501) staff       (20)     5086 2021-04-17 00:51:16.000000 borealis-fireworks-0.9.1/docs/changes.md
+-rw-r--r--   0 jerry      (501) staff       (20)     5781 2020-11-17 21:03:05.000000 borealis-fireworks-0.9.1/docs/developer-setup.md
+-rw-r--r--   0 jerry      (501) staff       (20)     6273 2020-10-25 21:47:05.000000 borealis-fireworks-0.9.1/docs/docker-build.md
+-rw-r--r--   0 jerry      (501) staff       (20)     3817 2021-04-13 06:19:47.000000 borealis-fireworks-0.9.1/docs/handy-links.md
+-rw-r--r--   0 jerry      (501) staff       (20)     4157 2020-10-25 21:45:59.000000 borealis-fireworks-0.9.1/docs/install-tools.md
+-rw-r--r--   0 jerry      (501) staff       (20)     3150 2020-05-13 07:43:26.000000 borealis-fireworks-0.9.1/docs/team-setup.md
+-rw-r--r--   0 jerry      (501) staff       (20)       38 2021-04-17 00:59:57.286819 borealis-fireworks-0.9.1/setup.cfg
+-rw-r--r--   0 jerry      (501) staff       (20)     2115 2021-04-17 00:49:51.000000 borealis-fireworks-0.9.1/setup.py
```

### Comparing `borealis-fireworks-0.9.0/LICENSE` & `borealis-fireworks-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/PKG-INFO` & `borealis-fireworks-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borealis-fireworks
-Version: 0.9.0
+Version: 0.9.1
 Summary: Run FireWorks workflows in Google Cloud
 Home-page: https://github.com/CovertLab/borealis
 Author: Jerry Morrison
 Author-email: j.erry.morrison@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/CovertLab/borealis
 Project-URL: Documentation, https://github.com/CovertLab/borealis#borealis
```

### Comparing `borealis-fireworks-0.9.0/README.md` & `borealis-fireworks-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/docker_task.py` & `borealis-fireworks-0.9.1/borealis/docker_task.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/fireworker.py` & `borealis-fireworks-0.9.1/borealis/fireworker.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/gce.py` & `borealis-fireworks-0.9.1/borealis/gce.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/setup/borealis-fireworker.service` & `borealis-fireworks-0.9.1/borealis/setup/borealis-fireworker.service`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/setup/example_mongo_ssh.sh` & `borealis-fireworks-0.9.1/borealis/setup/example_mongo_ssh.sh`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/setup/example_my_launchpad.yaml` & `borealis-fireworks-0.9.1/borealis/setup/example_my_launchpad.yaml`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/setup/how-to-install-gce-server.txt` & `borealis-fireworks-0.9.1/borealis/setup/how-to-install-gce-server.txt`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/setup/requirements.txt` & `borealis-fireworks-0.9.1/borealis/setup/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Direct requirements
+# dnspython is needed for pymongo to access server clusters.
+dnspython==2.1.0
 docker==5.0.0
 FireWorks==1.9.7
 google-cloud-logging==2.3.1
 google-cloud-storage==1.37.1
 requests==2.25.1
 ruamel.yaml==0.17.4
 ruamel.yaml.clib==0.2.2
@@ -15,15 +17,15 @@
 chardet==4.0.0
 click==7.1.2
 distlib==0.3.1
 filelock==3.0.12
 Flask==1.1.2
 flask-paginate==0.8.1
 google-api-core==1.26.3
-google-auth==1.28.1
+google-auth==1.29.0
 google-cloud-core==1.6.0
 google-crc32c==1.1.2
 google-resumable-media==1.2.0
 googleapis-common-protos==1.53.0
 grpcio==1.37.0
 gunicorn==20.1.0
 idna==2.10
```

### Comparing `borealis-fireworks-0.9.0/borealis/util/data.py` & `borealis-fireworks-0.9.1/borealis/util/data.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/util/filepath.py` & `borealis-fireworks-0.9.1/borealis/util/filepath.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/util/gcp.py` & `borealis-fireworks-0.9.1/borealis/util/gcp.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/util/log_filter.py` & `borealis-fireworks-0.9.1/borealis/util/log_filter.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis/util/storage.py` & `borealis-fireworks-0.9.1/borealis/util/storage.py`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/borealis_fireworks.egg-info/PKG-INFO` & `borealis-fireworks-0.9.1/borealis_fireworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borealis-fireworks
-Version: 0.9.0
+Version: 0.9.1
 Summary: Run FireWorks workflows in Google Cloud
 Home-page: https://github.com/CovertLab/borealis
 Author: Jerry Morrison
 Author-email: j.erry.morrison@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/CovertLab/borealis
 Project-URL: Documentation, https://github.com/CovertLab/borealis#borealis
```

### Comparing `borealis-fireworks-0.9.0/borealis_fireworks.egg-info/SOURCES.txt` & `borealis-fireworks-0.9.1/borealis_fireworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/docs/Borealis-Fireworks-on-Google-Cloud.png` & `borealis-fireworks-0.9.1/docs/Borealis-Fireworks-on-Google-Cloud.png`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/docs/changes.md` & `borealis-fireworks-0.9.1/docs/changes.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Change Log
 
+## v0.9.1
+* Add dnspython to requirements.txt so pymongo can access server clusters.
+* Update other pips in requirements.txt for good measure.
+
 ## v0.9.0
 * Let the GCE VM metadata override the MongoDB host, including is_uri mode.
 * Add gce.py help text for using the `-o network-interface=no-address` option to creates VMs without External IP addresses.
 * Update to Fireworks 1.9.7.
 * Improve the how-to docs.
 
 ## v0.8.0
```

### Comparing `borealis-fireworks-0.9.0/docs/developer-setup.md` & `borealis-fireworks-0.9.1/docs/developer-setup.md`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/docs/docker-build.md` & `borealis-fireworks-0.9.1/docs/docker-build.md`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/docs/handy-links.md` & `borealis-fireworks-0.9.1/docs/handy-links.md`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/docs/install-tools.md` & `borealis-fireworks-0.9.1/docs/install-tools.md`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/docs/team-setup.md` & `borealis-fireworks-0.9.1/docs/team-setup.md`

 * *Files identical despite different names*

### Comparing `borealis-fireworks-0.9.0/setup.py` & `borealis-fireworks-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = re.sub(
         r']\(([\w/.-]+)\)',
         r'](https://github.com/CovertLab/borealis/blob/master/\1)',
         description2)
 
 setup(
     name='borealis-fireworks',
-    version='0.9.0',
+    version='0.9.1',
     packages=['borealis', 'borealis.util'],
     url='https://github.com/CovertLab/borealis',
     project_urls={
         'Source': 'https://github.com/CovertLab/borealis',
         'Documentation': 'https://github.com/CovertLab/borealis#borealis',
         'Changelog': 'https://github.com/CovertLab/borealis/blob/master/docs/changes.md',
     },
```

