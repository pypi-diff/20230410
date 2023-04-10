# Comparing `tmp/buildapp-1.0.1.tar.gz` & `tmp/buildapp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildapp-1.0.1.tar", last modified: Mon Apr 10 19:35:47 2023, max compression
+gzip compressed data, was "buildapp-1.1.0.tar", last modified: Mon Apr 10 21:08:37 2023, max compression
```

## Comparing `buildapp-1.0.1.tar` & `buildapp-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 19:35:47.233462 buildapp-1.0.1/
--rw-rw-rw-   0        0        0      153 2023-04-10 19:35:47.233462 buildapp-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-04-10 19:10:02.000000 buildapp-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 19:35:47.217833 buildapp-1.0.1/buildapp/
--rw-rw-rw-   0        0        0        0 2023-04-10 19:31:18.000000 buildapp-1.0.1/buildapp/__init__.py
--rw-rw-rw-   0        0        0     3260 2023-04-10 19:16:39.000000 buildapp-1.0.1/buildapp/buildapp.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:35:47.233462 buildapp-1.0.1/buildapp.egg-info/
--rw-rw-rw-   0        0        0      153 2023-04-10 19:35:47.000000 buildapp-1.0.1/buildapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-10 19:35:47.000000 buildapp-1.0.1/buildapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 19:35:47.000000 buildapp-1.0.1/buildapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-10 19:35:47.000000 buildapp-1.0.1/buildapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 19:35:47.000000 buildapp-1.0.1/buildapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 19:35:47.233462 buildapp-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      349 2023-04-10 19:29:00.000000 buildapp-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:08:37.641981 buildapp-1.1.0/
+-rw-rw-rw-   0        0        0      153 2023-04-10 21:08:37.640973 buildapp-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2503 2023-04-10 19:54:01.000000 buildapp-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 21:08:37.622974 buildapp-1.1.0/buildapp/
+-rw-rw-rw-   0        0        0       33 2023-04-10 21:02:21.000000 buildapp-1.1.0/buildapp/__init__.py
+-rw-rw-rw-   0        0        0     3419 2023-04-10 21:01:25.000000 buildapp-1.1.0/buildapp/buildapp.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:08:37.639022 buildapp-1.1.0/buildapp.egg-info/
+-rw-rw-rw-   0        0        0      153 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 21:08:37.641981 buildapp-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      349 2023-04-10 21:04:15.000000 buildapp-1.1.0/setup.py
```

### Comparing `buildapp-1.0.1/README.md` & `buildapp-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # buildapp
 Corss-Platform script used to recompile APK that was decompiled by apktool <br/>
 That way, you can decompile an application, patch it's smali-source / resources / manifest / libs / ... <br />
 And rebuild it into a new apk you may install in your devices <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only!
 
+## Installation
+Simply
+> pip install buildapp
+
+Make sure to have python scripts folder in your path,
+And use the correct version of pip for python3
+
 ## Decompilation process
 Use [`apktool`](https://ibotpeaches.github.io/Apktool/install/) to decompile your application.
 
 Apktool decompilation syntax:
 > apktool d <apk_path> -o <output_folder>
 
 ## Patching process
```

### Comparing `buildapp-1.0.1/buildapp/buildapp.py` & `buildapp-1.1.0/buildapp/buildapp.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,26 +2,14 @@
 import argparse
 import subprocess
 
 KEYSTORE_ALIAS = 'defkeystorealias'
 KEYSTORE_PASSWORD = 'defkeystorepass'
 KEYSTORE_PATH = os.path.expanduser('~/buildapp-keystore.jks')
 
-def run_process(cmdline, input_string='', ignore_stderr=False):
-    print(f'Executing `{cmdline}`')
-
-    subprocess.run(
-        cmdline,
-        shell=True,
-        check=True,
-        stdout=subprocess.DEVNULL,
-        input=input_string.encode(),
-        stderr=subprocess.DEVNULL if ignore_stderr else subprocess.PIPE
-    )
-
 
 class CompileApp:
     def __init__(self, decompiled_path, output_apk_path):
         self.prealigned_file = f'{output_apk_path}_prealign'
         self.decompiled_path = decompiled_path
 
     def __enter__(self):
@@ -59,34 +47,51 @@
     def __del__(self):
         os.unlink(f'{self.output_apk_path}.idsig')
 
 class InstallApk:
     def __init__(self, apk_path):
         run_process(f'adb install {apk_path}')
 
+
+def run_process(cmdline, input_string='', ignore_stderr=False):
+    print(f'Executing `{cmdline}`')
+
+    subprocess.run(
+        cmdline,
+        shell=True,
+        check=True,
+        stdout=subprocess.DEVNULL,
+        input=input_string.encode(),
+        stderr=subprocess.DEVNULL if ignore_stderr else subprocess.PIPE
+    )
+
+
 def parse_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument('-o', '--output-apk-path', required=True, help='path of output apk file')
     parser.add_argument('-d', '--decompiled-path', required=True, help='decompiled apk directory')
-    parser.add_argument('-i', '--install', action=argparse.BooleanOptionalAction, help='install on the adb device')
+    parser.add_argument('-i', '--install', action='store_true', help='install on the adb device')
     parser.add_argument('-k', '--keystore-path', required=False, help='optional keystore final to sign the apk with')
 
     return parser.parse_args()
 
 
-def main():
-    args = parse_arguments()
-
-    with CompileApp(args.decompiled_path, args.output_apk_path):
-        AlignApk(args.output_apk_path)
-        ObtainKeystore(args.keystore_path)
-        SignApk(args.output_apk_path)
+def build_app(output_apk_path, decompiled_folder, keystore_path=None, install_after_build=False):
+    with CompileApp(decompiled_folder, output_apk_path):
+        AlignApk(output_apk_path)
+        ObtainKeystore(keystore_path)
+        SignApk(output_apk_path)
 
         print('Compiled successfully!')
 
-        if args.install:
-            InstallApk(args.output_apk_path)
+        if install_after_build:
+            InstallApk(output_apk_path)
             print('Installed successfully!')
 
 
+def main():
+    args = parse_arguments()
+    build_app(args.output_apk_path, args.decompiled_path, args.keystore_path, args.install)
+
+
 if __name__ == "__main__":
     main()
```

