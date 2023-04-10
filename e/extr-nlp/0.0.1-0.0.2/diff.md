# Comparing `tmp/extr-nlp-0.0.1.tar.gz` & `tmp/extr-nlp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-nlp-0.0.1.tar", last modified: Mon Apr 10 14:05:09 2023, max compression
+gzip compressed data, was "extr-nlp-0.0.2.tar", last modified: Mon Apr 10 14:11:29 2023, max compression
```

## Comparing `extr-nlp-0.0.1.tar` & `extr-nlp-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:09.566129 extr-nlp-0.0.1/
--rw-rw-rw-   0        0        0     2216 2023-04-10 14:05:09.545290 extr-nlp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1526 2023-04-10 13:31:15.000000 extr-nlp-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 14:05:09.571553 extr-nlp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-04-10 14:03:51.000000 extr-nlp-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:09.329332 extr-nlp-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:09.409722 extr-nlp-0.0.1/src/extr_nlp/
--rw-rw-rw-   0        0        0      226 2023-04-10 13:22:29.000000 extr-nlp-0.0.1/src/extr_nlp/__init__.py
--rw-rw-rw-   0        0        0     1526 2023-04-10 13:35:41.000000 extr-nlp-0.0.1/src/extr_nlp/entities.py
--rw-rw-rw-   0        0        0      158 2023-04-08 19:56:35.000000 extr-nlp-0.0.1/src/extr_nlp/iterutils.py
--rw-rw-rw-   0        0        0     1034 2023-04-10 13:02:05.000000 extr-nlp-0.0.1/src/extr_nlp/models.py
--rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-nlp-0.0.1/src/extr_nlp/regex.py
--rw-rw-rw-   0        0        0     1166 2023-04-10 13:13:58.000000 extr-nlp-0.0.1/src/extr_nlp/relations.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:09.531077 extr-nlp-0.0.1/src/extr_nlp.egg-info/
--rw-rw-rw-   0        0        0     2216 2023-04-10 14:05:08.000000 extr-nlp-0.0.1/src/extr_nlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-04-10 14:05:09.000000 extr-nlp-0.0.1/src/extr_nlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:05:08.000000 extr-nlp-0.0.1/src/extr_nlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 14:05:09.000000 extr-nlp-0.0.1/src/extr_nlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 14:11:29.593843 extr-nlp-0.0.2/
+-rw-rw-rw-   0        0        0     2356 2023-04-10 14:11:29.589145 extr-nlp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2023-04-10 14:08:55.000000 extr-nlp-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:11:29.598671 extr-nlp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-04-10 14:10:53.000000 extr-nlp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:11:29.482829 extr-nlp-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 14:11:29.529383 extr-nlp-0.0.2/src/extr_nlp/
+-rw-rw-rw-   0        0        0      226 2023-04-10 13:22:29.000000 extr-nlp-0.0.2/src/extr_nlp/__init__.py
+-rw-rw-rw-   0        0        0     1526 2023-04-10 13:35:41.000000 extr-nlp-0.0.2/src/extr_nlp/entities.py
+-rw-rw-rw-   0        0        0      158 2023-04-08 19:56:35.000000 extr-nlp-0.0.2/src/extr_nlp/iterutils.py
+-rw-rw-rw-   0        0        0     1034 2023-04-10 13:02:05.000000 extr-nlp-0.0.2/src/extr_nlp/models.py
+-rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-nlp-0.0.2/src/extr_nlp/regex.py
+-rw-rw-rw-   0        0        0     1166 2023-04-10 13:13:58.000000 extr-nlp-0.0.2/src/extr_nlp/relations.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:11:29.581464 extr-nlp-0.0.2/src/extr_nlp.egg-info/
+-rw-rw-rw-   0        0        0     2356 2023-04-10 14:11:29.000000 extr-nlp-0.0.2/src/extr_nlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-04-10 14:11:29.000000 extr-nlp-0.0.2/src/extr_nlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:11:29.000000 extr-nlp-0.0.2/src/extr_nlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 14:11:29.000000 extr-nlp-0.0.2/src/extr_nlp.egg-info/top_level.txt
```

### Comparing `extr-nlp-0.0.1/PKG-INFO` & `extr-nlp-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: extr-nlp
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
         
+        ## Install
+        
+        ```
+        pip install extr-nlp
+        ```
+        
+        ## Example
+        
         ```python
         text = 'Ted is a Pitcher.'
         ```
         
-        ## 1. Entity Extraction
+        ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtactor
+        from extr_nlp import RegEx, RegExLabel, EntityExtactor
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -33,20 +41,20 @@
         
         ## entities == [
         ##      <Entity label="POSITION" text="Pitcher" span=(9, 16)>,
         ##      <Entity label="PERSON" text="Ted" span=(0, 3)>
         ## ]
         ```
         
-        ## 2. Relation Extraction
+        ### 2. Relation Extraction
         > Annotate and Extract Relationships between Entities
         
         ```python
-        from extr import EntityAnnotator
-        from extr import RegExRelationLabelBuilder, RelationExtractor
+        from extr_nlp import EntityAnnotator
+        from extr_nlp import RegExRelationLabelBuilder, RelationExtractor
         
         ## define relationship between PERSON and POSITION
         relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON', ## e1
                 [
                     ## define how the relationship exists in nature
```

### Comparing `extr-nlp-0.0.1/README.md` & `extr-nlp-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # Extr - NLP
 
 > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 
 <br />
 
+## Install
+
+```
+pip install extr-nlp
+```
+
+## Example
+
 ```python
 text = 'Ted is a Pitcher.'
 ```
 
-## 1. Entity Extraction
+### 1. Entity Extraction
 > Find Named Entities from text.
 
 ```python
-from extr import RegEx, RegExLabel, EntityExtactor
+from extr_nlp import RegEx, RegExLabel, EntityExtactor
 
 entity_extractor = EntityExtactor([
     RegExLabel('PERSON', [
         RegEx([r'ted'], re.IGNORECASE)
     ]),
     RegExLabel('POSITION', [
         RegEx([r'pitcher'], re.IGNORECASE)
@@ -27,20 +35,20 @@
 
 ## entities == [
 ##      <Entity label="POSITION" text="Pitcher" span=(9, 16)>,
 ##      <Entity label="PERSON" text="Ted" span=(0, 3)>
 ## ]
 ```
 
-## 2. Relation Extraction
+### 2. Relation Extraction
 > Annotate and Extract Relationships between Entities
 
 ```python
-from extr import EntityAnnotator
-from extr import RegExRelationLabelBuilder, RelationExtractor
+from extr_nlp import EntityAnnotator
+from extr_nlp import RegExRelationLabelBuilder, RelationExtractor
 
 ## define relationship between PERSON and POSITION
 relationship = RegExRelationLabelBuilder('is_a') \
     .add_e1_to_e2(
         'PERSON', ## e1
         [
             ## define how the relationship exists in nature
```

### Comparing `extr-nlp-0.0.1/src/extr_nlp/entities.py` & `extr-nlp-0.0.2/src/extr_nlp/entities.py`

 * *Files identical despite different names*

### Comparing `extr-nlp-0.0.1/src/extr_nlp/models.py` & `extr-nlp-0.0.2/src/extr_nlp/models.py`

 * *Files identical despite different names*

### Comparing `extr-nlp-0.0.1/src/extr_nlp/regex.py` & `extr-nlp-0.0.2/src/extr_nlp/regex.py`

 * *Files identical despite different names*

### Comparing `extr-nlp-0.0.1/src/extr_nlp/relations.py` & `extr-nlp-0.0.2/src/extr_nlp/relations.py`

 * *Files identical despite different names*

### Comparing `extr-nlp-0.0.1/src/extr_nlp.egg-info/PKG-INFO` & `extr-nlp-0.0.2/src/extr_nlp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: extr-nlp
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
         
+        ## Install
+        
+        ```
+        pip install extr-nlp
+        ```
+        
+        ## Example
+        
         ```python
         text = 'Ted is a Pitcher.'
         ```
         
-        ## 1. Entity Extraction
+        ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtactor
+        from extr_nlp import RegEx, RegExLabel, EntityExtactor
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -33,20 +41,20 @@
         
         ## entities == [
         ##      <Entity label="POSITION" text="Pitcher" span=(9, 16)>,
         ##      <Entity label="PERSON" text="Ted" span=(0, 3)>
         ## ]
         ```
         
-        ## 2. Relation Extraction
+        ### 2. Relation Extraction
         > Annotate and Extract Relationships between Entities
         
         ```python
-        from extr import EntityAnnotator
-        from extr import RegExRelationLabelBuilder, RelationExtractor
+        from extr_nlp import EntityAnnotator
+        from extr_nlp import RegExRelationLabelBuilder, RelationExtractor
         
         ## define relationship between PERSON and POSITION
         relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON', ## e1
                 [
                     ## define how the relationship exists in nature
```

