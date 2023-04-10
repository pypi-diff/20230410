# Comparing `tmp/pysmells-1.0.6.tar.gz` & `tmp/pysmells-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmells-1.0.6.tar", last modified: Sun Apr  9 11:56:50 2023, max compression
+gzip compressed data, was "pysmells-1.0.7.tar", last modified: Mon Apr 10 01:20:21 2023, max compression
```

## Comparing `pysmells-1.0.6.tar` & `pysmells-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-09 11:56:50.729267 pysmells-1.0.6/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.6/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)     2169 2023-04-09 11:56:50.728026 pysmells-1.0.6/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.6/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-09 11:56:50.719250 pysmells-1.0.6/pysmells/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.6/pysmells/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3852 2023-04-09 11:51:48.000000 pysmells-1.0.6/pysmells/pysmells.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-09 11:56:50.726858 pysmells-1.0.6/pysmells.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)     2169 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      262 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        9 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-09 11:56:50.730623 pysmells-1.0.6/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)     1424 2023-04-08 18:38:59.000000 pysmells-1.0.6/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.423219 pysmells-1.0.7/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.7/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 01:20:21.422515 pysmells-1.0.7/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.7/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.414705 pysmells-1.0.7/pysmells/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.7/pysmells/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     3847 2023-04-10 01:13:06.000000 pysmells-1.0.7/pysmells/pysmells.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.420913 pysmells-1.0.7/pysmells.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      279 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       14 2023-04-10 01:20:21.000000 pysmells-1.0.7/pysmells.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-10 01:20:21.423490 pysmells-1.0.7/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1332 2023-04-09 19:55:04.000000 pysmells-1.0.7/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 01:20:21.421735 pysmells-1.0.7/test/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-09 23:44:38.000000 pysmells-1.0.7/test/__init__.py
```

### Comparing `pysmells-1.0.6/LICENSE` & `pysmells-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.6/PKG-INFO` & `pysmells-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.6
-Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies, programming style violations and the correctness of type annotations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
+Version: 1.0.7
+Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pysmells-1.0.6/README.md` & `pysmells-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.6/pysmells/pysmells.py` & `pysmells-1.0.7/pysmells/pysmells.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,17 +15,14 @@
     match = type_annotation_pattern.search(content)
     return bool(match)
 
 
 def analyze_file(directory, file_path, table_data):
     print(f"Analyzing the file: {file_path}\n")
 
-    # Check Type Annotations
-    type_annotations_present = check_type_annotations(file_path)
-
     # Run Pylint
     process = subprocess.run(["pylint", file_path], stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                              universal_newlines=True, check=False)
     pylint_output = process.stdout
 
     alert_count = Counter()
     alert_details = defaultdict(list)
@@ -51,59 +48,56 @@
     total_alerts = sum(alert_count.values())
     # Update the table data structure
     table_row = [file_path, total_alerts]
     for alert_type in alert_type_names.keys():
         table_row.append(alert_count[alert_type])
 
     table_row.append(", ".join(sorted(set(alert_code for alert_codes in alert_details.values() for alert_code in alert_codes))))
-    table_row.append("Yes" if type_annotations_present else "No")  # Adds the "Adopt Type Annotations?" field
-
-    # Run Mypy
-    mypy_process = subprocess.run(["mypy", file_path], stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-                                  universal_newlines=True, check=False)
-    mypy_output = mypy_process.stdout
-
-    mypy_output_no_newline = mypy_output.replace('\n', ' | ')
-    table_row.append(mypy_output_no_newline if type_annotations_present else "None")  # Adds the "Type Annotations Description" field
     table_data.append(table_row)
 
     return total_alerts
 
 def export_to_csv(table_data, headers, csv_output):
     with open(csv_output, 'w', newline='') as csvfile:
         csv_writer = csv.writer(csvfile)
         csv_writer.writerow(headers)
         for row in table_data:
             csv_writer.writerow(row)
 
 def main():
-    parser = argparse.ArgumentParser(description="Analyze Python files in the specified directory.")
-    parser.add_argument("directory", help="The directory path containing the Python files to analyze.")
-    parser.add_argument("-o", "--output", help="The path and file name for the CSV output.", type=str)
+    parser = argparse.ArgumentParser(description="Analyze Python files in the specified directories.")
+    parser.add_argument("-p", "--project", required=True, help="The project directory containing the subdirectories with Python files to analyze.")
+    parser.add_argument("-s", "--subdirs", nargs='+', required=True, help="The list of subdirectories in the project directory, each representing a software.")
+    parser.add_argument("-csv", "--csv_output", help="The path and file name for the CSV output.", type=str)
 
     args = parser.parse_args()
-    root_directory = args.directory
-    csv_output = args.output
+    project_directory = os.path.abspath(args.project)
+    subdirectories = args.subdirs
+    csv_output = args.csv_output
+
+    print(f"Project directory (absolute path): {project_directory}")
 
     table_data = []
     total_alerts_directory = 0
 
-    for root, dirs, files in os.walk(root_directory):
-        for file_name in files:
-            if file_name.endswith(".py"):
-                file_path = os.path.join(root, file_name)
-                total_alerts_directory += analyze_file(root, file_path, table_data)
-
-    print(f"\nTotal alerts found in the directory: {total_alerts_directory}\n")
-    headers = ["File", "Total Alerts", "Convention", "Refactor", "Warning", "Error", "Fatal", "Alert Codes",
-               "Adopt Type Annotations?", "Type Annotations Description"]
+    for subdir in subdirectories:
+        current_directory = os.path.abspath(os.path.join(project_directory, subdir))
+        print(f"Analyzing subdirectory (absolute path): {current_directory}")
+        if os.path.isdir(current_directory):
+            for root, dirs, files in os.walk(current_directory):
+                for file_name in files:
+                    if file_name.endswith(".py"):
+                        file_path = os.path.join(root, file_name)
+                        total_alerts_directory += analyze_file(root, file_path, table_data)
+        else:
+            print(f"Subdirectory not found: {current_directory}")
+
+    print(f"\nTotal alerts found in the directories: {total_alerts_directory}\n")
+    headers = ["File", "Total Alerts", "Convention", "Refactor", "Warning", "Error", "Fatal", "Alert Codes"]
     print(tabulate(table_data, headers=headers, tablefmt="grid"))
 
     if csv_output:
         export_to_csv(table_data, headers, csv_output)
         print(f"CSV file exported to: {csv_output}")
 
 if __name__ == "__main__":
     main()
-
-
-
```

### Comparing `pysmells-1.0.6/pysmells.egg-info/PKG-INFO` & `pysmells-1.0.7/pysmells.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.6
-Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies, programming style violations and the correctness of type annotations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
+Version: 1.0.7
+Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pysmells-1.0.6/setup.py` & `pysmells-1.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pysmells",
-    version="1.0.6",
+    version="1.0.7",
     author="Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto",
     author_email="msousa@museu-goeldi.br",
-    description="Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies, programming style violations and the correctness of type annotations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.",
+    description="Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pysmells/pysmells",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

