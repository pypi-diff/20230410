# Comparing `tmp/deg-1.0.0.tar.gz` & `tmp/deg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deg-1.0.0.tar", last modified: Mon Apr 10 10:45:01 2023, max compression
+gzip compressed data, was "deg-1.0.1.tar", last modified: Mon Apr 10 10:52:58 2023, max compression
```

## Comparing `deg-1.0.0.tar` & `deg-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:45:01.117124 deg-1.0.0/
--rwxrwxrwx   0 root         (0) root         (0)    11350 2023-03-29 03:10:59.000000 deg-1.0.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)    13470 2023-04-10 10:45:01.117539 deg-1.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-29 01:50:59.000000 deg-1.0.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:45:01.113948 deg-1.0.0/deg/
--rwxrwxrwx   0 root         (0) root         (0)     5172 2023-04-10 10:43:25.000000 deg-1.0.0/deg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:45:01.116777 deg-1.0.0/deg.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    13470 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      208 2023-04-10 10:45:01.000000 deg-1.0.0/deg.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        4 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-10 10:45:01.118024 deg-1.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1211 2023-04-10 10:44:57.000000 deg-1.0.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:52:58.821200 deg-1.0.1/
+-rwxrwxrwx   0 root         (0) root         (0)    11350 2023-03-29 03:10:59.000000 deg-1.0.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)    16557 2023-04-10 10:52:58.821744 deg-1.0.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3160 2023-04-10 10:51:45.000000 deg-1.0.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:52:58.817565 deg-1.0.1/deg/
+-rwxrwxrwx   0 root         (0) root         (0)     5172 2023-04-10 10:43:25.000000 deg-1.0.1/deg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:52:58.820824 deg-1.0.1/deg.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    16557 2023-04-10 10:52:58.000000 deg-1.0.1/deg.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      208 2023-04-10 10:52:58.000000 deg-1.0.1/deg.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 10:52:58.000000 deg-1.0.1/deg.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-04-10 10:52:58.000000 deg-1.0.1/deg.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        4 2023-04-10 10:52:58.000000 deg-1.0.1/deg.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 10:52:58.000000 deg-1.0.1/deg.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-10 10:52:58.822253 deg-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1211 2023-04-10 10:52:43.000000 deg-1.0.1/setup.py
```

### Comparing `deg-1.0.0/LICENSE` & `deg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deg-1.0.0/PKG-INFO` & `deg-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deg
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Graph library to manage inheritance rules
 Home-page: https://github.com/supratikchatterjee16/deg
 Author: Supratik Chatterjee
 Author-email: supratikdevm96@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -211,8 +211,85 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Depency Graph
 
-A Graph creation, analysis and visualizations library. 
+A Graph creation, analysis and visualizations library.
+
+## Installation
+
+```shell
+pip install deg
+```
+
+## Usage
+
+Can be used directly using the `DependencyNode` object or by extending the object into some other subjective structure.
+
+A sample usage would look as the following : 
+```python
+from deg import DependencyGraph, DependencyNode
+
+class Table(DependencyNode):
+    '''Class for representing each node of the tree.
+    This contains every piece of static information that may be required for analysis.
+    
+    '''
+    def __init__(self, name, cols=None):
+        super(Table, self).__init__(name)
+        self.cols=cols
+        self.visited = False
+        self.col_relations = None
+    
+    def add_cols(self, df : pd.DataFrame):
+        self.cols = df
+    def add_relations(self, df : pd.DataFrame):
+        self.col_relations = df
+    def generate_search_criteria(self, module=None):
+        selection = ''
+        if self.is_independent():
+            print('Ignoring rules for independent table :\n', self.col_relations.to_string())
+            selection = '''TRUNC({tablename}.{datecol}) BETWEEN (SELECT PRG_PERIOD_START FROM PURGE_MODULE_INPUT WHERE REQUEST_ID = PRG_BTCH_ID AND MODULE = '{module}' AND STATUS = 'INITIATED') AND (SELECT PRG_PERIOD_END FROM PURGE_MODULE_INPUT WHERE REQUEST_ID = PRG_BTCH_ID AND MODULE = '{module}' AND STATUS = 'INITIATED')'''.format(tablename=self.name,datecol=self.get_date_col(), module=module)
+        else :
+            for parent in self.parents:
+                criterias = ''
+                for _, row in self.col_relations[self.col_relations['r_table'] == parent.name].iterrows():
+                    if len(criterias) > 0:
+                        criterias += ' AND '
+                    criterias += '{0}.{1} = {2}.{3} '.format(row['table_name'], row['column_name'], row['r_table'], row['r_col'])
+                criterias += ' AND ' + parent.generate_search_criteria(module=module)
+                selection += 'INNER JOIN {parent_name} ON {criterias}'.format(parent_name = parent.name, criterias = criterias)
+        return selection
+    def get_cols(self) -> pd.DataFrame:
+        return self.cols
+    def is_visited(self) -> bool :
+        return self.visited
+    def set_visited(self) :
+        self.visited = True
+    def get_date_col(self):
+        try:
+            return self.cols[(self.cols['data_type'] == 'DATE') & (self.cols['nullable'] == 'N')].iloc[-1]['column_name']
+        except Exception as e:
+            # print(e)
+            return None
+    def __str__(self):
+        return 'Table({0}, {1})'.format(self.name, self.is_independent(), self.children)
+    def __repr__(self):
+        return 'Table({0}, {1})'.format(self.name, self.is_independent(), self.children)
+
+graph = DependencyGraph(Table)
+while True:
+    df = get_children(temp)
+    if df is None or df.shape == (0, 0) :
+        break
+    for val in df.itertuples():
+        graph.add(val[2], parent=val[1], relation = val[3])
+    temp = df.iloc[:, 1]
+    execution_limit -= 1
+    if execution_limit <= 0 :
+        break
+```
+
+Docstrings have been added to detail what functions such as `graph.add` does.
+
```

### Comparing `deg-1.0.0/deg/__init__.py` & `deg-1.0.1/deg/__init__.py`

 * *Files identical despite different names*

### Comparing `deg-1.0.0/deg.egg-info/PKG-INFO` & `deg-1.0.1/deg.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deg
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Graph library to manage inheritance rules
 Home-page: https://github.com/supratikchatterjee16/deg
 Author: Supratik Chatterjee
 Author-email: supratikdevm96@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -211,8 +211,85 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Depency Graph
 
-A Graph creation, analysis and visualizations library. 
+A Graph creation, analysis and visualizations library.
+
+## Installation
+
+```shell
+pip install deg
+```
+
+## Usage
+
+Can be used directly using the `DependencyNode` object or by extending the object into some other subjective structure.
+
+A sample usage would look as the following : 
+```python
+from deg import DependencyGraph, DependencyNode
+
+class Table(DependencyNode):
+    '''Class for representing each node of the tree.
+    This contains every piece of static information that may be required for analysis.
+    
+    '''
+    def __init__(self, name, cols=None):
+        super(Table, self).__init__(name)
+        self.cols=cols
+        self.visited = False
+        self.col_relations = None
+    
+    def add_cols(self, df : pd.DataFrame):
+        self.cols = df
+    def add_relations(self, df : pd.DataFrame):
+        self.col_relations = df
+    def generate_search_criteria(self, module=None):
+        selection = ''
+        if self.is_independent():
+            print('Ignoring rules for independent table :\n', self.col_relations.to_string())
+            selection = '''TRUNC({tablename}.{datecol}) BETWEEN (SELECT PRG_PERIOD_START FROM PURGE_MODULE_INPUT WHERE REQUEST_ID = PRG_BTCH_ID AND MODULE = '{module}' AND STATUS = 'INITIATED') AND (SELECT PRG_PERIOD_END FROM PURGE_MODULE_INPUT WHERE REQUEST_ID = PRG_BTCH_ID AND MODULE = '{module}' AND STATUS = 'INITIATED')'''.format(tablename=self.name,datecol=self.get_date_col(), module=module)
+        else :
+            for parent in self.parents:
+                criterias = ''
+                for _, row in self.col_relations[self.col_relations['r_table'] == parent.name].iterrows():
+                    if len(criterias) > 0:
+                        criterias += ' AND '
+                    criterias += '{0}.{1} = {2}.{3} '.format(row['table_name'], row['column_name'], row['r_table'], row['r_col'])
+                criterias += ' AND ' + parent.generate_search_criteria(module=module)
+                selection += 'INNER JOIN {parent_name} ON {criterias}'.format(parent_name = parent.name, criterias = criterias)
+        return selection
+    def get_cols(self) -> pd.DataFrame:
+        return self.cols
+    def is_visited(self) -> bool :
+        return self.visited
+    def set_visited(self) :
+        self.visited = True
+    def get_date_col(self):
+        try:
+            return self.cols[(self.cols['data_type'] == 'DATE') & (self.cols['nullable'] == 'N')].iloc[-1]['column_name']
+        except Exception as e:
+            # print(e)
+            return None
+    def __str__(self):
+        return 'Table({0}, {1})'.format(self.name, self.is_independent(), self.children)
+    def __repr__(self):
+        return 'Table({0}, {1})'.format(self.name, self.is_independent(), self.children)
+
+graph = DependencyGraph(Table)
+while True:
+    df = get_children(temp)
+    if df is None or df.shape == (0, 0) :
+        break
+    for val in df.itertuples():
+        graph.add(val[2], parent=val[1], relation = val[3])
+    temp = df.iloc[:, 1]
+    execution_limit -= 1
+    if execution_limit <= 0 :
+        break
+```
+
+Docstrings have been added to detail what functions such as `graph.add` does.
+
```

### Comparing `deg-1.0.0/setup.py` & `deg-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requirements_noversion = [
 	'networkx',
     'matplotlib'
 ]
 setup(
 	# Meta information
 	name				= 'deg',
-	version				= '1.0.0',
+	version				= '1.0.1',
 	author				= 'Supratik Chatterjee',
 	author_email			= 'supratikdevm96@gmail.com',
 	url				= 'https://github.com/supratikchatterjee16/deg',
 	description			= 'A Graph library to manage inheritance rules',
 	keywords			= ['graph', 'visualize', 'dependency', 'inheritance'],
 	install_requires		= requirements_noversion,
 	# build information
```

