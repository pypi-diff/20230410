# Comparing `tmp/buttervolume-3.8.tar.gz` & `tmp/buttervolume-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buttervolume-3.8.tar", last modified: Fri Oct  7 15:55:34 2022, max compression
+gzip compressed data, was "buttervolume-3.9.tar", last modified: Tue Oct 11 21:37:51 2022, max compression
```

## Comparing `buttervolume-3.8.tar` & `buttervolume-3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ccomb     (1000) ccomb     (1000)        0 2022-10-07 15:55:34.480548 buttervolume-3.8/
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)     2081 2022-10-07 15:38:55.000000 buttervolume-3.8/CHANGES.rst
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)    11358 2022-10-07 15:38:55.000000 buttervolume-3.8/LICENSE
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)       14 2022-10-07 15:38:55.000000 buttervolume-3.8/MANIFEST.in
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)    26119 2022-10-07 15:55:34.480548 buttervolume-3.8/PKG-INFO
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)    23435 2022-10-07 15:38:55.000000 buttervolume-3.8/README.rst
-drwxr-xr-x   0 ccomb     (1000) ccomb     (1000)        0 2022-10-07 15:55:34.476548 buttervolume-3.8/buttervolume/
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)        4 2022-10-07 15:38:55.000000 buttervolume-3.8/buttervolume/VERSION
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)        0 2022-10-07 15:38:55.000000 buttervolume-3.8/buttervolume/__init__.py
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)     1965 2022-10-07 15:38:55.000000 buttervolume-3.8/buttervolume/btrfs.py
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)    16207 2022-10-07 15:38:55.000000 buttervolume-3.8/buttervolume/cli.py
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)    17224 2022-10-07 15:38:55.000000 buttervolume-3.8/buttervolume/plugin.py
-drwxr-xr-x   0 ccomb     (1000) ccomb     (1000)        0 2022-10-07 15:55:34.480548 buttervolume-3.8/buttervolume.egg-info/
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)    26119 2022-10-07 15:55:34.000000 buttervolume-3.8/buttervolume.egg-info/PKG-INFO
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)      380 2022-10-07 15:55:34.000000 buttervolume-3.8/buttervolume.egg-info/SOURCES.txt
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)        1 2022-10-07 15:55:34.000000 buttervolume-3.8/buttervolume.egg-info/dependency_links.txt
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)       55 2022-10-07 15:55:34.000000 buttervolume-3.8/buttervolume.egg-info/entry_points.txt
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)       52 2022-10-07 15:55:34.000000 buttervolume-3.8/buttervolume.egg-info/requires.txt
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)       13 2022-10-07 15:55:34.000000 buttervolume-3.8/buttervolume.egg-info/top_level.txt
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)       38 2022-10-07 15:55:34.480548 buttervolume-3.8/setup.cfg
--rw-r--r--   0 ccomb     (1000) ccomb     (1000)     1462 2022-10-07 15:38:55.000000 buttervolume-3.8/setup.py
+drwxr-sr-x   0 ccomb     (1000) ccomb     (1000)        0 2022-10-11 21:37:51.851053 buttervolume-3.9/
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)     2253 2022-10-11 19:35:42.000000 buttervolume-3.9/CHANGES.rst
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)    11358 2019-04-12 14:12:21.000000 buttervolume-3.9/LICENSE
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)       30 2022-10-11 19:14:06.000000 buttervolume-3.9/MANIFEST.in
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)    26811 2022-10-11 21:37:51.851053 buttervolume-3.9/PKG-INFO
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)    23955 2022-10-11 21:36:59.000000 buttervolume-3.9/README.rst
+drwxr-sr-x   0 ccomb     (1000) ccomb     (1000)        0 2022-10-11 21:37:51.851053 buttervolume-3.9/buttervolume/
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)        4 2022-10-11 19:24:24.000000 buttervolume-3.9/buttervolume/VERSION
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)        0 2019-04-12 14:12:21.000000 buttervolume-3.9/buttervolume/__init__.py
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)     1965 2019-04-12 14:12:21.000000 buttervolume-3.9/buttervolume/btrfs.py
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)    16358 2022-10-11 19:53:40.000000 buttervolume-3.9/buttervolume/cli.py
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)    16958 2022-10-11 19:12:55.000000 buttervolume-3.9/buttervolume/plugin.py
+drwxr-sr-x   0 ccomb     (1000) ccomb     (1000)        0 2022-10-11 21:37:51.851053 buttervolume-3.9/buttervolume.egg-info/
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)    26811 2022-10-11 21:37:51.000000 buttervolume-3.9/buttervolume.egg-info/PKG-INFO
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)      380 2022-10-11 21:37:51.000000 buttervolume-3.9/buttervolume.egg-info/SOURCES.txt
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)        1 2022-10-11 21:37:51.000000 buttervolume-3.9/buttervolume.egg-info/dependency_links.txt
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)       55 2022-10-11 21:37:51.000000 buttervolume-3.9/buttervolume.egg-info/entry_points.txt
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)       52 2022-10-11 21:37:51.000000 buttervolume-3.9/buttervolume.egg-info/requires.txt
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)       13 2022-10-11 21:37:51.000000 buttervolume-3.9/buttervolume.egg-info/top_level.txt
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)       38 2022-10-11 21:37:51.851053 buttervolume-3.9/setup.cfg
+-rw-r--r--   0 ccomb     (1000) ccomb     (1000)     1462 2022-10-07 15:25:07.000000 buttervolume-3.9/setup.py
```

### Comparing `buttervolume-3.8/CHANGES.rst` & `buttervolume-3.9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGELOG
 =========
 
+3.9 (2022-10-11)
+****************
+
+- Fixed a crash when option_copyonwrite is not set
+- Restored the test suite
+- Improved and simplified the build script and test script
+
 3.8 (2022-10-07)
 ****************
 
 - Switched to copy-on-write by default
 - Allow to choose to enable/disable copy-on-write for each volume
 - Allow to change the default SSH_PORT in the plugin config
 - Updated the base docker image and dependencies
```

### Comparing `buttervolume-3.8/LICENSE` & `buttervolume-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `buttervolume-3.8/PKG-INFO` & `buttervolume-3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buttervolume
-Version: 3.8
+Version: 3.9
 Summary: Docker plugin to manage Docker Volumes as BTRFS subvolumes
 Home-page: https://github.com/anybox/buttervolume
 Author: Christophe Combelles
 Author-email: ccomb@anybox.fr
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,20 +18,40 @@
    :target: https://travis-ci.org/anybox/buttervolume
    :alt: Travis state
 
 
 BTRFS Volume plugin for Docker
 ==============================
 
-This package provides a Docker volume plugin that creates a BTRFS subvolume for
-each container volume.
+**What will Buttervolume allow you to do?**
+
+- Quickly recover recent data after an exploit or failure of your web sites or applications
+- Quickly rollback your data to a previous version after a failed upgrade
+- Implement automatic upgrade of your applications without fear
+- Keep an history of your data
+- Make many backups without consuming more disk space than needed
+- Build a resilient hosting cluster with data replication
+- Quickly move your applications between nodes
+- Create preconfigured or templated applications to deploy in seconds
+
+**What can Buttervolume do?**
+
+- Snapshot your Docker volumes
+- Restore a snapshot to its original volume or under a new volume
+- List and remove existing snapshots of your volumes
+- Clone your Docker volumes
+- Replicate or Sync your volumes to another host
+- Schedule periodic snapshots, sync or replication of your volumes
+- Schedule periodic removal of your old snapshots
+
+**How does it work?**
+
+Buttervolume is a Docker Volume Plugin that sits on top of a BTRFS partition
+and can manage and replicate BTRFS snapshots of your Docker volumes.
 
-Please note this is **not** a BTRFS storage driver for Docker, but a plugin to
-manage volumes. It means you can use any storage driver, such as AUFS, this is
-an independant topic.
 
 .. contents::
 
 
 Introduction
 ************
 
@@ -71,31 +91,30 @@
 ******************************
 
 If you want to be a contributor, read this chapter. Otherwise jump to the next section.
 
 You first need to create a root filesystem for the plugin, using the provided Dockerfile::
 
     git clone https://github.com/anybox/buttervolume
-    cd buttervolume/docker
-    ./rebuild_rootfs.sh
+    ./build.sh
 
-Then you can create the plugin::
+By default the plugin is built for the latest commit (HEAD). You can build another version by specifying it like this::
 
-    docker plugin create anybox/buttervolume .
+    ./build.sh 3.7
 
 At this point, you can set the SSH_PORT option for the plugin by running::
 
     docker plugin set anybox/buttervolume SSH_PORT=1122
 
 Note that this option is only relevant if you use the replication feature between two nodes.
 
 Now you can enable the plugin, which should start buttervolume in the plugin
 container::
 
-    docker plugin enable anybox/buttervolume
+    docker plugin enable anybox/buttervolume:HEAD
 
 You can check it is responding by running a buttervolume command::
 
     export RUNCROOT=/run/docker/runtime-runc/plugins.moby/ # or /run/docker/plugins/runtime-root/plugins.moby/
     alias drunc="sudo runc --root $RUNCROOT"
     alias buttervolume="drunc exec -t $(drunc list|tail -n+2|awk '{print $1}') buttervolume"
     sudo buttervolume scheduled
@@ -221,15 +240,15 @@
 
     docker volume create -d anybox/buttervolume:latest myvolume
 
 or::
 
     docker volume create --volume-driver=anybox/buttervolume:latest
 
-When creating a volume, you can choose to disable copy-on-write on a per -olume
+When creating a volume, you can choose to disable copy-on-write on a per-volume
 basis. Just use the `-o` or `--opt` option as defined in the `Docker documentation
 <https://docs.docker.com/engine/reference/commandline/volume_create/#options>`_ ::
 
     docker volume create -d anybox/buttervolume -o copyonwrite=false myvolume
 
 Running the plugin locally or in legacy mode
 --------------------------------------------
@@ -335,15 +354,15 @@
 
 
 Clone a volume
 ------------------
 
 You can clone a volume as a new volume. The current volume will be cloned
 as a new volume name given as parameter. Please take care of stopping the
-container before clonning a volume::
+container before cloning a volume::
 
     buttervolume clone <volume> <new_volume>
 
 ``<volume>`` is the name of the volume to be cloned, not the full path. It is expected
 to live in ``/var/lib/buttervolume/volumes``.
 ``<new_volume>`` is the name of the new volume to be created as clone of previous one,
 not the full path. It is expected to be created in ``/var/lib/buttervolume/volumes``.
@@ -391,16 +410,16 @@
 enabling the plugin.
 
 Synchronize a volume from another host volume
 ---------------------------------------------
 
 You can receive data from a remote volume, so in case there is a volume on
 the remote host with the **same name**, it will get new and most recent data
-from the distantant volume and replace in the local volume. Before running the
-``rsync`` command a snapshot is made on the locale machine to manage recovery::
+from the distant volume and replace in the local volume. Before running the
+``rsync`` command a snapshot is made on the local machine to manage recovery::
 
     buttervolume sync <volume> <host1> [<host2>][...]
 
 The intent is to synchronize a volume between multi hosts on running
 containers, so you should schedule that action on each nodes from all remote
 hosts.
 
@@ -516,39 +535,33 @@
 It will display the schedule in the same format used for adding the schedule,
 which is convenient to remove an existing schedule or add a similar one.
 
 
 Copy-on-write
 -------------
 
-Copy-On-Write is enabled by default. You can disable it if you want.
+Copy-On-Write is enabled by default. You can disable it if you really want.
 
 Why disabling copy-on-write? If your docker volume stores databases such as
 PostgreSQL or MariaDB, the copy-on-write feature may hurt performance, though
-the latest kernels have improve a lot. The good news is that disabling
+the latest kernels have improved a lot. The good news is that disabling
 copy-on-write does not prevent from doing snaphots.
 
 
-Test
-****
+Testing
+*******
 
 If your volumes directory is a BTRFS partition or volume, tests can be run
 with::
 
-    sudo SSH_PORT=22 python3 setup.py test
+    ./test.sh
 
-22 being the port of your running ssh server with authorized key,
-or using and testing the docker image (with python >= 3.5)::
 
-    docker build -t anybox/buttervolume docker/
-    sudo docker run -it --rm --privileged \
-      -v /var/lib/docker:/var/lib/docker \
-      -v "$PWD":/usr/src/buttervolume \
-      -w /usr/src/buttervolume \
-      anybox/buttervolume test
+Working without a BTRFS partition
+*********************************
 
 If you have no BTRFS partitions or volumes you can setup a virtual partition
 in a file as follows (tested on Debian 8):
 
 Setup BTRFS virtual partition::
 
     sudo qemu-img create /var/lib/docker/btrfs.img 10G
@@ -673,14 +686,21 @@
 - Christoph Rist
 - Philip Nagler-Frank
 - Yoann MOUGNIBAS
 
 CHANGELOG
 =========
 
+3.9 (2022-10-11)
+****************
+
+- Fixed a crash when option_copyonwrite is not set
+- Restored the test suite
+- Improved and simplified the build script and test script
+
 3.8 (2022-10-07)
 ****************
 
 - Switched to copy-on-write by default
 - Allow to choose to enable/disable copy-on-write for each volume
 - Allow to change the default SSH_PORT in the plugin config
 - Updated the base docker image and dependencies
```

### Comparing `buttervolume-3.8/README.rst` & `buttervolume-3.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,40 @@
    :target: https://travis-ci.org/anybox/buttervolume
    :alt: Travis state
 
 
 BTRFS Volume plugin for Docker
 ==============================
 
-This package provides a Docker volume plugin that creates a BTRFS subvolume for
-each container volume.
+**What will Buttervolume allow you to do?**
+
+- Quickly recover recent data after an exploit or failure of your web sites or applications
+- Quickly rollback your data to a previous version after a failed upgrade
+- Implement automatic upgrade of your applications without fear
+- Keep an history of your data
+- Make many backups without consuming more disk space than needed
+- Build a resilient hosting cluster with data replication
+- Quickly move your applications between nodes
+- Create preconfigured or templated applications to deploy in seconds
+
+**What can Buttervolume do?**
+
+- Snapshot your Docker volumes
+- Restore a snapshot to its original volume or under a new volume
+- List and remove existing snapshots of your volumes
+- Clone your Docker volumes
+- Replicate or Sync your volumes to another host
+- Schedule periodic snapshots, sync or replication of your volumes
+- Schedule periodic removal of your old snapshots
+
+**How does it work?**
+
+Buttervolume is a Docker Volume Plugin that sits on top of a BTRFS partition
+and can manage and replicate BTRFS snapshots of your Docker volumes.
 
-Please note this is **not** a BTRFS storage driver for Docker, but a plugin to
-manage volumes. It means you can use any storage driver, such as AUFS, this is
-an independant topic.
 
 .. contents::
 
 
 Introduction
 ************
 
@@ -55,31 +75,30 @@
 ******************************
 
 If you want to be a contributor, read this chapter. Otherwise jump to the next section.
 
 You first need to create a root filesystem for the plugin, using the provided Dockerfile::
 
     git clone https://github.com/anybox/buttervolume
-    cd buttervolume/docker
-    ./rebuild_rootfs.sh
+    ./build.sh
 
-Then you can create the plugin::
+By default the plugin is built for the latest commit (HEAD). You can build another version by specifying it like this::
 
-    docker plugin create anybox/buttervolume .
+    ./build.sh 3.7
 
 At this point, you can set the SSH_PORT option for the plugin by running::
 
     docker plugin set anybox/buttervolume SSH_PORT=1122
 
 Note that this option is only relevant if you use the replication feature between two nodes.
 
 Now you can enable the plugin, which should start buttervolume in the plugin
 container::
 
-    docker plugin enable anybox/buttervolume
+    docker plugin enable anybox/buttervolume:HEAD
 
 You can check it is responding by running a buttervolume command::
 
     export RUNCROOT=/run/docker/runtime-runc/plugins.moby/ # or /run/docker/plugins/runtime-root/plugins.moby/
     alias drunc="sudo runc --root $RUNCROOT"
     alias buttervolume="drunc exec -t $(drunc list|tail -n+2|awk '{print $1}') buttervolume"
     sudo buttervolume scheduled
@@ -205,15 +224,15 @@
 
     docker volume create -d anybox/buttervolume:latest myvolume
 
 or::
 
     docker volume create --volume-driver=anybox/buttervolume:latest
 
-When creating a volume, you can choose to disable copy-on-write on a per -olume
+When creating a volume, you can choose to disable copy-on-write on a per-volume
 basis. Just use the `-o` or `--opt` option as defined in the `Docker documentation
 <https://docs.docker.com/engine/reference/commandline/volume_create/#options>`_ ::
 
     docker volume create -d anybox/buttervolume -o copyonwrite=false myvolume
 
 Running the plugin locally or in legacy mode
 --------------------------------------------
@@ -319,15 +338,15 @@
 
 
 Clone a volume
 ------------------
 
 You can clone a volume as a new volume. The current volume will be cloned
 as a new volume name given as parameter. Please take care of stopping the
-container before clonning a volume::
+container before cloning a volume::
 
     buttervolume clone <volume> <new_volume>
 
 ``<volume>`` is the name of the volume to be cloned, not the full path. It is expected
 to live in ``/var/lib/buttervolume/volumes``.
 ``<new_volume>`` is the name of the new volume to be created as clone of previous one,
 not the full path. It is expected to be created in ``/var/lib/buttervolume/volumes``.
@@ -375,16 +394,16 @@
 enabling the plugin.
 
 Synchronize a volume from another host volume
 ---------------------------------------------
 
 You can receive data from a remote volume, so in case there is a volume on
 the remote host with the **same name**, it will get new and most recent data
-from the distantant volume and replace in the local volume. Before running the
-``rsync`` command a snapshot is made on the locale machine to manage recovery::
+from the distant volume and replace in the local volume. Before running the
+``rsync`` command a snapshot is made on the local machine to manage recovery::
 
     buttervolume sync <volume> <host1> [<host2>][...]
 
 The intent is to synchronize a volume between multi hosts on running
 containers, so you should schedule that action on each nodes from all remote
 hosts.
 
@@ -500,39 +519,33 @@
 It will display the schedule in the same format used for adding the schedule,
 which is convenient to remove an existing schedule or add a similar one.
 
 
 Copy-on-write
 -------------
 
-Copy-On-Write is enabled by default. You can disable it if you want.
+Copy-On-Write is enabled by default. You can disable it if you really want.
 
 Why disabling copy-on-write? If your docker volume stores databases such as
 PostgreSQL or MariaDB, the copy-on-write feature may hurt performance, though
-the latest kernels have improve a lot. The good news is that disabling
+the latest kernels have improved a lot. The good news is that disabling
 copy-on-write does not prevent from doing snaphots.
 
 
-Test
-****
+Testing
+*******
 
 If your volumes directory is a BTRFS partition or volume, tests can be run
 with::
 
-    sudo SSH_PORT=22 python3 setup.py test
+    ./test.sh
 
-22 being the port of your running ssh server with authorized key,
-or using and testing the docker image (with python >= 3.5)::
 
-    docker build -t anybox/buttervolume docker/
-    sudo docker run -it --rm --privileged \
-      -v /var/lib/docker:/var/lib/docker \
-      -v "$PWD":/usr/src/buttervolume \
-      -w /usr/src/buttervolume \
-      anybox/buttervolume test
+Working without a BTRFS partition
+*********************************
 
 If you have no BTRFS partitions or volumes you can setup a virtual partition
 in a file as follows (tested on Debian 8):
 
 Setup BTRFS virtual partition::
 
     sudo qemu-img create /var/lib/docker/btrfs.img 10G
```

### Comparing `buttervolume-3.8/buttervolume/btrfs.py` & `buttervolume-3.9/buttervolume/btrfs.py`

 * *Files identical despite different names*

### Comparing `buttervolume-3.8/buttervolume/cli.py` & `buttervolume-3.9/buttervolume/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     WARNING: this should be guaranteed against runtime errors
     otherwise the next scheduler won't run
     """
     global CURRENTTIMER
     log.info("New scheduler job at %s", datetime.now())
     # open the config and launch the tasks
     if not os.path.exists(config):
-        log.warn("No config file %s", config)
+        log.warning("No config file %s", config)
         if not test:
             CURRENTTIMER = Timer(TIMER, scheduler)
             CURRENTTIMER.start()
         return
     name = action = timer = ""
     # run each action in the schedule if time is elapsed since the last one
     with open(config) as f:
@@ -239,15 +239,15 @@
                 # just starting, we consider beeing late on snapshots
                 SCHEDULE_LOG.setdefault(action, {})
                 SCHEDULE_LOG[action].setdefault(name, now - timedelta(1))
                 last = SCHEDULE_LOG[action][name]
                 if now < last + timedelta(minutes=int(timer)):
                     continue
                 if action not in SCHEDULE_LOG.keys():
-                    log.warn("Skipping invalid action %s", action)
+                    log.warning("Skipping invalid action %s", action)
                     continue
                 # choose and run the right action
                 if action == "snapshot":
                     log.info("Starting scheduled snapshot of %s", name)
                     snap = snapshot(Arg(name=[name]), test=test)
                     if not snap:
                         log.info("Could not snapshot %s", name)
@@ -325,24 +325,27 @@
     if not os.path.exists(SNAPSHOTS_PATH):
         log.info("Creating %s", SNAPSHOTS_PATH)
         os.makedirs(SNAPSHOTS_PATH, exist_ok=True)
     # run a thread for the scheduled snapshots
     print("Starting scheduler job every {}s".format(TIMER))
     CURRENTTIMER = Timer(1, scheduler)
     CURRENTTIMER.start()
+    signal.signal(signal.SIGINT, shutdown)
     signal.signal(signal.SIGTERM, shutdown)
+    signal.signal(signal.SIGHUP, shutdown)
+    signal.signal(signal.SIGQUIT, shutdown)
     # listen to requests
-    print("Listening to requests...")
+    print("Listening to requests on %s..." % SOCKET)
     serve(app, unix_socket=SOCKET, unix_socket_perms="660")
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="buttervolume",
-        description="Command-line client for the docker btrfs volume plugin",
+        description="Command-line client for the BTRFS Docker Volume Plugin",
     )
     parser.add_argument("--version", action="version", version=f"%(prog)s {VERSION}")
     subparsers = parser.add_subparsers(help="sub-commands")
     parser_run = subparsers.add_parser("run", help="Run the plugin in foreground")
 
     parser_snapshot = subparsers.add_parser("snapshot", help="Snapshot a volume")
     parser_snapshot.add_argument(
```

### Comparing `buttervolume-3.8/buttervolume/plugin.py` & `buttervolume-3.9/buttervolume/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,37 +72,31 @@
     return {"Implements": ["VolumeDriver"]}
 
 
 @route("/VolumeDriver.Create", ["POST"])
 @add_debug_log
 def volume_create(req):
     name = req["Name"]
-    opts = req["Opts"]
+    opts = req.get("Opts", {})
 
     if "@" in name:
         return {"Err": '"@" is illegal in a volume name'}
     volpath = join(VOLUMES_PATH, name)
     # volume already exists?
     if name in [v["Name"] for v in list_volumes()["Volumes"]]:
         return {"Err": ""}
 
-    try:
-        option_copyonwrite = opts["copyonwrite"].lower()
-        if option_copyonwrite not in ["true", "false"]:
-            return {
-                "Err": f'Invalid option for copyonwrite: {option_copyonwrite}. Set to "true" or "false".'
-            }
-        option_copyonwrite = option_copyonwrite == "true"
-
-    except KeyError:
-        # use copy-on-write by default
-        option_copyonwrite = True
+    cow = opts.get("copyonwrite", "true").lower()
+    if cow not in ["true", "false"]:
+        return {
+            "Err": f'Invalid option for copyonwrite: {cow}. Set to "true" or "false".'
+        }
 
     try:
-        btrfs.Subvolume(volpath).create(cow=option_copyonwrite)
+        btrfs.Subvolume(volpath).create(cow=cow == "true")
     except CalledProcessError as e:
         return {"Err": e.stderr.decode()}
     except OSError as e:
         return {"Err": e.strerror}
     except Exception as e:
         return {"Err": str(e)}
     return {"Err": ""}
@@ -201,15 +195,14 @@
                     "rsync",
                     "-v",
                     "-r",
                     "-a",
                     "-z",
                     "-h",
                     "-P",
-                    "--update",
                     "-e",
                     "ssh -p {}".format(port),
                     "{}:{}/".format(remote_host, remote_volume_path),
                     local_volume_path,
                 ]
                 log.debug("Running %r", cmd)
                 run(cmd, check=True, stdout=PIPE, stderr=PIPE)
@@ -263,15 +256,15 @@
         'btrfs send {parent} "{snapshot_path}"'
         ' | ssh -p {port} {remote_host} "btrfs receive {remote_snapshots}"'
     )
     try:
         log.info(cmd.format(**locals()))
         run(cmd.format(**locals()), shell=True, check=True, stdout=PIPE, stderr=PIPE)
     except CalledProcessError as e:
-        log.warn(
+        log.warning(
             "Failed using parent %s. Sending full snapshot %s "
             "(stdout: %s, stderr: %s)",
             latest,
             snapshot_path,
             e.stdout,
             e.stderr,
         )
@@ -344,17 +337,15 @@
         return {"Err": str(e)}
     return {"Err": ""}
 
 
 @route("/VolumeDriver.Schedule", ["POST"])
 @add_debug_log
 def schedule(req):
-    """Schedule or unschedule a job
-    TODO add a lock
-    """
+    """Schedule or unschedule a job"""
     name = req["Name"]
     timer = req["Timer"]
     action = req["Action"]
     schedule = []
     if timer:  # 0 means unschedule!
         schedule.append((name, action, timer))
     if os.path.exists(SCHEDULE):
```

### Comparing `buttervolume-3.8/buttervolume.egg-info/PKG-INFO` & `buttervolume-3.9/buttervolume.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buttervolume
-Version: 3.8
+Version: 3.9
 Summary: Docker plugin to manage Docker Volumes as BTRFS subvolumes
 Home-page: https://github.com/anybox/buttervolume
 Author: Christophe Combelles
 Author-email: ccomb@anybox.fr
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,20 +18,40 @@
    :target: https://travis-ci.org/anybox/buttervolume
    :alt: Travis state
 
 
 BTRFS Volume plugin for Docker
 ==============================
 
-This package provides a Docker volume plugin that creates a BTRFS subvolume for
-each container volume.
+**What will Buttervolume allow you to do?**
+
+- Quickly recover recent data after an exploit or failure of your web sites or applications
+- Quickly rollback your data to a previous version after a failed upgrade
+- Implement automatic upgrade of your applications without fear
+- Keep an history of your data
+- Make many backups without consuming more disk space than needed
+- Build a resilient hosting cluster with data replication
+- Quickly move your applications between nodes
+- Create preconfigured or templated applications to deploy in seconds
+
+**What can Buttervolume do?**
+
+- Snapshot your Docker volumes
+- Restore a snapshot to its original volume or under a new volume
+- List and remove existing snapshots of your volumes
+- Clone your Docker volumes
+- Replicate or Sync your volumes to another host
+- Schedule periodic snapshots, sync or replication of your volumes
+- Schedule periodic removal of your old snapshots
+
+**How does it work?**
+
+Buttervolume is a Docker Volume Plugin that sits on top of a BTRFS partition
+and can manage and replicate BTRFS snapshots of your Docker volumes.
 
-Please note this is **not** a BTRFS storage driver for Docker, but a plugin to
-manage volumes. It means you can use any storage driver, such as AUFS, this is
-an independant topic.
 
 .. contents::
 
 
 Introduction
 ************
 
@@ -71,31 +91,30 @@
 ******************************
 
 If you want to be a contributor, read this chapter. Otherwise jump to the next section.
 
 You first need to create a root filesystem for the plugin, using the provided Dockerfile::
 
     git clone https://github.com/anybox/buttervolume
-    cd buttervolume/docker
-    ./rebuild_rootfs.sh
+    ./build.sh
 
-Then you can create the plugin::
+By default the plugin is built for the latest commit (HEAD). You can build another version by specifying it like this::
 
-    docker plugin create anybox/buttervolume .
+    ./build.sh 3.7
 
 At this point, you can set the SSH_PORT option for the plugin by running::
 
     docker plugin set anybox/buttervolume SSH_PORT=1122
 
 Note that this option is only relevant if you use the replication feature between two nodes.
 
 Now you can enable the plugin, which should start buttervolume in the plugin
 container::
 
-    docker plugin enable anybox/buttervolume
+    docker plugin enable anybox/buttervolume:HEAD
 
 You can check it is responding by running a buttervolume command::
 
     export RUNCROOT=/run/docker/runtime-runc/plugins.moby/ # or /run/docker/plugins/runtime-root/plugins.moby/
     alias drunc="sudo runc --root $RUNCROOT"
     alias buttervolume="drunc exec -t $(drunc list|tail -n+2|awk '{print $1}') buttervolume"
     sudo buttervolume scheduled
@@ -221,15 +240,15 @@
 
     docker volume create -d anybox/buttervolume:latest myvolume
 
 or::
 
     docker volume create --volume-driver=anybox/buttervolume:latest
 
-When creating a volume, you can choose to disable copy-on-write on a per -olume
+When creating a volume, you can choose to disable copy-on-write on a per-volume
 basis. Just use the `-o` or `--opt` option as defined in the `Docker documentation
 <https://docs.docker.com/engine/reference/commandline/volume_create/#options>`_ ::
 
     docker volume create -d anybox/buttervolume -o copyonwrite=false myvolume
 
 Running the plugin locally or in legacy mode
 --------------------------------------------
@@ -335,15 +354,15 @@
 
 
 Clone a volume
 ------------------
 
 You can clone a volume as a new volume. The current volume will be cloned
 as a new volume name given as parameter. Please take care of stopping the
-container before clonning a volume::
+container before cloning a volume::
 
     buttervolume clone <volume> <new_volume>
 
 ``<volume>`` is the name of the volume to be cloned, not the full path. It is expected
 to live in ``/var/lib/buttervolume/volumes``.
 ``<new_volume>`` is the name of the new volume to be created as clone of previous one,
 not the full path. It is expected to be created in ``/var/lib/buttervolume/volumes``.
@@ -391,16 +410,16 @@
 enabling the plugin.
 
 Synchronize a volume from another host volume
 ---------------------------------------------
 
 You can receive data from a remote volume, so in case there is a volume on
 the remote host with the **same name**, it will get new and most recent data
-from the distantant volume and replace in the local volume. Before running the
-``rsync`` command a snapshot is made on the locale machine to manage recovery::
+from the distant volume and replace in the local volume. Before running the
+``rsync`` command a snapshot is made on the local machine to manage recovery::
 
     buttervolume sync <volume> <host1> [<host2>][...]
 
 The intent is to synchronize a volume between multi hosts on running
 containers, so you should schedule that action on each nodes from all remote
 hosts.
 
@@ -516,39 +535,33 @@
 It will display the schedule in the same format used for adding the schedule,
 which is convenient to remove an existing schedule or add a similar one.
 
 
 Copy-on-write
 -------------
 
-Copy-On-Write is enabled by default. You can disable it if you want.
+Copy-On-Write is enabled by default. You can disable it if you really want.
 
 Why disabling copy-on-write? If your docker volume stores databases such as
 PostgreSQL or MariaDB, the copy-on-write feature may hurt performance, though
-the latest kernels have improve a lot. The good news is that disabling
+the latest kernels have improved a lot. The good news is that disabling
 copy-on-write does not prevent from doing snaphots.
 
 
-Test
-****
+Testing
+*******
 
 If your volumes directory is a BTRFS partition or volume, tests can be run
 with::
 
-    sudo SSH_PORT=22 python3 setup.py test
+    ./test.sh
 
-22 being the port of your running ssh server with authorized key,
-or using and testing the docker image (with python >= 3.5)::
 
-    docker build -t anybox/buttervolume docker/
-    sudo docker run -it --rm --privileged \
-      -v /var/lib/docker:/var/lib/docker \
-      -v "$PWD":/usr/src/buttervolume \
-      -w /usr/src/buttervolume \
-      anybox/buttervolume test
+Working without a BTRFS partition
+*********************************
 
 If you have no BTRFS partitions or volumes you can setup a virtual partition
 in a file as follows (tested on Debian 8):
 
 Setup BTRFS virtual partition::
 
     sudo qemu-img create /var/lib/docker/btrfs.img 10G
@@ -673,14 +686,21 @@
 - Christoph Rist
 - Philip Nagler-Frank
 - Yoann MOUGNIBAS
 
 CHANGELOG
 =========
 
+3.9 (2022-10-11)
+****************
+
+- Fixed a crash when option_copyonwrite is not set
+- Restored the test suite
+- Improved and simplified the build script and test script
+
 3.8 (2022-10-07)
 ****************
 
 - Switched to copy-on-write by default
 - Allow to choose to enable/disable copy-on-write for each volume
 - Allow to change the default SSH_PORT in the plugin config
 - Updated the base docker image and dependencies
```

### Comparing `buttervolume-3.8/setup.py` & `buttervolume-3.9/setup.py`

 * *Files identical despite different names*

