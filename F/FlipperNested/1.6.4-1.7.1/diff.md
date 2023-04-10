# Comparing `tmp/FlipperNested-1.6.4.tar.gz` & `tmp/FlipperNested-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.6.4.tar", last modified: Wed Apr  5 15:50:02 2023, max compression
+gzip compressed data, was "FlipperNested-1.7.1.tar", last modified: Mon Apr 10 20:26:40 2023, max compression
```

## Comparing `FlipperNested-1.6.4.tar` & `FlipperNested-1.7.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:50:02.217605 FlipperNested-1.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:50:02.209605 FlipperNested-1.6.4/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:50:02.217605 FlipperNested-1.6.4/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:50:02.217605 FlipperNested-1.6.4/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-05 15:50:02.000000 FlipperNested-1.6.4/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-05 15:50:02.000000 FlipperNested-1.6.4/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:50:02.000000 FlipperNested-1.6.4/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-05 15:50:02.000000 FlipperNested-1.6.4/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-05 15:50:02.000000 FlipperNested-1.6.4/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-05 15:50:02.000000 FlipperNested-1.6.4/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:50:02.217605 FlipperNested-1.6.4/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/common.h
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-05 15:50:02.217605 FlipperNested-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:50:02.217605 FlipperNested-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:50:02.217605 FlipperNested-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-05 15:49:52.000000 FlipperNested-1.6.4/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/tests/test_parse.py
```

### Comparing `FlipperNested-1.6.4/FlipperNested/bridge.py` & `FlipperNested-1.7.1/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/FlipperNested/cli.py` & `FlipperNested-1.7.1/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/FlipperNested/main.py` & `FlipperNested-1.7.1/FlipperNested/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             lines.pop()
         for line in lines:
             values = self.parse_line(line)
             sec, key_type = values[-2:]
             if not sec in self.nonces[key_type].keys():
                 self.nonces[key_type][sec] = []
             self.nonces[key_type][sec].append(values)
-        return len(self.nonces['A']) + len(self.nonces['B']) > 0
+        return len(self.nonces["A"]) + len(self.nonces["B"]) > 0
 
     def extract_nonces_from_flipper(self, args=None):
         for file in self.connection.get_files("/ext/nfc/nested"):
             if file["name"].endswith(".nonces"):
                 if args and args.uid:
                     if file["name"].split(".")[0] != args.uid.upper():
                         continue
@@ -134,14 +134,18 @@
     def save_keys_to_string(self):
         output = ""
         for key_type in self.found_keys.keys():
             for sector in self.found_keys[key_type].keys():
                 for key in self.found_keys[key_type][sector]:
                     output += f"Key {key_type} sector {str(sector).zfill(2)}: " + " ".join(
                         [key.upper()[i:i + 2] for i in range(0, len(key), 2)]) + "\n"
+
+        keys = output.count('Key')
+        if keys:
+            print("Found potential {} keys, use \"Check found keys\" in app".format(keys))
         return output.strip()
 
     def save_keys_to_file(self):
         output = self.save_keys_to_string()
         if not output:
             print("No keys found!")
             return
@@ -150,23 +154,23 @@
         print("Saved keys to", filename)
 
     def save_keys_to_flipper(self, save=False):
         output = self.save_keys_to_string()
         if not output:
             print("No keys found!")
             return
-        filename = self.filename.replace('nonces', 'keys')
+        filename = self.filename.replace("nonces", "keys")
         if save:
-            open(filename, 'w+').write(output)
+            open(filename, "w+").write(output)
             print("Saved keys to", filename)
         try:
             self.connection.file_write("/ext/nfc/nested/" + filename, output.encode())
         except:
             if not save:
-                open(filename, 'w+').write(output)
+                open(filename, "w+").write(output)
                 print("Lost connection to Flipper!")
                 print("Saved keys to", filename)
 
     @staticmethod
     def parse_line(line):
         result = re.search(
             r"Nested: Key ([A-B]) cuid (0x[0-9a-f]*) nt0 (0x[0-9a-f]*) ks0 (0x[0-9a-f]*) par0 ([0-9a-f]*) nt1 (0x[0-9a-f]*) ks1 (0x[0-9a-f]*) par1 ([0-9a-f]*) sec (\d{1,2})",
```

### Comparing `FlipperNested-1.6.4/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-1.7.1/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/FlipperNested/proto/storage_pb2.py` & `FlipperNested-1.7.1/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-1.7.1/FlipperNested.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.6.4
+Version: 1.7.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Flipper Nested Recovery script
 
 Script recovers keys from collected authorization attempts (nonces).
@@ -31,21 +32,14 @@
 or, install from sources:
 ```bash
 pip install --upgrade pyserial protobuf wheel setuptools
 python setup.py sdist bdist_wheel
 pip install --user --upgrade --find-links=./dist FlipperNested
 ```
 
-or, install on Windows (install and run https://www.msys2.org/):
-```bash
-pacman -Sy python python-pip base-devel gcc
-pip install --upgrade pyserial protobuf wheel setuptools
-pip install --upgrade FlipperNested
-```
-
 ## Usage
 
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
 Calculating for key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
```

### Comparing `FlipperNested-1.6.4/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-1.7.1/FlipperNested.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 FlipperNested.egg-info/requires.txt
 FlipperNested.egg-info/top_level.txt
 FlipperNested/proto/__init__.py
 FlipperNested/proto/flipper_pb2.py
 FlipperNested/proto/storage_pb2.py
 NestedSolver/bucketsort.c
 NestedSolver/bucketsort.h
-NestedSolver/common.h
 NestedSolver/crapto1.c
 NestedSolver/crapto1.h
 NestedSolver/crypto1.c
 NestedSolver/library.c
 NestedSolver/library.h
 NestedSolver/parity.h
 NestedSolver/python.c
```

### Comparing `FlipperNested-1.6.4/LICENSE.md` & `FlipperNested-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/NestedSolver/bucketsort.c` & `FlipperNested-1.7.1/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/NestedSolver/bucketsort.h` & `FlipperNested-1.7.1/NestedSolver/bucketsort.h`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // See LICENSE.txt for the text of the license.
 //-----------------------------------------------------------------------------
 #ifndef BUCKETSORT_H__
 #define BUCKETSORT_H__
-
-#include "common.h"
+#include <stdio.h>
+#include <stdint.h>
 
 typedef struct bucket {
     uint32_t *head;
     uint32_t *bp;
 } bucket_t;
 
 typedef bucket_t bucket_array_t[2][0x100];
@@ -32,8 +32,8 @@
     uint32_t numbuckets;
 } bucket_info_t;
 
 void bucket_sort_intersect(uint32_t *const estart, uint32_t *const estop,
                            uint32_t *const ostart, uint32_t *const ostop,
                            bucket_info_t *bucket_info, bucket_array_t bucket);
 
-#endif
+#endif
```

### Comparing `FlipperNested-1.6.4/NestedSolver/crapto1.c` & `FlipperNested-1.7.1/NestedSolver/crapto1.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,14 @@
 #include "crapto1.h"
 
 #include "bucketsort.h"
 
 #include <stdlib.h>
 #include "parity.h"
 
-#if !defined LOWMEM && defined __GNUC__
-static uint8_t filterlut[1 << 20];
-static void __attribute__((constructor)) fill_lut(void) {
-    uint32_t i;
-    for (i = 0; i < 1 << 20; ++i)
-        filterlut[i] = filter(i);
-}
-#define filter(x) (filterlut[(x) & 0xfffff])
-#endif
-
 /** update_contribution
  * helper, calculates the partial linear feedback contributions and puts in MSB
  */
 static inline void update_contribution(uint32_t *item, const uint32_t mask1, const uint32_t mask2) {
     uint32_t p = *item >> 25;
 
     p = p << 1 | (evenparity32(*item & mask1));
```

### Comparing `FlipperNested-1.6.4/NestedSolver/crapto1.h` & `FlipperNested-1.7.1/NestedSolver/crapto1.h`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,26 @@
 #include <stdint.h>
 #include <stddef.h>
 #include <stdbool.h>
 
 struct Crypto1State {uint32_t odd, even;};
 void crypto1_init(struct Crypto1State *state, uint64_t key);
 void crypto1_deinit(struct Crypto1State *);
-#if !defined(__arm__) || defined(__linux__) || defined(_WIN32) || defined(__APPLE__) // bare metal ARM Proxmark lacks malloc()/free()
 struct Crypto1State *crypto1_create(uint64_t key);
 void crypto1_destroy(struct Crypto1State *);
-#endif
 void crypto1_get_lfsr(struct Crypto1State *, uint64_t *);
 uint8_t crypto1_bit(struct Crypto1State *, uint8_t, int);
 uint8_t crypto1_byte(struct Crypto1State *, uint8_t, int);
 uint32_t crypto1_word(struct Crypto1State *, uint32_t, int);
 uint32_t prng_successor(uint32_t x, uint32_t n);
 
-#if !defined(__arm__) || defined(__linux__) || defined(_WIN32) || defined(__APPLE__) // bare metal ARM Proxmark lacks malloc()/free()
 struct Crypto1State *lfsr_recovery32(uint32_t ks2, uint32_t in);
 struct Crypto1State *lfsr_recovery64(uint32_t ks2, uint32_t ks3);
 struct Crypto1State *
 lfsr_common_prefix(uint32_t pfx, uint32_t rr, uint8_t ks[8], uint8_t par[8][8], uint32_t no_par);
-#endif
 uint32_t *lfsr_prefix_ks(const uint8_t ks[8], int isodd);
 
 
 uint8_t lfsr_rollback_bit(struct Crypto1State *s, uint32_t in, int fb);
 uint8_t lfsr_rollback_byte(struct Crypto1State *s, uint32_t in, int fb);
 uint32_t lfsr_rollback_word(struct Crypto1State *s, uint32_t in, int fb);
 int nonce_distance(uint32_t from, uint32_t to);
@@ -59,22 +55,18 @@
                 __M = prng_successor(__M, (__i == 7) ? 48 : 8);\
             else
 
 #define LF_POLY_ODD (0x29CE5C)
 #define LF_POLY_EVEN (0x870804)
 #define BIT(x, n) ((x) >> (n) & 1)
 #define BEBIT(x, n) BIT(x, (n) ^ 24)
-#ifdef __OPTIMIZE_SIZE__
-int filter(uint32_t const x);
-#else
 static inline int filter(uint32_t const x) {
     uint32_t f;
 
     f  = 0xf22c0 >> (x       & 0xf) & 16;
     f |= 0x6c9c0 >> (x >>  4 & 0xf) &  8;
     f |= 0x3c8b0 >> (x >>  8 & 0xf) &  4;
     f |= 0x1e458 >> (x >> 12 & 0xf) &  2;
     f |= 0x0d938 >> (x >> 16 & 0xf) &  1;
     return BIT(0xEC57E80A, f);
 }
-#endif
-#endif
+#endif
```

### Comparing `FlipperNested-1.6.4/NestedSolver/crypto1.c` & `FlipperNested-1.7.1/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/NestedSolver/library.c` & `FlipperNested-1.7.1/NestedSolver/library.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+#include <pthread.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
-#include <pthread.h>
 #include <inttypes.h>
 #include "library.h"
 #include "crapto1.h"
 #include "parity.h"
 
 static int compare_uint64(const void *a, const void *b) {
     if (*(uint64_t *) b == *(uint64_t *) a) return 0;
@@ -18,24 +18,24 @@
     if (listA == NULL || listB == NULL)
         return 0;
 
     uint64_t *p1, *p2, *p3;
     p1 = p3 = listA;
     p2 = listB;
 
-    while (*p1 != UINT64_C(-1) && *p2 != UINT64_C(-1)) {
+    while (*p1 != UINT64_MAX && *p2 != UINT64_MAX) {
         if (compare_uint64(p1, p2) == 0) {
             *p3++ = *p1++;
             p2++;
         } else {
             while (compare_uint64(p1, p2) < 0) ++p1;
             while (compare_uint64(p1, p2) > 0) ++p2;
         }
     }
-    *p3 = UINT64_C(-1);
+    *p3 = UINT64_MAX;
     return p3 - listA;
 }
 
 static int compare_16bits(const void *a, const void *b) {
     if ((*(uint64_t *) b & 0x00ff000000ff0000) == (*(uint64_t *) a & 0x00ff000000ff0000)) return 0;
     if ((*(uint64_t *) b & 0x00ff000000ff0000) > (*(uint64_t *) a & 0x00ff000000ff0000)) return 1;
     return -1;
@@ -191,20 +191,24 @@
     nested_calculate(info);
     return info->keys;
 }
 
 char *
 run_full_nested(uint32_t uid, uint32_t nt0, uint32_t ks0, uint32_t par0, uint32_t nt1, uint32_t ks1, uint32_t par1,
                 int from, int to) {
-    pthread_t thread_id[to];
-    uint32_t found_second_array[to];
+    #if _MSC_VER
+        pthread_t thread_id[16384];
+        uint32_t found_second_array[16384];
+    #else
+        pthread_t thread_id[to];
+        uint32_t found_second_array[to];
+    #endif
     uint32_t found_first, found_second;
     bool found = false;
     uint32_t i;
-
     for (int first = from; first < to; first++) {
         i = 0;
         void *status = NULL;
 
         for (int second = from; second < to; second++) {
             uint8_t *par0_decoded = decode_parity(par0);
             uint8_t *par1_decoded = decode_parity(par1);
```

### Comparing `FlipperNested-1.6.4/NestedSolver/library.h` & `FlipperNested-1.7.1/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.6.4/NestedSolver/parity.h` & `FlipperNested-1.7.1/NestedSolver/parity.h`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,22 @@
 // Parity functions
 //-----------------------------------------------------------------------------
 
 // all functions defined in header file by purpose. Allows compiler optimizations.
 
 #ifndef __PARITY_H
 #define __PARITY_H
-
-#include "common.h"
+#define _CRT_NONSTDC_NO_WARNINGS
+#define _CRT_SECURE_NO_WARNINGS
+#define _CRT_NON_CONFORMING_SWPRINTFS
+
+#define restrict __restrict
+#define inline __inline
+#include <stdio.h>
+#include <stdint.h>
 
 static const uint8_t g_odd_byte_parity[256] = {
     1, 0, 0, 1, 0, 1, 1, 0, 0, 1, 1, 0, 1, 0, 0, 1,
     0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0,
     0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0,
     1, 0, 0, 1, 0, 1, 1, 0, 0, 1, 1, 0, 1, 0, 0, 1,
     0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0,
@@ -38,31 +44,29 @@
     0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0,
     1, 0, 0, 1, 0, 1, 1, 0, 0, 1, 1, 0, 1, 0, 0, 1,
     0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0,
     0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0,
     1, 0, 0, 1, 0, 1, 1, 0, 0, 1, 1, 0, 1, 0, 0, 1
 };
 
-//extern const uint8_t OddByteParity[256];
-
-#define ODD_PARITY8(x)   { g_odd_byte_parity[x] }
-#define EVEN_PARITY8(x)  { !g_odd_byte_parity[x] }
+#define ODD_PARITY8(x)   (g_odd_byte_parity[x])
+#define EVEN_PARITY8(x)  (!g_odd_byte_parity[x])
 
 static inline uint8_t oddparity8(const uint8_t x) {
     return g_odd_byte_parity[x];
 }
 
 static inline uint8_t evenparity8(const uint8_t x) {
     return !g_odd_byte_parity[x];
 }
 
 static inline uint8_t evenparity16(uint16_t x) {
 #if !defined __GNUC__
     x ^= x >> 8;
-    return EVEN_PARITY8(x) ;
+    return EVEN_PARITY8(x);
 #else
     return (__builtin_parity(x) & 0xFF);
 #endif
 }
 
 static inline uint8_t oddparity16(uint16_t x) {
 #if !defined __GNUC__
@@ -70,27 +74,39 @@
     return ODD_PARITY8(x);
 #else
     return !__builtin_parity(x);
 #endif
 }
 
 static inline uint8_t evenparity32(uint32_t x) {
-#if !defined __GNUC__
+#if _MSC_VER
+    x ^= x >> 16;
+    x ^= x >> 8;
+    x ^= x >> 4;
+    x &= 0xf;
+    return (0x6996 >> x) & 1;
+#elif !defined __GNUC__
     x ^= x >> 16;
     x ^= x >> 8;
     return EVEN_PARITY8(x);
 #else
     return (__builtin_parity(x) & 0xFF);
 #endif
 }
 
 static inline uint8_t oddparity32(uint32_t x) {
-#if !defined __GNUC__
+#if _MSC_VER
+    x ^= x >> 16;
+    x ^= x >> 8;
+    x ^= x >> 4;
+    x &= 0xf;
+    return ((0x6996 >> x) & 1) ^ 1;
+#elif !defined __GNUC__
     x ^= x >> 16;
     x ^= x >> 8;
     return ODD_PARITY8(x);
 #else
     return !__builtin_parity(x);
 #endif
 }
 
-#endif /* __PARITY_H */
+#endif /* __PARITY_H */
```

### Comparing `FlipperNested-1.6.4/NestedSolver/python.c` & `FlipperNested-1.7.1/NestedSolver/python.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #include "Python.h"
 #include "library.h"
 
 static PyObject *run_nested_python(PyObject *self, PyObject *args) {
     uint64_t uid, nt0, ks0, nt1, ks1;
-    if (!PyArg_ParseTuple(args, "lllll", &uid, &nt0, &ks0, &nt1, &ks1)) {
+    if (!PyArg_ParseTuple(args, "kkkkk", &uid, &nt0, &ks0, &nt1, &ks1)) {
         return NULL;
     }
 
     char *output = run_nested((uint32_t) uid, (uint32_t) nt0, (uint32_t) ks0, (uint32_t) nt1, (uint32_t) ks1);
 
     return Py_BuildValue("s", output);
 }
 
 static PyObject *run_full_nested_python(PyObject *self, PyObject *args) {
     uint64_t uid, nt0, ks0, par0, nt1, ks1, par1;
     int from, to;
-    if (!PyArg_ParseTuple(args, "lllllllii", &uid, &nt0, &ks0, &par0, &nt1, &ks1, &par1, &from, &to)) {
+    if (!PyArg_ParseTuple(args, "kkkkkkkii", &uid, &nt0, &ks0, &par0, &nt1, &ks1, &par1, &from, &to)) {
         return NULL;
     }
 
     char *output = run_full_nested((uint32_t) uid, (uint32_t) nt0, (uint32_t) ks0, (uint32_t) par0, (uint32_t) nt1,
                                    (uint32_t) ks1, (uint32_t) par1, from, to);
 
     return Py_BuildValue("s", output);
```

### Comparing `FlipperNested-1.6.4/PKG-INFO` & `FlipperNested-1.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.6.4
+Version: 1.7.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Flipper Nested Recovery script
 
 Script recovers keys from collected authorization attempts (nonces).
@@ -31,21 +32,14 @@
 or, install from sources:
 ```bash
 pip install --upgrade pyserial protobuf wheel setuptools
 python setup.py sdist bdist_wheel
 pip install --user --upgrade --find-links=./dist FlipperNested
 ```
 
-or, install on Windows (install and run https://www.msys2.org/):
-```bash
-pacman -Sy python python-pip base-devel gcc
-pip install --upgrade pyserial protobuf wheel setuptools
-pip install --upgrade FlipperNested
-```
-
 ## Usage
 
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
 Calculating for key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
```

### Comparing `FlipperNested-1.6.4/README.md` & `FlipperNested-1.7.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -14,21 +14,14 @@
 or, install from sources:
 ```bash
 pip install --upgrade pyserial protobuf wheel setuptools
 python setup.py sdist bdist_wheel
 pip install --user --upgrade --find-links=./dist FlipperNested
 ```
 
-or, install on Windows (install and run https://www.msys2.org/):
-```bash
-pacman -Sy python python-pip base-devel gcc
-pip install --upgrade pyserial protobuf wheel setuptools
-pip install --upgrade FlipperNested
-```
-
 ## Usage
 
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
 Calculating for key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
```

### Comparing `FlipperNested-1.6.4/setup.py` & `FlipperNested-1.7.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from distutils.core import Extension
 import setuptools
+import os
+
+include_dirs = []
+extra_compile_args = []
+libraries = []
+
+if os.name == 'nt':
+    include_dirs = ['build\\pthreads']
+    extra_compile_args = ['-DNEED_FTIME']
+    libraries = ['pthreadVC2']
 
 nested_solver = Extension('nested',
-                          sources=['NestedSolver/python.c', 'NestedSolver/library.c', 'NestedSolver/bucketsort.c',
-                                   'NestedSolver/crypto1.c', 'NestedSolver/crapto1.c'])
+                          sources=['NestedSolver/python.c', 'NestedSolver/crapto1.c', 'NestedSolver/library.c',
+                                   'NestedSolver/bucketsort.c', 'NestedSolver/crypto1.c'], include_dirs=include_dirs,
+                          library_dirs=include_dirs, extra_compile_args=extra_compile_args, libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="1.6.4",
+    version="1.7.1",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
@@ -24,12 +35,13 @@
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: MacOS",
-        "Operating System :: POSIX :: Linux"
+        "Operating System :: POSIX :: Linux",
+        "Operating System :: Microsoft :: Windows"
     ],
     headers=['NestedSolver/library.h', 'NestedSolver/parity.h',
-             'NestedSolver/crapto1.h', 'NestedSolver/bucketsort.h', 'NestedSolver/common.h']
-)
+             'NestedSolver/crapto1.h', 'NestedSolver/bucketsort.h'],
+)
```

