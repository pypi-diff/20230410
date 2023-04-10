# Comparing `tmp/B0tHe1Per_test_api-0.1.tar.gz` & `tmp/B0tHe1Per_test_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "B0tHe1Per_test_api-0.1.tar", last modified: Fri Mar 24 21:17:19 2023, max compression
+gzip compressed data, was "B0tHe1Per_test_api-0.2.tar", last modified: Mon Apr 10 11:42:58 2023, max compression
```

## Comparing `B0tHe1Per_test_api-0.1.tar` & `B0tHe1Per_test_api-0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 21:17:19.817667 B0tHe1Per_test_api-0.1/
-drwxrwxrwx   0        0        0        0 2023-03-24 21:17:19.715801 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/
--rw-rw-rw-   0        0        0      396 2023-03-24 20:35:35.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/__init__.py
--rw-rw-rw-   0        0        0     5001 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/address_book.py
--rw-rw-rw-   0        0        0     6014 2023-03-24 20:45:52.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/bot_interface.py
--rw-rw-rw-   0        0        0     3726 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/file_sorter.py
--rw-rw-rw-   0        0        0     2390 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/notes_classes.py
--rw-rw-rw-   0        0        0     2777 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/notes_main.py
-drwxrwxrwx   0        0        0        0 2023-03-24 21:17:19.816668 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api.egg-info/
--rw-rw-rw-   0        0        0      208 2023-03-24 21:17:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-03-24 21:17:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 21:17:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-03-24 21:17:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       69 2023-03-24 21:17:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-24 21:17:19.000000 B0tHe1Per_test_api-0.1/B0tHe1Per_test_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      208 2023-03-24 21:17:19.818649 B0tHe1Per_test_api-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-03-24 21:17:19.822489 B0tHe1Per_test_api-0.1/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-03-24 21:16:44.000000 B0tHe1Per_test_api-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:42:58.247443 B0tHe1Per_test_api-0.2/
+drwxrwxrwx   0        0        0        0 2023-04-10 11:42:58.191509 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/
+-rw-rw-rw-   0        0        0      396 2023-03-24 20:35:35.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/__init__.py
+-rw-rw-rw-   0        0        0     5001 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/address_book.py
+-rw-rw-rw-   0        0        0     6057 2023-03-24 21:42:15.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/bot_interface.py
+-rw-rw-rw-   0        0        0     3726 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/file_sorter.py
+-rw-rw-rw-   0        0        0     2390 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_classes.py
+-rw-rw-rw-   0        0        0     2777 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_main.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:42:58.244402 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/
+-rw-rw-rw-   0        0        0      208 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:42:57.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      208 2023-04-10 11:42:58.248391 B0tHe1Per_test_api-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-04-10 11:42:58.252375 B0tHe1Per_test_api-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      468 2023-04-10 11:39:30.000000 B0tHe1Per_test_api-0.2/setup.py
```

### Comparing `B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/address_book.py` & `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/address_book.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/bot_interface.py` & `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/bot_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,11 +123,13 @@
     
     def exit(self):
         self.close_current_process()
         self.root.destroy()
         
     def run(self):
         self.root.mainloop()
-      
+        
+    def main(self):
+        self.run()
 if __name__ == "__main__":
     bot = BotInterface()
     bot.run()
```

### Comparing `B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/file_sorter.py` & `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/file_sorter.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/notes_classes.py` & `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_classes.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.1/B0tHe1Per_test_api/notes_main.py` & `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_main.py`

 * *Files identical despite different names*

