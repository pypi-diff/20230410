# Comparing `tmp/pygedcom-0.1.4.tar.gz` & `tmp/pygedcom-0.1.5.tar.gz`

## Comparing `pygedcom-0.1.4.tar` & `pygedcom-0.1.5.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.4/main.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pygedcom-0.1.4/requirements.txt
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pygedcom-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.4/.github/workflows/test_and_doc.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/Makefile
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/conf.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/make.bat
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/export.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomElement.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomParser.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomRootElement.rst
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomSubElement.rst
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/getting_started.rst
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/parsing.rst
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/__init__.py
--rw-r--r--   0        0        0    20052 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/gedcom_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/__init__.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/element.py
--rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/mapping.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/__init__.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/family.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/head.py
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/individual.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/note.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/object.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/repository.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/rootElement.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/source.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/submitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/__init__.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/commonEvent.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/date.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/map.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/place.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/__init__.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_add_elements.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_export.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_parse.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_remove_element.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_verify.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/00_simple_individual_record.ged
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/01_simple_family_record.ged
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/02_simple_source_record.ged
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/03_simple_repository_record.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/04_simple_date_formats.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/05_all_date_modifiers.ged
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/10_invalid_level.ged
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/20_complex_sample.ged
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.4/LICENSE
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pygedcom-0.1.4/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pygedcom-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.5/main.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pygedcom-0.1.5/requirements.txt
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.5/.github/workflows/test_and_doc.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/Makefile
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/conf.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/make.bat
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/export.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomElement.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomParser.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomRootElement.rst
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomSubElement.rst
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/getting_started.rst
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/parsing.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/__init__.py
+-rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/gedcom_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/__init__.py
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/element.py
+-rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/mapping.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/__init__.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/family.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/head.py
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/individual.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/note.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/object.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/repository.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/rootElement.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/source.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/submitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/__init__.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/commonEvent.py
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/date.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/map.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/place.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_add_elements.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_export.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_parse.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_remove_element.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_set_prop.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_verify.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/00_simple_individual_record.ged
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/01_simple_family_record.ged
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/02_simple_source_record.ged
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/03_simple_repository_record.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/04_simple_date_formats.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/05_all_date_modifiers.ged
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/10_invalid_level.ged
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/20_complex_sample.ged
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pygedcom-0.1.5/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pygedcom-0.1.5/PKG-INFO
```

### Comparing `pygedcom-0.1.4/requirements.txt` & `pygedcom-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/.github/workflows/python-publish.yml` & `pygedcom-0.1.5/.github/workflows/python-publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
 name: Upload Python Package
 
 on:
-  release:
-    types: [published]
+  push:
+    tags:
+      - "v*"
 
 permissions:
   contents: read
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
```

### Comparing `pygedcom-0.1.4/.github/workflows/test_and_doc.yml` & `pygedcom-0.1.5/.github/workflows/test_and_doc.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/Makefile` & `pygedcom-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/conf.py` & `pygedcom-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/index.rst` & `pygedcom-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/make.bat` & `pygedcom-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/sources/export.rst` & `pygedcom-0.1.5/docs/sources/export.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/sources/gedcomRootElement.rst` & `pygedcom-0.1.5/docs/sources/gedcomRootElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/sources/gedcomSubElement.rst` & `pygedcom-0.1.5/docs/sources/gedcomSubElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/sources/getting_started.rst` & `pygedcom-0.1.5/docs/sources/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/docs/sources/parsing.rst` & `pygedcom-0.1.5/docs/sources/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/gedcom_parser.py` & `pygedcom-0.1.5/src/pygedcom/gedcom_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -432,45 +432,53 @@
             raise KeyError(
                 "Individual with xref " + individual.get_xref() + " already exists."
             )
 
     def add_family(self, family: GedcomFamily):
         """Add a family to the collection.
 
+        This checks :
+            - if the family passed is of type GedcomFamily.
+            - if the family passed does not already exist (by xref).
+            - if every parent and child exists (their xref are in the individual collection).
+
+
         :param family: The family to add.
         :type family: GedcomFamily
         :raises KeyError: If the family already exists.
         :raises TypeError: If the family is not of type GedcomFamily.
         """
+        if self.find_individual(family.get_husband()) is None:
+            raise KeyError("Husband with xref " + family.get_husband() + " not found.")
+        if self.find_individual(family.get_wife()) is None:
+            raise KeyError("Wife with xref " + family.get_wife() + " not found.")
+        for child in family.get_children():
+            if self.find_individual(child) is None:
+                raise KeyError("Child with xref " + child + " not found.")
         if not isinstance(family, GedcomFamily):
             raise TypeError("Family must be of type GedcomFamily.")
         try:
             self.__add_root_element(self.families, family)
         except KeyError:
-            raise KeyError(
-                "Family with xref " + family.get_xref() + " already exists."
-            )
-        self.families.append(family)
+            raise KeyError("Family with xref " + family.get_xref() + " already exists.")
 
     def add_source(self, source: GedcomSource):
         """Add a source to the collection.
 
         :param source: The source to add.
         :type source: GedcomSource
         :raises KeyError: If the source already exists.
         :raises TypeError: If the source is not of type GedcomSource.
         """
         if not isinstance(source, GedcomSource):
             raise TypeError("Source must be of type GedcomSource.")
         try:
             self.__add_root_element(self.sources, source)
         except KeyError:
-            raise KeyError(
-                "Source with xref " + source.get_xref() + " already exists."
-            )
+            raise KeyError("Source with xref " + source.get_xref() + " already exists.")
         self.sources.append(source)
 
     def add_object(self, object: GedcomObject):
         """Add an object to the collection.
 
         :param object: The object to add.
         :type object: GedcomObject
@@ -478,17 +486,15 @@
         :raises TypeError: If the object is not of type GedcomObject.
         """
         if not isinstance(object, GedcomObject):
             raise TypeError("Object must be of type GedcomObject.")
         try:
             self.__add_root_element(self.objects, object)
         except KeyError:
-            raise KeyError(
-                "Object with xref " + object.get_xref() + " already exists."
-            )
+            raise KeyError("Object with xref " + object.get_xref() + " already exists.")
         self.objects.append(object)
 
     def add_repository(self, repository: GedcomRepository):
         """Add a repository to the collection.
 
         :param repository: The repository to add.
         :type repository: GedcomRepository
@@ -516,15 +522,15 @@
         """
         element = self.__find_root_element(collection, xref)
         if not element:
             raise KeyError()
         collection.remove(element)
 
     def remove_individual(self, xref: str):
-        """Remove an individual from the collection.
+        """Remove an individual from the collection and all mentions of it in families.
 
         :param xref: The xref of the individual to remove.
         :type xref: str
         :raises KeyError: If the individual does not exist.
         """
         try:
             individual = self.find_individual(xref)
@@ -534,7 +540,26 @@
         xref = individual.get_xref()
 
         for family in self.families:
             family.remove_parent(xref)
             family.remove_child(xref)
 
         self.__remove_root_element(self.individuals, xref)
+
+    def remove_family(self, xref: str):
+        """Remove a family from the collection.
+
+        :param xref: The xref of the family to remove.
+        :type xref: str
+        :raises KeyError: If the family does not exist.
+        """
+        try:
+            family = self.find_family(xref)
+        except KeyError:
+            raise KeyError("Family with xref " + xref + " does not exist.")
+
+        xref = family.get_xref()
+
+        for individual in self.individuals:
+            individual.remove_family(xref)
+
+        self.__remove_root_element(self.families, xref)
```

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/element.py` & `pygedcom-0.1.5/src/pygedcom/elements/element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/mapping.json` & `pygedcom-0.1.5/src/pygedcom/elements/mapping.json`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/head.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/head.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/individual.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/individual.py`

 * *Files 9% similar despite different names*

```diff
@@ -168,29 +168,53 @@
         """
         self.__export_first_name = first_name
         self.__export_name = f"{first_name} /{self.__export_last_name}/"
         name_element = self.find_sub_element("NAME")
         if name_element != []:
             name_element[0].set_value(self.__export_name)
         else:
-            self.add_sub_element(2, "NAME", [], value=self.__export_name)
+            self.add_sub_element(1, "NAME", [], value=self.__export_name)
 
     def set_last_name(self, last_name: str):
         """Set the last name of the individual.
 
         :param last_name: The last name of the individual.
         :type last_name: str
         """
         self.__export_last_name = last_name
         self.__export_name = f"{self.__export_first_name} /{last_name}/"
         name_element = self.find_sub_element("NAME")
         if name_element != []:
             name_element[0].set_value(self.__export_name)
         else:
-            self.add_sub_element(2, "NAME", [], value=self.__export_name)
+            self.add_sub_element(1, "NAME", [], value=self.__export_name)
+
+    def set_sex(self, sex_value: str):
+        """Set the sex of the individual. This is not changing family relations.
+
+        :param sex_value: The sex value of the individual.
+        :type sex_value: str
+        """
+        self.__export_sex = sex_value
+        sex_element = self.find_sub_element("SEX")
+        if sex_element != []:
+            sex_element[0].set_value(self.__export_sex)
+        else:
+            self.add_sub_element(1, "SEX", [], value=self.__export_sex)
+
+    def remove_family(self, family_xref: str):
+        """Remove the family from the individual.
+
+        :param family_xref: The family xref to remove.
+        :type family_xref: str
+        """
+        for fam_tag in ["FAMC", "FAMS"]:
+            for fam in self.find_sub_element(fam_tag):
+                if fam.get_value() == family_xref:
+                    self.remove_sub_element(fam)
 
     def __str__(self):
         """Get the string representation of the individual.
 
         :return: The string representation of the individual.
         :rtype: str
         """
```

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/note.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/note.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/object.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/object.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/repository.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/repository.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/rootElement.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/rootElement.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/source.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/source.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/rootElements/submitter.py` & `pygedcom-0.1.5/src/pygedcom/elements/rootElements/submitter.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/subElements/commonEvent.py` & `pygedcom-0.1.5/src/pygedcom/elements/subElements/commonEvent.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/subElements/date.py` & `pygedcom-0.1.5/src/pygedcom/elements/subElements/date.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/subElements/map.py` & `pygedcom-0.1.5/src/pygedcom/elements/subElements/map.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/src/pygedcom/elements/subElements/place.py` & `pygedcom-0.1.5/src/pygedcom/elements/subElements/place.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/test/test_export.py` & `pygedcom-0.1.5/test/test_export.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/test/test_parse.py` & `pygedcom-0.1.5/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/test/test_verify.py` & `pygedcom-0.1.5/test/test_verify.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/test/samples/20_complex_sample.ged` & `pygedcom-0.1.5/test/samples/20_complex_sample.ged`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/.gitignore` & `pygedcom-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/LICENSE` & `pygedcom-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/README.md` & `pygedcom-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.4/pyproject.toml` & `pygedcom-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygedcom"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     { name="Theo Petit", email="theo.p83@gmail.com" },
 ]
 description = "A gedcom utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygedcom-0.1.4/PKG-INFO` & `pygedcom-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygedcom
-Version: 0.1.4
+Version: 0.1.5
 Summary: A gedcom utility library
 Project-URL: Homepage, https://github.com/topetit/pygedcom
 Project-URL: Bug Tracker, https://github.com/topetit/pygedcom/issues
 Author-email: Theo Petit <theo.p83@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

