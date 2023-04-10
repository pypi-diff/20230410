# Comparing `tmp/pysmells-1.0.7.tar.gz` & `tmp/pysmells-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmells-1.0.7.tar", last modified: Mon Apr 10 01:20:21 2023, max compression
+gzip compressed data, was "pysmells-1.0.8.tar", last modified: Mon Apr 10 10:47:00 2023, max compression
```

## Comparing `pysmells-1.0.7.tar` & `pysmells-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.423219 pysmells-1.0.7/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.7/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 01:20:21.422515 pysmells-1.0.7/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.7/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.414705 pysmells-1.0.7/pysmells/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.7/pysmells/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3847 2023-04-10 01:13:06.000000 pysmells-1.0.7/pysmells/pysmells.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.420913 pysmells-1.0.7/pysmells.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      279 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       14 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-10 01:20:21.423490 pysmells-1.0.7/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)     1332 2023-04-09 19:55:04.000000 pysmells-1.0.7/setup.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.421735 pysmells-1.0.7/test/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-09 23:44:38.000000 pysmells-1.0.7/test/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.670003 pysmells-1.0.8/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.8/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 10:47:00.668395 pysmells-1.0.8/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.8/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.653426 pysmells-1.0.8/pysmells/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.8/pysmells/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     4162 2023-04-10 10:39:40.000000 pysmells-1.0.8/pysmells/pysmells.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.665753 pysmells-1.0.8/pysmells.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      279 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       14 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-10 10:47:00.670644 pysmells-1.0.8/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1332 2023-04-10 10:45:40.000000 pysmells-1.0.8/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.666605 pysmells-1.0.8/test/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-09 23:44:38.000000 pysmells-1.0.8/test/__init__.py
```

### Comparing `pysmells-1.0.7/LICENSE` & `pysmells-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.7/PKG-INFO` & `pysmells-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.7
+Version: 1.0.8
 Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pysmells-1.0.7/README.md` & `pysmells-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.7/pysmells/pysmells.py` & `pysmells-1.0.8/pysmells/pysmells.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,15 @@
 import argparse
 import subprocess
 import csv
 from collections import Counter, defaultdict
 from tabulate import tabulate
 
 
-def check_type_annotations(file_path):
-    with open(file_path, "r") as file:
-        content = file.read()
-
-    type_annotation_pattern = re.compile(r'(?<=:)\s*([a-zA-Z_][a-zA-Z0-9_]*|\s*List\s*\[[a-zA-Z0-9_, ]+\])\s*')
-    match = type_annotation_pattern.search(content)
-    return bool(match)
-
-
-def analyze_file(directory, file_path, table_data):
+def analyze_file(directory, file_path):
     print(f"Analyzing the file: {file_path}\n")
 
     # Run Pylint
     process = subprocess.run(["pylint", file_path], stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                              universal_newlines=True, check=False)
     pylint_output = process.stdout
 
@@ -41,24 +32,15 @@
         match = alert_pattern.search(line)
         if match:
             alert_code = match.group(0)
             alert_type = alert_code[0]
             alert_count[alert_type] += 1
             alert_details[alert_type].append(alert_code)
 
-    total_alerts = sum(alert_count.values())
-    # Update the table data structure
-    table_row = [file_path, total_alerts]
-    for alert_type in alert_type_names.keys():
-        table_row.append(alert_count[alert_type])
-
-    table_row.append(", ".join(sorted(set(alert_code for alert_codes in alert_details.values() for alert_code in alert_codes))))
-    table_data.append(table_row)
-
-    return total_alerts
+    return alert_count, alert_details
 
 def export_to_csv(table_data, headers, csv_output):
     with open(csv_output, 'w', newline='') as csvfile:
         csv_writer = csv.writer(csvfile)
         csv_writer.writerow(headers)
         for row in table_data:
             csv_writer.writerow(row)
@@ -73,31 +55,53 @@
     project_directory = os.path.abspath(args.project)
     subdirectories = args.subdirs
     csv_output = args.csv_output
 
     print(f"Project directory (absolute path): {project_directory}")
 
     table_data = []
-    total_alerts_directory = 0
 
     for subdir in subdirectories:
         current_directory = os.path.abspath(os.path.join(project_directory, subdir))
         print(f"Analyzing subdirectory (absolute path): {current_directory}")
+
+        subdir_alert_count = Counter()
+        subdir_alert_details = defaultdict(list)
+
         if os.path.isdir(current_directory):
             for root, dirs, files in os.walk(current_directory):
                 for file_name in files:
                     if file_name.endswith(".py"):
                         file_path = os.path.join(root, file_name)
-                        total_alerts_directory += analyze_file(root, file_path, table_data)
+                        file_alert_count, file_alert_details = analyze_file(root, file_path)
+
+                        subdir_alert_count.update(file_alert_count)
+                        for alert_type, alert_codes in file_alert_details.items():
+                            subdir_alert_details[alert_type].extend(alert_codes)
+
+                        file_row = [file_path, sum(file_alert_count.values())]
+                        for alert_type in 'CRWEF':
+                            file_row.append(file_alert_count[alert_type])
+
+                        file_row.append(", ".join(sorted(set(alert_code for alert_codes in file_alert_details.values() for alert_code in alert_codes))))
+                        table_data.append(file_row)
+
+            subdir_row = [current_directory, sum(subdir_alert_count.values())]
+            for alert_type in 'CRWEF':
+                subdir_row.append(subdir_alert_count[alert_type])
+
+            subdir_row.append(", ".join(sorted(set(alert_code for alert_codes in subdir_alert_details.values() for alert_code in alert_codes))))
+            table_data.append(subdir_row)
         else:
             print(f"Subdirectory not found: {current_directory}")
 
-    print(f"\nTotal alerts found in the directories: {total_alerts_directory}\n")
-    headers = ["File", "Total Alerts", "Convention", "Refactor", "Warning", "Error", "Fatal", "Alert Codes"]
+    headers = ["Path", "Total Alerts", "Convention", "Refactor", "Warning", "Error", "Fatal", "Alert Codes"]
     print(tabulate(table_data, headers=headers, tablefmt="grid"))
 
     if csv_output:
         export_to_csv(table_data, headers, csv_output)
         print(f"CSV file exported to: {csv_output}")
 
 if __name__ == "__main__":
     main()
+
+
```

### Comparing `pysmells-1.0.7/pysmells.egg-info/PKG-INFO` & `pysmells-1.0.8/pysmells.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.7
+Version: 1.0.8
 Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pysmells-1.0.7/setup.py` & `pysmells-1.0.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pysmells",
-    version="1.0.7",
+    version="1.0.8",
     author="Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto",
     author_email="msousa@museu-goeldi.br",
     description="Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pysmells/pysmells",
     packages=find_packages(),
```

