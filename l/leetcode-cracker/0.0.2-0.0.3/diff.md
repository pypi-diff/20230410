# Comparing `tmp/leetcode_cracker-0.0.2.tar.gz` & `tmp/leetcode_cracker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetcode_cracker-0.0.2.tar", last modified: Fri Apr  7 10:02:28 2023, max compression
+gzip compressed data, was "leetcode_cracker-0.0.3.tar", last modified: Mon Apr 10 10:33:59 2023, max compression
```

## Comparing `leetcode_cracker-0.0.2.tar` & `leetcode_cracker-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:28.658671 leetcode_cracker-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1702 2023-04-07 10:02:28.657431 leetcode_cracker-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-04-06 22:32:41.000000 leetcode_cracker-0.0.2/README.md
--rw-rw-rw-   0        0        0      658 2023-04-06 23:36:59.000000 leetcode_cracker-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 10:02:28.659668 leetcode_cracker-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:28.619460 leetcode_cracker-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:28.640933 leetcode_cracker-0.0.2/src/leetcode_cracker/
--rw-rw-rw-   0        0        0       21 2023-04-07 10:01:07.000000 leetcode_cracker-0.0.2/src/leetcode_cracker/__init__.py
--rw-rw-rw-   0        0        0      677 2023-04-07 07:19:57.000000 leetcode_cracker-0.0.2/src/leetcode_cracker/question_392.py
--rw-rw-rw-   0        0        0       37 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.2/src/leetcode_cracker/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:28.655933 leetcode_cracker-0.0.2/src/leetcode_cracker.egg-info/
--rw-rw-rw-   0        0        0     1702 2023-04-07 10:02:28.000000 leetcode_cracker-0.0.2/src/leetcode_cracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-07 10:02:28.000000 leetcode_cracker-0.0.2/src/leetcode_cracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 10:02:28.000000 leetcode_cracker-0.0.2/src/leetcode_cracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-07 10:02:28.000000 leetcode_cracker-0.0.2/src/leetcode_cracker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.655075 leetcode_cracker-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-04-10 10:33:59.654078 leetcode_cracker-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2023-04-08 07:25:56.000000 leetcode_cracker-0.0.3/README.md
+-rw-rw-rw-   0        0        0      658 2023-04-06 23:36:59.000000 leetcode_cracker-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 10:33:59.655075 leetcode_cracker-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.563600 leetcode_cracker-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.636638 leetcode_cracker-0.0.3/src/leetcode_cracker/
+-rw-rw-rw-   0        0        0       21 2023-04-10 10:32:27.000000 leetcode_cracker-0.0.3/src/leetcode_cracker/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-04-10 10:32:09.000000 leetcode_cracker-0.0.3/src/leetcode_cracker/question_392.py
+-rw-rw-rw-   0        0        0       37 2023-04-06 22:21:06.000000 leetcode_cracker-0.0.3/src/leetcode_cracker/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:33:59.652085 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-10 10:33:59.000000 leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/top_level.txt
```

### Comparing `leetcode_cracker-0.0.2/LICENSE` & `leetcode_cracker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.2/PKG-INFO` & `leetcode_cracker-0.0.3/src/leetcode_cracker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: leetcode_cracker
-Version: 0.0.2
+Name: leetcode-cracker
+Version: 0.0.3
 Summary: package to assist in solving Leetcode Problems
 Author-email: Albert <albertyqyao@gmail.com>
 Project-URL: Homepage, https://github.com/AlbertY123/leetcode-cracker
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -17,7 +17,13 @@
 - Search for a specific question by its title or ID
 - Get a summary of the question, including its difficulty level, acceptance rate, tags, and company frequency
 - Get a step-by-step explanation of the optimal solution, along with the time and space complexity analysis
 - Get the Python code for the optimal solution, along with comments and test cases
 - Compare your code with other solutions and learn from different approaches
 
 Leetcode Cracker is designed to help you improve your coding skills and ace your technical interviews. It is easy to install and use.
+
+# How to use the package
+
+1. Import the package: `pip install leetcode-cracker`
+2. Import package locally: `from leetcode_cracker import question_question number`
+3. Call a command: `question_question number.print_solution()`
```

### Comparing `leetcode_cracker-0.0.2/README.md` & `leetcode_cracker-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,29 @@
+Metadata-Version: 2.1
+Name: leetcode_cracker
+Version: 0.0.3
+Summary: package to assist in solving Leetcode Problems
+Author-email: Albert <albertyqyao@gmail.com>
+Project-URL: Homepage, https://github.com/AlbertY123/leetcode-cracker
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Leetcode Cracker Info
 Leetcode Cracker is a Python package that allows you to get LeetCode question explanations and answers. LeetCode is a popular online platform for practicing coding skills and preparing for technical interviews. LeetCode offers hundreds of problems covering various topics, such as arrays, strings, trees, graphs, dynamic programming, etc. However, sometimes the official solutions and explanations are not clear enough or not available at all. Leetcode Cracker solves this problem by providing you with detailed and easy-to-understand explanations and answers for any LeetCode question. You can soon use Leetcode Cracker to:
 
 - Search for a specific question by its title or ID
 - Get a summary of the question, including its difficulty level, acceptance rate, tags, and company frequency
 - Get a step-by-step explanation of the optimal solution, along with the time and space complexity analysis
 - Get the Python code for the optimal solution, along with comments and test cases
 - Compare your code with other solutions and learn from different approaches
 
 Leetcode Cracker is designed to help you improve your coding skills and ace your technical interviews. It is easy to install and use.
+
+# How to use the package
+
+1. Import the package: `pip install leetcode-cracker`
+2. Import package locally: `from leetcode_cracker import question_question number`
+3. Call a command: `question_question number.print_solution()`
```

### Comparing `leetcode_cracker-0.0.2/pyproject.toml` & `leetcode_cracker-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `leetcode_cracker-0.0.2/src/leetcode_cracker/question_392.py` & `leetcode_cracker-0.0.3/src/leetcode_cracker/question_392.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+def print_question():
+    print("""Given two strings s and t, return true if s is a subsequence of t, or false otherwise.
+
+            A subsequence of a string is a new string that is formed from the original string by deleting some (can be none) of the characters without disturbing the relative positions of the remaining characters. (i.e., "ace" is a subsequence of "abcde" while "aec" is not).
+        """)
 def print_solution():
 
     print("""
    class Solution:
     
     def isSubsequence(self, s: str, t: str) -> bool:
         # Init Both Variables
```

### Comparing `leetcode_cracker-0.0.2/src/leetcode_cracker.egg-info/PKG-INFO` & `leetcode_cracker-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-Metadata-Version: 2.1
-Name: leetcode-cracker
-Version: 0.0.2
-Summary: package to assist in solving Leetcode Problems
-Author-email: Albert <albertyqyao@gmail.com>
-Project-URL: Homepage, https://github.com/AlbertY123/leetcode-cracker
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Leetcode Cracker Info
 Leetcode Cracker is a Python package that allows you to get LeetCode question explanations and answers. LeetCode is a popular online platform for practicing coding skills and preparing for technical interviews. LeetCode offers hundreds of problems covering various topics, such as arrays, strings, trees, graphs, dynamic programming, etc. However, sometimes the official solutions and explanations are not clear enough or not available at all. Leetcode Cracker solves this problem by providing you with detailed and easy-to-understand explanations and answers for any LeetCode question. You can soon use Leetcode Cracker to:
 
 - Search for a specific question by its title or ID
 - Get a summary of the question, including its difficulty level, acceptance rate, tags, and company frequency
 - Get a step-by-step explanation of the optimal solution, along with the time and space complexity analysis
 - Get the Python code for the optimal solution, along with comments and test cases
 - Compare your code with other solutions and learn from different approaches
 
 Leetcode Cracker is designed to help you improve your coding skills and ace your technical interviews. It is easy to install and use.
+
+# How to use the package
+
+1. Import the package: `pip install leetcode-cracker`
+2. Import package locally: `from leetcode_cracker import question_question number`
+3. Call a command: `question_question number.print_solution()`
```

